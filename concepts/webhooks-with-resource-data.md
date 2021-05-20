---
title: 设置包含资源数据的更改通知
description: Microsoft Graph 使用 Webhook 机制将更改通知传递到客户端。 更改通知可以包含资源属性。
author: davidmu1
ms.prod: non-product-specific
localization_priority: Priority
ms.openlocfilehash: 4da690a646c47ef857de860d36bde17a4ee26761
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547181"
---
# <a name="set-up-change-notifications-that-include-resource-data"></a><span data-ttu-id="2b2a5-104">设置包含资源数据的更改通知</span><span class="sxs-lookup"><span data-stu-id="2b2a5-104">Set up change notifications that include resource data</span></span>

<span data-ttu-id="2b2a5-105">Microsoft Graph 允许应用通过 [webhooks](webhooks.md)来订阅资源更改通知。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-105">Microsoft Graph allows apps to subscribe to change notifications for resources via [webhooks](webhooks.md).</span></span> <span data-ttu-id="2b2a5-106">你可以设置订阅，以将更改后的资源数据（例如 Microsoft Teams 聊天消息的内容或 Microsoft Teams 状态信息）包括在更改通知中。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-106">You can set up subscriptions to include the changed resource data (such as the content of a Microsoft Teams chat message or Microsoft Teams presence information) in change notifications.</span></span> <span data-ttu-id="2b2a5-107">随后，应用程序可运行其业务逻辑，无需调用单独的 API 来获取更改的资源。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-107">Your app can then run its business logic without having to make a separate API call to fetch the changed resource.</span></span> <span data-ttu-id="2b2a5-108">因此，应用程序的 API 调用更少，对于大型方案非常有用。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-108">As a result, the app performs better by making fewer API calls, which is beneficial in large scale scenarios.</span></span>

<span data-ttu-id="2b2a5-109">若要将资源数据作为更改通知的一部分，需要实现以下附加逻辑，来满足数据访问和安全要求：</span><span class="sxs-lookup"><span data-stu-id="2b2a5-109">Including resource data as part of change notifications requires you to implement the following additional logic to satisfy data access and security requirements:</span></span> 

- <span data-ttu-id="2b2a5-110">[处理](webhooks-lifecycle.md#responding-to-reauthorizationrequired-notifications)）特殊订阅生命周期通知（预览），以保持数据的不间断流动。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-110">[Handle](webhooks-lifecycle.md#responding-to-reauthorizationrequired-notifications)) special subscription lifecycle notifications (preview) to maintain an uninterrupted flow of data.</span></span> <span data-ttu-id="2b2a5-111">Microsoft Graph 会不时发送生命周期通知，以要求应用重新授权，确保更改通知中所包含的数据不会意外发生访问问题。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-111">Microsoft Graph sends lifecycle notifications from time to time to require an app to re-authorize, to make sure access issues have not unexpectedly cropped up for including resource data in change notifications.</span></span>
- <span data-ttu-id="2b2a5-112">[验证](#validating-the-authenticity-of-notifications)来自 Microsoft Graph 的更改通知的真实性。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-112">[Validate](#validating-the-authenticity-of-notifications) the authenticity of change notifications as having originated from Microsoft Graph.</span></span>
- <span data-ttu-id="2b2a5-113">[提供](#decrypting-resource-data-from-change-notifications)公共加密密钥并使用私钥解密通过更改通知所接收的资源数据。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-113">[Provide](#decrypting-resource-data-from-change-notifications) a public encryption key and use a private key to decrypt resource data received through change notifications.</span></span>

## <a name="resource-data-in-notification-payload"></a><span data-ttu-id="2b2a5-114">通知负载中的资源数据</span><span class="sxs-lookup"><span data-stu-id="2b2a5-114">Resource data in notification payload</span></span>

<span data-ttu-id="2b2a5-115">通常情况下，此类更改通知包括负载中的以下资源数据：</span><span class="sxs-lookup"><span data-stu-id="2b2a5-115">In general, this type of change notifications include the following resource data in the payload:</span></span>

- <span data-ttu-id="2b2a5-116">**resourceData** 属性中返回的已更改资源实例的ID和类型。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-116">ID and type of the changed resource instance, returned in the **resourceData** property.</span></span>
- <span data-ttu-id="2b2a5-117">按照订阅中规定内容加密、在 **encryptedContent** 属性中返回的资源实例的所有属性值。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-117">All the property values of that resource instance, encrypted as specified in the subscription, returned in the **encryptedContent** property.</span></span>
- <span data-ttu-id="2b2a5-118">或者，具体取决于资源、**resourceData** 属性中返回的特定属性。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-118">Or, depending on the resource, specific properties returned in the **resourceData** property.</span></span> <span data-ttu-id="2b2a5-119">若要仅获取特定属性，请使用 `$select` 参数，将其指定为订阅中的 **资源** URL 的一部分。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-119">To get only specific properties, specify them as part of the **resource** URL in the subscription, using a `$select` parameter.</span></span>  


## <a name="supported-resources"></a><span data-ttu-id="2b2a5-120">支持的资源</span><span class="sxs-lookup"><span data-stu-id="2b2a5-120">Supported resources</span></span>

<span data-ttu-id="2b2a5-121">目前，Microsoft Teams [chatMessage](/graph/api/resources/chatmessage) 以及 Microsoft Teams [presence](/graph/api/resources/presence)（预览）资源支持包括资源数据的更改通知。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-121">Currently, the Microsoft Teams [chatMessage](/graph/api/resources/chatmessage) as well as the Microsoft Teams [presence](/graph/api/resources/presence) (preview) resources supports change notifications that include resource data.</span></span> <span data-ttu-id="2b2a5-122">具体而言，可设置应用以下内容之一的订阅：</span><span class="sxs-lookup"><span data-stu-id="2b2a5-122">Specifically, you can set up a subscription that applies to one of the following:</span></span>

- <span data-ttu-id="2b2a5-123">特定 Teams 频道中新增或已更改的消息：`/teams/{id}/channels/{id}/messages`</span><span class="sxs-lookup"><span data-stu-id="2b2a5-123">New or changed messages in a specific Teams channel: `/teams/{id}/channels/{id}/messages`</span></span>
- <span data-ttu-id="2b2a5-124">整个组织（租户）中所有团队频道中的新消息或已更改消息： `/teams/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="2b2a5-124">New or changed messages in all Teams channels: `/teams/getAllMessages`</span></span>
- <span data-ttu-id="2b2a5-125">指定团队聊天中的新增或已更改消息： `/chats/{id}/messages`</span><span class="sxs-lookup"><span data-stu-id="2b2a5-125">New or changed messages in a specific Teams chat: `/chats/{id}/messages`</span></span>
- <span data-ttu-id="2b2a5-126">整个组织（租户）中所有聊天的新消息或已更改消息： `/chats/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="2b2a5-126">New or changed messages in all Teams chats: `/chats/getAllMessages`</span></span>
- <span data-ttu-id="2b2a5-127">用户的状态信息更新：`/communications/presences/{id}`</span><span class="sxs-lookup"><span data-stu-id="2b2a5-127">User's presence information update: `/communications/presences/{id}`</span></span>

<span data-ttu-id="2b2a5-128">含有更改通知中所有已更改实例属性的 **chatMessage** 和 **presence** （预览）支持。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-128">The **chatMessage** and the **presence** (preview) resources support including all the properties of a changed instance in a change notification.</span></span> <span data-ttu-id="2b2a5-129">它们不支持仅返回实例的选择性属性。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-129">They do not support returning only selective properties of the instance.</span></span> 

<span data-ttu-id="2b2a5-130">本文介绍订阅 Teams 通道中的消息更改通知的示例，各更改通知包含已更改 **chatMessage** 实例的完整资源数据。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-130">This article walks through an example that shows you how to subscribe to change notifications for messages in a Teams channel, with each change notification including the full resource data of the changed **chatMessage** instance.</span></span> <span data-ttu-id="2b2a5-131">有关基于 **chatMessage** 的订阅的更多详细信息，请参阅 [获取聊天和频道消息的更改通知](teams-changenotifications-chatmessage.md)。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-131">For more details about **chatMessage**-based subscriptions, see [Get change notifications for chat and channel messages](teams-changenotifications-chatmessage.md).</span></span>

## <a name="creating-a-subscription"></a><span data-ttu-id="2b2a5-132">创建订阅</span><span class="sxs-lookup"><span data-stu-id="2b2a5-132">Creating a subscription</span></span>

<span data-ttu-id="2b2a5-133">若要将资源数据包含在更改通知中，除了 [创建订阅](webhooks.md#creating-a-subscription)时通常指定的属性外，**必须** 指定下列属性：</span><span class="sxs-lookup"><span data-stu-id="2b2a5-133">To have resource data included in change notifications, you **must** specify the following properties, in addition to those that are usually specified when [creating a subscription](webhooks.md#creating-a-subscription):</span></span>

- <span data-ttu-id="2b2a5-134">**includeResourceData**，应设置为 `true` 以明确请求资源数据。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-134">**includeResourceData** which should be set to `true` to explicitly request resource data.</span></span>
- <span data-ttu-id="2b2a5-135">**encryptionCertificate**，仅包含 Microsoft Graph 用于加密资源数据的公钥。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-135">**encryptionCertificate** which contains only the public key that Microsoft Graph uses to encrypt resource data.</span></span> <span data-ttu-id="2b2a5-136">保留相应的私钥，以[解密内容](#decrypting-resource-data-from-change-notifications)。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-136">Keep the corresponding private key to [decrypt the content](#decrypting-resource-data-from-change-notifications).</span></span>
- <span data-ttu-id="2b2a5-137">**encryptionCertificateId**，是证书的自有标识符。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-137">**encryptionCertificateId** which is your own identifier for the certificate.</span></span> <span data-ttu-id="2b2a5-138">使用此 ID 在各更改通知中匹配用于解密的证书。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-138">Use this ID to match in each change notification, which certificate to use for decryption.</span></span>

<span data-ttu-id="2b2a5-139">请注意下列事项：</span><span class="sxs-lookup"><span data-stu-id="2b2a5-139">Keep the following in mind:</span></span>

- <span data-ttu-id="2b2a5-140">按[通知终结点验证](webhooks.md#notification-endpoint-validation)中所述，验证两个终结点。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-140">Validate both endpoints as described in [Notification endpoint validation](webhooks.md#notification-endpoint-validation).</span></span> <span data-ttu-id="2b2a5-141">如果选择针对两个终结点使用同一 URL，将收到并响应两个验证请求。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-141">If you choose to use the same URL for both endpoints, you will receive and respond to two validation requests.</span></span>

### <a name="subscription-request-example"></a><span data-ttu-id="2b2a5-142">订阅请求示例</span><span class="sxs-lookup"><span data-stu-id="2b2a5-142">Subscription request example</span></span>

<span data-ttu-id="2b2a5-143">以下示例为订阅 Microsoft Teams 中创建或更新的频道消息。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-143">The following example subscribes to channel messages being created or updated in Microsoft Teams.</span></span>

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}/channels/{id}/messages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="subscription-response"></a><span data-ttu-id="2b2a5-144">订阅响应</span><span class="sxs-lookup"><span data-stu-id="2b2a5-144">Subscription response</span></span>
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}/channels/{id}/messages",
  "includeResourceData": true,
  "encryptionCertificateId": "{custom ID}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secret client state}"
}
```

## <a name="subscription-lifecycle-notifications-preview"></a><span data-ttu-id="2b2a5-145">订阅生命周期通知（预览）</span><span class="sxs-lookup"><span data-stu-id="2b2a5-145">Subscription lifecycle notifications (preview)</span></span>

<span data-ttu-id="2b2a5-146">某些事件可能会干扰现有订阅中的更改通知流。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-146">Certain events can interfere with change notification flow in an existing subscription.</span></span> <span data-ttu-id="2b2a5-147">订阅生命周期通知将通知你要采取的操作，以保持流不中断。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-147">Subscription lifecycle notifications inform you actions to take in order to maintain an uninterrupted flow.</span></span> <span data-ttu-id="2b2a5-148">不同于资源更改通知（用于通知资源实例更改），生命周期通知涉及订阅自身及其在生命周期中的最新状态。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-148">Unlike a resource change notification which informs a change to a resource instance, a lifecycle notification is about the subscription itself, and its current state in the lifecycle.</span></span> 

<span data-ttu-id="2b2a5-149">有关如何接收和响应生命周期通知（预览）的详细信息，请参阅[减少缺失的订阅和更改通知（预览）](webhooks-lifecycle.md)</span><span class="sxs-lookup"><span data-stu-id="2b2a5-149">For more information about how to receive, and respond to, lifecycle notifications (preview), see [Reduce missing subscriptions and change notifications (preview)](webhooks-lifecycle.md)</span></span>

## <a name="validating-the-authenticity-of-notifications"></a><span data-ttu-id="2b2a5-150">验证通知的真实性</span><span class="sxs-lookup"><span data-stu-id="2b2a5-150">Validating the authenticity of notifications</span></span>

<span data-ttu-id="2b2a5-151">应用通常根据更改通知中包含的资源数据运行业务逻辑。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-151">Apps often run business logic based on resource data included in change notifications.</span></span> <span data-ttu-id="2b2a5-152">首先验证每个更改通知的真实性非常重要。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-152">Verifying the authenticity of each change notification first is important.</span></span> <span data-ttu-id="2b2a5-153">否则，第三方可能会以错误的更改通知欺骗你的应用，使其错误地运行其业务逻辑并导致安全事件。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-153">Otherwise, a third party can spoof your app with false change notifications and make it run its business logic incorrectly, and this can lead to a security incident.</span></span>

<span data-ttu-id="2b2a5-154">对于不包含资源数据的基本更改通知，只需根据 [处理更改通知](webhooks.md#processing-the-change-notification)中所述的 **clientState** 值来验证它们。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-154">For basic change notifications that do not contain resource data, simply validate them based on the **clientState** value as described in [Processing the change notification](webhooks.md#processing-the-change-notification).</span></span> <span data-ttu-id="2b2a5-155">这是可以接受的，因为可以进行后续调用受信任的 Microsoft Graph 来访问资源数据，因此，任何尝试欺骗的影响都是有限的。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-155">This is acceptable, as you can make subsequent trusted Microsoft Graph calls to get access to resource data, and therefore the impact of any spoofing attempts is limited.</span></span> 

<span data-ttu-id="2b2a5-156">对于传递资源数据的更改通知，请在处理数据之前执行更全面的验证。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-156">For change notifications that deliver resource data, perform a more thorough validation before processing the data.</span></span>

<span data-ttu-id="2b2a5-157">本节内容：</span><span class="sxs-lookup"><span data-stu-id="2b2a5-157">In this section:</span></span>

- [<span data-ttu-id="2b2a5-158">更改通知中的验证令牌</span><span class="sxs-lookup"><span data-stu-id="2b2a5-158">Validation tokens in the change notification</span></span>](#validation-tokens-in-the-change-notification)
- [<span data-ttu-id="2b2a5-159">如何验证</span><span class="sxs-lookup"><span data-stu-id="2b2a5-159">How to validate</span></span>](#how-to-validate)
- [<span data-ttu-id="2b2a5-160"> JWT 令牌示例</span><span class="sxs-lookup"><span data-stu-id="2b2a5-160">Example JWT token</span></span>](#example-jwt-token)

### <a name="validation-tokens-in-the-change-notification"></a><span data-ttu-id="2b2a5-161">更改通知中的验证令牌</span><span class="sxs-lookup"><span data-stu-id="2b2a5-161">Validation tokens in the change notification</span></span>

<span data-ttu-id="2b2a5-162">带有资源数据的更改通知包含一个附加属性 **validationTokens**，其包含 Microsoft Graph 生成的 JWT 令牌数组。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-162">A change notification with resource data contains an additional property, **validationTokens**, which contains an array of JWT tokens generated by Microsoft Graph.</span></span> <span data-ttu-id="2b2a5-163">Microsoft Graph 将为每个不同的应用和在 **值** 数组中有项的租户对，生成单独的令牌。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-163">Microsoft Graph generates a single token for each distinct app and tenant pair for whom there is an item in the **value** array.</span></span> <span data-ttu-id="2b2a5-164">请记住，通知可能包含使用同一 **notificationUrl** 订阅的各种应用和租户的混合项。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-164">Keep in mind that change notifications may contain a mix of items for various apps and tenants that subscribed using the same **notificationUrl**.</span></span>

<span data-ttu-id="2b2a5-165">在以下示例中，更改通知包含同一应用和两个不同租户的两个项目，因此 **validationTokens** 数组包含两个需要验证的令牌。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-165">In the following example, the change notification contains two items for the same app, and for two different tenants, therefore the **validationTokens** array contains two tokens that need to be validated.</span></span>

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

> <span data-ttu-id="2b2a5-166">**注意：** 有关传递更改通知时发送的数据的完整说明，请参阅 [changeNotificationCollection](/graph/api/resources/changenotificationcollection)。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-166">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>

### <a name="how-to-validate"></a><span data-ttu-id="2b2a5-167">如何验证</span><span class="sxs-lookup"><span data-stu-id="2b2a5-167">How to validate</span></span>

<span data-ttu-id="2b2a5-168">如果你没有使用过令牌验证，请参阅[令牌验证原理](http://www.cloudidentity.com/blog/2014/03/03/principles-of-token-validation/)以获取概述。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-168">If you're new to token validation, see [Principles of Token Validation](http://www.cloudidentity.com/blog/2014/03/03/principles-of-token-validation/) for an overview.</span></span> <span data-ttu-id="2b2a5-169">使用 SDK，例如用于 .NET 的 [System.IdentityModel.Tokens.Jwt](https://www.nuget.org/packages/System.IdentityModel.Tokens.Jwt/) 库或用于不同平台的第三方库。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-169">Use an SDK, such as the [System.IdentityModel.Tokens.Jwt](https://www.nuget.org/packages/System.IdentityModel.Tokens.Jwt/) library for .NET, or a third-party library for a different platform.</span></span>

<span data-ttu-id="2b2a5-170">注意以下事项：</span><span class="sxs-lookup"><span data-stu-id="2b2a5-170">Be mindful of the following:</span></span> 

- <span data-ttu-id="2b2a5-171">确保始终发送 `HTTP 202 Accepted` 状态代码作为更改通知响应的一部分。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-171">Make sure to always send an `HTTP 202 Accepted` status code as part of the response to the change notification.</span></span> 
- <span data-ttu-id="2b2a5-172">可在验证更改通知前（例如，将更改通知存储在队列中以供后续处理）或在验证更改通知后（如果即时处理了通知）进行响应，即使验证失败也是如此。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-172">Respond before validating the change notification (for example, if you store change notifications in queues for later processing) or after (if you process them on the fly), even if validation failed.</span></span>
- <span data-ttu-id="2b2a5-173">接受更改通知可以防止不必要的传递重试，还可以防止任何潜在的恶意行为者查明他们是否通过了验证。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-173">Accepting a change notification prevents unnecessary delivery retries and it also prevents any potential rogue actors from finding out if they passed or failed validation.</span></span> <span data-ttu-id="2b2a5-174">接受无效的更改通知后，你始终可以选择忽略它。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-174">You can always choose to ignore an invalid change notification after you have accepted it.</span></span>

<span data-ttu-id="2b2a5-175">具体而言，针对 **validationTokens** 集合中的各个 JWT 令牌进行验证。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-175">In particular, perform validation on every JWT token in the **validationTokens** collection.</span></span> <span data-ttu-id="2b2a5-176">如果任何令牌失败，请考虑更改通知可疑并进一步调查。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-176">If any tokens fail, consider the change notification suspicious and investigate further.</span></span> 

<span data-ttu-id="2b2a5-177">使用下列步骤验证令牌和生成令牌的应用程序：</span><span class="sxs-lookup"><span data-stu-id="2b2a5-177">Use the following steps to validate tokens and apps that generate tokens:</span></span>

1. <span data-ttu-id="2b2a5-178">验证令牌是否未过期。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-178">Validate that the token has not expired.</span></span>

2. <span data-ttu-id="2b2a5-179">验证令牌未被篡改，并且由预期机构（Microsoft 标识平台）颁发：</span><span class="sxs-lookup"><span data-stu-id="2b2a5-179">Validate the token has not been tampered with and was issued by the expected authority, Microsoft identity platform:</span></span>

    - <span data-ttu-id="2b2a5-180">从公用配置终结点获取签名密钥：`https://login.microsoftonline.com/common/.well-known/openid-configuration`。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-180">Obtain the signing keys from the common configuration endpoint: `https://login.microsoftonline.com/common/.well-known/openid-configuration`.</span></span> <span data-ttu-id="2b2a5-181">此配置由应用程序缓存一段时间。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-181">This configuration is cached by your app for a period of time.</span></span> <span data-ttu-id="2b2a5-182">请注意，由于签名密钥每日都会轮换，因此配置会经常更新。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-182">Be aware that the configuration is updated frequently as signing keys are rotated daily.</span></span>
    - <span data-ttu-id="2b2a5-183">使用这些密钥验证 JWT 令牌的签名。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-183">Verify the signature of the JWT token using those keys.</span></span>

    <span data-ttu-id="2b2a5-184">不要接受任何其他机构颁发的令牌。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-184">Do not accept tokens issued by any other authority.</span></span>

3. <span data-ttu-id="2b2a5-185">验证口令已为订阅更改通知的应用程序颁发。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-185">Validate that the token was issued for your app that is subscribing to change notifications.</span></span>

    <span data-ttu-id="2b2a5-186">下列步骤是 JWT 令牌库中标准验证逻辑的一部分，通常可作为单个函数调用执行。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-186">The following steps are part of standard validation logic in JWT token libraries and can typically be executed as a single function call.</span></span> 
    - <span data-ttu-id="2b2a5-187">在与应用程序ID匹配的令牌中验证“受众”。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-187">Validate the "audience" in the token matches your app ID.</span></span>
    - <span data-ttu-id="2b2a5-188">如果有多个应用收到更改通知，请务必检查是否有多个 ID。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-188">If you have more than one app receiving change notifications, make sure to check for multiple IDs.</span></span>


4. <span data-ttu-id="2b2a5-189">**关键**：验证生成令牌的应用程序是否代表着 Microsoft Graph 更改通知的发布者。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-189">**Critical**: Validate that the app that generated the token represents the Microsoft Graph change notification publisher.</span></span> 

    - <span data-ttu-id="2b2a5-190">在与 `0bf30f3b-4a52-48df-9a82-234910c4a086`期望值匹配的令牌中检查 **appid** 属性。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-190">Check that the **appid** property in the token matches the expected value of `0bf30f3b-4a52-48df-9a82-234910c4a086`.</span></span>
    - <span data-ttu-id="2b2a5-191">这样可以确保更改通知不会由不是 Microsoft Graph 的其他应用发送的。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-191">This ensures that change notifications are not sent by a different app that is not Microsoft Graph.</span></span>


### <a name="example-jwt-token"></a><span data-ttu-id="2b2a5-192">JWT 令牌示例</span><span class="sxs-lookup"><span data-stu-id="2b2a5-192">Example JWT token</span></span>

<span data-ttu-id="2b2a5-193">下面是验证所需的 JWT 令牌中所含属性的示例。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-193">The following is an example of the properties included in the JWT token that are needed for validation.</span></span>

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

### <a name="example-verifying-validation-tokens"></a><span data-ttu-id="2b2a5-194">示例：对验证令牌进行验证</span><span class="sxs-lookup"><span data-stu-id="2b2a5-194">Example: Verifying validation tokens</span></span>

```csharp
// add Microsoft.IdentityModel.Protocols.OpenIdConnect and System.IdentityModel.Tokens.Jwt nuget packages to your project
public async Task<bool> ValidateToken(string token, string tenantId, IEnumerable<string> appIds)
{
    var configurationManager = new ConfigurationManager<OpenIdConnectConfiguration>("https://login.microsoftonline.com/common/v2.0/.well-known/openid-configuration", new OpenIdConnectConfigurationRetriever());
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
```JavaScript
import jwt from 'jsonwebtoken';
import jkwsClient from 'jwks-rsa';

const client = jkwsClient({
  jwksUri: 'https://login.microsoftonline.com/common/discovery/v2.0/keys'
});

export function getKey(header, callback) {
  client.getSigningKey(header.kid, (err, key) => {
    var signingKey = key.publicKey || key.rsaPublicKey;
    callback(null, signingKey);
  });
}

export function isTokenValid(token, appId, tenantId) {
  return new Promise((resolve) => {
    const options = {
      audience: [appId],
      issuer: [`https://sts.windows.net/${tenantId}/`]
    };
    jwt.verify(token, getKey, options, (err) => {
      if (err) {
        // eslint-disable-next-line no-console
        console.error(err);
        resolve(false);
      } else {
        resolve(true);
      }
    });
  });
}
```
<span data-ttu-id="2b2a5-195">还必须实现 `JwkKeyResolver`，这样 Java 示例才能正常运行。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-195">For the Java sample to work, you will also need to implement the `JwkKeyResolver`.</span></span>  
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

## <a name="decrypting-resource-data-from-change-notifications"></a><span data-ttu-id="2b2a5-196">解密更改通知资源数据</span><span class="sxs-lookup"><span data-stu-id="2b2a5-196">Decrypting resource data from change notifications</span></span>

<span data-ttu-id="2b2a5-197">更改通知的 **resourceData** 属性仅包含资源实例的基本 ID 和类型信息。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-197">The **resourceData** property of a change notification includes only the basic ID and type information of a resource instance.</span></span> <span data-ttu-id="2b2a5-198">**encryptedData** 属性包含由 Microsoft Graph 使用订阅中所提供密钥解密的完整资源数据。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-198">The **encryptedData** property contains the full resource data, encrypted by Microsoft Graph using the public key provided in the subscription.</span></span> <span data-ttu-id="2b2a5-199">此属性还含有验证和解密所需的数值。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-199">The property also contains values required for verification and decryption.</span></span> <span data-ttu-id="2b2a5-200">这样做是为了提高通过更改通知访问的客户数据的安全性。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-200">This is done to increase the security of customer data accessed via change notifications.</span></span> <span data-ttu-id="2b2a5-201">你有责任保护私钥，以确保客户数据不能由第三方解密，即使他们设法截取原始更改通知也是如此。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-201">It is your responsibility to secure the private key to ensure that customer data cannot be decrypted by a third party, even if they manage to intercept the original change notifications.</span></span>

<span data-ttu-id="2b2a5-202">本节内容：</span><span class="sxs-lookup"><span data-stu-id="2b2a5-202">In this section:</span></span>

- [<span data-ttu-id="2b2a5-203">管理加密密钥</span><span class="sxs-lookup"><span data-stu-id="2b2a5-203">Managing encryption keys</span></span>](#managing-encryption-keys)
- [<span data-ttu-id="2b2a5-204">解密资源数据</span><span class="sxs-lookup"><span data-stu-id="2b2a5-204">Decrypting resource data</span></span>](#decrypting-resource-data)
- [<span data-ttu-id="2b2a5-205">示例：使用加密资源数据解密通知</span><span class="sxs-lookup"><span data-stu-id="2b2a5-205">Example: decrypting a notification with encrypted resource data</span></span>](#example-decrypting-a-notification-with-encrypted-resource-data)

### <a name="managing-encryption-keys"></a><span data-ttu-id="2b2a5-206">管理加密密钥</span><span class="sxs-lookup"><span data-stu-id="2b2a5-206">Managing encryption keys</span></span>

1. <span data-ttu-id="2b2a5-207">使用非对称密钥对获取证书。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-207">Obtain a certificate with a pair of asymmetric keys.</span></span>

    - <span data-ttu-id="2b2a5-208">可自行对证书进行签名，因为 Microsoft Graph 不会验证证书颁发者，并且仅将公共密钥用于加密。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-208">You can self-sign the certificate, since Microsoft Graph does not verify the certificate issuer, and uses the public key for only encryption.</span></span> 
    - <span data-ttu-id="2b2a5-209">使用[Azure 密钥存储库](/azure/key-vault/key-vault-whatis)作为创建、轮换和安全管理证书的解决方案。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-209">Use [Azure Key Vault](/azure/key-vault/key-vault-whatis) as the solution to create, rotate, and securely manage certificates.</span></span> <span data-ttu-id="2b2a5-210">确保密钥符合下列条件：</span><span class="sxs-lookup"><span data-stu-id="2b2a5-210">Make sure the keys satisfy the following criteria:</span></span>

        - <span data-ttu-id="2b2a5-211">密钥必须属于类型 `RSA`</span><span class="sxs-lookup"><span data-stu-id="2b2a5-211">The key must be of type `RSA`</span></span>
        - <span data-ttu-id="2b2a5-212">密钥大小必须在2048和4096位之间。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-212">The key size must be between 2048 and 4096 bits</span></span>

2. <span data-ttu-id="2b2a5-213">采用base64编码X.509格式导出证书，且 **仅包括公钥**。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-213">Export the certificate in base64-encoded X.509 format, and **include only the public key**.</span></span> 

3. <span data-ttu-id="2b2a5-214">创建订阅时：</span><span class="sxs-lookup"><span data-stu-id="2b2a5-214">When creating a subscription:</span></span>

    - <span data-ttu-id="2b2a5-215">使用导入证书的base64基编码内容，在 **encryptionCertificate** 属性中提供证书。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-215">Provide the certificate in the **encryptionCertificate** property, using the base64-encoded content that the certificate was exported in.</span></span>
    - <span data-ttu-id="2b2a5-216">在 **encryptionCertificateId** 属性中提供自己的标识符。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-216">Provide your own identifier in the **encryptionCertificateId** property.</span></span> 
  
        <span data-ttu-id="2b2a5-p121">此标识符能够将你的证书与接收的更改通知匹配，并从证书存储中检索证书。标识符最长 128 个字符。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-p121">This identifier allows you to match your certificates to the change notifications you receive, and to retrieve certificates from your certificate store. The identifier can be up to 128 characters.</span></span>

4. <span data-ttu-id="2b2a5-219">安全地管理私钥，以便更改通知处理代码可以访问私钥来解密资源数据。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-219">Manage the private key securely, so that your change notification processing code can access the private key to decrypt resource data.</span></span>

#### <a name="rotating-keys"></a><span data-ttu-id="2b2a5-220">轮换密钥</span><span class="sxs-lookup"><span data-stu-id="2b2a5-220">Rotating keys</span></span>

<span data-ttu-id="2b2a5-221">若要将私钥泄露的风险降至最低，请定期更改非对称密钥。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-221">To minimize the risk of a private key becoming compromised, periodically change your asymmetric keys.</span></span> <span data-ttu-id="2b2a5-222">请按照以下步骤介绍一对新密钥：</span><span class="sxs-lookup"><span data-stu-id="2b2a5-222">Follow these steps to introduce a new pair of keys:</span></span>

1. <span data-ttu-id="2b2a5-223">使用新非对称密钥对获取新证书。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-223">Obtain a new certificate with a new pair of asymmetric keys.</span></span> <span data-ttu-id="2b2a5-224">将其用于创建的所有新订阅。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-224">Use it for all new subscriptions being created.</span></span>

2. <span data-ttu-id="2b2a5-225">使用新的证书密钥更新现有订阅。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-225">Update existing subscriptions with the new certificate key.</span></span>

    - <span data-ttu-id="2b2a5-226">作为定期续订订阅的一部分执行此操作。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-226">Do this as part of regular subscription renewal.</span></span> 
    - <span data-ttu-id="2b2a5-227">或者，枚举所有订阅并提供密钥。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-227">Or, enumerate all subscriptions and provide the key.</span></span> <span data-ttu-id="2b2a5-228">使用 [订阅修补程序操作](/graph/api/subscription-update)并更新 **encryptionCertificate** 和 **encryptionCertificateId** 属性。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-228">Use the [PATCH operation on the subscription](/graph/api/subscription-update) and update the **encryptionCertificate** and **encryptionCertificateId** properties.</span></span>

3. <span data-ttu-id="2b2a5-229">请记住下列事项：</span><span class="sxs-lookup"><span data-stu-id="2b2a5-229">Keep in mind the following:</span></span>
    - <span data-ttu-id="2b2a5-230">在一段时间内，旧证书仍可用于加密。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-230">For a period of time, the old certificate may still be used for encryption.</span></span> <span data-ttu-id="2b2a5-231">应用程序必须具有访问新旧证书的权限，以能够对内容进行解密。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-231">Your app must have access to both old and new certificates to be able to decrypt content.</span></span>
    - <span data-ttu-id="2b2a5-232">使用各更改通知中的 **encryptionCertificateId** 属性来确定要使用的正确密钥。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-232">Use the **encryptionCertificateId** property in each change notification to identify the correct key to use.</span></span>
    - <span data-ttu-id="2b2a5-233">只有在没有看到最近任何更改通知引用旧证书时，才可以丢弃旧证书。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-233">Discard of the old certificate only when you have seen no recent change notifications referencing it.</span></span>

### <a name="decrypting-resource-data"></a><span data-ttu-id="2b2a5-234">解密资源数据</span><span class="sxs-lookup"><span data-stu-id="2b2a5-234">Decrypting resource data</span></span>

<span data-ttu-id="2b2a5-235">为优化性能，Microsoft Graph 使用两步加密过程：</span><span class="sxs-lookup"><span data-stu-id="2b2a5-235">To optimize performance, Microsoft Graph uses a two-step encryption process:</span></span>
  - <span data-ttu-id="2b2a5-236">它会生成一个使用对称密钥，并用来加密资源数据。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-236">It generates a single use symmetric key, and uses it to encrypt resource data.</span></span>
  - <span data-ttu-id="2b2a5-237">它使用公共非对称密钥（订阅时提供）加密对称密钥，并将之包含在订阅的各更改通知中。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-237">It uses the public asymmetric key (that you provided when subscribing) to encrypt the symmetric key and includes it in each change notification of that subscription.</span></span>

<span data-ttu-id="2b2a5-238">始终假设更改通知中各项的对称密钥不同。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-238">Always assume that the symmetric key is different for each item in the change notification.</span></span>

<span data-ttu-id="2b2a5-239">若要对资源数据进行解密，应用应使用各更改通知 **encryptedContent** 下的属性执行反向操作：</span><span class="sxs-lookup"><span data-stu-id="2b2a5-239">To decrypt resource data, your app should perform the reverse steps, using the properties under **encryptedContent** in each change notification:</span></span>

1. <span data-ttu-id="2b2a5-240">使用 **encryptionCertificateId** 属性标识要使用的证书。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-240">Use the **encryptionCertificateId** property to identify the certificate to use.</span></span>

2. <span data-ttu-id="2b2a5-241">使用私钥初始化 RSA 加密组件（如 .NET [RSACryptoServiceProvider](/dotnet/api/system.security.cryptography.rsacryptoserviceprovider.decrypt?view=netframework-4.8)）。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-241">Initialize an RSA cryptographic component (such as the .NET [RSACryptoServiceProvider](/dotnet/api/system.security.cryptography.rsacryptoserviceprovider.decrypt?view=netframework-4.8)) with the private key.</span></span>

3. <span data-ttu-id="2b2a5-242">解密更改通知中各项的 **dataKey** 属性中提供的对称密钥。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-242">Decrypt the symmetric key delivered in the **dataKey** property of each item in the change notification.</span></span>

    <span data-ttu-id="2b2a5-243">使用适用于解密算法的最佳非对称加密填充（OAEP）。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-243">Use Optimal Asymmetric Encryption Padding (OAEP) for the decryption algorithm.</span></span>

4. <span data-ttu-id="2b2a5-244">使用对称密钥计算 **数据** 中数值的 HMAC-SHA256 签名。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-244">Use the symmetric key to calculate the HMAC-SHA256 signature of the value in **data**.</span></span>
  
    <span data-ttu-id="2b2a5-245">将其与 **dataSignature** 中的值进行比较。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-245">Compare it to the value in **dataSignature**.</span></span> <span data-ttu-id="2b2a5-246">如果不匹配，则假定有效负载已被篡改，并且不对其进行解密。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-246">If they do not match, assume the payload has been tampered with and do not decrypt it.</span></span>

5. <span data-ttu-id="2b2a5-247">将对称密钥与高级加密标准（AES）（例如 .NET [AesCryptoServiceProvider](/dotnet/api/system.security.cryptography.aescryptoserviceprovider?view=netframework-4.8)）结合使用，解密 **数据** 中的内容。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-247">Use the symmetric key with an Advanced Encryption Standard (AES) (such as the .NET [AesCryptoServiceProvider](/dotnet/api/system.security.cryptography.aescryptoserviceprovider?view=netframework-4.8)) to decrypt the content in **data**.</span></span>

    - <span data-ttu-id="2b2a5-248">将以下解密参数用于 AES 算法：</span><span class="sxs-lookup"><span data-stu-id="2b2a5-248">Use the following decryption parameters for the AES algorithm:</span></span>

        - <span data-ttu-id="2b2a5-249">填充： PKCS7</span><span class="sxs-lookup"><span data-stu-id="2b2a5-249">Padding: PKCS7</span></span>
        - <span data-ttu-id="2b2a5-250">密码模式： CBC</span><span class="sxs-lookup"><span data-stu-id="2b2a5-250">Cipher mode: CBC</span></span>
    - <span data-ttu-id="2b2a5-251">通过复制用于解密的对称密钥的前16个字节来设置 "初始化向量"。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-251">Set the "initialization vector" by copying the first 16 bytes of the symmetric key used for decryption.</span></span>

6. <span data-ttu-id="2b2a5-252">解密值是一个 JSON 字符串，表示更改通知中的资源实例。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-252">The decrypted value is a JSON string that represents the resource instance in the change notification.</span></span>


### <a name="example-decrypting-a-notification-with-encrypted-resource-data"></a><span data-ttu-id="2b2a5-253">示例：使用加密资源数据解密通知</span><span class="sxs-lookup"><span data-stu-id="2b2a5-253">Example: decrypting a notification with encrypted resource data</span></span>

<span data-ttu-id="2b2a5-254">下面是一个示例更改通知，其中包含频道消息中 **chatMessage** 实例的解密属性值。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-254">The following is an example change notification that includes encrypted property values of a **chatMessage** instance in a channel message.</span></span> <span data-ttu-id="2b2a5-255">实例由 `@odata.id` 值指定。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-255">The instance is specified by the `@odata.id` value.</span></span>

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

> <span data-ttu-id="2b2a5-256">**注意：** 有关传递更改通知时发送的数据的完整说明，请参阅 [changeNotificationCollection](/graph/api/resources/changenotificationcollection)。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-256">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>


<span data-ttu-id="2b2a5-257">本节包含一些有用的代码片段，它们针对解密的各个阶段使用C# 和NET。</span><span class="sxs-lookup"><span data-stu-id="2b2a5-257">This section contains some useful code snippets that use C# and .NET for each stage of decryption.</span></span>

#### <a name="decrypt-the-symmetric-key"></a><span data-ttu-id="2b2a5-258">解密对称密钥</span><span class="sxs-lookup"><span data-stu-id="2b2a5-258">Decrypt the symmetric key</span></span>

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
```JavaScript
const base64encodedKey = 'base 64 encoded dataKey value';
const asymetricPrivateKey = 'pem encoded private key';
const decodedKey = Buffer.from(base64encodedKey, 'base64');
const decryptedSymetricKey = crypto.privateDecrypt(asymetricPrivateKey, decodedKey);
// Can now use decryptedSymmetricKey with the AES algorithm.
```

#### <a name="compare-data-signature-using-hmac-sha256"></a><span data-ttu-id="2b2a5-259">使用 HMAC-SHA256 比较数据签名</span><span class="sxs-lookup"><span data-stu-id="2b2a5-259">Compare data signature using HMAC-SHA256</span></span>

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
if (comparisonSignature.equals(encodedHashedData))
{
    // Continue with decryption of the encryptedPayload.
}
else
{
    // Do not attempt to decrypt encryptedPayload. Assume notification payload has been tampered with and investigate.
}
```
```JavaScript
const decryptedSymetricKey = []; //Buffer provided by previous step
const base64encodedSignature = 'base64 encodded value from the dataSignature property';
const hmac = crypto.createHmac('sha256', decryptedSymetricKey);
hmac.write(base64encodedPayload, 'base64');
if(base64encodedSignature === hmac.digest('base64'))
{
    // Continue with decryption of the encryptedPayload.
}
else
{
    // Do not attempt to decrypt encryptedPayload. Assume notification payload has been tampered with and investigate.
}
```

#### <a name="decrypt-the-resource-data-content"></a><span data-ttu-id="2b2a5-260">解密资源数据内容</span><span class="sxs-lookup"><span data-stu-id="2b2a5-260">Decrypt the resource data content</span></span>

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
```JavaScript
const base64encodedPayload = 'base64 encoded value from data property';
const decryptedSymetricKey = []; //Buffer provided by previous step
const iv = Buffer.alloc(16, 0);
decryptedSymetricKey.copy(iv, 0, 0, 16);
const decipher = crypto.createDecipheriv('aes-256-cbc', decryptedSymetricKey, iv);
let decryptedPayload = decipher.update(base64encodedPayload, 'base64', 'utf8');
decryptedPayload += decipher.final('utf8');
```

## <a name="see-also"></a><span data-ttu-id="2b2a5-261">另请参阅</span><span class="sxs-lookup"><span data-stu-id="2b2a5-261">See also</span></span>

- [<span data-ttu-id="2b2a5-262">设置用户数据更改的通知</span><span class="sxs-lookup"><span data-stu-id="2b2a5-262">Set up notifications for changes in user data</span></span>](webhooks.md)
- [<span data-ttu-id="2b2a5-263">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="2b2a5-263">Subscription resource type</span></span>](/graph/api/resources/subscription)
- [<span data-ttu-id="2b2a5-264">获取订阅</span><span class="sxs-lookup"><span data-stu-id="2b2a5-264">Get subscription</span></span>](/graph/api/subscription-get)
- [<span data-ttu-id="2b2a5-265">创建订阅</span><span class="sxs-lookup"><span data-stu-id="2b2a5-265">Create subscription</span></span>](/graph/api/subscription-post-subscriptions)
- [<span data-ttu-id="2b2a5-266">更新订阅</span><span class="sxs-lookup"><span data-stu-id="2b2a5-266">Update subscription</span></span>](/graph/api/subscription-update)
