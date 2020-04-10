---
title: 设置包含资源数据的更改通知（预览版）
description: Microsoft Graph 使用 Webhook 机制将更改通知传递到客户端。 通知中可以包含资源属性。
author: baywet
ms.prod: non-product-specific
localization_priority: Priority
ms.openlocfilehash: 41cf03e94bef399142135c899d812820651338b7
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/09/2020
ms.locfileid: "43200213"
---
# <a name="set-up-change-notifications-that-include-resource-data-preview"></a><span data-ttu-id="c27c5-104">设置包含资源数据的更改通知（预览版）</span><span class="sxs-lookup"><span data-stu-id="c27c5-104">Set up change notifications that include resource data (preview)</span></span>

<span data-ttu-id="c27c5-105">Microsoft Graph 允许应用通过 [webhooks](webhooks.md)来订阅资源更改通知。</span><span class="sxs-lookup"><span data-stu-id="c27c5-105">Microsoft Graph allows apps to subscribe to change notifications for resources via [webhooks](webhooks.md).</span></span> <span data-ttu-id="c27c5-106">现在可以在通知中设置订阅，将已更改资源数据（如 Microsoft 团队聊天消息内容）包含在中。</span><span class="sxs-lookup"><span data-stu-id="c27c5-106">You can now set up subscriptions to include the changed resource data (such as the content of a Microsoft Teams chat message) in notifications.</span></span> <span data-ttu-id="c27c5-107">随后，应用程序可运行其业务逻辑，无需调用单独的 API 来获取更改的资源。</span><span class="sxs-lookup"><span data-stu-id="c27c5-107">Your app can then run its business logic without having to make a separate API call to fetch the changed resource.</span></span> <span data-ttu-id="c27c5-108">因此，应用程序的 API 调用更少，对于大型方案非常有用。</span><span class="sxs-lookup"><span data-stu-id="c27c5-108">As a result, the app performs better by making fewer API calls, which is beneficial in large scale scenarios.</span></span>

<span data-ttu-id="c27c5-109">若要将资源数据作为通知的一部分，需要实现以下附加逻辑，来满足数据访问和安全要求：</span><span class="sxs-lookup"><span data-stu-id="c27c5-109">Including resource data as part of notifications requires you to implement the following additional logic to satisfy data access and security requirements:</span></span> 

- <span data-ttu-id="c27c5-110">[处理](#subscription-life-cycle-notifications)特殊订阅_生命周期_通知，以保持数据的不间断流动。</span><span class="sxs-lookup"><span data-stu-id="c27c5-110">[Handle](#subscription-life-cycle-notifications) special subscription _life cycle_ notifications to maintain an uninterrupted flow of data.</span></span> <span data-ttu-id="c27c5-111">Microsoft Graph 会不时发送生命周期通知，以要求应用程序重新授权，确保通知中所包含的数据不会意外发生存取问题。</span><span class="sxs-lookup"><span data-stu-id="c27c5-111">Microsoft Graph sends life cycle notifications from time to time to require an app to re-authorize, to make sure access issues have not unexpectedly cropped up for including resource data in notifications.</span></span>
- <span data-ttu-id="c27c5-112">[验证](#validating-the-authenticity-of-notifications)来自 Microsoft Graph 通知的真实性。</span><span class="sxs-lookup"><span data-stu-id="c27c5-112">[Validate](#validating-the-authenticity-of-notifications) the authenticity of notifications as having originated from Microsoft Graph.</span></span>
- <span data-ttu-id="c27c5-113">[提供](#decrypting-resource-data-from-change-notifications)公共加密密钥并使用私钥解密通过通知所接收的资源数据。</span><span class="sxs-lookup"><span data-stu-id="c27c5-113">[Provide](#decrypting-resource-data-from-change-notifications) a public encryption key and use a private key to decrypt resource data received through notifications.</span></span>

## <a name="resource-data-in-notification-payload"></a><span data-ttu-id="c27c5-114">通知负载中的资源数据</span><span class="sxs-lookup"><span data-stu-id="c27c5-114">Resource data in notification payload</span></span>

<span data-ttu-id="c27c5-115">通常情况下，此类更改通知包括负载中的以下资源数据：</span><span class="sxs-lookup"><span data-stu-id="c27c5-115">In general, this type of change notifications include the following resource data in the payload:</span></span>

- <span data-ttu-id="c27c5-116">**resourceData**属性中返回的已更改资源实例的ID和类型。</span><span class="sxs-lookup"><span data-stu-id="c27c5-116">ID and type of the changed resource instance, returned in the **resourceData** property.</span></span>
- <span data-ttu-id="c27c5-117">按照订阅中规定内容加密、在 **encryptedContent** 属性中返回的资源实例的所有属性值。</span><span class="sxs-lookup"><span data-stu-id="c27c5-117">All the property values of that resource instance, encrypted as specified in the subscription, returned in the **encryptedContent** property.</span></span>
- <span data-ttu-id="c27c5-118">或者，具体取决于资源、**resourceData**属性中返回的特定属性。</span><span class="sxs-lookup"><span data-stu-id="c27c5-118">Or, depending on the resource, specific properties returned in the **resourceData** property.</span></span> <span data-ttu-id="c27c5-119">若要仅获取特定属性，请使用 `$select` 参数，将其指定为订阅中的**资源**URL 的一部分。</span><span class="sxs-lookup"><span data-stu-id="c27c5-119">To get only specific properties, specify them as part of the **resource** URL in the subscription, using a `$select` parameter.</span></span>  


## <a name="supported-resources"></a><span data-ttu-id="c27c5-120">支持的资源</span><span class="sxs-lookup"><span data-stu-id="c27c5-120">Supported resources</span></span>

<span data-ttu-id="c27c5-121">目前，Microsoft 团队 [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) （预览版）资源支持包括资源数据的更改通知。</span><span class="sxs-lookup"><span data-stu-id="c27c5-121">Currently, the Microsoft Teams [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) (preview) resource supports change notifications that include resource data.</span></span> <span data-ttu-id="c27c5-122">具体而言，可设置应用以下内容之一的订阅：</span><span class="sxs-lookup"><span data-stu-id="c27c5-122">Specifically, you can set up a subscription that applies to one of the following:</span></span>

- <span data-ttu-id="c27c5-123">特定 Teams 频道中新增或已更改的消息：`/teams/{id}/channels/{id}/messages`</span><span class="sxs-lookup"><span data-stu-id="c27c5-123">New or changed messages in a specific Teams channel: `/teams/{id}/channels/{id}/messages`</span></span>
- <span data-ttu-id="c27c5-124">指定团队聊天中的新增或已更改消息： `/chats/{id}/messages`</span><span class="sxs-lookup"><span data-stu-id="c27c5-124">New or changed messages in a specific Teams chat: `/chats/{id}/messages`</span></span>

<span data-ttu-id="c27c5-125">含有通知中所有已更改实例属性的 **chatMessage** 支持。</span><span class="sxs-lookup"><span data-stu-id="c27c5-125">The **chatMessage** resource supports including all the properties of a changed instance in a notification.</span></span> <span data-ttu-id="c27c5-126">它不支持只返回指定实例属性。</span><span class="sxs-lookup"><span data-stu-id="c27c5-126">It does not support returning only selective properties of the instance.</span></span> 

<span data-ttu-id="c27c5-127">本文介绍订阅 "团队频道" 中的消息更改通知的示例，各通知包含已更改**chatMessage** 实例的完整资源数据。</span><span class="sxs-lookup"><span data-stu-id="c27c5-127">This article walks through an example of subscribing to change notifications of messages in a Teams channel, with each notification including the full resource data of the changed **chatMessage** instance.</span></span>

## <a name="creating-a-subscription"></a><span data-ttu-id="c27c5-128">创建订阅</span><span class="sxs-lookup"><span data-stu-id="c27c5-128">Creating a subscription</span></span>

<span data-ttu-id="c27c5-129">若要将资源数据包含在更改通知中，除了[创建订阅](webhooks.md#creating-a-subscription)时通常指定的属性外，**必须**指定下列属性：</span><span class="sxs-lookup"><span data-stu-id="c27c5-129">To have resource data included in change notifications, you **must** specify the following properties, in addition to those that are usually specified when [creating a subscription](webhooks.md#creating-a-subscription):</span></span>

- <span data-ttu-id="c27c5-130">**includeResourceData**，应设置为 `true` 以明确请求资源数据。</span><span class="sxs-lookup"><span data-stu-id="c27c5-130">**includeResourceData** which should be set to `true` to explicitly request resource data.</span></span>
- <span data-ttu-id="c27c5-131">**lifecycleNotificationUrl**，它是传递[life cycle notifications](#subscription-life-cycle-notifications)的终结点。</span><span class="sxs-lookup"><span data-stu-id="c27c5-131">**lifecycleNotificationUrl** which is an endpoint where [life cycle notifications](#subscription-life-cycle-notifications) are delivered.</span></span> <span data-ttu-id="c27c5-132">这可以与**notificationUrl**相同或不同。</span><span class="sxs-lookup"><span data-stu-id="c27c5-132">This can be the same or different as **notificationUrl**.</span></span>
- <span data-ttu-id="c27c5-133">**encryptionCertificate**，仅包含 Microsoft Graph 用于加密资源数据的公钥。</span><span class="sxs-lookup"><span data-stu-id="c27c5-133">**encryptionCertificate** which contains only the public key that Microsoft Graph uses to encrypt resource data.</span></span> <span data-ttu-id="c27c5-134">保留相应的私钥，以[解密内容](#decrypting-resource-data-from-change-notifications)。</span><span class="sxs-lookup"><span data-stu-id="c27c5-134">Keep the corresponding private key to [decrypt the content](#decrypting-resource-data-from-change-notifications).</span></span>
- <span data-ttu-id="c27c5-135">**encryptionCertificateId**，是证书的自有标识符。</span><span class="sxs-lookup"><span data-stu-id="c27c5-135">**encryptionCertificateId** which is your own identifier for the certificate.</span></span> <span data-ttu-id="c27c5-136">使用此 ID 在各通知中匹配用于解密的证书。</span><span class="sxs-lookup"><span data-stu-id="c27c5-136">Use this ID to match in each notification, which certificate to use for decryption.</span></span>

<span data-ttu-id="c27c5-137">请注意下列事项：</span><span class="sxs-lookup"><span data-stu-id="c27c5-137">Keep the following in mind:</span></span>

- <span data-ttu-id="c27c5-138">将相同的主机名用于两个通知终结点（**notificationUrl** 和 **lifecycleNotificationUrl**）。</span><span class="sxs-lookup"><span data-stu-id="c27c5-138">Use the same host name for both notification endpoints (**notificationUrl** and **lifecycleNotificationUrl**).</span></span>
- <span data-ttu-id="c27c5-139">如[此处](webhooks.md#notification-endpoint-validation)所述，验证两个通知终结点。</span><span class="sxs-lookup"><span data-stu-id="c27c5-139">Validate both notification endpoints as described [here](webhooks.md#notification-endpoint-validation).</span></span> <span data-ttu-id="c27c5-140">如果选择针对两个终结点使用同一 URL，将收到并响应两个验证请求。</span><span class="sxs-lookup"><span data-stu-id="c27c5-140">If you choose to use the same URL for both endpoints, you will receive and respond to two validation requests.</span></span>
- <span data-ttu-id="c27c5-141">无法更新（`PATCH`）现有订阅来添加**lifecycleNotificationUrl**属性。</span><span class="sxs-lookup"><span data-stu-id="c27c5-141">You cannot update (`PATCH`) an existing subscription to add the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="c27c5-142">应删除此类现有订阅，创建新订阅以包含 **lifecycleNotificationUrl** 属性。</span><span class="sxs-lookup"><span data-stu-id="c27c5-142">You should remove the existing subscription, and create a new subscription to include the **lifecycleNotificationUrl** property.</span></span>

### <a name="subscription-request-example"></a><span data-ttu-id="c27c5-143">订阅请求示例</span><span class="sxs-lookup"><span data-stu-id="c27c5-143">Subscription request example</span></span>

<span data-ttu-id="c27c5-144">下面的示例订阅了两种类型的通知：</span><span class="sxs-lookup"><span data-stu-id="c27c5-144">The following example subscribes to two types of notifications:</span></span> 

- <span data-ttu-id="c27c5-145">资源更改-Microsoft 团队中创建或更新的频道消息</span><span class="sxs-lookup"><span data-stu-id="c27c5-145">Resource changes - channel messages being created or updated in Microsoft Teams</span></span>
- <span data-ttu-id="c27c5-146">可能影响更改通知流的订阅生命周期事件。</span><span class="sxs-lookup"><span data-stu-id="c27c5-146">Subscription life cycle events which can affect the flow of change notifications.</span></span> <span data-ttu-id="c27c5-147">有关详细信息，请参阅[下一节](#subscription-life-cycle-notifications)中的生命周期通知。</span><span class="sxs-lookup"><span data-stu-id="c27c5-147">See more details about life cycle notifications in the [next section](#subscription-life-cycle-notifications).</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "lifecycleNotificationUrl": "https://webhook.azurewebsites.net/api/lifecycleNotifications",
  "resource": "/teams/{id}/channels/{id}/messages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="subscription-response"></a><span data-ttu-id="c27c5-148">订阅响应</span><span class="sxs-lookup"><span data-stu-id="c27c5-148">Subscription response</span></span>
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "lifecycleNotificationUrl": "https://webhook.azurewebsites.net/api/lifecycleNotifications",
  "resource": "/teams/{id}/channels/{id}/messages",
  "includeResourceData": true,
  "encryptionCertificateId": "{custom ID}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secret client state}"
}
```

## <a name="subscription-life-cycle-notifications"></a><span data-ttu-id="c27c5-149">订阅生命周期通知</span><span class="sxs-lookup"><span data-stu-id="c27c5-149">Subscription life cycle notifications</span></span>

<span data-ttu-id="c27c5-150">某些事件可能会干扰现有订阅中的正常通知流。</span><span class="sxs-lookup"><span data-stu-id="c27c5-150">Certain events can interfere with normal notification flow in an existing subscription.</span></span> <span data-ttu-id="c27c5-151">订阅_生命周期通知_将通知执行的操作，以保持无中断的流动。</span><span class="sxs-lookup"><span data-stu-id="c27c5-151">Subscription _life cycle notifications_ inform you actions to take in order to maintain an uninterrupted flow.</span></span> <span data-ttu-id="c27c5-152">不同于资源更改通知（用于通知资源实例），生命周期通知涉及订阅自身，和其在生命周期中的最新状态。</span><span class="sxs-lookup"><span data-stu-id="c27c5-152">Unlike a resource change notification which informs a change to a resource instance, a life cycle notification is about the subscription itself, and its current state in the life cycle.</span></span> 

<span data-ttu-id="c27c5-153">生命周期通知将传递到 **lifecycleNotificationUrl**。</span><span class="sxs-lookup"><span data-stu-id="c27c5-153">Life cycle notifications are delivered to the **lifecycleNotificationUrl**.</span></span> 

<span data-ttu-id="c27c5-154">本节内容：</span><span class="sxs-lookup"><span data-stu-id="c27c5-154">In this section:</span></span>

- [<span data-ttu-id="c27c5-155">质询订阅授权的生命周期通知</span><span class="sxs-lookup"><span data-stu-id="c27c5-155">Life cycle notification that challenges subscription authorization</span></span>](#life-cycle-notification-that-challenges-subscription-authorization)
- [<span data-ttu-id="c27c5-156">授权质询流</span><span class="sxs-lookup"><span data-stu-id="c27c5-156">Authorization challenge flow</span></span>](#authorization-challenge-flow)
- [<span data-ttu-id="c27c5-157">授权质询示例</span><span class="sxs-lookup"><span data-stu-id="c27c5-157">Example authorization challenge</span></span>](#example-authorization-challenge)
- [<span data-ttu-id="c27c5-158">授权质询响应</span><span class="sxs-lookup"><span data-stu-id="c27c5-158">Responding to an authorization challenge</span></span>](#responding-to-an-authorization-challenge)
- [<span data-ttu-id="c27c5-159">提示</span><span class="sxs-lookup"><span data-stu-id="c27c5-159">Tips</span></span>](#tips)
- [<span data-ttu-id="c27c5-160">代码应符合未来需要，以处理其它类型的生命周期通知</span><span class="sxs-lookup"><span data-stu-id="c27c5-160">Future-proof your code to handle other types of life cycle notifications</span></span>](#future-proof-your-code-to-handle-other-types-of-life-cycle-notifications)

### <a name="life-cycle-notification-that-challenges-subscription-authorization"></a><span data-ttu-id="c27c5-161">质询订阅授权的生命周期通知</span><span class="sxs-lookup"><span data-stu-id="c27c5-161">Life cycle notification that challenges subscription authorization</span></span>

<span data-ttu-id="c27c5-162">一种类型的活动订阅授权状态的生命周期通知质询。</span><span class="sxs-lookup"><span data-stu-id="c27c5-162">One type of life cycle notifications challenges the authorized state of an active subscription.</span></span> <span data-ttu-id="c27c5-163">当通知中的 **lifecycleEvent** 属性表示 `reauthorizationRequired`时，必须重新授权该订阅，以保持数据流。</span><span class="sxs-lookup"><span data-stu-id="c27c5-163">When the **lifecycleEvent** property in a notification indicates `reauthorizationRequired`, you must re-authorize the subscription to maintain the data flow.</span></span>

<span data-ttu-id="c27c5-164">创建长期订阅（例如，持续3天的订阅）时，资源数据通知将流动到 **notificationUrl**中的指定位置。</span><span class="sxs-lookup"><span data-stu-id="c27c5-164">When you create a long-lived subscription (for example, one that lasts for 3 days), resource data notifications flows to the location indicated in **notificationUrl**.</span></span> <span data-ttu-id="c27c5-165">但是，在任何时候，Microsoft Graph 可能要求您重新授权订阅，以证明自订阅创建起访问条件发生变化时，仍能访问资源数据。</span><span class="sxs-lookup"><span data-stu-id="c27c5-165">However, at any point in time, Microsoft Graph may require that you re-authorize the subscription to prove that you still have access to resource data, in case the conditions of access have changed since the subscription was created.</span></span> <span data-ttu-id="c27c5-166">下面是影响数据访问的更改示例：</span><span class="sxs-lookup"><span data-stu-id="c27c5-166">The following are examples of changes that affect your access to data:</span></span>

- <span data-ttu-id="c27c5-167">租户管理员可能会吊销应用程序读取资源的权限。</span><span class="sxs-lookup"><span data-stu-id="c27c5-167">A tenant administrator may revoke your app's permissions to read a resource.</span></span>
- <span data-ttu-id="c27c5-168">在交互方案中，向应用程序提供身份验证令牌的用户，可能会受限于基于多种因素的动态策略，如位置、设备状态或风险评估。</span><span class="sxs-lookup"><span data-stu-id="c27c5-168">In an interactive scenario, the user who provides the authentication token to your app may be subject to dynamic policies based on various factors, such as their location, device state, or risk assesment.</span></span> <span data-ttu-id="c27c5-169">例如，如果用户更改了物理位置，则该用户可能无法再访问该数据，并且应用程序无法重新授权订阅。</span><span class="sxs-lookup"><span data-stu-id="c27c5-169">For example, if the user changes their physical location, the user may no longer be allowed to access the data, and your app will not be able to re-authorize the subscription.</span></span> <span data-ttu-id="c27c5-170">有关控制访问的动态策略的详细信息，请参阅 [Azure AD 条件性访问策略](https://docs.microsoft.com/azure/active-directory/conditional-access/overview)。</span><span class="sxs-lookup"><span data-stu-id="c27c5-170">For more information on dynamic policies that control access, see [Azure AD conditional access policies](https://docs.microsoft.com/azure/active-directory/conditional-access/overview).</span></span> 

### <a name="authorization-challenge-flow"></a><span data-ttu-id="c27c5-171">授权质询流</span><span class="sxs-lookup"><span data-stu-id="c27c5-171">Authorization challenge flow</span></span>

<span data-ttu-id="c27c5-172">活动的、未过期订阅的授权质询流如下所示：</span><span class="sxs-lookup"><span data-stu-id="c27c5-172">The flow of an authorization challenge for an active, non-expired subscription looks as follows:</span></span>

1. <span data-ttu-id="c27c5-173">Microsoft Graph 需要重新授权的订阅</span><span class="sxs-lookup"><span data-stu-id="c27c5-173">Microsoft Graph requires a subscription to be re-authorized</span></span>
    
    <span data-ttu-id="c27c5-174">发生这种情况的原因可能随资源而异，可能随着时间推移而发生变化。</span><span class="sxs-lookup"><span data-stu-id="c27c5-174">The reasons for this may vary from resource to resource, and may change over time.</span></span> <span data-ttu-id="c27c5-175">无论重新授权事件的原因，都需要对其进行响应。</span><span class="sxs-lookup"><span data-stu-id="c27c5-175">Regardless of the cause of the re-authorization event, you will need to respond to it.</span></span>

2. <span data-ttu-id="c27c5-176">Microsoft Graph 向 **lifecycleNotificationUrl** 发送授权质询通知</span><span class="sxs-lookup"><span data-stu-id="c27c5-176">Microsoft Graph sends an authorization challenge notification to the **lifecycleNotificationUrl**</span></span>

    <span data-ttu-id="c27c5-177">请注意，资源通知流可能持续一段时间，为你提供额外的响应时间。</span><span class="sxs-lookup"><span data-stu-id="c27c5-177">Note that the flow of resource notifications may continue for a while, giving you extra time to respond.</span></span> <span data-ttu-id="c27c5-178">但是资源通知传递将最终暂停，直至执行了所需操作。</span><span class="sxs-lookup"><span data-stu-id="c27c5-178">However, eventually resource notification delivery will pause, until you take the required action.</span></span>

3. <span data-ttu-id="c27c5-179">采用以下两种方法之一来响应此通知：</span><span class="sxs-lookup"><span data-stu-id="c27c5-179">Respond to this notification in one of two ways:</span></span>
    1. <span data-ttu-id="c27c5-180">重新授权订阅。</span><span class="sxs-lookup"><span data-stu-id="c27c5-180">Re-authorize the subscription.</span></span> <span data-ttu-id="c27c5-181">这不会延长订阅的到期日期。</span><span class="sxs-lookup"><span data-stu-id="c27c5-181">This does not extend the expiry date of the subscription.</span></span>
    2. <span data-ttu-id="c27c5-182">续订订阅。</span><span class="sxs-lookup"><span data-stu-id="c27c5-182">Renew the subscription.</span></span> <span data-ttu-id="c27c5-183">这将重新授权并延长到期日期。</span><span class="sxs-lookup"><span data-stu-id="c27c5-183">This both re-authorizes and extends the expiry date.</span></span>

    <span data-ttu-id="c27c5-184">注意：两项操作都要求提供有效的身份验证令牌，类似于[新建订阅](webhooks.md#creating-a-subscription)或[到期前续订订阅](webhooks.md#renewing-a-subscription)。</span><span class="sxs-lookup"><span data-stu-id="c27c5-184">Note: Both actions require you to present a valid authentication token, similar to [creating a new subscription](webhooks.md#creating-a-subscription) or [renewing a subscription before its expiry](webhooks.md#renewing-a-subscription).</span></span>

4. <span data-ttu-id="c27c5-185">如果成功重新授权或续订订阅，资源通知将继续。</span><span class="sxs-lookup"><span data-stu-id="c27c5-185">If you successfully re-authorize or renew the subscription, resource notifications continue.</span></span> <span data-ttu-id="c27c5-186">否则，资源通知保持暂停。</span><span class="sxs-lookup"><span data-stu-id="c27c5-186">Otherwise, resource notifications remain paused.</span></span>
    
### <a name="example-authorization-challenge"></a><span data-ttu-id="c27c5-187">授权质询示例</span><span class="sxs-lookup"><span data-stu-id="c27c5-187">Example authorization challenge</span></span>

<span data-ttu-id="c27c5-188">下面是需要重新授权订阅的生命周期示例。</span><span class="sxs-lookup"><span data-stu-id="c27c5-188">Below is an example life cycle notification that requests re-authorizing a subscription.</span></span> 

<span data-ttu-id="c27c5-189">请注意以下几点：</span><span class="sxs-lookup"><span data-stu-id="c27c5-189">Note the following:</span></span>

- <span data-ttu-id="c27c5-190">"`"lifecycleEvent": "reauthorizationRequired"`" 字段将通知标识为授权质询。</span><span class="sxs-lookup"><span data-stu-id="c27c5-190">The `"lifecycleEvent": "reauthorizationRequired"` field identifies this notification as an authorization challenge.</span></span>
- <span data-ttu-id="c27c5-191">通知不包含有关特定资源的任何信息，因为它与资源更改无关，而与订阅状态更改有关。</span><span class="sxs-lookup"><span data-stu-id="c27c5-191">The notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="c27c5-192">与资源通知类似，可以共同对生命周期通知进行批处理（**值**集），各通知可能有不同的**lifecycleEvent**值。</span><span class="sxs-lookup"><span data-stu-id="c27c5-192">Similar to resource notifications, you can batch life cycle notifications together (in the **value** collection), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="c27c5-193">相应地批处理每个通知。</span><span class="sxs-lookup"><span data-stu-id="c27c5-193">Process each notification in the batch accordingly.</span></span>

```json
{
  "value": [
    {
      "lifecycleEvent": "reauthorizationRequired",
      "subscriptionId": "e3898f08-5cd0-4a6a-80fc-6addbfb73b7b",
      "subscriptionExpirationDateTime": "2019-09-18T00:52:45.9696658+00:00",
      "clientState": "{secret client state}",
      "tenantId": "84bd8158-6d4d-4958-8b9f-9d6445542f95"
    }
  ]
}
```

### <a name="responding-to-an-authorization-challenge"></a><span data-ttu-id="c27c5-194">授权质询响应</span><span class="sxs-lookup"><span data-stu-id="c27c5-194">Responding to an authorization challenge</span></span>

<span data-ttu-id="c27c5-195">执行以下步骤以处理授权质询生命周期通知。</span><span class="sxs-lookup"><span data-stu-id="c27c5-195">Take the following steps to process an authorization challenge life cycle notification.</span></span> <span data-ttu-id="c27c5-196">确认和验证生命周期通知的前两步与 [响应资源更改通知](webhooks.md#processing-the-notification)类似。</span><span class="sxs-lookup"><span data-stu-id="c27c5-196">The first two steps of acknowledging and validating the life cycle notification is similar to [responding to a resource change notification](webhooks.md#processing-the-notification).</span></span>

1. <span data-ttu-id="c27c5-197">通过使用 `HTTP 202 Accepted`来响应 POST 调用，确认收到通知。</span><span class="sxs-lookup"><span data-stu-id="c27c5-197">Acknowledge the receipt of the notification, by responding to the POST call with `HTTP 202 Accepted`.</span></span>
2. <span data-ttu-id="c27c5-198">验证通知的真实性。</span><span class="sxs-lookup"><span data-stu-id="c27c5-198">Validate the authenticity of the notification.</span></span> <span data-ttu-id="c27c5-199">更多详情参见[下列内容](#validating-the-authenticity-of-notifications)。</span><span class="sxs-lookup"><span data-stu-id="c27c5-199">Further details [below](#validating-the-authenticity-of-notifications).</span></span>
3. <span data-ttu-id="c27c5-200">确保应用程序具有执行下一步的有效的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="c27c5-200">Ensure the app has a valid access token to take the next step.</span></span> 

    <span data-ttu-id="c27c5-201">如果正在使用一个[身份验证库](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries)，则库会通过重用有效的缓存令牌，或通过提示用户使用新密码再次登录，来处理此问题。</span><span class="sxs-lookup"><span data-stu-id="c27c5-201">If you are using one of the [authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries), the library handles this for you by either reusing a valid cached token, or obtaining a new token from prompting the user to log in again with a new password.</span></span> <span data-ttu-id="c27c5-202">但是，获得新的令牌可能会失败，因为存取条件可能已更改，用户可能不再被允许访问资源数据。</span><span class="sxs-lookup"><span data-stu-id="c27c5-202">However, obtaining a new token may fail, since the conditions of access may have changed, and the user may no longer be allowed access to the resource data.</span></span>

4. <span data-ttu-id="c27c5-203">调用下列两个API中的任意一个。</span><span class="sxs-lookup"><span data-stu-id="c27c5-203">Call either of the following two APIs.</span></span> <span data-ttu-id="c27c5-204">如果 API 调用成功，则资源通知流将继续。</span><span class="sxs-lookup"><span data-stu-id="c27c5-204">If the API call succeeds, the resource notification flow resumes.</span></span>

    - <span data-ttu-id="c27c5-205">调用`/reauthorize`操作以重新批准订阅，但不延长到期日期：</span><span class="sxs-lookup"><span data-stu-id="c27c5-205">Call the `/reauthorize` action to re-authorize the subscription without extending its expiration date:</span></span>
        ```http
        POST  https://graph.microsoft.com/beta/subscriptions/{id}/reauthorize
        Content-type: application/json
        ```
    - <span data-ttu-id="c27c5-206">执行定期续订操作，以同时进行重新授权和续订：</span><span class="sxs-lookup"><span data-stu-id="c27c5-206">Perform a regular renew action to re-authorize and renew the subscription at the same time:</span></span>
        ```http
        PATCH https://graph.microsoft.com/beta/subscriptions/{id}
        Content-Type: application/json

        {
           "expirationDateTime": "2019-09-21T11:00:00.0000000Z"
        }
        ```

      <span data-ttu-id="c27c5-207">续订可能会失败，因为系统执行的授权检查可能会拒绝应用程序或用户对资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="c27c5-207">Renewing may fail, because the authorization checks performed by the system may deny the app or the user access to the resource.</span></span> <span data-ttu-id="c27c5-208">应用程序可能需要从用户获取新的访问令牌以成功重新授权订阅。</span><span class="sxs-lookup"><span data-stu-id="c27c5-208">It may be necessary for the app to obtain a new access token from the user to successfully re-authorize a subscription.</span></span> 
      
      <span data-ttu-id="c27c5-209">以后可以随时重试这些操作，例如访问条件发生变化时。</span><span class="sxs-lookup"><span data-stu-id="c27c5-209">You may retry these actions later, at any time, and succeed if the conditions of access change.</span></span> <span data-ttu-id="c27c5-210">生命周期通知发送时至应用程序最终成功重新创建订阅时之间的，有关资源更改的任何通知将丢失。</span><span class="sxs-lookup"><span data-stu-id="c27c5-210">Any notifications about resource changes that happen between the time the life cycle notification was sent, and the time when the app eventually re-creates the subscription successfully, would be lost.</span></span> <span data-ttu-id="c27c5-211">在这种情况下，应用程序应单独获取这些更改。</span><span class="sxs-lookup"><span data-stu-id="c27c5-211">In such cases, the app should separately fetch those changes.</span></span>

### <a name="tips"></a><span data-ttu-id="c27c5-212">提示</span><span class="sxs-lookup"><span data-stu-id="c27c5-212">Tips</span></span>

<span data-ttu-id="c27c5-213">请注意下列事项：</span><span class="sxs-lookup"><span data-stu-id="c27c5-213">Keep the following in mind:</span></span>

1. <span data-ttu-id="c27c5-214">授权质询不会替代到期前续订资源更改通知的需要。</span><span class="sxs-lookup"><span data-stu-id="c27c5-214">Authorization challenges do not replace the need to renew a resource change subscription before it expires.</span></span> 

    <span data-ttu-id="c27c5-215">虽然可以选择在收到授权质询时续订订阅，但 Microsoft Graph 可能不会对所有订阅进行质询。</span><span class="sxs-lookup"><span data-stu-id="c27c5-215">While you can choose to renew a subscription when you receive an authorization challenge, Microsoft Graph may not challenge all of your subscriptions.</span></span> <span data-ttu-id="c27c5-216">例如，没有任何活动且没有资源通知挂起传递的订阅，不表示对应用程序有任何重新授权质询。</span><span class="sxs-lookup"><span data-stu-id="c27c5-216">For example, a subscription that does not have any activity and has no resource notifications pending delivery may not signal any re-authorization challenges to your app.</span></span> <span data-ttu-id="c27c5-217">请务必在订阅到期前 [续订订阅](webhooks.md#renewing-a-subscription)。</span><span class="sxs-lookup"><span data-stu-id="c27c5-217">Make sure to [renew subscriptions](webhooks.md#renewing-a-subscription) before they expire.</span></span>

2. <span data-ttu-id="c27c5-218">授权质询的频率可能会发生更改。</span><span class="sxs-lookup"><span data-stu-id="c27c5-218">The frequency of authorization challenges is subject to change.</span></span>

    <span data-ttu-id="c27c5-219">不要对授权质询频率进行假设。</span><span class="sxs-lookup"><span data-stu-id="c27c5-219">Do not make assumptions about the frequency of authorization challenges.</span></span> <span data-ttu-id="c27c5-220">这些通知会告诉你执行操作的时间，无需跟踪需要重新授权的订阅。</span><span class="sxs-lookup"><span data-stu-id="c27c5-220">These notifications tell you when to take actions, saving you from having to track which subscriptions require re-authorization.</span></span> <span data-ttu-id="c27c5-221">准备好每隔几分钟处理每个订阅的授权质询，极少情况下，只针对部分订阅。</span><span class="sxs-lookup"><span data-stu-id="c27c5-221">Be ready to handle authorization challenges anywhere from once a few minutes for every subscription, to rarely for only some of your subscriptions.</span></span>

### <a name="future-proof-your-code-to-handle-other-types-of-life-cycle-notifications"></a><span data-ttu-id="c27c5-222">代码应符合未来需要，以处理其它类型的生命周期通知</span><span class="sxs-lookup"><span data-stu-id="c27c5-222">Future-proof your code to handle other types of life cycle notifications</span></span>

<span data-ttu-id="c27c5-223">预计发布至 **lifecycleNotificationUrl** 指定相同终结点的订阅生命周期。</span><span class="sxs-lookup"><span data-stu-id="c27c5-223">Expect subscription life cycle notifications to be posted to the same endpoint specified by **lifecycleNotificationUrl**.</span></span> <span data-ttu-id="c27c5-224">它们通过 **lifecycleEvent** 属性进行区分，可能包含略微不同的架构和属性，以提供它们所解决的方案。</span><span class="sxs-lookup"><span data-stu-id="c27c5-224">They differentiate by the **lifecycleEvent** property and may contain slightly different schema and properties to serve the scenarios they address.</span></span>

<span data-ttu-id="c27c5-225">预期新的生命周期通知类型时实现代码：</span><span class="sxs-lookup"><span data-stu-id="c27c5-225">Implement your code in anticipation of new types of life cycle notifications:</span></span>

1. <span data-ttu-id="c27c5-226">使用 **lifecycleEvent** 属性标识通知类型，以确定相应的响应。</span><span class="sxs-lookup"><span data-stu-id="c27c5-226">Use the **lifecycleEvent** property to identify the type of notification so to determine the appropriate response.</span></span> <span data-ttu-id="c27c5-227">例如，查找 `"lifecycleEvent": "reauthorizationRequired"` 属性标识特定事件并处理它。</span><span class="sxs-lookup"><span data-stu-id="c27c5-227">For example, look for the `"lifecycleEvent": "reauthorizationRequired"` property to identify a specific event, and handle it.</span></span>

1. <span data-ttu-id="c27c5-228">记录应用程序无法识别获得认知的生命周期事件。</span><span class="sxs-lookup"><span data-stu-id="c27c5-228">Log any life cycle events that your app does not recognize to gain awareness.</span></span>

1. <span data-ttu-id="c27c5-229">订阅 [的 Microsoft Graph 开发人员博客](https://developer.microsoft.com/graph/blogs/)，以监视新方案的生命周期通知的公告。</span><span class="sxs-lookup"><span data-stu-id="c27c5-229">Subscribe to the [Microsoft Graph Developer Blog](https://developer.microsoft.com/graph/blogs/) to watch for announcements of life cycle notifications for new scenarios.</span></span>

1. <span data-ttu-id="c27c5-230">可以自行决定查找新生命周期通知的相关文档，并根据需要提供支持。</span><span class="sxs-lookup"><span data-stu-id="c27c5-230">Look up related documentation for new life cycle notifications and implement support for them as appropriate.</span></span>

## <a name="validating-the-authenticity-of-notifications"></a><span data-ttu-id="c27c5-231">正在验证通知的真实性</span><span class="sxs-lookup"><span data-stu-id="c27c5-231">Validating the authenticity of notifications</span></span>

<span data-ttu-id="c27c5-232">应用程序通常执行基于通知中所包含资源数据的商业逻辑。</span><span class="sxs-lookup"><span data-stu-id="c27c5-232">Apps often execute business logic based on resource data included in notifications.</span></span> <span data-ttu-id="c27c5-233">首先验证每个通知的真实性非常重要。</span><span class="sxs-lookup"><span data-stu-id="c27c5-233">Having first verified the authenticity of each notification is important.</span></span> <span data-ttu-id="c27c5-234">此外，第三方可以通过错误通知来欺骗应用程序，使其正确地执行业务逻辑，并导致安全事件发生。</span><span class="sxs-lookup"><span data-stu-id="c27c5-234">Otherwise, a third party could spoof your app with false notifications, make it execute its business logic incorrectly, and lead to a security incident.</span></span>

<span data-ttu-id="c27c5-235">对于不包含资源数据的基本通知，只需根据 **clientState** 值进行验证，具体如[此处](webhooks.md#processing-the-notification)所述。</span><span class="sxs-lookup"><span data-stu-id="c27c5-235">For basic notifications which do not contain resource data, simply validate them based on the **clientState** value as described [here](webhooks.md#processing-the-notification).</span></span> <span data-ttu-id="c27c5-236">这是可以接受的，因为可以进行后续调用受信任的 Microsoft Graph 来访问资源数据，因此，任何尝试欺骗的影响都是有限的。</span><span class="sxs-lookup"><span data-stu-id="c27c5-236">This is acceptable, as you can make subsequent trusted Microsoft Graph calls to get access to resource data, and therefore the impact of any spoofing attempts is limited.</span></span> 

<span data-ttu-id="c27c5-237">对于传递资源数据的通知，请在处理数据之前执行更全面的验证。</span><span class="sxs-lookup"><span data-stu-id="c27c5-237">For notifications that deliver resource data, perform a more thorough validation before processing the data.</span></span>

<span data-ttu-id="c27c5-238">本节内容：</span><span class="sxs-lookup"><span data-stu-id="c27c5-238">In this section:</span></span>

- [<span data-ttu-id="c27c5-239">通知验证令牌</span><span class="sxs-lookup"><span data-stu-id="c27c5-239">Validation tokens in the notification</span></span>](#validation-tokens-in-the-notification)
- [<span data-ttu-id="c27c5-240">如何验证</span><span class="sxs-lookup"><span data-stu-id="c27c5-240">How to validate</span></span>](#how-to-validate)
- [<span data-ttu-id="c27c5-241"> JWT 令牌示例</span><span class="sxs-lookup"><span data-stu-id="c27c5-241">Example JWT token</span></span>](#example-jwt-token)

### <a name="validation-tokens-in-the-notification"></a><span data-ttu-id="c27c5-242">通知验证令牌</span><span class="sxs-lookup"><span data-stu-id="c27c5-242">Validation tokens in the notification</span></span>

<span data-ttu-id="c27c5-243">包含资源数据的通知，含有附加属性 **validationTokens**，该属性包含由Microsoft Graph 生成的 JWT 令牌数组。</span><span class="sxs-lookup"><span data-stu-id="c27c5-243">A notification with resource data contains an additional property, **validationTokens**, which contains an array of JWT tokens generated by Microsoft Graph.</span></span> <span data-ttu-id="c27c5-244">Microsoft Graph 将为每个不同的应用和在**值**数组中有项的租户对，生成单独的令牌。</span><span class="sxs-lookup"><span data-stu-id="c27c5-244">Microsoft Graph generates a single token for each distinct app and tenant pair for whom there is an item in the **value** array.</span></span> <span data-ttu-id="c27c5-245">请记住，通知可能包含使用同一 **notificationUrl**订阅的各种应用和租户的混合项。</span><span class="sxs-lookup"><span data-stu-id="c27c5-245">Keep in mind that notifications may contain a mix of items for various apps and tenants that subscribed using the same **notificationUrl**.</span></span>

<span data-ttu-id="c27c5-246">在下面示例中，通知针对相同应用和两个不同租户包含两个项，因此 **validationTokens** 数组中包含两个需要验证的令牌。</span><span class="sxs-lookup"><span data-stu-id="c27c5-246">In the following example, the notification contains two items for the same app, and for two different tenants, therefore the **validationTokens** array contains two tokens that need to be validated.</span></span>

```json
{
    "value": [
          {
            "subscriptionId": "76619225-ff6b-4489-96ca-4ef547e78b22",
      "tenantId": "84bd8158-6d4d-4958-8b9f-9d6445542f95",
            "changeType": "created",
            ...
          },
      {
            "subscriptionId": "e990d58f-fd93-40af-acf7-a7c907c5d8ea",
      "tenantId": "46d9e3bd-6309-4177-a016-b256a411e30f",
            "changeType": "created",
            ...
            }
    ],
    "validationTokens": [
        "eyJ0eXAiOiJKV1QiLCJhb...",
    "cGlkYWNyIjoiMiIsImlkc..."
    ]
}
```
### <a name="how-to-validate"></a><span data-ttu-id="c27c5-247">如何验证</span><span class="sxs-lookup"><span data-stu-id="c27c5-247">How to validate</span></span>

<span data-ttu-id="c27c5-248">如果没有使用过令牌验证，请参阅本 [博客文章](http://www.cloudidentity.com/blog/2014/03/03/principles-of-token-validation/)，了解有用的概述信息。</span><span class="sxs-lookup"><span data-stu-id="c27c5-248">If you are new to token validation, refer to this [blog article](http://www.cloudidentity.com/blog/2014/03/03/principles-of-token-validation/) for a useful overview.</span></span> <span data-ttu-id="c27c5-249">使用SDK，例如Microsoft的用于.NET的 [System.IdentityModel.Tokens.Jwt](https://www.nuget.org/packages/System.IdentityModel.Tokens.Jwt/)库，或用于其它平台的第三方库。</span><span class="sxs-lookup"><span data-stu-id="c27c5-249">Use an SDK, such as Microsoft's [System.IdentityModel.Tokens.Jwt](https://www.nuget.org/packages/System.IdentityModel.Tokens.Jwt/) library for .NET, or a third party library for a different platform.</span></span>

<span data-ttu-id="c27c5-250">注意以下事项：</span><span class="sxs-lookup"><span data-stu-id="c27c5-250">Be mindful of the following:</span></span> 

- <span data-ttu-id="c27c5-251">确保始终发送`HTTP 202 Accepted`状态代码作为通知响应的一部分。</span><span class="sxs-lookup"><span data-stu-id="c27c5-251">Make sure to always send an `HTTP 202 Accepted` status code as part of the response to the notification.</span></span> 
- <span data-ttu-id="c27c5-252">验证通知前，请执行此操作（例如存储通知至队列中以供后续处理）或在验证后执行操作（如果即时处理了通知），即使验证失败。</span><span class="sxs-lookup"><span data-stu-id="c27c5-252">Do that before validating the notification (for example, if you store notifications in queues for later processing) or after (if you process them on the fly), even if validation failed.</span></span>
- <span data-ttu-id="c27c5-253">接受通知可以防止不必要的传递重试，还可以防止任何潜在的恶意行为者发现他们是否通过验证。</span><span class="sxs-lookup"><span data-stu-id="c27c5-253">Accepting a notification prevents unnecessary delivery retries and it also prevents any potential rogue actors from finding out if they passed or failed validation.</span></span> <span data-ttu-id="c27c5-254">可随时在接受后选择忽略无效的通知。</span><span class="sxs-lookup"><span data-stu-id="c27c5-254">You can always choose to ignore an invalid notification after you have accepted it.</span></span>

<span data-ttu-id="c27c5-255">具体而言，针对**validationTokens**集中各JWT令牌进行验证。</span><span class="sxs-lookup"><span data-stu-id="c27c5-255">In particular, perform validation on every JWT token in the **validationTokens** collection.</span></span> <span data-ttu-id="c27c5-256">如果任何令牌失败，请考虑通知可疑并进一步调查。</span><span class="sxs-lookup"><span data-stu-id="c27c5-256">If any tokens fail, consider the notification suspicious and investigate further.</span></span> 

<span data-ttu-id="c27c5-257">使用下列步骤验证令牌和生成令牌的应用程序：</span><span class="sxs-lookup"><span data-stu-id="c27c5-257">Use the following steps to validate tokens and apps that generate tokens:</span></span>

1. <span data-ttu-id="c27c5-258">验证令牌是否未过期。</span><span class="sxs-lookup"><span data-stu-id="c27c5-258">Validate that the token has not expired.</span></span>

2. <span data-ttu-id="c27c5-259">验证令牌未被篡改，并且由预期机构（Microsoft Azure Active Directory）颁发：</span><span class="sxs-lookup"><span data-stu-id="c27c5-259">Validate the token has not been tampered with and was issued by the expected authority, Microsoft Azure Active Directory:</span></span>

    - <span data-ttu-id="c27c5-260">从公用配置终结点获取签名密钥：`https://login.microsoftonline.com/common/.well-known/openid-configuration`。</span><span class="sxs-lookup"><span data-stu-id="c27c5-260">Obtain the signing keys from the common configuration endpoint: `https://login.microsoftonline.com/common/.well-known/openid-configuration`.</span></span> <span data-ttu-id="c27c5-261">此配置由应用程序缓存一段时间。</span><span class="sxs-lookup"><span data-stu-id="c27c5-261">This configuration is cached by your app for a period of time.</span></span> <span data-ttu-id="c27c5-262">请注意，由于签名密钥每日都会轮换，因此配置会经常更新。</span><span class="sxs-lookup"><span data-stu-id="c27c5-262">Be aware that the configuration is updated frequently as signing keys are rotated daily.</span></span>
    - <span data-ttu-id="c27c5-263">使用这些密钥验证 JWT 令牌的签名。</span><span class="sxs-lookup"><span data-stu-id="c27c5-263">Verify the signature of the JWT token using those keys.</span></span>

    <span data-ttu-id="c27c5-264">不要接受任何其他机构颁发的令牌。</span><span class="sxs-lookup"><span data-stu-id="c27c5-264">Do not accept tokens issued by any other authority.</span></span>

3. <span data-ttu-id="c27c5-265">验证口令已为订阅更改通知的应用程序颁发。</span><span class="sxs-lookup"><span data-stu-id="c27c5-265">Validate that the token was issued for your app that is subscribing to change notifications.</span></span>

    <span data-ttu-id="c27c5-266">下列步骤是 JWT 令牌库中标准验证逻辑的一部分，通常可作为单个函数调用执行。</span><span class="sxs-lookup"><span data-stu-id="c27c5-266">The following steps are part of standard validation logic in JWT token libraries and can typically be executed as a single function call.</span></span> 
    - <span data-ttu-id="c27c5-267">在与应用程序ID匹配的令牌中验证“受众”。</span><span class="sxs-lookup"><span data-stu-id="c27c5-267">Validate the "audience" in the token matches your app ID.</span></span>
    - <span data-ttu-id="c27c5-268">如果有多个应用收到通知，请务必检查是否有多个 ID。</span><span class="sxs-lookup"><span data-stu-id="c27c5-268">If you have more than one app receiving notifications, make sure to check for multiple IDs.</span></span>


4. <span data-ttu-id="c27c5-269">**关键**：验证生成令牌的应用程序是否代表着 Microsoft Graph 更改通知的发布者。</span><span class="sxs-lookup"><span data-stu-id="c27c5-269">**Critical**: Validate that the app that generated the token represents the Microsoft Graph change notification publisher.</span></span> 

    - <span data-ttu-id="c27c5-270">在与 `0bf30f3b-4a52-48df-9a82-234910c4a086`期望值匹配的令牌中检查 **appid** 属性。</span><span class="sxs-lookup"><span data-stu-id="c27c5-270">Check that the **appid** property in the token matches the expected value of `0bf30f3b-4a52-48df-9a82-234910c4a086`.</span></span>
    - <span data-ttu-id="c27c5-271">这可确保通知不是由不是 Microsoft Graph 的其它应用程序发送。</span><span class="sxs-lookup"><span data-stu-id="c27c5-271">This ensures that notifications are not sent by a different app that is not Microsoft Graph.</span></span>


### <a name="example-jwt-token"></a><span data-ttu-id="c27c5-272">JWT 令牌示例</span><span class="sxs-lookup"><span data-stu-id="c27c5-272">Example JWT token</span></span>

<span data-ttu-id="c27c5-273">下面是验证所需的 JWT 令牌中所含属性的示例：</span><span class="sxs-lookup"><span data-stu-id="c27c5-273">Here is an example of the properties included in the JWT token that are needed for validation:</span></span>

```json
{
  // aud is your app's id 
  "aud": "8e460676-ae3f-4b1e-8790-ee0fb5d6148f",                           
  "iss": "https://sts.windows.net/84bd8158-6d4d-4958-8b9f-9d6445542f95/",
  "iat": 1565046813,
  "nbf": 1565046813,
  // Expiration date 
  "exp": 1565075913,                                                        
  "aio": "42FgYKhZ+uOZrHa7p+7tfruauq1HAA==",
  // appid represents the notification publisher and must always be the same value of 0bf30f3b-4a52-48df-9a82-234910c4a086 
  "appid": "0bf30f3b-4a52-48df-9a82-234910c4a086",                          
  "appidacr": "2",
  "idp": "https://sts.windows.net/84bd8158-6d4d-4958-8b9f-9d6445542f95/",
  "tid": "84bd8158-6d4d-4958-8b9f-9d6445542f95",
  "uti": "-KoJHevhgEGnN4kwuixpAA",
  "ver": "1.0"
}
```

### <a name="example-verifying-validation-tokens"></a><span data-ttu-id="c27c5-274">示例：对验证令牌进行验证</span><span class="sxs-lookup"><span data-stu-id="c27c5-274">Example: Verifying validation tokens</span></span>

```csharp
// add Microsoft.IdentityModel.Protocols.OpenIdConnect and System.IdentityModel.Tokens.Jwt nuget packages to your project
public async Task<bool> ValidateToken(string token, string tenantId, IEnumerable<string> appIds)
{
    var configurationManager = new ConfigurationManager<OpenIdConnectConfiguration>("https://login.microsoftonline.com/common/.well-known/openid-configuration", new OpenIdConnectConfigurationRetriever());
    var openIdConfig = await configurationManager.GetConfigurationAsync();
    var handler = new JwtSecurityTokenHandler();
    try
    {
    handler.ValidateToken(token, new TokenValidationParameters
    {
        ValidateIssuer = true,
        ValidateAudience = true,
        ValidateIssuerSigningKey = true,
        ValidateLifetime = true,
        ValidIssuer = $"https://sts.windows.net/{tenantId}/",
        ValidAudiences = appIds,
        IssuerSigningKeys = openIdConfig.SigningKeys
    }, out _);
    return true;
    }
    catch (Exception ex)
    {
    Trace.TraceError($"{ex.Message}:{ex.StackTrace}");
    return false;
    }
}
```
```java
private boolean IsValidationTokenValid(String[] appIds, String tenantId, String serializedToken) {
    try {
        JwkKeyResolver jwksResolver = new JwkKeyResolver();
        Jws<Claims> token = Jwts.parserBuilder()
        .setSigningKeyResolver(jwksResolver)
        .build()
        .parseClaimsJws(serializedToken);
        Claims body = token.getBody();
        String audience = body.getAudience();
        boolean isAudienceValid = false;
        for(String appId : appIds) {
        isAudienceValid = isAudienceValid || appId.equals(audience);
        }
        boolean isTenantValid = body.getIssuer().endsWith(tenantId + "/");
        return isAudienceValid  && isTenantValid; //nbf,exp and signature are already validated by library
    } catch (Exception e) {
        LOGGER.error("could not validate token");
        LOGGER.error(e.getMessage());
        return false;
    }
}
```
<span data-ttu-id="c27c5-275">还必须实现 `JwkKeyResolver`，这样 Java 示例才能正常运行。</span><span class="sxs-lookup"><span data-stu-id="c27c5-275">For the Java sample to work, you will also need to implement the `JwkKeyResolver`.</span></span>  
```java
package com.example.restservice;

import com.auth0.jwk.JwkProvider;
import com.auth0.jwk.UrlJwkProvider;
import com.auth0.jwk.Jwk;
import io.jsonwebtoken.Claims;
import io.jsonwebtoken.JwsHeader;
import io.jsonwebtoken.SigningKeyResolverAdapter;
import java.security.Key;
import java.net.URI;
import org.slf4j.Logger;
import org.slf4j.LoggerFactory;

public class JwkKeyResolver extends SigningKeyResolverAdapter {
    private JwkProvider keyStore;
    private final Logger LOGGER = LoggerFactory.getLogger(this.getClass());
    public JwkKeyResolver() throws java.net.URISyntaxException, java.net.MalformedURLException {
        this.keyStore = new UrlJwkProvider((new URI("https://login.microsoftonline.com/common/discovery/keys").toURL()));
    }
    @Override
    public Key resolveSigningKey(JwsHeader jwsHeader, Claims claims) {
        try {
            String keyId = jwsHeader.getKeyId();
            Jwk pub = keyStore.get(keyId);
            return pub.getPublicKey();
        } catch (Exception e) {
            LOGGER.error(e.getMessage());
            return null;
        }
    }
}
```

## <a name="decrypting-resource-data-from-change-notifications"></a><span data-ttu-id="c27c5-276">解密更改通知资源数据</span><span class="sxs-lookup"><span data-stu-id="c27c5-276">Decrypting resource data from change notifications</span></span>

<span data-ttu-id="c27c5-277">通知的 **resourceData** 属性仅包含资源实例的基本 ID 和类型信息。</span><span class="sxs-lookup"><span data-stu-id="c27c5-277">The **resourceData** property of a notification includes only the basic ID and type information of a resource instance.</span></span> <span data-ttu-id="c27c5-278">**encryptedData**属性包含由 Microsoft Graph 使用订阅中所提供密钥解密的完整资源数据。</span><span class="sxs-lookup"><span data-stu-id="c27c5-278">The **encryptedData** property contains the full resource data, encrypted by Microsoft Graph using the public key provided in the subscription.</span></span> <span data-ttu-id="c27c5-279">此属性还含有验证和解密所需的数值。</span><span class="sxs-lookup"><span data-stu-id="c27c5-279">The property also contains values required for verification and decryption.</span></span> <span data-ttu-id="c27c5-280">这样是为了保证通过通知访问客户数据的安全性。</span><span class="sxs-lookup"><span data-stu-id="c27c5-280">This is done to increase the security of customer data accessed via notifications.</span></span> <span data-ttu-id="c27c5-281">您有责任保护私钥，确保客户数据不能由第三方解密，即使他们设法截取原始通知。</span><span class="sxs-lookup"><span data-stu-id="c27c5-281">It is your responsibility to secure the private key to ensure that customer data cannot be decrypted by a third party, even if they manage to intercept the original notifications.</span></span>

<span data-ttu-id="c27c5-282">本节内容：</span><span class="sxs-lookup"><span data-stu-id="c27c5-282">In this section:</span></span>

- [<span data-ttu-id="c27c5-283">管理加密密钥</span><span class="sxs-lookup"><span data-stu-id="c27c5-283">Managing encryption keys</span></span>](#managing-encryption-keys)
- [<span data-ttu-id="c27c5-284">解密资源数据</span><span class="sxs-lookup"><span data-stu-id="c27c5-284">Decrypting resource data</span></span>](#decrypting-resource-data)
- [<span data-ttu-id="c27c5-285">示例：使用加密资源数据解密通知</span><span class="sxs-lookup"><span data-stu-id="c27c5-285">Example: decrypting a notification with encrypted resource data</span></span>](#example-decrypting-a-notification-with-encrypted-resource-data)

### <a name="managing-encryption-keys"></a><span data-ttu-id="c27c5-286">管理加密密钥</span><span class="sxs-lookup"><span data-stu-id="c27c5-286">Managing encryption keys</span></span>

1. <span data-ttu-id="c27c5-287">使用非对称密钥对获取证书。</span><span class="sxs-lookup"><span data-stu-id="c27c5-287">Obtain a certificate with a pair of asymmetric keys.</span></span>

    - <span data-ttu-id="c27c5-288">可自行对证书进行签名，因为 Microsoft Graph 不会验证证书颁发者，并且仅将公共密钥用于加密。</span><span class="sxs-lookup"><span data-stu-id="c27c5-288">You can self-sign the certificate, since Microsoft Graph does not verify the certificate issuer, and uses the public key for only encryption.</span></span> 
    - <span data-ttu-id="c27c5-289">使用[Azure 密钥存储库](https://docs.microsoft.com/azure/key-vault/key-vault-whatis)作为创建、轮换和安全管理证书的解决方案。</span><span class="sxs-lookup"><span data-stu-id="c27c5-289">Use [Azure Key Vault](https://docs.microsoft.com/azure/key-vault/key-vault-whatis) as the solution to create, rotate, and securely manage certificates.</span></span> <span data-ttu-id="c27c5-290">确保密钥符合下列条件：</span><span class="sxs-lookup"><span data-stu-id="c27c5-290">Make sure the keys satisfy the following criteria:</span></span>

        - <span data-ttu-id="c27c5-291">密钥必须属于类型 `RSA`</span><span class="sxs-lookup"><span data-stu-id="c27c5-291">The key must be of type `RSA`</span></span>
        - <span data-ttu-id="c27c5-292">密钥大小必须在2048和4096位之间。</span><span class="sxs-lookup"><span data-stu-id="c27c5-292">The key size must be between 2048 and 4096 bits</span></span>

2. <span data-ttu-id="c27c5-293">采用base64编码X.509格式导出证书，且**仅包括公钥**。</span><span class="sxs-lookup"><span data-stu-id="c27c5-293">Export the certificate in base64-encoded X.509 format, and **include only the public key**.</span></span> 

3. <span data-ttu-id="c27c5-294">创建订阅时：</span><span class="sxs-lookup"><span data-stu-id="c27c5-294">When creating a subscription:</span></span>

    - <span data-ttu-id="c27c5-295">使用导入证书的base64基编码内容，在**encryptionCertificate**属性中提供证书。</span><span class="sxs-lookup"><span data-stu-id="c27c5-295">Provide the certificate in the **encryptionCertificate** property, using the base64-encoded content that the certificate was exported in.</span></span>
    - <span data-ttu-id="c27c5-296">在 **encryptionCertificateId** 属性中提供自己的标识符。</span><span class="sxs-lookup"><span data-stu-id="c27c5-296">Provide your own identifier in the **encryptionCertificateId** property.</span></span> 
  
        <span data-ttu-id="c27c5-297">此标识符能够将你的证书与接收的通知匹配，并从证书存储中检索证书。</span><span class="sxs-lookup"><span data-stu-id="c27c5-297">This identifier allows you to match your certificates to the notifications you receive, and to retrieve certificates from your certificate store.</span></span> <span data-ttu-id="c27c5-298">标识符最长 128 个字符。</span><span class="sxs-lookup"><span data-stu-id="c27c5-298">The identifier can be up to 128 characters.</span></span>

4. <span data-ttu-id="c27c5-299">安全管理私钥，以便通知处理代码可以访问私钥来解密资源数据。</span><span class="sxs-lookup"><span data-stu-id="c27c5-299">Manage the private key securely, so that your notification processing code can access the private key to decrypt resource data.</span></span>

#### <a name="rotating-keys"></a><span data-ttu-id="c27c5-300">轮换密钥</span><span class="sxs-lookup"><span data-stu-id="c27c5-300">Rotating keys</span></span>

<span data-ttu-id="c27c5-301">若要将私钥泄露的风险降至最低，请定期更改非对称密钥。</span><span class="sxs-lookup"><span data-stu-id="c27c5-301">To minimize the risk of a private key becoming compromised, periodically change your asymmetric keys.</span></span> <span data-ttu-id="c27c5-302">请按照以下步骤介绍一对新密钥：</span><span class="sxs-lookup"><span data-stu-id="c27c5-302">Follow these steps to introduce a new pair of keys:</span></span>

1. <span data-ttu-id="c27c5-303">使用新非对称密钥对获取新证书。</span><span class="sxs-lookup"><span data-stu-id="c27c5-303">Obtain a new certificate with a new pair of asymmetric keys.</span></span> <span data-ttu-id="c27c5-304">将其用于创建的所有新订阅。</span><span class="sxs-lookup"><span data-stu-id="c27c5-304">Use it for all new subscriptions being created.</span></span>

2. <span data-ttu-id="c27c5-305">使用新的证书密钥更新现有订阅。</span><span class="sxs-lookup"><span data-stu-id="c27c5-305">Update existing subscriptions with the new certificate key.</span></span>

    - <span data-ttu-id="c27c5-306">作为定期续订订阅的一部分执行此操作。</span><span class="sxs-lookup"><span data-stu-id="c27c5-306">Do this as part of regular subscription renewal.</span></span> 
    - <span data-ttu-id="c27c5-307">或者，枚举所有订阅并提供密钥。</span><span class="sxs-lookup"><span data-stu-id="c27c5-307">Or, enumerate all subscriptions and provide the key.</span></span> <span data-ttu-id="c27c5-308">使用[订阅修补程序操作](/graph/api/subscription-update?view=graph-rest-1.0)并更新**encryptionCertificate**和**encryptionCertificateId**属性。</span><span class="sxs-lookup"><span data-stu-id="c27c5-308">Use the [PATCH operation on the subscription](/graph/api/subscription-update?view=graph-rest-1.0) and update the **encryptionCertificate** and **encryptionCertificateId** properties.</span></span>

3. <span data-ttu-id="c27c5-309">请记住下列事项：</span><span class="sxs-lookup"><span data-stu-id="c27c5-309">Keep in mind the following:</span></span>
    - <span data-ttu-id="c27c5-310">在一段时间内，旧证书仍可用于加密。</span><span class="sxs-lookup"><span data-stu-id="c27c5-310">For a period of time, the old certificate may still be used for encryption.</span></span> <span data-ttu-id="c27c5-311">应用程序必须具有访问新旧证书的权限，以能够对内容进行解密。</span><span class="sxs-lookup"><span data-stu-id="c27c5-311">Your app must have access to both old and new certificates to be able to decrypt content.</span></span>
    - <span data-ttu-id="c27c5-312">使用各通知中的 **encryptionCertificateId** 属性来确定要使用的正确密钥。</span><span class="sxs-lookup"><span data-stu-id="c27c5-312">Use the **encryptionCertificateId** property in each notification to identify the correct key to use.</span></span>
    - <span data-ttu-id="c27c5-313">只有在没有看到最近任何通知引用证书时，才可以丢弃旧证书。</span><span class="sxs-lookup"><span data-stu-id="c27c5-313">Discard of the old certificate only when you have seen no recent notifications referencing it.</span></span>

### <a name="decrypting-resource-data"></a><span data-ttu-id="c27c5-314">解密资源数据</span><span class="sxs-lookup"><span data-stu-id="c27c5-314">Decrypting resource data</span></span>

<span data-ttu-id="c27c5-315">为优化性能，Microsoft Graph 使用两步加密过程：</span><span class="sxs-lookup"><span data-stu-id="c27c5-315">To optimize performance, Microsoft Graph uses a two-step encryption process:</span></span>
  - <span data-ttu-id="c27c5-316">它会生成一个使用对称密钥，并用来加密资源数据。</span><span class="sxs-lookup"><span data-stu-id="c27c5-316">It generates a single use symmetric key, and uses it to encrypt resource data.</span></span>
  - <span data-ttu-id="c27c5-317">它使用公共非对称密钥（订阅时提供）加密对称密钥，并将之包含在订阅的各通知中。</span><span class="sxs-lookup"><span data-stu-id="c27c5-317">It uses the public asymmetric key (that you provided when subscribing) to encrypt the symmetric key and includes it in each notification of that subscription.</span></span>

<span data-ttu-id="c27c5-318">始终假设通知中各项的对称密钥不同。</span><span class="sxs-lookup"><span data-stu-id="c27c5-318">Always assume that the symmetric key is different for each item in the notification.</span></span>

<span data-ttu-id="c27c5-319">若要对资源数据进行解密，应用程序应使用各通知 **encryptedContent** 下的属性执行反向操作：</span><span class="sxs-lookup"><span data-stu-id="c27c5-319">To decrypt resource data, your app should perform the reverse steps, using the properties under **encryptedContent** in each notification:</span></span>

1. <span data-ttu-id="c27c5-320">使用 **encryptionCertificateId** 属性标识要使用的证书。</span><span class="sxs-lookup"><span data-stu-id="c27c5-320">Use the **encryptionCertificateId** property to identify the certificate to use.</span></span>

2. <span data-ttu-id="c27c5-321">使用私钥初始化 RSA 加密组件（如 .NET [RSACryptoServiceProvider](https://docs.microsoft.com/dotnet/api/system.security.cryptography.rsacryptoserviceprovider.decrypt?view=netframework-4.8)）。</span><span class="sxs-lookup"><span data-stu-id="c27c5-321">Initialize an RSA cryptographic component (such as the .NET [RSACryptoServiceProvider](https://docs.microsoft.com/dotnet/api/system.security.cryptography.rsacryptoserviceprovider.decrypt?view=netframework-4.8)) with the private key.</span></span>

3. <span data-ttu-id="c27c5-322">解密通知中各项的**dataKey** 属性中提供的对称密钥。</span><span class="sxs-lookup"><span data-stu-id="c27c5-322">Decrypt the symmetric key delivered in the **dataKey** property of each item in the notification.</span></span>

    <span data-ttu-id="c27c5-323">使用适用于解密算法的最佳非对称加密填充（OAEP）。</span><span class="sxs-lookup"><span data-stu-id="c27c5-323">Use Optimal Asymmetric Encryption Padding (OAEP) for the decryption algorithm.</span></span>

4. <span data-ttu-id="c27c5-324">使用对称密钥计算**数据**中数值的 HMAC-SHA256 签名。</span><span class="sxs-lookup"><span data-stu-id="c27c5-324">Use the symmetric key to calculate the HMAC-SHA256 signature of the value in **data**.</span></span>
  
    <span data-ttu-id="c27c5-325">将其与 **dataSignature**中的值进行比较。</span><span class="sxs-lookup"><span data-stu-id="c27c5-325">Compare it to the value in **dataSignature**.</span></span> <span data-ttu-id="c27c5-326">如果不匹配，则假定有效负载已被篡改，并且不对其进行解密。</span><span class="sxs-lookup"><span data-stu-id="c27c5-326">If they do not match, assume the payload has been tampered with and do not decrypt it.</span></span>

5. <span data-ttu-id="c27c5-327">将对称密钥与高级加密标准（AES）（例如 .NET [AesCryptoServiceProvider](https://docs.microsoft.com/dotnet/api/system.security.cryptography.aescryptoserviceprovider?view=netframework-4.8)）结合使用，解密 **数据**中的内容。</span><span class="sxs-lookup"><span data-stu-id="c27c5-327">Use the symmetric key with an Advanced Encryption Standard (AES) (such as the .NET [AesCryptoServiceProvider](https://docs.microsoft.com/dotnet/api/system.security.cryptography.aescryptoserviceprovider?view=netframework-4.8)) to decrypt the content in **data**.</span></span>

    - <span data-ttu-id="c27c5-328">将以下解密参数用于 AES 算法：</span><span class="sxs-lookup"><span data-stu-id="c27c5-328">Use the following decryption parameters for the AES algorithm:</span></span>

        - <span data-ttu-id="c27c5-329">填充： PKCS7</span><span class="sxs-lookup"><span data-stu-id="c27c5-329">Padding: PKCS7</span></span>
        - <span data-ttu-id="c27c5-330">密码模式： CBC</span><span class="sxs-lookup"><span data-stu-id="c27c5-330">Cipher mode: CBC</span></span>
    - <span data-ttu-id="c27c5-331">通过复制用于解密的对称密钥的前16个字节来设置 "初始化向量"。</span><span class="sxs-lookup"><span data-stu-id="c27c5-331">Set the "initialization vector" by copying the first 16 bytes of the symmetric key used for decryption.</span></span>

6. <span data-ttu-id="c27c5-332">解密值是一个 JSON 字符串，表示通知中的资源实例。</span><span class="sxs-lookup"><span data-stu-id="c27c5-332">The decrypted value is a JSON string that represents the resource instance in the notification.</span></span>


### <a name="example-decrypting-a-notification-with-encrypted-resource-data"></a><span data-ttu-id="c27c5-333">示例：使用加密资源数据解密通知</span><span class="sxs-lookup"><span data-stu-id="c27c5-333">Example: decrypting a notification with encrypted resource data</span></span>

<span data-ttu-id="c27c5-334">下面是一个示例通知，其中包含频道消息中**chatMessage**实例的解密属性值。</span><span class="sxs-lookup"><span data-stu-id="c27c5-334">The following is an example notification that includes encrypted property values of a **chatMessage** instance in a channel message.</span></span> <span data-ttu-id="c27c5-335">实例由 `@odata.id` 值指定。</span><span class="sxs-lookup"><span data-stu-id="c27c5-335">The instance is specified by the `@odata.id` value.</span></span>

```json
{
    "value": [
        {
            "subscriptionId": "76222963-cc7b-42d2-882d-8aaa69cb2ba3",
            "changeType": "created",
            // Other properties typical in a resource change notification
            "resource": "teams('d29828b8-c04d-4e2a-b2f6-07da6982f0f0')/channels('19:f127a8c55ad949d1a238464d22f0f99e@thread.skype')/messages('1565045424600')/replies('1565047490246')",
            "resourceData": {
                "id": "1565293727947",
                "@odata.type": "#Microsoft.Graph.ChatMessage",
                "@odata.id": "teams('88cbc8fc-164b-44f0-b6a6-b59b4a1559d3')/channels('19:8d9da062ec7647d4bb1976126e788b47@thread.tacv2')/messages('1565293727947')/replies('1565293727947')"
            },
            "encryptedContent": {
                "data": "{encrypted data that produces a full resource}",
        "dataSignature": "<HMAC-SHA256 hash>",
                "dataKey": "{encrypted symmetric key from Microsoft Graph}",
                "encryptionCertificateId": "MySelfSignedCert/DDC9651A-D7BC-4D74-86BC-A8923584B0AB",
                "encryptionCertificateThumbprint": "07293748CC064953A3052FB978C735FB89E61C3D"
            }
        }
    ],
    "validationTokens": [
        "eyJ0eXAiOiJKV1QiLCJhbGciOiJSU..."
    ]
}
```

<span data-ttu-id="c27c5-336">本节包含一些有用的代码片段，它们针对解密的各个阶段使用C# 和NET。</span><span class="sxs-lookup"><span data-stu-id="c27c5-336">This section contains some useful code snippets that use C# and .NET for each stage of decryption.</span></span>

#### <a name="decrypt-the-symmetric-key"></a><span data-ttu-id="c27c5-337">解密对称密钥</span><span class="sxs-lookup"><span data-stu-id="c27c5-337">Decrypt the symmetric key</span></span>

```csharp
// Initialize with the private key that matches the encryptionCertificateId.
RSACryptoServiceProvider rsaProvider = ...;        
byte[] encryptedSymmetricKey = Convert.FromBase64String(<value from dataKey property>);

// Decrypt using OAEP padding.
byte[] decryptedSymmetricKey = rsaProvider.Decrypt(encryptedSymmetricKey, fOAEP: true);

// Can now use decryptedSymmetricKey with the AES algorithm.
```
```Java
String storename = ""; //name/path of the jks store
String storepass = ""; //password used to open the jks store
String alias = ""; //alias of the certificate when store in the jks store, should be passed as encryptionCertificateId when subscribing and retrieved from the notification
KeyStore ks = KeyStore.getInstance("JKS");
ks.load(new FileInputStream(storename), storepass.toCharArray());
Key asymmetricKey = ks.getKey(alias, storepass.toCharArray());
byte[] encryptedSymetricKey = Base64.decodeBase64("<value from dataKey property>");
Cipher cipher = Cipher.getInstance("RSA/ECB/OAEPWithSHA1AndMGF1Padding");
cipher.init(Cipher.DECRYPT_MODE, asymmetricKey);
byte[] decryptedSymmetricKey = cipher.doFinal(encryptedSymetricKey);
// Can now use decryptedSymmetricKey with the AES algorithm.
```

#### <a name="compare-data-signature-using-hmac-sha256"></a><span data-ttu-id="c27c5-338">使用 HMAC-SHA256 比较数据签名</span><span class="sxs-lookup"><span data-stu-id="c27c5-338">Compare data signature using HMAC-SHA256</span></span>

```csharp
byte[] decryptedSymmetricKey = <the aes key decrypted in the previous step>;
byte[] encryptedPayload = <the value from the data property, still encrypted>;
byte[] expectedSignature = <the value from the dataSignature property>;
byte[] actualSignature;

using (HMACSHA256 hmac = new HMACSHA256(decryptedSymmetricKey))
{
    actualSignature = hmac.ComputeHash(encryptedPayload);
}
if (actualSignature.SequenceEqual(expectedSignature))
{
    // Continue with decryption of the encryptedPayload.
}
else
{
    // Do not attempt to decrypt encryptedPayload. Assume notification payload has been tampered with and investigate.
}
```
```Java
byte[] decryptedSymmetricKey = "<the aes key decrypted in the previous step>";
byte[] decodedEncryptedData = Base64.decodeBase64("data property from encryptedContent object");
Mac mac = Mac.getInstance("HMACSHA256");
SecretKey skey = new SecretKeySpec(decryptedSymmetricKey, "HMACSHA256");
mac.init(skey);
byte[] hashedData = mac.doFinal(decodedEncryptedData);
String encodedHashedData = new String(Base64.encodeBase64(hashedData));
if (comparisonSignature.equals(encodedHashedData);)
{
    // Continue with decryption of the encryptedPayload.
}
else
{
    // Do not attempt to decrypt encryptedPayload. Assume notification payload has been tampered with and investigate.
}
```

#### <a name="decrypt-the-resource-data-content"></a><span data-ttu-id="c27c5-339">解密资源数据内容</span><span class="sxs-lookup"><span data-stu-id="c27c5-339">Decrypt the resource data content</span></span>

```csharp
AesCryptoServiceProvider aesProvider = new AesCryptoServiceProvider();
aesProvider.Key = decryptedSymmetricKey;
aesProvider.Padding = PaddingMode.PKCS7;
aesProvider.Mode = CipherMode.CBC;

// Obtain the intialization vector from the symmetric key itself.
int vectorSize = 16;
byte[] iv = new byte[vectorSize];
Array.Copy(decryptedSymmetricKey, iv, vectorSize);
aesProvider.IV = iv;

byte[] encryptedPayload = Convert.FromBase64String(<value from dataKey property>);

string decryptedResourceData;
// Decrypt the resource data content.
using (var decryptor = aesProvider.CreateDecryptor())
{
  using (MemoryStream msDecrypt = new MemoryStream(encryptedPayload))
  {
      using (CryptoStream csDecrypt = new CryptoStream(msDecrypt, decryptor, CryptoStreamMode.Read))
      {
          using (StreamReader srDecrypt = new StreamReader(csDecrypt))
          {
              decryptedResourceData = srDecrypt.ReadToEnd();
          }
      }
  }
}

// decryptedResourceData now contains a JSON string that represents the resource.
```
```Java
SecretKey skey = new SecretKeySpec(decryptedSymmetricKey, "AES");
IvParameterSpec ivspec = new IvParameterSpec(Arrays.copyOf(decryptedSymmetricKey, 16));
Cipher cipher = Cipher.getInstance("AES/CBC/PKCS5PADDING");
cipher.init(Cipher.DECRYPT_MODE, skey, ivspec);
String decryptedResourceData = new String(cipher.doFinal(Base64.decodeBase64(encryptedData)));
```

## <a name="see-also"></a><span data-ttu-id="c27c5-340">另请参阅</span><span class="sxs-lookup"><span data-stu-id="c27c5-340">See also</span></span>

- [<span data-ttu-id="c27c5-341">设置用户数据更改的通知</span><span class="sxs-lookup"><span data-stu-id="c27c5-341">Set up notifications for changes in user data</span></span>](webhooks.md)
- [<span data-ttu-id="c27c5-342">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="c27c5-342">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-beta)
- [<span data-ttu-id="c27c5-343">获取订阅</span><span class="sxs-lookup"><span data-stu-id="c27c5-343">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="c27c5-344">创建订阅</span><span class="sxs-lookup"><span data-stu-id="c27c5-344">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [<span data-ttu-id="c27c5-345">更新订阅</span><span class="sxs-lookup"><span data-stu-id="c27c5-345">Update subscription</span></span>](/graph/api/subscription-update?view=graph-rest-1.0)
