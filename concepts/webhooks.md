---
title: 设置用户数据更改的通知
description: Microsoft Graph API 使用 Webhook 机制将通知传递到客户端。客户端是用于配置自身的 URL 以接收通知的 Web 服务。客户端应用使用通知在更改时更新其状态。
author: baywet
ms.prod: non-product-specific
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 099a5af3dafe3d1f7531f88583236cb1ab381ab7
ms.sourcegitcommit: dbc547a845e507aa934025f9dc73563c13b4fb90
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2020
ms.locfileid: "42606846"
---
# <a name="set-up-notifications-for-changes-in-user-data"></a><span data-ttu-id="84ad7-105">设置用户数据更改的通知</span><span class="sxs-lookup"><span data-stu-id="84ad7-105">Set up notifications for changes in user data</span></span>

<span data-ttu-id="84ad7-p102">Microsoft Graph API 使用 Webhook 机制将通知传递到客户端。客户端是用于配置自身的 URL 以接收通知的 Web 服务。客户端应用使用通知在更改时更新其状态。</span><span class="sxs-lookup"><span data-stu-id="84ad7-p102">The Microsoft Graph API uses a webhook mechanism to deliver notifications to clients. A client is a web service that configures its own URL to receive notifications. Client apps use notifications to update their state upon changes.</span></span>

<span data-ttu-id="84ad7-109">Microsoft Graph 接受订阅请求之后，将通知推送到订阅中指定的 URL。</span><span class="sxs-lookup"><span data-stu-id="84ad7-109">After Microsoft Graph accepts the subscription request, it pushes notifications to the URL specified in the subscription.</span></span> <span data-ttu-id="84ad7-110">然后应用根据其业务逻辑执行操作。</span><span class="sxs-lookup"><span data-stu-id="84ad7-110">The app then takes action according to its business logic.</span></span> <span data-ttu-id="84ad7-111">例如，它提取更多数据、更新缓存和视图等。</span><span class="sxs-lookup"><span data-stu-id="84ad7-111">For example, it fetches more data, updates its cache and views, and so on.</span></span>


> [!VIDEO https://www.youtube-nocookie.com/embed/rC1bunenaq4]
 
> [!div class="nextstepaction"]
> [<span data-ttu-id="84ad7-112">使用 .NET Core 生成 Webhook 应用</span><span class="sxs-lookup"><span data-stu-id="84ad7-112">Build a webhook app with .NET Core</span></span>](/graph/tutorials/change-notifications)

<span data-ttu-id="84ad7-113">默认情况下，更改通知不包含资源数据，`id` 除外。</span><span class="sxs-lookup"><span data-stu-id="84ad7-113">By default, change notifications do not contain resource data, other than the `id`.</span></span> <span data-ttu-id="84ad7-114">如果应用需要资源数据，则可以调用 Microsoft Graph API 以获取完整资源。</span><span class="sxs-lookup"><span data-stu-id="84ad7-114">If the app requires resource data, it can make calls to Microsoft Graph APIs to get the full resource.</span></span> <span data-ttu-id="84ad7-115">本文使用**用户**资源作为使用通知的示例。</span><span class="sxs-lookup"><span data-stu-id="84ad7-115">This article uses the **user** resource as an example for working with notifications.</span></span>

<span data-ttu-id="84ad7-116">应用还可订阅包含资源数据的更改通知，避免执行其他 API 调用来访问数据。</span><span class="sxs-lookup"><span data-stu-id="84ad7-116">An app can also subscribe to change notifications that include resource data, to avoid having to make additonal API calls to access the data.</span></span> <span data-ttu-id="84ad7-117">此类应用将需要实现额外的代码来处理此类通知的要求，具体而言：响应订阅生命周期通知，验证通知的真实性，以及解密资源数据。</span><span class="sxs-lookup"><span data-stu-id="84ad7-117">Such apps will need to implement extra code to handle the requirements of such notifications, specifically: responding to subscription lifecycle notifications, validating the authenticity of notifications, and decrypting the resource data.</span></span> <span data-ttu-id="84ad7-118">将来会有更多资源类型支持此类型的通知。</span><span class="sxs-lookup"><span data-stu-id="84ad7-118">More resource types will support this type of notifications in the future.</span></span> <span data-ttu-id="84ad7-119">有关如何使用这些通知的详细信息，请参阅[设置包含资源数据的更改通知（预览版）](webhooks-with-resource-data.md)。</span><span class="sxs-lookup"><span data-stu-id="84ad7-119">For details about how to work with these notificatios, see [Set up change notifications that include resource data (preview)](webhooks-with-resource-data.md).</span></span>

## <a name="supported-resources"></a><span data-ttu-id="84ad7-120">支持的资源</span><span class="sxs-lookup"><span data-stu-id="84ad7-120">Supported resources</span></span>

<span data-ttu-id="84ad7-121">使用 Microsoft Graph API，应用可以订阅以下资源的更改：</span><span class="sxs-lookup"><span data-stu-id="84ad7-121">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="84ad7-122">Outlook [邮件][]</span><span class="sxs-lookup"><span data-stu-id="84ad7-122">Outlook [message][]</span></span>
- <span data-ttu-id="84ad7-123">Outlook [事件][]</span><span class="sxs-lookup"><span data-stu-id="84ad7-123">Outlook [event][]</span></span>
- <span data-ttu-id="84ad7-124">Outlook 个人[联系人][]</span><span class="sxs-lookup"><span data-stu-id="84ad7-124">Outlook personal [contact][]</span></span>
- <span data-ttu-id="84ad7-125">[用户][]</span><span class="sxs-lookup"><span data-stu-id="84ad7-125">[user][]</span></span>
- <span data-ttu-id="84ad7-126">[组][]</span><span class="sxs-lookup"><span data-stu-id="84ad7-126">[group][]</span></span>
- <span data-ttu-id="84ad7-127">Office 365 组[对话][]</span><span class="sxs-lookup"><span data-stu-id="84ad7-127">Office 365 group [conversation][]</span></span>
- <span data-ttu-id="84ad7-128">用户个人 OneDrive 上_任何_ [driveItem][] 文件夹层次结构内的内容</span><span class="sxs-lookup"><span data-stu-id="84ad7-128">Content within the hierarchy of _any folder_ [driveItem][] on a user's personal OneDrive</span></span>
- <span data-ttu-id="84ad7-129">OneDrive for Business 上 [driveItem][] _根文件夹_层次结构内的内容</span><span class="sxs-lookup"><span data-stu-id="84ad7-129">Content within the hierarchy of the _root folder_ [driveItem][] on OneDrive for Business</span></span>
- <span data-ttu-id="84ad7-130">安全[警报][]</span><span class="sxs-lookup"><span data-stu-id="84ad7-130">Security [alert][]</span></span>
- <span data-ttu-id="84ad7-131">Teams [callRecord][]（预览版）</span><span class="sxs-lookup"><span data-stu-id="84ad7-131">Teams [callRecord][] (preview)</span></span>

<span data-ttu-id="84ad7-132">可以创建对特定 Outlook 文件夹的订阅，例如收件箱：`me/mailFolders('inbox')/messages`</span><span class="sxs-lookup"><span data-stu-id="84ad7-132">You can create a subscription to a specific Outlook folder such as the Inbox: `me/mailFolders('inbox')/messages`</span></span>

<span data-ttu-id="84ad7-133">或以下顶级资源的订阅：`me/messages`、`me/contacts`、`me/events`、`users` 或 `groups`</span><span class="sxs-lookup"><span data-stu-id="84ad7-133">Or to a top-level resource: `me/messages`, `me/contacts`, `me/events`, `users`, or `groups`</span></span>

<span data-ttu-id="84ad7-134">或以下特定资源实例的订阅：`users/{id}`、`groups/{id}`、`groups/{id}/conversations`</span><span class="sxs-lookup"><span data-stu-id="84ad7-134">Or to a specific resource instance: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span></span>

<span data-ttu-id="84ad7-135">或用户个人 OneDrive 中任何文件夹的订阅：`/drives/{id}/root`
`/drives/{id}/root/subfolder`</span><span class="sxs-lookup"><span data-stu-id="84ad7-135">Or to any folder in a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

<span data-ttu-id="84ad7-136">或 SharePoint/OneDrive for Business 驱动器根文件夹的订阅：`/drive/root`</span><span class="sxs-lookup"><span data-stu-id="84ad7-136">Or to the root folder of a SharePoint/OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="84ad7-137">或对新[安全性 API](security-concept-overview.md) 警报的订阅：`/security/alerts?$filter=status eq 'newAlert'`、`/security/alerts?$filter=vendorInformation/provider eq 'ASC'`</span><span class="sxs-lookup"><span data-stu-id="84ad7-137">Or to a new [Security API](security-concept-overview.md) alert: `/security/alerts?$filter=status eq 'newAlert'`, `/security/alerts?$filter=vendorInformation/provider eq 'ASC'`</span></span>

### <a name="azure-ad-resource-limitations"></a><span data-ttu-id="84ad7-138">Azure AD 资源限制</span><span class="sxs-lookup"><span data-stu-id="84ad7-138">Azure AD resource limitations</span></span>

<span data-ttu-id="84ad7-139">基于 Azure AD 的资源（用户、组）采用了某些限制，超出限制时将会产生错误：</span><span class="sxs-lookup"><span data-stu-id="84ad7-139">Certain limits apply to Azure AD based resources (users, groups) and will generate errors when exceeded:</span></span>

> <span data-ttu-id="84ad7-140">**请注意**：这些限制不适用于来自 Azure AD 以外的服务的资源。</span><span class="sxs-lookup"><span data-stu-id="84ad7-140">**Note**: These limits do not apply to resources from services other than Azure AD.</span></span> <span data-ttu-id="84ad7-141">例如，应用可以创建许多更多的 `message` 或 `event` 资源订阅，这些订阅受到 Microsoft Graph 中的 Exchange Online 服务支持。</span><span class="sxs-lookup"><span data-stu-id="84ad7-141">For example, an app can create many more subscriptions to `message` or `event` resources, which are supported by the Exchange Online service as part of Microsoft Graph.</span></span>

- <span data-ttu-id="84ad7-142">最大订阅配额：</span><span class="sxs-lookup"><span data-stu-id="84ad7-142">Maximum subscription quotas:</span></span>

  - <span data-ttu-id="84ad7-143">每个应用：总订阅数 50,000</span><span class="sxs-lookup"><span data-stu-id="84ad7-143">Per app: 50,000 total subscriptions</span></span>
  - <span data-ttu-id="84ad7-144">每个租户：所有应用的总订阅数 1000</span><span class="sxs-lookup"><span data-stu-id="84ad7-144">Per tenant: 1000 total subscriptions across all apps</span></span>
  - <span data-ttu-id="84ad7-145">每个应用和租户组合：总订阅数 100</span><span class="sxs-lookup"><span data-stu-id="84ad7-145">Per app and tenant combination: 100 total subscriptions</span></span>

<span data-ttu-id="84ad7-146">超出限制时，尝试创建订阅将导致[错误响应](errors.md) - `403 Forbidden`。</span><span class="sxs-lookup"><span data-stu-id="84ad7-146">When the limits are exceeded, attempts to create a subscription will result in an [error response](errors.md) - `403 Forbidden`.</span></span> <span data-ttu-id="84ad7-147">`message` 属性将说明已超出什么限制。</span><span class="sxs-lookup"><span data-stu-id="84ad7-147">The `message` property will explain which limit has been exceeded.</span></span>

- <span data-ttu-id="84ad7-148">不支持 Azure AD B2C 租户。</span><span class="sxs-lookup"><span data-stu-id="84ad7-148">Azure AD B2C tenants are not supported.</span></span>

- <span data-ttu-id="84ad7-149">个人 Microsoft 帐户不支持用户实体的通知。</span><span class="sxs-lookup"><span data-stu-id="84ad7-149">Notification for user entities are not supported for personal Microsoft accounts.</span></span>

### <a name="outlook-resource-limitations"></a><span data-ttu-id="84ad7-150">Outlook 资源限制</span><span class="sxs-lookup"><span data-stu-id="84ad7-150">Outlook resource limitations</span></span>

<span data-ttu-id="84ad7-151">订阅 Outlook 资源（如**邮件**、**事件**或**联系人**）时，如果选择使用资源路径中的*用户主体名称* UPN，则在 UPN 包含撇号的情况下，订阅请求可能会失败。</span><span class="sxs-lookup"><span data-stu-id="84ad7-151">When subscribing to Outlook resources such as **messages**, **events** or **contacts**, if you choose to use the *user principal name* UPN in the resource path, the subscription request might fail if the UPN contains an apostrophe.</span></span> <span data-ttu-id="84ad7-152">请考虑使用 GUID 用户 ID 而不是 UPN，以避免遇到此问题。</span><span class="sxs-lookup"><span data-stu-id="84ad7-152">Consider using GUID user IDs instead of UPNs to avoid running into this problem.</span></span> <span data-ttu-id="84ad7-153">例如，请勿使用资源路径：</span><span class="sxs-lookup"><span data-stu-id="84ad7-153">For example, instead of using resource path:</span></span>

`/users/sh.o'neal@contoso.com/messages`

<span data-ttu-id="84ad7-154">请使用：</span><span class="sxs-lookup"><span data-stu-id="84ad7-154">Use:</span></span> 

`/users/{guid-user-id}/messages`

## <a name="subscription-lifetime"></a><span data-ttu-id="84ad7-155">订阅生命周期</span><span class="sxs-lookup"><span data-stu-id="84ad7-155">Subscription lifetime</span></span>

<span data-ttu-id="84ad7-156">订阅的生命周期有限。</span><span class="sxs-lookup"><span data-stu-id="84ad7-156">Subscriptions have a limited lifetime.</span></span> <span data-ttu-id="84ad7-157">应用需要在订阅到期前续订订阅。</span><span class="sxs-lookup"><span data-stu-id="84ad7-157">Apps need to renew their subscriptions before the expiration time.</span></span> <span data-ttu-id="84ad7-158">否则，需要新建订阅。</span><span class="sxs-lookup"><span data-stu-id="84ad7-158">Otherwise, they need to create a new subscription.</span></span> <span data-ttu-id="84ad7-159">有关最长有效期的列表，请参阅[每个资源类型的最长订阅有效期](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type)。</span><span class="sxs-lookup"><span data-stu-id="84ad7-159">For a list of maximum expiration times, see [Maximum length of subscription per resource type](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span></span>

<span data-ttu-id="84ad7-160">应用还可以随时取消订阅，以停止接收通知。</span><span class="sxs-lookup"><span data-stu-id="84ad7-160">Apps can also unsubscribe at any time to stop getting notifications.</span></span>

## <a name="managing-subscriptions"></a><span data-ttu-id="84ad7-161">管理订阅</span><span class="sxs-lookup"><span data-stu-id="84ad7-161">Managing subscriptions</span></span>

<span data-ttu-id="84ad7-162">客户端可以创建订阅、续订订阅和删除订阅。</span><span class="sxs-lookup"><span data-stu-id="84ad7-162">Clients can create subscriptions, renew subscriptions, and delete subscriptions.</span></span>

### <a name="creating-a-subscription"></a><span data-ttu-id="84ad7-163">创建订阅</span><span class="sxs-lookup"><span data-stu-id="84ad7-163">Creating a subscription</span></span>

<span data-ttu-id="84ad7-p110">创建订阅是开始接收资源通知的第一步。订阅流程如下所示：</span><span class="sxs-lookup"><span data-stu-id="84ad7-p110">Creating a subscription is the first step to start receiving notifications for a resource. The subscription process is as follows:</span></span>

1. <span data-ttu-id="84ad7-166">客户端发送特定资源的订阅 (POST) 请求。</span><span class="sxs-lookup"><span data-stu-id="84ad7-166">The client sends a subscription (POST) request for a specific resource.</span></span>

1. <span data-ttu-id="84ad7-167">Microsoft Graph 验证请求。</span><span class="sxs-lookup"><span data-stu-id="84ad7-167">Microsoft Graph verifies the request.</span></span>

    - <span data-ttu-id="84ad7-168">如果请求有效，Microsoft Graph 将验证令牌发送到通知 URL。</span><span class="sxs-lookup"><span data-stu-id="84ad7-168">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
    - <span data-ttu-id="84ad7-169">如果该请求无效，Microsoft Graph 将发送包含代码和详细信息的错误响应。</span><span class="sxs-lookup"><span data-stu-id="84ad7-169">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>

1. <span data-ttu-id="84ad7-170">客户端将验证令牌发送回 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="84ad7-170">The client sends the validation token back to Microsoft Graph.</span></span>

1. <span data-ttu-id="84ad7-171">Microsoft Graph 将响应发送回客户端。</span><span class="sxs-lookup"><span data-stu-id="84ad7-171">The Microsoft Graph sends a response back to the client.</span></span>

<span data-ttu-id="84ad7-172">客户端必须存储订阅 ID 以便将通知与订阅关联。</span><span class="sxs-lookup"><span data-stu-id="84ad7-172">The client must store the subscription ID to correlate notifications with the subscription.</span></span>

#### <a name="subscription-request-example"></a><span data-ttu-id="84ad7-173">订阅请求示例</span><span class="sxs-lookup"><span data-stu-id="84ad7-173">Subscription request example</span></span>

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

<span data-ttu-id="84ad7-174">`changeType`、`notificationUrl`、`resource` 和 `expirationDateTime` 属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="84ad7-174">The `changeType`, `notificationUrl`, `resource`, and `expirationDateTime` properties are required.</span></span> <span data-ttu-id="84ad7-175">如需属性定义和值，请参阅[订阅资源类型](/graph/api/resources/subscription?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="84ad7-175">See [subscription resource type](/graph/api/resources/subscription?view=graph-rest-1.0) for property definitions and values.</span></span>

<span data-ttu-id="84ad7-176">`resource` 属性指定要被监视以进行更改的资源。</span><span class="sxs-lookup"><span data-stu-id="84ad7-176">The `resource` property specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="84ad7-177">例如，可以创建特定邮件文件夹的订阅：`me/mailFolders('inbox')/messages`，或代表由管理员同意的用户：`users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`。</span><span class="sxs-lookup"><span data-stu-id="84ad7-177">For example, you can create a subscription to a specific mail folder: `me/mailFolders('inbox')/messages` or on behalf of a user given by an administrator  consent: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span></span>

<span data-ttu-id="84ad7-178">虽然不需要 `clientState`，但必须包括它才能符合我们建议的通知处理过程。</span><span class="sxs-lookup"><span data-stu-id="84ad7-178">Although `clientState` is not required, you must include it to comply with our recommended notification handling process.</span></span> <span data-ttu-id="84ad7-179">通过设置此属性后，可以确认收到的通知来自 Microsoft Graph 服务。</span><span class="sxs-lookup"><span data-stu-id="84ad7-179">Setting this property will allow you to confirm that notifications you receive originate from the Microsoft Graph service.</span></span> <span data-ttu-id="84ad7-180">因此，该属性的值应保密，并且只有你的应用程序和 Microsoft Graph 服务知道。</span><span class="sxs-lookup"><span data-stu-id="84ad7-180">For this reason, the value of the property should remain secret and known only to your application and the Microsoft Graph service.</span></span>

<span data-ttu-id="84ad7-181">如果成功，Microsoft Graph 将在正文中返回 `201 Created` 代码和 [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) 对象。</span><span class="sxs-lookup"><span data-stu-id="84ad7-181">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span>

#### <a name="notification-endpoint-validation"></a><span data-ttu-id="84ad7-182">通知终结点验证</span><span class="sxs-lookup"><span data-stu-id="84ad7-182">Notification endpoint validation</span></span>

<span data-ttu-id="84ad7-183">Microsoft Graph 在创建订阅之前验证订阅请求的 `notificationUrl` 属性中提供的通知终结点。</span><span class="sxs-lookup"><span data-stu-id="84ad7-183">Microsoft Graph validates the notification endpoint provided in the `notificationUrl` property of the subscription request before creating the subscription.</span></span> <span data-ttu-id="84ad7-184">验证流程如下所示：</span><span class="sxs-lookup"><span data-stu-id="84ad7-184">The validation process occurs as follows:</span></span>

1. <span data-ttu-id="84ad7-185">Microsoft Graph 将 POST 请求发送到通知 URL：</span><span class="sxs-lookup"><span data-stu-id="84ad7-185">Microsoft Graph sends a POST request to the notification URL:</span></span>

    ``` http
    Content-Type: text/plain; charset=utf-8
    POST https://{notificationUrl}?validationToken={opaqueTokenCreatedByMicrosoftGraph}
    ```

    > <span data-ttu-id="84ad7-186">**重要说明：** 由于 `validationToken` 是查询参数，因此客户端必须根据 HTTP 编码做法正确解码它。</span><span class="sxs-lookup"><span data-stu-id="84ad7-186">**Important:** Since the `validationToken` is a query parameter it must be properly decoded by the client, as per HTTP coding practices.</span></span> <span data-ttu-id="84ad7-187">如果客户端没有解码令牌，而是在下一步（响应）中使用已编码值，那么验证将会失败。</span><span class="sxs-lookup"><span data-stu-id="84ad7-187">If the client does not decode the token, and instead uses the encoded value in the next step (response), validation will fail.</span></span> <span data-ttu-id="84ad7-188">此外，客户端还应将令牌值视为不透明，因为令牌格式今后可能会更改，而不另行通知。</span><span class="sxs-lookup"><span data-stu-id="84ad7-188">Also, the client should treat the token value as opaque since the token format may change in the future, without notice.</span></span>

1. <span data-ttu-id="84ad7-189">客户端必须在 10 秒内提供具有以下特性的响应：</span><span class="sxs-lookup"><span data-stu-id="84ad7-189">The client must provide a response with the following characteristics within 10 seconds:</span></span>

    - <span data-ttu-id="84ad7-190">200 (OK) 状态代码。</span><span class="sxs-lookup"><span data-stu-id="84ad7-190">A 200 (OK) status code.</span></span>
    - <span data-ttu-id="84ad7-191">内容类型必须是 `text/plain`。</span><span class="sxs-lookup"><span data-stu-id="84ad7-191">The content type must be `text/plain`.</span></span>
    - <span data-ttu-id="84ad7-192">正文必须包括 Microsoft Graph 提供的验证令牌。</span><span class="sxs-lookup"><span data-stu-id="84ad7-192">The body must include the validation token provided by Microsoft Graph.</span></span>

<span data-ttu-id="84ad7-193">在响应中提供验证令牌之后，客户端应放弃验证令牌。</span><span class="sxs-lookup"><span data-stu-id="84ad7-193">The client should discard the validation token after providing it in the response.</span></span>

### <a name="renewing-a-subscription"></a><span data-ttu-id="84ad7-194">续订订阅</span><span class="sxs-lookup"><span data-stu-id="84ad7-194">Renewing a subscription</span></span>

<span data-ttu-id="84ad7-195">客户端可以续订特定过期日期的订阅，自请求时间起长达三天。</span><span class="sxs-lookup"><span data-stu-id="84ad7-195">The client can renew a subscription with a specific expiration date of up to three days from the time of request.</span></span> <span data-ttu-id="84ad7-196">`expirationDateTime` 属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="84ad7-196">The `expirationDateTime` property is required.</span></span>

#### <a name="subscription-renewal-example"></a><span data-ttu-id="84ad7-197">订阅续订示例</span><span class="sxs-lookup"><span data-stu-id="84ad7-197">Subscription renewal example</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-Type: application/json

{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="84ad7-198">如果成功，Microsoft Graph 将在正文中返回 `200 OK` 代码和 [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) 对象。</span><span class="sxs-lookup"><span data-stu-id="84ad7-198">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span> <span data-ttu-id="84ad7-199">subscription 对象包括新的 `expirationDateTime` 值。</span><span class="sxs-lookup"><span data-stu-id="84ad7-199">The subscription object includes the new `expirationDateTime` value.</span></span>

### <a name="deleting-a-subscription"></a><span data-ttu-id="84ad7-200">删除订阅</span><span class="sxs-lookup"><span data-stu-id="84ad7-200">Deleting a subscription</span></span>

<span data-ttu-id="84ad7-201">客户端可以通过使用其 ID 删除订阅来停止接收通知。</span><span class="sxs-lookup"><span data-stu-id="84ad7-201">The client can stop receiving notifications by deleting the subscription using its ID.</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="84ad7-202">如果成功，Microsoft Graph 将返回 `204 No Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="84ad7-202">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

## <a name="notifications"></a><span data-ttu-id="84ad7-203">通知</span><span class="sxs-lookup"><span data-stu-id="84ad7-203">Notifications</span></span>

<span data-ttu-id="84ad7-204">客户端在创建订阅后开始接收通知。</span><span class="sxs-lookup"><span data-stu-id="84ad7-204">The client starts receiving notifications after creating the subscription.</span></span> <span data-ttu-id="84ad7-205">资源发生更改时，Microsoft Graph 将 POST 请求发送到通知 URL。</span><span class="sxs-lookup"><span data-stu-id="84ad7-205">Microsoft Graph sends a POST request to the notification URL when the resource changes.</span></span> <span data-ttu-id="84ad7-206">仅针对订阅中指定类型的更改发送通知，例如 `created`。</span><span class="sxs-lookup"><span data-stu-id="84ad7-206">Notification are sent only for the changes of the type specified in the subscription, for example, `created`.</span></span>

> <span data-ttu-id="84ad7-207">**注意：** 使用监视同一资源类型并使用同一通知 URL 的多个订阅时，可以发送包含具有不同订阅 ID 的多个通知的 POST。</span><span class="sxs-lookup"><span data-stu-id="84ad7-207">**Note:** When using multiple subscriptions that monitor the same resource type and use the same notification URL, a POST can be sent that will contain multiple notifications with different subscription IDs.</span></span> <span data-ttu-id="84ad7-208">无法保证 POST 中的所有通知都属于单个订阅。</span><span class="sxs-lookup"><span data-stu-id="84ad7-208">There is no guarantee that all notifications in the POST will belong to a single subscription.</span></span>

### <a name="notification-properties"></a><span data-ttu-id="84ad7-209">通知属性</span><span class="sxs-lookup"><span data-stu-id="84ad7-209">Notification properties</span></span>

<span data-ttu-id="84ad7-210">notification 对象具有以下属性：</span><span class="sxs-lookup"><span data-stu-id="84ad7-210">The notification object has the following properties:</span></span>

| <span data-ttu-id="84ad7-211">属性</span><span class="sxs-lookup"><span data-stu-id="84ad7-211">Property</span></span> | <span data-ttu-id="84ad7-212">类型</span><span class="sxs-lookup"><span data-stu-id="84ad7-212">Type</span></span> | <span data-ttu-id="84ad7-213">说明</span><span class="sxs-lookup"><span data-stu-id="84ad7-213">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="84ad7-214">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="84ad7-214">subscriptionId</span></span> | <span data-ttu-id="84ad7-215">string</span><span class="sxs-lookup"><span data-stu-id="84ad7-215">string</span></span> | <span data-ttu-id="84ad7-216">生成通知的订阅的 ID。</span><span class="sxs-lookup"><span data-stu-id="84ad7-216">The ID of the subscription that generated the notification.</span></span> |
| <span data-ttu-id="84ad7-217">subscriptionExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="84ad7-217">subscriptionExpirationDateTime</span></span> | [<span data-ttu-id="84ad7-218">dateTime</span><span class="sxs-lookup"><span data-stu-id="84ad7-218">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="84ad7-219">订阅的过期时间。</span><span class="sxs-lookup"><span data-stu-id="84ad7-219">The expiration time for the subscription.</span></span> |
| <span data-ttu-id="84ad7-220">clientState</span><span class="sxs-lookup"><span data-stu-id="84ad7-220">clientState</span></span> | <span data-ttu-id="84ad7-221">string</span><span class="sxs-lookup"><span data-stu-id="84ad7-221">string</span></span> | <span data-ttu-id="84ad7-222">订阅请求中指定的 `clientState` 属性（如果有）。</span><span class="sxs-lookup"><span data-stu-id="84ad7-222">The `clientState` property specified in the subscription request (if any).</span></span> |
| <span data-ttu-id="84ad7-223">changeType</span><span class="sxs-lookup"><span data-stu-id="84ad7-223">changeType</span></span> | <span data-ttu-id="84ad7-224">string</span><span class="sxs-lookup"><span data-stu-id="84ad7-224">string</span></span> | <span data-ttu-id="84ad7-225">引发通知的事件类型。</span><span class="sxs-lookup"><span data-stu-id="84ad7-225">The event type that caused the notification.</span></span> <span data-ttu-id="84ad7-226">例如，邮件接收时为 `created`，或将邮件标记为已读时为 `updated`。</span><span class="sxs-lookup"><span data-stu-id="84ad7-226">For example, `created` on mail receive, or `updated` on marking a message read.</span></span> |
| <span data-ttu-id="84ad7-227">resource</span><span class="sxs-lookup"><span data-stu-id="84ad7-227">resource</span></span> | <span data-ttu-id="84ad7-228">string</span><span class="sxs-lookup"><span data-stu-id="84ad7-228">string</span></span> | <span data-ttu-id="84ad7-229">资源相对于 `https://graph.microsoft.com` 的 URI。</span><span class="sxs-lookup"><span data-stu-id="84ad7-229">The URI of the resource relative to `https://graph.microsoft.com`.</span></span> |
| <span data-ttu-id="84ad7-230">resourceData</span><span class="sxs-lookup"><span data-stu-id="84ad7-230">resourceData</span></span> | <span data-ttu-id="84ad7-231">object</span><span class="sxs-lookup"><span data-stu-id="84ad7-231">object</span></span> | <span data-ttu-id="84ad7-232">此属性的内容取决于要订阅资源的类型。</span><span class="sxs-lookup"><span data-stu-id="84ad7-232">The content of this property depends on the type of resource being subscribed to.</span></span> |
| <span data-ttu-id="84ad7-233">tenantId</span><span class="sxs-lookup"><span data-stu-id="84ad7-233">tenantId</span></span> | <span data-ttu-id="84ad7-234">string</span><span class="sxs-lookup"><span data-stu-id="84ad7-234">string</span></span> | <span data-ttu-id="84ad7-235">发出通知的租户的 ID。</span><span class="sxs-lookup"><span data-stu-id="84ad7-235">The ID of the tenant the notification originated from.</span></span> |

<span data-ttu-id="84ad7-236">例如，对于 Outlook 资源，`resourceData` 包含以下字段：</span><span class="sxs-lookup"><span data-stu-id="84ad7-236">For example, for Outlook resources, `resourceData` contains the following fields:</span></span>

| <span data-ttu-id="84ad7-237">属性</span><span class="sxs-lookup"><span data-stu-id="84ad7-237">Property</span></span> | <span data-ttu-id="84ad7-238">类型</span><span class="sxs-lookup"><span data-stu-id="84ad7-238">Type</span></span> | <span data-ttu-id="84ad7-239">说明</span><span class="sxs-lookup"><span data-stu-id="84ad7-239">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="84ad7-240">@odata.type</span><span class="sxs-lookup"><span data-stu-id="84ad7-240">@odata.type</span></span> | <span data-ttu-id="84ad7-241">string</span><span class="sxs-lookup"><span data-stu-id="84ad7-241">string</span></span> | <span data-ttu-id="84ad7-242">Microsoft Graph 中描述所表示对象的 OData 实体类型。</span><span class="sxs-lookup"><span data-stu-id="84ad7-242">The OData entity type in Microsoft Graph that describes the represented object.</span></span> |
| <span data-ttu-id="84ad7-243">@odata.id</span><span class="sxs-lookup"><span data-stu-id="84ad7-243">@odata.id</span></span> | <span data-ttu-id="84ad7-244">string</span><span class="sxs-lookup"><span data-stu-id="84ad7-244">string</span></span> | <span data-ttu-id="84ad7-245">对象的 OData 标识符。</span><span class="sxs-lookup"><span data-stu-id="84ad7-245">The OData identifier of the object.</span></span> |
| <span data-ttu-id="84ad7-246">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="84ad7-246">@odata.etag</span></span> | <span data-ttu-id="84ad7-247">string</span><span class="sxs-lookup"><span data-stu-id="84ad7-247">string</span></span> | <span data-ttu-id="84ad7-248">表示对象版本的 HTTP 实体标记。</span><span class="sxs-lookup"><span data-stu-id="84ad7-248">The HTTP entity tag that represents the version of the object.</span></span> |
| <span data-ttu-id="84ad7-249">id</span><span class="sxs-lookup"><span data-stu-id="84ad7-249">id</span></span> | <span data-ttu-id="84ad7-250">string</span><span class="sxs-lookup"><span data-stu-id="84ad7-250">string</span></span> | <span data-ttu-id="84ad7-251">对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="84ad7-251">The identifier of the object.</span></span> |

> <span data-ttu-id="84ad7-252">**注意：**`resourceData` 中提供的 `id` 值在生成通知时有效。</span><span class="sxs-lookup"><span data-stu-id="84ad7-252">**Note:** The `id` value provided in `resourceData` is valid at the time the notification was generated.</span></span> <span data-ttu-id="84ad7-253">某些操作（例如将邮件移动到另一个文件夹）可能会导致 `id` 在处理通知时不再有效。</span><span class="sxs-lookup"><span data-stu-id="84ad7-253">Some actions, such as moving a message to another folder, may result in the `id` no longer being valid when the notification is processed.</span></span>

### <a name="notification-example"></a><span data-ttu-id="84ad7-254">通知示例</span><span class="sxs-lookup"><span data-stu-id="84ad7-254">Notification example</span></span>

<span data-ttu-id="84ad7-255">用户收到电子邮件时，Microsoft Graph 将发送如下所示的通知：</span><span class="sxs-lookup"><span data-stu-id="84ad7-255">When the user receives an email, Microsoft Graph sends a notification like the following:</span></span>

```json
{
  "value": [
    {
      "subscriptionId":"<subscription_guid>",
      "subscriptionExpirationDateTime":"2016-03-19T22:11:09.952Z",
      "clientState":"secretClientValue",
      "changeType":"created",
      "resource":"users/{user_guid}@<tenant_guid>/messages/{long_id_string}",
      "tenantId": "84bd8158-6d4d-4958-8b9f-9d6445542f95",
      "resourceData":
      {
        "@odata.type":"#Microsoft.Graph.Message",
        "@odata.id":"Users/{user_guid}@<tenant_guid>/Messages/{long_id_string}",
        "@odata.etag":"W/\"CQAAABYAAADkrWGo7bouTKlsgTZMr9KwAAAUWRHf\"",
        "id":"<long_id_string>"
      }
    }
  ]
}
```

<span data-ttu-id="84ad7-256">请注意，`value` 字段是一个对象数组。</span><span class="sxs-lookup"><span data-stu-id="84ad7-256">Note the `value` field is an array of objects.</span></span> <span data-ttu-id="84ad7-257">如果有很多排队的通知，Microsoft Graph 可能会在单个请求中发送多个项目。</span><span class="sxs-lookup"><span data-stu-id="84ad7-257">When there are many queued notifications, Microsoft Graph may send multiple items in a single request.</span></span> <span data-ttu-id="84ad7-258">来自不同订阅的通知可以包含在同一通知请求中。</span><span class="sxs-lookup"><span data-stu-id="84ad7-258">Notifications from different subscriptions can be included in the same notification request.</span></span>

### <a name="processing-the-notification"></a><span data-ttu-id="84ad7-259">处理通知</span><span class="sxs-lookup"><span data-stu-id="84ad7-259">Processing the notification</span></span>

<span data-ttu-id="84ad7-260">应处理你的应用收到的每个通知。</span><span class="sxs-lookup"><span data-stu-id="84ad7-260">Each notification received by your app should be processed.</span></span> <span data-ttu-id="84ad7-261">应用程序必须至少执行以下任务来处理通知：</span><span class="sxs-lookup"><span data-stu-id="84ad7-261">The following are the minimum tasks that your app must perform to process a notification:</span></span>

1. <span data-ttu-id="84ad7-262">将响应中的 `202 - Accepted` 状态代码发送到 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="84ad7-262">Send a `202 - Accepted` status code in your response to Microsoft Graph.</span></span> <span data-ttu-id="84ad7-263">如果 Microsoft Graph 未收到 2xx 类代码，它将在大约 4 小时的一段时间内尝试多次发布通知，之后，通知将被删除，且不会发送。</span><span class="sxs-lookup"><span data-stu-id="84ad7-263">If Microsoft Graph doesn't receive a 2xx class code, it will try to publishing the notification a number of times, for a period of about 4 hours; after that, the notification will be dropped and won't be delivered.</span></span>

    > <span data-ttu-id="84ad7-264">**注意：** 收到通知后立即发送 `202 - Accepted` 状态代码，甚至在验证其真实性之前。</span><span class="sxs-lookup"><span data-stu-id="84ad7-264">**Note:** Send a `202 - Accepted` status code as soon as you receive the notification, even before validating its authenticity.</span></span> <span data-ttu-id="84ad7-265">只是确认接收通知，防止不必要的重试。</span><span class="sxs-lookup"><span data-stu-id="84ad7-265">You are simply acknowledging the receipt of the notification and preventing unnecessary retries.</span></span> <span data-ttu-id="84ad7-266">当前超时是 30 秒，但将来可能会减少，以优化服务性能。</span><span class="sxs-lookup"><span data-stu-id="84ad7-266">The current timeout is 30 seconds, but it might be reduced in the future to optimize service performance.</span></span>

1. <span data-ttu-id="84ad7-267">验证 `clientState` 属性。</span><span class="sxs-lookup"><span data-stu-id="84ad7-267">Validate the `clientState` property.</span></span> <span data-ttu-id="84ad7-268">它必须与最初使用订阅创建请求提交的值匹配。</span><span class="sxs-lookup"><span data-stu-id="84ad7-268">It must match the value originally submitted with the subscription creation request.</span></span>

    > <span data-ttu-id="84ad7-269">**注意：** 如果不符合这个条件，无需将其视为有效通知。</span><span class="sxs-lookup"><span data-stu-id="84ad7-269">**Note:** If this isn't true, you should not consider this a valid notification.</span></span> <span data-ttu-id="84ad7-270">通知可能不是来自 Microsoft Graph，并且可能是由未授权操作者发送的。</span><span class="sxs-lookup"><span data-stu-id="84ad7-270">It is possible that the notification has not originated from Microsoft Graph and may have been sent by a rogue actor.</span></span> <span data-ttu-id="84ad7-271">还应调查通知来自何处并采取适当的措施。</span><span class="sxs-lookup"><span data-stu-id="84ad7-271">You should also investigate where the notification comes from and take appropriate action.</span></span>

1. <span data-ttu-id="84ad7-272">基于业务逻辑更新应用程序。</span><span class="sxs-lookup"><span data-stu-id="84ad7-272">Update your application based on your business logic.</span></span>

<span data-ttu-id="84ad7-273">对请求中的其他通知重复该过程。</span><span class="sxs-lookup"><span data-stu-id="84ad7-273">Repeat for other notifications in the request.</span></span>

## <a name="code-samples"></a><span data-ttu-id="84ad7-274">代码示例</span><span class="sxs-lookup"><span data-stu-id="84ad7-274">Code samples</span></span>

<span data-ttu-id="84ad7-275">可在 GitHub 上获取以下代码示例。</span><span class="sxs-lookup"><span data-stu-id="84ad7-275">The following code samples are available on GitHub.</span></span>

- [<span data-ttu-id="84ad7-276">Microsoft Graph 培训模块 - 在 Microsoft Graph 中使用变更通知和变更跟踪</span><span class="sxs-lookup"><span data-stu-id="84ad7-276">Microsoft Graph Training Module - Using Change Notifications and Track Changes with Microsoft Graph</span></span>](https://github.com/microsoftgraph/msgraph-training-changenotifications)
- [<span data-ttu-id="84ad7-277">面向 Node.js 的 Microsoft Graph Webhooks 示例</span><span class="sxs-lookup"><span data-stu-id="84ad7-277">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
- [<span data-ttu-id="84ad7-278">面向 ASP.NET 的 Microsoft Graph Webhooks 示例</span><span class="sxs-lookup"><span data-stu-id="84ad7-278">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)
- [<span data-ttu-id="84ad7-279">使用 WebJobs SDK 的 Microsoft Graph 用户 Webhooks 示例</span><span class="sxs-lookup"><span data-stu-id="84ad7-279">Microsoft Graph User Webhooks Sample using WebJobs SDK</span></span>](https://github.com/microsoftgraph/webjobs-webhooks-sample)

## <a name="see-also"></a><span data-ttu-id="84ad7-280">另请参阅</span><span class="sxs-lookup"><span data-stu-id="84ad7-280">See also</span></span>

- [<span data-ttu-id="84ad7-281">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="84ad7-281">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="84ad7-282">获取订阅</span><span class="sxs-lookup"><span data-stu-id="84ad7-282">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="84ad7-283">创建订阅</span><span class="sxs-lookup"><span data-stu-id="84ad7-283">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [<span data-ttu-id="84ad7-284">更改通知教程</span><span class="sxs-lookup"><span data-stu-id="84ad7-284">Change notifications tutorial</span></span>](/graph/tutorials/change-notifications)
- [<span data-ttu-id="84ad7-285">生命周期通知（预览版）</span><span class="sxs-lookup"><span data-stu-id="84ad7-285">Lifecycle notifications (preview)</span></span>](/graph/concepts/webhooks-outlook-authz.md)

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
[callRecord]: /graph/api/resources/callrecords-callrecord?view=graph-rest-beta
