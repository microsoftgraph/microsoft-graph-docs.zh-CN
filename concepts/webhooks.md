---
title: 设置用户数据更改的通知
description: The Microsoft Graph API uses a webhook mechanism to deliver change notifications to clients. A client is a web service that configures its own URL to receive change notifications. Client apps use change notifications to update their state upon changes.
author: baywet
ms.prod: non-product-specific
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 7db6b2498d039a4f6474b530023a9f4c0e199119
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "44989777"
---
# <a name="set-up-notifications-for-changes-in-user-data"></a><span data-ttu-id="7206d-105">设置用户数据更改的通知</span><span class="sxs-lookup"><span data-stu-id="7206d-105">Set up notifications for changes in user data</span></span>

<span data-ttu-id="7206d-106">The Microsoft Graph API uses a webhook mechanism to deliver change notifications to clients.</span><span class="sxs-lookup"><span data-stu-id="7206d-106">The Microsoft Graph API uses a webhook mechanism to deliver change notifications to clients.</span></span> <span data-ttu-id="7206d-107">A client is a web service that configures its own URL to receive change notifications.</span><span class="sxs-lookup"><span data-stu-id="7206d-107">A client is a web service that configures its own URL to receive change notifications.</span></span> <span data-ttu-id="7206d-108">Client apps use change notifications to update their state upon changes.</span><span class="sxs-lookup"><span data-stu-id="7206d-108">Client apps use change notifications to update their state upon changes.</span></span>

<span data-ttu-id="7206d-109">在 Microsoft Graph 接受订阅请求后，它会将更改通知推送到订阅中指定的 URL。</span><span class="sxs-lookup"><span data-stu-id="7206d-109">After Microsoft Graph accepts the subscription request, it pushes change notifications to the URL specified in the subscription.</span></span> <span data-ttu-id="7206d-110">然后应用根据其业务逻辑执行操作。</span><span class="sxs-lookup"><span data-stu-id="7206d-110">The app then takes action according to its business logic.</span></span> <span data-ttu-id="7206d-111">例如，它提取更多数据、更新缓存和视图等。</span><span class="sxs-lookup"><span data-stu-id="7206d-111">For example, it fetches more data, updates its cache and views, and so on.</span></span>


> [!VIDEO https://www.youtube-nocookie.com/embed/rC1bunenaq4]
 
> [!div class="nextstepaction"]
> [<span data-ttu-id="7206d-112">教程：使用更改通知和跟踪 Microsoft Graph 中的更改</span><span class="sxs-lookup"><span data-stu-id="7206d-112">Tutorial: Use Change Notifications and Track Changes with Microsoft Graph</span></span>](/learn/modules/msgraph-changenotifications-trackchanges)

<span data-ttu-id="7206d-113">默认情况下，更改通知不包含资源数据，`id` 除外。</span><span class="sxs-lookup"><span data-stu-id="7206d-113">By default, change notifications do not contain resource data, other than the `id`.</span></span> <span data-ttu-id="7206d-114">如果应用需要资源数据，则可以调用 Microsoft Graph API 以获取完整资源。</span><span class="sxs-lookup"><span data-stu-id="7206d-114">If the app requires resource data, it can make calls to Microsoft Graph APIs to get the full resource.</span></span> <span data-ttu-id="7206d-115">本文使用**用户**资源作为使用更改通知的示例。</span><span class="sxs-lookup"><span data-stu-id="7206d-115">This article uses the **user** resource as an example for working with change notifications.</span></span>

<span data-ttu-id="7206d-116">应用还可订阅包含资源数据的更改通知，避免执行其他 API 调用来访问数据。</span><span class="sxs-lookup"><span data-stu-id="7206d-116">An app can also subscribe to change notifications that include resource data, to avoid having to make additonal API calls to access the data.</span></span> <span data-ttu-id="7206d-117">此类应用将需要实现额外的代码来处理此类通知的要求，具体而言：响应订阅生命周期通知，验证通知的真实性，以及解密资源数据。</span><span class="sxs-lookup"><span data-stu-id="7206d-117">Such apps will need to implement extra code to handle the requirements of such notifications, specifically: responding to subscription lifecycle notifications, validating the authenticity of notifications, and decrypting the resource data.</span></span> <span data-ttu-id="7206d-118">将来会有更多资源类型支持此类型的通知。</span><span class="sxs-lookup"><span data-stu-id="7206d-118">More resource types will support this type of notifications in the future.</span></span> <span data-ttu-id="7206d-119">有关如何使用这些通知的详细信息，请参阅[设置包含资源数据的更改通知（预览版）](webhooks-with-resource-data.md)。</span><span class="sxs-lookup"><span data-stu-id="7206d-119">For details about how to work with these notificatios, see [Set up change notifications that include resource data (preview)](webhooks-with-resource-data.md).</span></span>

## <a name="supported-resources"></a><span data-ttu-id="7206d-120">支持的资源</span><span class="sxs-lookup"><span data-stu-id="7206d-120">Supported resources</span></span>

<span data-ttu-id="7206d-121">使用 Microsoft Graph API，应用可以订阅以下资源的更改：</span><span class="sxs-lookup"><span data-stu-id="7206d-121">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="7206d-122">Outlook [邮件][]</span><span class="sxs-lookup"><span data-stu-id="7206d-122">Outlook [message][]</span></span>
- <span data-ttu-id="7206d-123">Outlook [事件][]</span><span class="sxs-lookup"><span data-stu-id="7206d-123">Outlook [event][]</span></span>
- <span data-ttu-id="7206d-124">Outlook 个人[联系人][]</span><span class="sxs-lookup"><span data-stu-id="7206d-124">Outlook personal [contact][]</span></span>
- <span data-ttu-id="7206d-125">[用户][]</span><span class="sxs-lookup"><span data-stu-id="7206d-125">[user][]</span></span>
- <span data-ttu-id="7206d-126">[组][]</span><span class="sxs-lookup"><span data-stu-id="7206d-126">[group][]</span></span>
- <span data-ttu-id="7206d-127">Microsoft 365 组[对话][]</span><span class="sxs-lookup"><span data-stu-id="7206d-127">Microsoft 365 group [conversation][]</span></span>
- <span data-ttu-id="7206d-128">用户个人 OneDrive 上_任何_ [driveItem][] 文件夹层次结构内的内容</span><span class="sxs-lookup"><span data-stu-id="7206d-128">Content within the hierarchy of _any folder_ [driveItem][] on a user's personal OneDrive</span></span>
- <span data-ttu-id="7206d-129">OneDrive for Business 上 [driveItem][] _根文件夹_层次结构内的内容</span><span class="sxs-lookup"><span data-stu-id="7206d-129">Content within the hierarchy of the _root folder_ [driveItem][] on OneDrive for Business</span></span>
- <span data-ttu-id="7206d-130">安全[警报][]</span><span class="sxs-lookup"><span data-stu-id="7206d-130">Security [alert][]</span></span>
- <span data-ttu-id="7206d-131">团队[callRecord][]</span><span class="sxs-lookup"><span data-stu-id="7206d-131">Teams [callRecord][]</span></span>
- <span data-ttu-id="7206d-132">Teams [chatMessage][]（预览）</span><span class="sxs-lookup"><span data-stu-id="7206d-132">Teams [chatMessage][] (preview)</span></span>

<span data-ttu-id="7206d-133">可以创建对特定 Outlook 文件夹的订阅，例如收件箱：`me/mailFolders('inbox')/messages`</span><span class="sxs-lookup"><span data-stu-id="7206d-133">You can create a subscription to a specific Outlook folder such as the Inbox: `me/mailFolders('inbox')/messages`</span></span>

<span data-ttu-id="7206d-134">或者顶级资源：、、、、 `/me/messages` `/me/contacts` `/me/events` `users` `groups` 或`/communications/callRecords`</span><span class="sxs-lookup"><span data-stu-id="7206d-134">Or to a top-level resource: `/me/messages`, `/me/contacts`, `/me/events`, `users`, `groups`, or `/communications/callRecords`</span></span>

<span data-ttu-id="7206d-135">或以下特定资源实例的订阅：`users/{id}`、`groups/{id}`、`groups/{id}/conversations`</span><span class="sxs-lookup"><span data-stu-id="7206d-135">Or to a specific resource instance: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span></span>

<span data-ttu-id="7206d-136">或用户个人 OneDrive 中任何文件夹的订阅：`/drives/{id}/root`
`/drives/{id}/root/subfolder`</span><span class="sxs-lookup"><span data-stu-id="7206d-136">Or to any folder in a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

<span data-ttu-id="7206d-137">或 SharePoint/OneDrive for Business 驱动器根文件夹的订阅：`/drive/root`</span><span class="sxs-lookup"><span data-stu-id="7206d-137">Or to the root folder of a SharePoint/OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="7206d-138">或对新[安全性 API](security-concept-overview.md) 警报的订阅：`/security/alerts?$filter=status eq 'newAlert'`、`/security/alerts?$filter=vendorInformation/provider eq 'ASC'`</span><span class="sxs-lookup"><span data-stu-id="7206d-138">Or to a new [Security API](security-concept-overview.md) alert: `/security/alerts?$filter=status eq 'newAlert'`, `/security/alerts?$filter=vendorInformation/provider eq 'ASC'`</span></span>

### <a name="azure-ad-resource-limitations"></a><span data-ttu-id="7206d-139">Azure AD 资源限制</span><span class="sxs-lookup"><span data-stu-id="7206d-139">Azure AD resource limitations</span></span>

<span data-ttu-id="7206d-140">基于 Azure AD 的资源（用户、组）采用了某些限制，超出限制时将会产生错误：</span><span class="sxs-lookup"><span data-stu-id="7206d-140">Certain limits apply to Azure AD based resources (users, groups) and will generate errors when exceeded:</span></span>

> <span data-ttu-id="7206d-141">**请注意**：这些限制不适用于来自 Azure AD 以外的服务的资源。</span><span class="sxs-lookup"><span data-stu-id="7206d-141">**Note**: These limits do not apply to resources from services other than Azure AD.</span></span> <span data-ttu-id="7206d-142">例如，应用可以创建许多更多的 `message` 或 `event` 资源订阅，这些订阅受到 Microsoft Graph 中的 Exchange Online 服务支持。</span><span class="sxs-lookup"><span data-stu-id="7206d-142">For example, an app can create many more subscriptions to `message` or `event` resources, which are supported by the Exchange Online service as part of Microsoft Graph.</span></span>

- <span data-ttu-id="7206d-143">最大订阅配额：</span><span class="sxs-lookup"><span data-stu-id="7206d-143">Maximum subscription quotas:</span></span>

  - <span data-ttu-id="7206d-144">每个应用（所有租户组合）：50000订阅总数</span><span class="sxs-lookup"><span data-stu-id="7206d-144">Per app (for all tenants combined): 50,000 total subscriptions</span></span>
  - <span data-ttu-id="7206d-145">每个租户（组合所有应用程序）：1000所有应用的订阅总数</span><span class="sxs-lookup"><span data-stu-id="7206d-145">Per tenant (for all applications combined): 1000 total subscriptions across all apps</span></span>
  - <span data-ttu-id="7206d-146">每个应用和租户组合：总订阅数 100</span><span class="sxs-lookup"><span data-stu-id="7206d-146">Per app and tenant combination: 100 total subscriptions</span></span>

<span data-ttu-id="7206d-147">超出任何限制时，创建订阅的尝试将导致[错误响应](errors.md)  -  `403 Forbidden` 。</span><span class="sxs-lookup"><span data-stu-id="7206d-147">When any limit is exceeded, attempts to create a subscription will result in an [error response](errors.md) - `403 Forbidden`.</span></span> <span data-ttu-id="7206d-148">`message` 属性将说明已超出什么限制。</span><span class="sxs-lookup"><span data-stu-id="7206d-148">The `message` property will explain which limit has been exceeded.</span></span>

- <span data-ttu-id="7206d-149">不支持 Azure AD B2C 租户。</span><span class="sxs-lookup"><span data-stu-id="7206d-149">Azure AD B2C tenants are not supported.</span></span>

- <span data-ttu-id="7206d-150">个人 Microsoft 帐户不支持用户实体的 Changfe 通知。</span><span class="sxs-lookup"><span data-stu-id="7206d-150">Changfe notification for user entities are not supported for personal Microsoft accounts.</span></span>

- <span data-ttu-id="7206d-151">用户和租订阅存在一个[已知问题](known-issues.md#change-notifications)。</span><span class="sxs-lookup"><span data-stu-id="7206d-151">A [known issue](known-issues.md#change-notifications) exists with user and group subscriptions.</span></span>

### <a name="outlook-resource-limitations"></a><span data-ttu-id="7206d-152">Outlook 资源限制</span><span class="sxs-lookup"><span data-stu-id="7206d-152">Outlook resource limitations</span></span>

<span data-ttu-id="7206d-153">订阅 Outlook 资源（如**邮件**、**事件**或**联系人**）时，如果选择使用资源路径中的*用户主体名称* UPN，则在 UPN 包含撇号的情况下，订阅请求可能会失败。</span><span class="sxs-lookup"><span data-stu-id="7206d-153">When subscribing to Outlook resources such as **messages**, **events** or **contacts**, if you choose to use the *user principal name* UPN in the resource path, the subscription request might fail if the UPN contains an apostrophe.</span></span> <span data-ttu-id="7206d-154">请考虑使用 GUID 用户 ID 而不是 UPN，以避免遇到此问题。</span><span class="sxs-lookup"><span data-stu-id="7206d-154">Consider using GUID user IDs instead of UPNs to avoid running into this problem.</span></span> <span data-ttu-id="7206d-155">例如，请勿使用资源路径：</span><span class="sxs-lookup"><span data-stu-id="7206d-155">For example, instead of using resource path:</span></span>

`/users/sh.o'neal@contoso.com/messages`

<span data-ttu-id="7206d-156">请使用：</span><span class="sxs-lookup"><span data-stu-id="7206d-156">Use:</span></span> 

`/users/{guid-user-id}/messages`

## <a name="subscription-lifetime"></a><span data-ttu-id="7206d-157">订阅生命周期</span><span class="sxs-lookup"><span data-stu-id="7206d-157">Subscription lifetime</span></span>

<span data-ttu-id="7206d-158">订阅的生命周期有限。</span><span class="sxs-lookup"><span data-stu-id="7206d-158">Subscriptions have a limited lifetime.</span></span> <span data-ttu-id="7206d-159">应用需要在订阅到期前续订订阅。</span><span class="sxs-lookup"><span data-stu-id="7206d-159">Apps need to renew their subscriptions before the expiration time.</span></span> <span data-ttu-id="7206d-160">否则，需要新建订阅。</span><span class="sxs-lookup"><span data-stu-id="7206d-160">Otherwise, they need to create a new subscription.</span></span> <span data-ttu-id="7206d-161">有关最长有效期的列表，请参阅[每个资源类型的最长订阅有效期](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type)。</span><span class="sxs-lookup"><span data-stu-id="7206d-161">For a list of maximum expiration times, see [Maximum length of subscription per resource type](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span></span>

<span data-ttu-id="7206d-162">应用还可以随时取消订阅以停止获取更改通知。</span><span class="sxs-lookup"><span data-stu-id="7206d-162">Apps can also unsubscribe at any time to stop getting change notifications.</span></span>

## <a name="managing-subscriptions"></a><span data-ttu-id="7206d-163">管理订阅</span><span class="sxs-lookup"><span data-stu-id="7206d-163">Managing subscriptions</span></span>

<span data-ttu-id="7206d-164">客户端可以创建订阅、续订订阅和删除订阅。</span><span class="sxs-lookup"><span data-stu-id="7206d-164">Clients can create subscriptions, renew subscriptions, and delete subscriptions.</span></span>

### <a name="creating-a-subscription"></a><span data-ttu-id="7206d-165">创建订阅</span><span class="sxs-lookup"><span data-stu-id="7206d-165">Creating a subscription</span></span>

<span data-ttu-id="7206d-166">Creating a subscription is the first step to start receiving change notifications for a resource.</span><span class="sxs-lookup"><span data-stu-id="7206d-166">Creating a subscription is the first step to start receiving change notifications for a resource.</span></span> <span data-ttu-id="7206d-167">The subscription process is as follows:</span><span class="sxs-lookup"><span data-stu-id="7206d-167">The subscription process is as follows:</span></span>

1. <span data-ttu-id="7206d-168">客户端发送特定资源的订阅 (POST) 请求。</span><span class="sxs-lookup"><span data-stu-id="7206d-168">The client sends a subscription (POST) request for a specific resource.</span></span>

1. <span data-ttu-id="7206d-169">Microsoft Graph 验证请求。</span><span class="sxs-lookup"><span data-stu-id="7206d-169">Microsoft Graph verifies the request.</span></span>

    - <span data-ttu-id="7206d-170">如果请求有效，Microsoft Graph 将验证令牌发送到通知 URL。</span><span class="sxs-lookup"><span data-stu-id="7206d-170">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
    - <span data-ttu-id="7206d-171">如果该请求无效，Microsoft Graph 将发送包含代码和详细信息的错误响应。</span><span class="sxs-lookup"><span data-stu-id="7206d-171">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>

1. <span data-ttu-id="7206d-172">客户端将验证令牌发送回 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="7206d-172">The client sends the validation token back to Microsoft Graph.</span></span>

1. <span data-ttu-id="7206d-173">Microsoft Graph 将响应发送回客户端。</span><span class="sxs-lookup"><span data-stu-id="7206d-173">The Microsoft Graph sends a response back to the client.</span></span>

<span data-ttu-id="7206d-174">客户端必须存储订阅 ID，才能将更改通知与订阅关联。</span><span class="sxs-lookup"><span data-stu-id="7206d-174">The client must store the subscription ID to correlate change notifications with the subscription.</span></span>

#### <a name="subscription-request-example"></a><span data-ttu-id="7206d-175">订阅请求示例</span><span class="sxs-lookup"><span data-stu-id="7206d-175">Subscription request example</span></span>

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/notificationClient",
  "resource": "/me/mailfolders('inbox')/messages",
  "expirationDateTime": "2016-03-20T11:00:00.0000000Z",
  "clientState": "SecretClientState"
}
```

<span data-ttu-id="7206d-176">`changeType`、`notificationUrl`、`resource` 和 `expirationDateTime` 属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="7206d-176">The `changeType`, `notificationUrl`, `resource`, and `expirationDateTime` properties are required.</span></span> <span data-ttu-id="7206d-177">如需属性定义和值，请参阅[订阅资源类型](/graph/api/resources/subscription?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="7206d-177">See [subscription resource type](/graph/api/resources/subscription?view=graph-rest-1.0) for property definitions and values.</span></span>

<span data-ttu-id="7206d-178">`resource` 属性指定要被监视以进行更改的资源。</span><span class="sxs-lookup"><span data-stu-id="7206d-178">The `resource` property specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="7206d-179">例如，可以创建特定邮件文件夹的订阅：`me/mailFolders('inbox')/messages`，或代表由管理员同意的用户：`users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`。</span><span class="sxs-lookup"><span data-stu-id="7206d-179">For example, you can create a subscription to a specific mail folder: `me/mailFolders('inbox')/messages` or on behalf of a user given by an administrator  consent: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span></span>

<span data-ttu-id="7206d-180">尽管 `clientState` 不是必需的，但必须将其包括在内，才能符合我们建议的更改通知处理过程。</span><span class="sxs-lookup"><span data-stu-id="7206d-180">Although `clientState` is not required, you must include it to comply with our recommended change notification handling process.</span></span> <span data-ttu-id="7206d-181">通过设置此属性，可以确认收到的更改通知来自 Microsoft Graph 服务。</span><span class="sxs-lookup"><span data-stu-id="7206d-181">Setting this property will allow you to confirm that change notifications you receive originate from the Microsoft Graph service.</span></span> <span data-ttu-id="7206d-182">因此，该属性的值应保密，并且只有你的应用程序和 Microsoft Graph 服务知道。</span><span class="sxs-lookup"><span data-stu-id="7206d-182">For this reason, the value of the property should remain secret and known only to your application and the Microsoft Graph service.</span></span>

<span data-ttu-id="7206d-183">如果成功，Microsoft Graph 将在正文中返回 `201 Created` 代码和 [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) 对象。</span><span class="sxs-lookup"><span data-stu-id="7206d-183">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span>

#### <a name="notification-endpoint-validation"></a><span data-ttu-id="7206d-184">通知终结点验证</span><span class="sxs-lookup"><span data-stu-id="7206d-184">Notification endpoint validation</span></span>

<span data-ttu-id="7206d-185">Microsoft Graph 在创建订阅之前验证订阅请求的 `notificationUrl` 属性中提供的通知终结点。</span><span class="sxs-lookup"><span data-stu-id="7206d-185">Microsoft Graph validates the notification endpoint provided in the `notificationUrl` property of the subscription request before creating the subscription.</span></span> <span data-ttu-id="7206d-186">验证流程如下所示：</span><span class="sxs-lookup"><span data-stu-id="7206d-186">The validation process occurs as follows:</span></span>

1. <span data-ttu-id="7206d-187">Microsoft Graph 将 POST 请求发送到通知 URL：</span><span class="sxs-lookup"><span data-stu-id="7206d-187">Microsoft Graph sends a POST request to the notification URL:</span></span>

    ``` http
    Content-Type: text/plain; charset=utf-8
    POST https://{notificationUrl}?validationToken={opaqueTokenCreatedByMicrosoftGraph}
    ```

    > <span data-ttu-id="7206d-188">**重要说明：** 由于 `validationToken` 是查询参数，因此客户端必须根据 HTTP 编码做法正确解码它。</span><span class="sxs-lookup"><span data-stu-id="7206d-188">**Important:** Since the `validationToken` is a query parameter it must be properly decoded by the client, as per HTTP coding practices.</span></span> <span data-ttu-id="7206d-189">如果客户端没有解码令牌，而是在下一步（响应）中使用已编码值，那么验证将会失败。</span><span class="sxs-lookup"><span data-stu-id="7206d-189">If the client does not decode the token, and instead uses the encoded value in the next step (response), validation will fail.</span></span> <span data-ttu-id="7206d-190">此外，客户端还应将令牌值视为不透明，因为令牌格式今后可能会更改，而不另行通知。</span><span class="sxs-lookup"><span data-stu-id="7206d-190">Also, the client should treat the token value as opaque since the token format may change in the future, without notice.</span></span>

1. <span data-ttu-id="7206d-191">客户端必须在 10 秒内提供具有以下特性的响应：</span><span class="sxs-lookup"><span data-stu-id="7206d-191">The client must provide a response with the following characteristics within 10 seconds:</span></span>

    - <span data-ttu-id="7206d-192">200 (OK) 状态代码。</span><span class="sxs-lookup"><span data-stu-id="7206d-192">A 200 (OK) status code.</span></span>
    - <span data-ttu-id="7206d-193">内容类型必须是 `text/plain`。</span><span class="sxs-lookup"><span data-stu-id="7206d-193">The content type must be `text/plain`.</span></span>
    - <span data-ttu-id="7206d-194">正文必须包括 Microsoft Graph 提供的验证令牌。</span><span class="sxs-lookup"><span data-stu-id="7206d-194">The body must include the validation token provided by Microsoft Graph.</span></span>

<span data-ttu-id="7206d-195">在响应中提供验证令牌之后，客户端应放弃验证令牌。</span><span class="sxs-lookup"><span data-stu-id="7206d-195">The client should discard the validation token after providing it in the response.</span></span>

<span data-ttu-id="7206d-196">另外，可以使用 [Microsoft Graph Postman Collection](use-postman.md) 来确认终结点能否正确实现验证请求。</span><span class="sxs-lookup"><span data-stu-id="7206d-196">Additionally, you can use the [Microsoft Graph Postman collection](use-postman.md) to confirm that your endpoint properly implements the validation request.</span></span> <span data-ttu-id="7206d-197">“杂项”\*\*\*\* 文件夹中的“订阅验证”\*\*\*\* 请求提供了单元测试，可验证终结点提供的响应。</span><span class="sxs-lookup"><span data-stu-id="7206d-197">The **Subscription Validation** request in the **Misc** folder provides unit tests that validate the response provided by your endpoint.</span></span>  

![验证响应测试结果](images/change-notifications/validation-request-tests-results.png)

### <a name="renewing-a-subscription"></a><span data-ttu-id="7206d-199">续订订阅</span><span class="sxs-lookup"><span data-stu-id="7206d-199">Renewing a subscription</span></span>

<span data-ttu-id="7206d-200">客户端可以续订特定过期日期的订阅，自请求时间起长达三天。</span><span class="sxs-lookup"><span data-stu-id="7206d-200">The client can renew a subscription with a specific expiration date of up to three days from the time of request.</span></span> <span data-ttu-id="7206d-201">`expirationDateTime` 属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="7206d-201">The `expirationDateTime` property is required.</span></span>

#### <a name="subscription-renewal-example"></a><span data-ttu-id="7206d-202">订阅续订示例</span><span class="sxs-lookup"><span data-stu-id="7206d-202">Subscription renewal example</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-Type: application/json

{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="7206d-203">如果成功，Microsoft Graph 将在正文中返回 `200 OK` 代码和 [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) 对象。</span><span class="sxs-lookup"><span data-stu-id="7206d-203">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span> <span data-ttu-id="7206d-204">subscription 对象包括新的 `expirationDateTime` 值。</span><span class="sxs-lookup"><span data-stu-id="7206d-204">The subscription object includes the new `expirationDateTime` value.</span></span>

### <a name="deleting-a-subscription"></a><span data-ttu-id="7206d-205">删除订阅</span><span class="sxs-lookup"><span data-stu-id="7206d-205">Deleting a subscription</span></span>

<span data-ttu-id="7206d-206">客户端可以通过使用其 ID 删除订阅来停止接收更改通知。</span><span class="sxs-lookup"><span data-stu-id="7206d-206">The client can stop receiving change notifications by deleting the subscription using its ID.</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="7206d-207">如果成功，Microsoft Graph 将返回 `204 No Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="7206d-207">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

## <a name="change-notifications"></a><span data-ttu-id="7206d-208">更改通知</span><span class="sxs-lookup"><span data-stu-id="7206d-208">Change notifications</span></span>

<span data-ttu-id="7206d-209">通过客户端订阅对资源的更改，Microsoft Graph 会在 `POST` 资源发生更改时向通知 URL 发送请求。</span><span class="sxs-lookup"><span data-stu-id="7206d-209">With a client subscribing to changes to a resource, Microsoft Graph sends a `POST` request to the notification URL whenever the resource changes.</span></span> <span data-ttu-id="7206d-210">仅发送订阅中指定类型的更改通知，例如 `created` 。</span><span class="sxs-lookup"><span data-stu-id="7206d-210">It sends notifications only for changes of the type that's specified in the subscription, for example, `created`.</span></span>

> <span data-ttu-id="7206d-211">**注意：** 如果客户端具有多个订阅，用于监视同一资源并使用相同的通知 URL，则 Microsoft Graph 可以发送与不同订阅相对应的多个更改通知，每个订阅都显示相应的订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="7206d-211">**Note:** If a client has multiple subscriptions that monitor the same resource and use the same notification URL, Microsoft Graph can send multiple change notifications that correspond to different subscriptions, each showing the corresponding subscription ID.</span></span> <span data-ttu-id="7206d-212">无法保证请求中的所有更改通知都 `POST` 属于单个订阅。</span><span class="sxs-lookup"><span data-stu-id="7206d-212">There is no guarantee that all change notifications in the `POST` request belong to a single subscription.</span></span>

### <a name="change-notification-example"></a><span data-ttu-id="7206d-213">更改通知示例</span><span class="sxs-lookup"><span data-stu-id="7206d-213">Change notification example</span></span>

<span data-ttu-id="7206d-214">此部分显示邮件创建通知的示例。</span><span class="sxs-lookup"><span data-stu-id="7206d-214">This section shows an example of a notification for a message creation.</span></span> <span data-ttu-id="7206d-215">当用户收到电子邮件时，Microsoft Graph 将发送更改通知，如以下示例中所示。</span><span class="sxs-lookup"><span data-stu-id="7206d-215">When the user receives an email, Microsoft Graph sends a change notification as shown in the following example.</span></span>
<span data-ttu-id="7206d-216">请注意，通知位于字段中所示的集合中 `value` 。</span><span class="sxs-lookup"><span data-stu-id="7206d-216">Note that the notification is in a collection represented in the `value` field.</span></span> <span data-ttu-id="7206d-217">有关通知负载的详细信息，请参阅[changeNotificationCollection](/graph/api/resources/changenotificationcollection) 。</span><span class="sxs-lookup"><span data-stu-id="7206d-217">See [changeNotificationCollection](/graph/api/resources/changenotificationcollection) for details of the notification payload.</span></span> 

<span data-ttu-id="7206d-218">当发生许多更改时，Microsoft Graph 可能会发送多个与同一请求中的不同订阅对应的通知 `POST` 。</span><span class="sxs-lookup"><span data-stu-id="7206d-218">When many changes occur, Microsoft Graph may send multiple notifications that correspond to different subscriptions in the same `POST` request.</span></span>

```json
{
  "value": [
    {
      "id": "lsgTZMr9KwAAA",
      "sequenceNumber": 10,
      "subscriptionId":"{subscription_guid}",
      "subscriptionExpirationDateTime":"2016-03-19T22:11:09.952Z",
      "clientState":"secretClientValue",
      "changeType":"created",
      "resource":"users/{user_guid}@{tenant_guid}/messages/{long_id_string}",
      "tenantId": "84bd8158-6d4d-4958-8b9f-9d6445542f95",
      "resourceData":
      {
        "@odata.type":"#Microsoft.Graph.Message",
        "@odata.id":"Users/{user_guid}@{tenant_guid}/Messages/{long_id_string}",
        "@odata.etag":"W/\"CQAAABYAAADkrWGo7bouTKlsgTZMr9KwAAAUWRHf\"",
        "id":"{long_id_string}"
      }
    }
  ]
}
```

### <a name="processing-the-change-notification"></a><span data-ttu-id="7206d-219">处理更改通知</span><span class="sxs-lookup"><span data-stu-id="7206d-219">Processing the change notification</span></span>

<span data-ttu-id="7206d-220">您的过程应处理收到的每个更改通知。</span><span class="sxs-lookup"><span data-stu-id="7206d-220">Your process should process every change notification it receives.</span></span> <span data-ttu-id="7206d-221">以下是您的应用程序处理更改通知时必须执行的最低任务：</span><span class="sxs-lookup"><span data-stu-id="7206d-221">The following are the minimum tasks that your app must perform to process a change notification:</span></span>

1. <span data-ttu-id="7206d-222">将响应中的 `202 - Accepted` 状态代码发送到 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="7206d-222">Send a `202 - Accepted` status code in your response to Microsoft Graph.</span></span> <span data-ttu-id="7206d-223">如果 Microsoft Graph 没有收到2xx 类代码，它会在大约4小时的一段时间内尝试发布更改通知一段时间。之后，更改通知将被丢弃，并且不会被传递。</span><span class="sxs-lookup"><span data-stu-id="7206d-223">If Microsoft Graph doesn't receive a 2xx class code, it will try to publishing the change notification a number of times, for a period of about 4 hours; after that, the change notification will be dropped and won't be delivered.</span></span>

    > <span data-ttu-id="7206d-224">**注意：**`202 - Accepted`收到更改通知后立即发送状态代码，即使在验证其真实性之前也是如此。</span><span class="sxs-lookup"><span data-stu-id="7206d-224">**Note:** Send a `202 - Accepted` status code as soon as you receive the change notification, even before validating its authenticity.</span></span> <span data-ttu-id="7206d-225">您只需确认收到更改通知并防止不必要的重试。</span><span class="sxs-lookup"><span data-stu-id="7206d-225">You are simply acknowledging the receipt of the change notification and preventing unnecessary retries.</span></span> <span data-ttu-id="7206d-226">当前超时是 30 秒，但将来可能会减少，以优化服务性能。</span><span class="sxs-lookup"><span data-stu-id="7206d-226">The current timeout is 30 seconds, but it might be reduced in the future to optimize service performance.</span></span> <span data-ttu-id="7206d-227">如果通知 URL 在30秒内未在10分钟内答复来自 Microsoft Graph 的10% 以上的请求，则所有以下通知都将延迟并在4小时内重试。</span><span class="sxs-lookup"><span data-stu-id="7206d-227">If the notification URL doesn't reply within 30 seconds for more than 10% of the requests from Microsoft Graph over a 10 minute period, all following notifications will be delayed and retried for a period of 4 hours.</span></span> <span data-ttu-id="7206d-228">如果在10分钟内通知 URL 未在30秒内答复来自 Microsoft Graph 的20% 以上的请求，则将删除以下所有通知。</span><span class="sxs-lookup"><span data-stu-id="7206d-228">If a notification URL doesn't reply within 30 seconds for more than 20% of the requests from Microsoft Graph over a 10 minute period, all following notifications will be dropped.</span></span>

1. <span data-ttu-id="7206d-229">验证 `clientState` 属性。</span><span class="sxs-lookup"><span data-stu-id="7206d-229">Validate the `clientState` property.</span></span> <span data-ttu-id="7206d-230">它必须与最初使用订阅创建请求提交的值匹配。</span><span class="sxs-lookup"><span data-stu-id="7206d-230">It must match the value originally submitted with the subscription creation request.</span></span>

    > <span data-ttu-id="7206d-231">**注意：** 如果不满足此条件，则不应将其视为有效的更改通知。</span><span class="sxs-lookup"><span data-stu-id="7206d-231">**Note:** If this isn't true, you should not consider this a valid change notification.</span></span> <span data-ttu-id="7206d-232">更改通知可能不是来自 Microsoft Graph，可能是由恶意参与者发送的。</span><span class="sxs-lookup"><span data-stu-id="7206d-232">It is possible that the change notification has not originated from Microsoft Graph and may have been sent by a rogue actor.</span></span> <span data-ttu-id="7206d-233">您还应调查更改通知的来源，并采取相应的措施。</span><span class="sxs-lookup"><span data-stu-id="7206d-233">You should also investigate where the change notification comes from and take appropriate action.</span></span>

1. <span data-ttu-id="7206d-234">基于业务逻辑更新应用程序。</span><span class="sxs-lookup"><span data-stu-id="7206d-234">Update your application based on your business logic.</span></span>

<span data-ttu-id="7206d-235">对请求中的其他更改通知重复此操作。</span><span class="sxs-lookup"><span data-stu-id="7206d-235">Repeat for other change notifications in the request.</span></span>

## <a name="code-samples"></a><span data-ttu-id="7206d-236">代码示例</span><span class="sxs-lookup"><span data-stu-id="7206d-236">Code samples</span></span>

<span data-ttu-id="7206d-237">可在 GitHub 上获取以下代码示例。</span><span class="sxs-lookup"><span data-stu-id="7206d-237">The following code samples are available on GitHub.</span></span>

- [<span data-ttu-id="7206d-238">Microsoft Graph 培训模块 - 在 Microsoft Graph 中使用变更通知和变更跟踪</span><span class="sxs-lookup"><span data-stu-id="7206d-238">Microsoft Graph Training Module - Using Change Notifications and Track Changes with Microsoft Graph</span></span>](https://github.com/microsoftgraph/msgraph-training-changenotifications)
- [<span data-ttu-id="7206d-239">面向 Node.js 的 Microsoft Graph Webhooks 示例</span><span class="sxs-lookup"><span data-stu-id="7206d-239">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/microsoftgraph/nodejs-webhooks-rest-sample)
- [<span data-ttu-id="7206d-240">适用于 ASP.NET Core 的 Microsoft Graph Webhook 示例</span><span class="sxs-lookup"><span data-stu-id="7206d-240">Microsoft Graph Webhooks Sample for ASP.NET Core</span></span>](https://github.com/microsoftgraph/aspnetcore-webhooks-sample)
- [<span data-ttu-id="7206d-241">面向 Java Spring 的 Microsoft Graph Webhooks 示例</span><span class="sxs-lookup"><span data-stu-id="7206d-241">Microsoft Graph Webhooks Sample for Java Spring</span></span>](https://github.com/microsoftgraph/java-spring-webhooks-sample)

## <a name="firewall-configuration"></a><span data-ttu-id="7206d-242">防火墙配置</span><span class="sxs-lookup"><span data-stu-id="7206d-242">Firewall configuration</span></span>

<span data-ttu-id="7206d-243">可选择性地配置防火墙，以保护通知 URL，仅允许来自 Microsoft Graph 的入站连接。</span><span class="sxs-lookup"><span data-stu-id="7206d-243">You can optionally configure the firewall that protects your notification URL to allow inbound connections only from Microsoft Graph.</span></span> <span data-ttu-id="7206d-244">这使您可以减少发送到通知 URL 的无效更改通知的暴露风险。</span><span class="sxs-lookup"><span data-stu-id="7206d-244">This allows you to reduce further exposure to invalid change notifications that are sent to your notification URL.</span></span> <span data-ttu-id="7206d-245">这些无效的更改通知可尝试触发您实现的自定义逻辑。</span><span class="sxs-lookup"><span data-stu-id="7206d-245">These invalid change notifications can be trying to trigger the custom logic that you implemented.</span></span> <span data-ttu-id="7206d-246">若要获取 Microsoft Graph 用于传递更改通知的 IP 地址的完整列表，请参阅[microsoft 365 的其他终结点](https://docs.microsoft.com/office365/enterprise/additional-office365-ip-addresses-and-urls)。</span><span class="sxs-lookup"><span data-stu-id="7206d-246">For a complete list of IP addresses used by Microsoft Graph to deliver change notifications, see [additional endpoints for Microsoft 365](https://docs.microsoft.com/office365/enterprise/additional-office365-ip-addresses-and-urls).</span></span>

> <span data-ttu-id="7206d-247">**注意：** 用于传递更改通知的已列出 IP 地址可以随时更新，恕不另行通知。</span><span class="sxs-lookup"><span data-stu-id="7206d-247">**Note:** The listed IP addresses that are used to deliver change notifications can be updated at any time without notice.</span></span>

## <a name="see-also"></a><span data-ttu-id="7206d-248">另请参阅</span><span class="sxs-lookup"><span data-stu-id="7206d-248">See also</span></span>

- [<span data-ttu-id="7206d-249">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="7206d-249">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="7206d-250">获取订阅</span><span class="sxs-lookup"><span data-stu-id="7206d-250">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="7206d-251">创建订阅</span><span class="sxs-lookup"><span data-stu-id="7206d-251">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- <span data-ttu-id="7206d-252">[changeNotification](/graph/api/resources/changenotification?view=graph-rest-beta)资源类型</span><span class="sxs-lookup"><span data-stu-id="7206d-252">[changeNotification](/graph/api/resources/changenotification?view=graph-rest-beta) resource type</span></span>
- <span data-ttu-id="7206d-253">[changeNotificationCollection](/graph/api/resources/changenotificationcollection?view=graph-rest-beta)资源类型</span><span class="sxs-lookup"><span data-stu-id="7206d-253">[changeNotificationCollection](/graph/api/resources/changenotificationcollection?view=graph-rest-beta) resource type</span></span>
- [<span data-ttu-id="7206d-254">更改通知和更改跟踪教程</span><span class="sxs-lookup"><span data-stu-id="7206d-254">Change notifications and change tracking tutorial</span></span>](/learn/modules/msgraph-changenotifications-trackchanges)
- [<span data-ttu-id="7206d-255">生命周期通知（预览版）</span><span class="sxs-lookup"><span data-stu-id="7206d-255">Lifecycle notifications (preview)</span></span>](/graph/concepts/webhooks-outlook-authz.md)

[联系人]: /graph/api/resources/contact?view=graph-rest-1.0
[contact]: /graph/api/resources/contact?view=graph-rest-1.0
[对话]: /graph/api/resources/conversation?view=graph-rest-1.0
[conversation]: /graph/api/resources/conversation?view=graph-rest-1.0
[driveItem]: /graph/api/resources/driveitem?view=graph-rest-1.0
[事件]: /graph/api/resources/event?view=graph-rest-1.0
[event]: /graph/api/resources/event?view=graph-rest-1.0
[组]: /graph/api/resources/group?view=graph-rest-1.0
[group]: /graph/api/resources/group?view=graph-rest-1.0
[邮件]: /graph/api/resources/message?view=graph-rest-1.0
[message]: /graph/api/resources/message?view=graph-rest-1.0
[用户]: /graph/api/resources/user?view=graph-rest-1.0
[user]: /graph/api/resources/user?view=graph-rest-1.0
[警报]: /graph/api/resources/alert?view=graph-rest-1.0
[alert]: /graph/api/resources/alert?view=graph-rest-1.0
[callRecord]: /graph/api/resources/callrecords-callrecord?view=graph-rest-1.0
[chatMessage]: /graph/api/resources/chatmessage
