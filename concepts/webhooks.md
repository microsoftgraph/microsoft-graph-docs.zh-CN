---
title: 设置用户数据更改的通知
description: Microsoft Graph API 使用 Webhook 机制将通知传递到客户端。客户端是用于配置自身的 URL 以接收通知的 Web 服务。客户端应用使用通知在更改时更新其状态。
author: piotrci
ms.openlocfilehash: 6af6f3c54a7956d6a505c88bfc82fc8233dccdad
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337042"
---
# <a name="set-up-notifications-for-changes-in-user-data"></a><span data-ttu-id="20d04-105">设置用户数据更改的通知</span><span class="sxs-lookup"><span data-stu-id="20d04-105">Set up notifications for changes in user data</span></span>

<span data-ttu-id="20d04-p102">Microsoft Graph API 使用 Webhook 机制将通知传递到客户端。客户端是用于配置自身的 URL 以接收通知的 Web 服务。客户端应用使用通知在更改时更新其状态。</span><span class="sxs-lookup"><span data-stu-id="20d04-p102">The Microsoft Graph API uses a webhook mechanism to deliver notifications to clients. A client is a web service that configures its own URL to receive notifications. Client apps use notifications to update their state upon changes.</span></span>

<span data-ttu-id="20d04-109">Microsoft Graph 接受订阅请求之后，将通知推送到订阅中指定的 URL。</span><span class="sxs-lookup"><span data-stu-id="20d04-109">After Microsoft Graph accepts the subscription request, it pushes notifications to the URL specified in the subscription.</span></span> <span data-ttu-id="20d04-110">然后应用根据其业务逻辑执行操作。</span><span class="sxs-lookup"><span data-stu-id="20d04-110">The app then takes action according to its business logic.</span></span> <span data-ttu-id="20d04-111">例如，它将获取更多数据、更新其缓存和视图等。</span><span class="sxs-lookup"><span data-stu-id="20d04-111">For example, it fetches more data, updates its cache and views, etc.</span></span>

## <a name="supported-resources"></a><span data-ttu-id="20d04-112">支持的资源</span><span class="sxs-lookup"><span data-stu-id="20d04-112">Supported resources</span></span>

<span data-ttu-id="20d04-113">使用 Microsoft Graph API，应用可以订阅以下资源的更改：</span><span class="sxs-lookup"><span data-stu-id="20d04-113">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="20d04-114">邮件</span><span class="sxs-lookup"><span data-stu-id="20d04-114">Messages</span></span>
- <span data-ttu-id="20d04-115">事件</span><span class="sxs-lookup"><span data-stu-id="20d04-115">Events</span></span>
- <span data-ttu-id="20d04-116">联系人</span><span class="sxs-lookup"><span data-stu-id="20d04-116">Contacts</span></span>
- <span data-ttu-id="20d04-117">用户</span><span class="sxs-lookup"><span data-stu-id="20d04-117">Users</span></span>
- <span data-ttu-id="20d04-118">组</span><span class="sxs-lookup"><span data-stu-id="20d04-118">Groups</span></span>
- <span data-ttu-id="20d04-119">组对话</span><span class="sxs-lookup"><span data-stu-id="20d04-119">Group conversations</span></span>
- <span data-ttu-id="20d04-120">OneDrive 上共享的内容，包括与 SharePoint 网站关联的驱动器。</span><span class="sxs-lookup"><span data-stu-id="20d04-120">Content shared on OneDrive including drives associated with SharePoint sites</span></span>
- <span data-ttu-id="20d04-121">用户的个人 OneDrive 文件夹</span><span class="sxs-lookup"><span data-stu-id="20d04-121">User's personal OneDrive folders</span></span>
- <span data-ttu-id="20d04-122">安全警报</span><span class="sxs-lookup"><span data-stu-id="20d04-122">Security Alerts</span></span>

<span data-ttu-id="20d04-123">例如，可以创建对特定邮件文件夹的订阅：`me/mailFolders('inbox')/messages`</span><span class="sxs-lookup"><span data-stu-id="20d04-123">For instance, you can create a subscription to a specific mail folder: `me/mailFolders('inbox')/messages`</span></span>

<span data-ttu-id="20d04-124">或以下顶级资源的订阅：`me/messages`、`me/contacts`、`me/events`、`users` 或 `groups`</span><span class="sxs-lookup"><span data-stu-id="20d04-124">Or to a top-level resource: `me/messages`, `me/contacts`, `me/events`, `users`, or `groups`</span></span>

<span data-ttu-id="20d04-125">或以下特定资源实例的订阅：`users/{id}`、`groups/{id}`、`groups/{id}/conversations`</span><span class="sxs-lookup"><span data-stu-id="20d04-125">Or to a specific resource instance: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`</span></span>

<span data-ttu-id="20d04-126">或以下 Sharepoint/OneDrive for Business 驱动器的订阅：`/drive/root`</span><span class="sxs-lookup"><span data-stu-id="20d04-126">Or to a SharePoint/OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="20d04-127">或对用户个人 OneDrive 的订阅：`/drives/{id}/root`
`/drives/{id}/root/subfolder`</span><span class="sxs-lookup"><span data-stu-id="20d04-127">Or to a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

<span data-ttu-id="20d04-128">或对新[安全性 API 警报](security-concept-overview.md)的订阅：`/security/alerts?$filter=status eq ‘New’`、`/security/alerts?$filter=vendorInformation/provider eq ‘ASC’`</span><span class="sxs-lookup"><span data-stu-id="20d04-128">Or to a new [Security API alert](security-concept-overview.md): `/security/alerts?$filter=status eq ‘New’`, `/security/alerts?$filter=vendorInformation/provider eq ‘ASC’`</span></span>

### <a name="azure-ad-resource-limitations"></a><span data-ttu-id="20d04-129">Azure AD 资源限制</span><span class="sxs-lookup"><span data-stu-id="20d04-129">Azure AD resource limitations</span></span>

<span data-ttu-id="20d04-130">基于 Azure AD 的资源（用户、组）采用了某些限制，超出限制时可能会产生错误：</span><span class="sxs-lookup"><span data-stu-id="20d04-130">Certain limits apply to Azure AD based resources (users, groups) and may generate errors when exceeded:</span></span>

- <span data-ttu-id="20d04-131">最大订阅配额：</span><span class="sxs-lookup"><span data-stu-id="20d04-131">Maximum subscription quotas:</span></span>

  - <span data-ttu-id="20d04-132">每个应用：总订阅数 50,000</span><span class="sxs-lookup"><span data-stu-id="20d04-132">Per app: 50,000 total subscriptions</span></span>
  - <span data-ttu-id="20d04-133">每个租户：所有应用的总订阅数 35</span><span class="sxs-lookup"><span data-stu-id="20d04-133">Per tenant: 35 total subscriptions across all apps</span></span>
  - <span data-ttu-id="20d04-134">每个应用和租户组合：总订阅数 7</span><span class="sxs-lookup"><span data-stu-id="20d04-134">Per app and tenant combination: 7 total subscriptions</span></span>

- <span data-ttu-id="20d04-135">不支持 Azure AD B2C 租户。</span><span class="sxs-lookup"><span data-stu-id="20d04-135">Azure AD B2C tenants are not supported.</span></span>

- <span data-ttu-id="20d04-136">个人 Microsoft 帐户不支持用户实体的通知。</span><span class="sxs-lookup"><span data-stu-id="20d04-136">Notification for user entities are not supported for personal Microsoft accounts.</span></span>

## <a name="subscription-lifetime"></a><span data-ttu-id="20d04-137">订阅生命周期</span><span class="sxs-lookup"><span data-stu-id="20d04-137">Subscription lifetime</span></span>

<span data-ttu-id="20d04-138">订阅的生命周期有限。</span><span class="sxs-lookup"><span data-stu-id="20d04-138">Subscriptions have a limited lifetime.</span></span> <span data-ttu-id="20d04-139">应用需要在订阅到期前续订订阅。</span><span class="sxs-lookup"><span data-stu-id="20d04-139">Apps need to renew their subscriptions before the expiration time.</span></span> <span data-ttu-id="20d04-140">否则，需要新建订阅。</span><span class="sxs-lookup"><span data-stu-id="20d04-140">Otherwise, they need to create a new subscription.</span></span> <span data-ttu-id="20d04-141">有关最长有效期的列表，请参阅[每个资源类型的最长订阅有效期](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type)。</span><span class="sxs-lookup"><span data-stu-id="20d04-141">For a list of maximum expiration times, see [Maximum length of subscription per resource type](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).</span></span>

<span data-ttu-id="20d04-142">应用还可以随时取消订阅，以停止接收通知。</span><span class="sxs-lookup"><span data-stu-id="20d04-142">Apps can also unsubscribe at any time to stop getting notifications.</span></span>

## <a name="managing-subscriptions"></a><span data-ttu-id="20d04-143">管理订阅</span><span class="sxs-lookup"><span data-stu-id="20d04-143">Managing subscriptions</span></span>

<span data-ttu-id="20d04-144">客户端可以创建订阅、续订订阅和删除订阅。</span><span class="sxs-lookup"><span data-stu-id="20d04-144">Clients can create subscriptions, renew subscriptions, and delete subscriptions.</span></span>

### <a name="creating-a-subscription"></a><span data-ttu-id="20d04-145">创建订阅</span><span class="sxs-lookup"><span data-stu-id="20d04-145">Creating a subscription</span></span>

<span data-ttu-id="20d04-p105">创建订阅是开始接收资源通知的第一步。订阅流程如下所示：</span><span class="sxs-lookup"><span data-stu-id="20d04-p105">Creating a subscription is the first step to start receiving notifications for a resource. The subscription process is as follows:</span></span>

1. <span data-ttu-id="20d04-148">客户端发送特定资源的订阅 (POST) 请求。</span><span class="sxs-lookup"><span data-stu-id="20d04-148">The client sends a subscription (POST) request for a specific resource.</span></span>

1. <span data-ttu-id="20d04-149">Microsoft Graph 验证请求。</span><span class="sxs-lookup"><span data-stu-id="20d04-149">Microsoft Graph verifies the request.</span></span>

    - <span data-ttu-id="20d04-150">如果请求有效，Microsoft Graph 将验证令牌发送到通知 URL。</span><span class="sxs-lookup"><span data-stu-id="20d04-150">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
    - <span data-ttu-id="20d04-151">如果该请求无效，Microsoft Graph 将发送包含代码和详细信息的错误响应。</span><span class="sxs-lookup"><span data-stu-id="20d04-151">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>

1. <span data-ttu-id="20d04-152">客户端将验证令牌发送回 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="20d04-152">The client sends the validation token back to Microsoft Graph.</span></span>

1. <span data-ttu-id="20d04-153">Microsoft Graph 将响应发送回客户端。</span><span class="sxs-lookup"><span data-stu-id="20d04-153">The Microsoft Graph sends a response back to the client.</span></span>

<span data-ttu-id="20d04-154">客户端必须存储订阅 ID 以便将通知与订阅关联。</span><span class="sxs-lookup"><span data-stu-id="20d04-154">The client must store the subscription ID to correlate notifications with the subscription.</span></span>

#### <a name="subscription-request-example"></a><span data-ttu-id="20d04-155">订阅请求示例</span><span class="sxs-lookup"><span data-stu-id="20d04-155">Subscription request example</span></span>

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

<span data-ttu-id="20d04-156">`changeType`、`notificationUrl`、`resource` 和 `expirationDateTime` 属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="20d04-156">The `changeType`, `notificationUrl`, `resource`, and `expirationDateTime` properties are required.</span></span> <span data-ttu-id="20d04-157">如需属性定义和值，请参阅[订阅资源类型](/graph/api/resources/subscription?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="20d04-157">See [subscription resource type](/graph/api/resources/subscription?view=graph-rest-1.0) for property definitions and values.</span></span>

<span data-ttu-id="20d04-158">`resource` 属性指定要被监视以进行更改的资源。</span><span class="sxs-lookup"><span data-stu-id="20d04-158">The `resource` property specifies the resource that will be monitored for changes.</span></span> <span data-ttu-id="20d04-159">例如，可以创建特定邮件文件夹的订阅：`me/mailFolders('inbox')/messages`，或代表由管理员同意的用户：`users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`。</span><span class="sxs-lookup"><span data-stu-id="20d04-159">For example, you can create a subscription to a specific mail folder: `me/mailFolders('inbox')/messages` or on behalf of a user given by an administrator  consent: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.</span></span>

<span data-ttu-id="20d04-160">虽然不需要 `clientState`，但必须包括它才能符合我们建议的通知处理过程。</span><span class="sxs-lookup"><span data-stu-id="20d04-160">Although `clientState` is not required, you must include it to comply with our recommended notification handling process.</span></span> <span data-ttu-id="20d04-161">通过设置此属性后，可以确认收到的通知来自 Microsoft Graph 服务。</span><span class="sxs-lookup"><span data-stu-id="20d04-161">Setting this property will allow you to confirm that notifications you receive originate from the Microsoft Graph service.</span></span> <span data-ttu-id="20d04-162">因此，该属性的值应保密，并且只有你的应用程序和 Microsoft Graph 服务知道。</span><span class="sxs-lookup"><span data-stu-id="20d04-162">For this reason, the value of the property should remain secret and known only to your application and the Microsoft Graph service.</span></span>

<span data-ttu-id="20d04-163">如果成功，Microsoft Graph 将在正文中返回 `201 Created` 代码和 [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) 对象。</span><span class="sxs-lookup"><span data-stu-id="20d04-163">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span>

#### <a name="notification-endpoint-validation"></a><span data-ttu-id="20d04-164">通知终结点验证</span><span class="sxs-lookup"><span data-stu-id="20d04-164">Notification endpoint validation</span></span>

<span data-ttu-id="20d04-165">Microsoft Graph 在创建订阅之前验证订阅请求的 `notificationUrl` 属性中提供的通知终结点。</span><span class="sxs-lookup"><span data-stu-id="20d04-165">Microsoft Graph validates the notification endpoint provided in the `notificationUrl` property of the subscription request before creating the subscription.</span></span> <span data-ttu-id="20d04-166">验证流程如下所示：</span><span class="sxs-lookup"><span data-stu-id="20d04-166">The validation process occurs as follows:</span></span>

1. <span data-ttu-id="20d04-167">Microsoft Graph 将 POST 请求发送到通知 URL：</span><span class="sxs-lookup"><span data-stu-id="20d04-167">Microsoft Graph sends a POST request to the notification URL:</span></span>

    ``` http
    POST https://{notificationUrl}?validationToken={opaqueTokenCreatedByMicrosoftGraph}
    ```

    > <span data-ttu-id="20d04-168">**重要说明：** 由于 `validationToken` 是查询参数，因此客户端必须根据 HTTP 编码做法正确解码它。</span><span class="sxs-lookup"><span data-stu-id="20d04-168">**Important:** Since the `validationToken` is a query parameter it must be properly decoded by the client, as per HTTP coding practices.</span></span> <span data-ttu-id="20d04-169">如果客户端没有解码令牌，而是在下一步（响应）中使用已编码值，那么验证将会失败。</span><span class="sxs-lookup"><span data-stu-id="20d04-169">If the client does not decode the token, and instead uses the encoded value in the next step (response), validation will fail.</span></span> <span data-ttu-id="20d04-170">此外，客户端还应将令牌值视为不透明，因为令牌格式今后可能会更改，而不另行通知。</span><span class="sxs-lookup"><span data-stu-id="20d04-170">Also, the client should treat the token value as opaque since the token format may change in the future, without notice.</span></span>

1. <span data-ttu-id="20d04-171">客户端必须在 10 秒内提供具有以下特性的响应：</span><span class="sxs-lookup"><span data-stu-id="20d04-171">The client must provide a response with the following characteristics within 10 seconds:</span></span>

    - <span data-ttu-id="20d04-172">200 (OK) 状态代码。</span><span class="sxs-lookup"><span data-stu-id="20d04-172">A 200 (OK) status code.</span></span>
    - <span data-ttu-id="20d04-173">内容类型必须是 `text/plain`。</span><span class="sxs-lookup"><span data-stu-id="20d04-173">The content type must be `text/plain`.</span></span>
    - <span data-ttu-id="20d04-174">正文必须包括 Microsoft Graph 提供的验证令牌。</span><span class="sxs-lookup"><span data-stu-id="20d04-174">The body must include the validation token provided by Microsoft Graph.</span></span>

<span data-ttu-id="20d04-175">在响应中提供验证令牌之后，客户端应放弃验证令牌。</span><span class="sxs-lookup"><span data-stu-id="20d04-175">The client should discard the validation token after providing it in the response.</span></span>

### <a name="renewing-a-subscription"></a><span data-ttu-id="20d04-176">续订订阅</span><span class="sxs-lookup"><span data-stu-id="20d04-176">Renewing a subscription</span></span>

<span data-ttu-id="20d04-177">客户端可以续订特定过期日期的订阅，自请求时间起长达三天。</span><span class="sxs-lookup"><span data-stu-id="20d04-177">The client can renew a subscription with a specific expiration date of up to three days from the time of request.</span></span> <span data-ttu-id="20d04-178">`expirationDateTime` 属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="20d04-178">The `expirationDateTime` property is required.</span></span>

#### <a name="subscription-renewal-example"></a><span data-ttu-id="20d04-179">订阅续订示例</span><span class="sxs-lookup"><span data-stu-id="20d04-179">Subscription renewal example</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-Type: application/json

{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="20d04-180">如果成功，Microsoft Graph 将在正文中返回 `200 OK` 代码和 [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) 对象。</span><span class="sxs-lookup"><span data-stu-id="20d04-180">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) object in the body.</span></span> <span data-ttu-id="20d04-181">subscription 对象包括新的 `expirationDateTime` 值。</span><span class="sxs-lookup"><span data-stu-id="20d04-181">The subscription object includes the new `expirationDateTime` value.</span></span>

### <a name="deleting-a-subscription"></a><span data-ttu-id="20d04-182">删除订阅</span><span class="sxs-lookup"><span data-stu-id="20d04-182">Deleting a subscription</span></span>

<span data-ttu-id="20d04-183">客户端可以通过使用其 ID 删除订阅来停止接收通知。</span><span class="sxs-lookup"><span data-stu-id="20d04-183">The client can stop receiving notifications by deleting the subscription using its ID.</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="20d04-184">如果成功，Microsoft Graph 将返回 `204 No Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="20d04-184">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

## <a name="notifications"></a><span data-ttu-id="20d04-185">通知</span><span class="sxs-lookup"><span data-stu-id="20d04-185">Notifications</span></span>

<span data-ttu-id="20d04-186">客户端在创建订阅后开始接收通知。</span><span class="sxs-lookup"><span data-stu-id="20d04-186">The client starts receiving notifications after creating the subscription.</span></span> <span data-ttu-id="20d04-187">资源发生更改时，Microsoft Graph 将 POST 请求发送到通知 URL。</span><span class="sxs-lookup"><span data-stu-id="20d04-187">Microsoft Graph sends a POST request to the notification URL when the resource changes.</span></span> <span data-ttu-id="20d04-188">仅针对订阅中指定类型的更改发送通知，例如 `created`。</span><span class="sxs-lookup"><span data-stu-id="20d04-188">Notification are sent only for the changes of the type specified in the subscription, for example, `created`.</span></span>

> <span data-ttu-id="20d04-189">**注意：** 使用监视同一资源类型并使用同一通知 URL 的多个订阅时，可以发送包含具有不同订阅 ID 的多个通知的 POST。</span><span class="sxs-lookup"><span data-stu-id="20d04-189">**Note:** When using multiple subscriptions that monitor the same resource type and use the same notification URL, a POST can be sent that will contain multiple notifications with different subscription IDs.</span></span> <span data-ttu-id="20d04-190">无法保证 POST 中的所有通知都属于单个订阅。</span><span class="sxs-lookup"><span data-stu-id="20d04-190">There is no guarantee that all notifications in the POST will belong to a single subscription.</span></span>

### <a name="notification-properties"></a><span data-ttu-id="20d04-191">通知属性</span><span class="sxs-lookup"><span data-stu-id="20d04-191">Notification properties</span></span>

<span data-ttu-id="20d04-192">notification 对象具有以下属性：</span><span class="sxs-lookup"><span data-stu-id="20d04-192">The notification object has the following properties:</span></span>

| <span data-ttu-id="20d04-193">属性</span><span class="sxs-lookup"><span data-stu-id="20d04-193">Property</span></span> | <span data-ttu-id="20d04-194">类型</span><span class="sxs-lookup"><span data-stu-id="20d04-194">Type</span></span> | <span data-ttu-id="20d04-195">说明</span><span class="sxs-lookup"><span data-stu-id="20d04-195">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="20d04-196">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="20d04-196">subscriptionId</span></span> | <span data-ttu-id="20d04-197">string</span><span class="sxs-lookup"><span data-stu-id="20d04-197">string</span></span> | <span data-ttu-id="20d04-198">生成通知的订阅的 ID。</span><span class="sxs-lookup"><span data-stu-id="20d04-198">The ID of the subscription that generated the notification.</span></span> |
| <span data-ttu-id="20d04-199">subscriptionExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="20d04-199">subscriptionExpirationDateTime</span></span> | [<span data-ttu-id="20d04-200">dateTime</span><span class="sxs-lookup"><span data-stu-id="20d04-200">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="20d04-201">订阅的过期时间。</span><span class="sxs-lookup"><span data-stu-id="20d04-201">The expiration time for the subscription.</span></span> |
| <span data-ttu-id="20d04-202">clientState</span><span class="sxs-lookup"><span data-stu-id="20d04-202">clientState</span></span> | <span data-ttu-id="20d04-203">string</span><span class="sxs-lookup"><span data-stu-id="20d04-203">string</span></span> | <span data-ttu-id="20d04-204">订阅请求中指定的 `clientState` 属性（如果有）。</span><span class="sxs-lookup"><span data-stu-id="20d04-204">The `clientState` property specified in the subscription request (if any).</span></span> |
| <span data-ttu-id="20d04-205">changeType</span><span class="sxs-lookup"><span data-stu-id="20d04-205">changeType</span></span> | <span data-ttu-id="20d04-206">string</span><span class="sxs-lookup"><span data-stu-id="20d04-206">string</span></span> | <span data-ttu-id="20d04-207">引发通知的事件类型。</span><span class="sxs-lookup"><span data-stu-id="20d04-207">The event type that caused the notification.</span></span> <span data-ttu-id="20d04-208">例如，邮件接收时为 `created`，或将邮件标记为已读时为 `updated`。</span><span class="sxs-lookup"><span data-stu-id="20d04-208">For example, `created` on mail receive, or `updated` on marking a message read.</span></span> |
| <span data-ttu-id="20d04-209">resource</span><span class="sxs-lookup"><span data-stu-id="20d04-209">resource</span></span> | <span data-ttu-id="20d04-210">string</span><span class="sxs-lookup"><span data-stu-id="20d04-210">string</span></span> | <span data-ttu-id="20d04-211">资源相对于 `https://graph.microsoft.com` 的 URI。</span><span class="sxs-lookup"><span data-stu-id="20d04-211">The URI of the resource relative to `https://graph.microsoft.com`.</span></span> |
| <span data-ttu-id="20d04-212">resourceData</span><span class="sxs-lookup"><span data-stu-id="20d04-212">resourceData</span></span> | <span data-ttu-id="20d04-213">object</span><span class="sxs-lookup"><span data-stu-id="20d04-213">object</span></span> | <span data-ttu-id="20d04-214">此属性的内容取决于要订阅资源的类型。</span><span class="sxs-lookup"><span data-stu-id="20d04-214">The content of this property depends on the type of resource being subscribed to.</span></span> |

<span data-ttu-id="20d04-215">例如，对于 Outlook 资源，`resourceData` 包含以下字段：</span><span class="sxs-lookup"><span data-stu-id="20d04-215">For example, for Outlook resources, `resourceData` contains the following fields:</span></span>

| <span data-ttu-id="20d04-216">属性</span><span class="sxs-lookup"><span data-stu-id="20d04-216">Property</span></span> | <span data-ttu-id="20d04-217">类型</span><span class="sxs-lookup"><span data-stu-id="20d04-217">Type</span></span> | <span data-ttu-id="20d04-218">说明</span><span class="sxs-lookup"><span data-stu-id="20d04-218">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="20d04-219">@odata.type</span><span class="sxs-lookup"><span data-stu-id="20d04-219">@odata.type</span></span> | <span data-ttu-id="20d04-220">string</span><span class="sxs-lookup"><span data-stu-id="20d04-220">string</span></span> | <span data-ttu-id="20d04-221">Microsoft Graph 中描述所表示对象的 OData 实体类型。</span><span class="sxs-lookup"><span data-stu-id="20d04-221">The OData entity type in Microsoft Graph that describes the represented object.</span></span> |
| <span data-ttu-id="20d04-222">@odata.id</span><span class="sxs-lookup"><span data-stu-id="20d04-222">@odata.id</span></span> | <span data-ttu-id="20d04-223">string</span><span class="sxs-lookup"><span data-stu-id="20d04-223">string</span></span> | <span data-ttu-id="20d04-224">对象的 OData 标识符。</span><span class="sxs-lookup"><span data-stu-id="20d04-224">The OData identifier of the object.</span></span> |
| <span data-ttu-id="20d04-225">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="20d04-225">@odata.etag</span></span> | <span data-ttu-id="20d04-226">string</span><span class="sxs-lookup"><span data-stu-id="20d04-226">string</span></span> | <span data-ttu-id="20d04-227">表示对象版本的 HTTP 实体标记。</span><span class="sxs-lookup"><span data-stu-id="20d04-227">The HTTP entity tag that represents the version of the object.</span></span> |
| <span data-ttu-id="20d04-228">id</span><span class="sxs-lookup"><span data-stu-id="20d04-228">id</span></span> | <span data-ttu-id="20d04-229">string</span><span class="sxs-lookup"><span data-stu-id="20d04-229">string</span></span> | <span data-ttu-id="20d04-230">对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="20d04-230">The identifier of the object.</span></span> |

> <span data-ttu-id="20d04-231">**注意：**`resourceData` 中提供的 `id` 值在生成通知时有效。</span><span class="sxs-lookup"><span data-stu-id="20d04-231">**Note:** The `id` value provided in `resourceData` is valid at the time the notification was generated.</span></span> <span data-ttu-id="20d04-232">某些操作（例如将邮件移动到另一个文件夹）可能会导致 `id` 在处理通知时不再有效。</span><span class="sxs-lookup"><span data-stu-id="20d04-232">Some actions, such as moving a message to another folder, may result in the `id` no longer being valid when the notification is processed.</span></span>

### <a name="notification-example"></a><span data-ttu-id="20d04-233">通知示例</span><span class="sxs-lookup"><span data-stu-id="20d04-233">Notification example</span></span>

<span data-ttu-id="20d04-234">用户收到电子邮件时，Microsoft Graph 将发送如下所示的通知：</span><span class="sxs-lookup"><span data-stu-id="20d04-234">When the user receives an email, Microsoft Graph sends a notification like the following:</span></span>

```json
{
  "value": [
    {
      "subscriptionId":"<subscription_guid>",
      "subscriptionExpirationDateTime":"2016-03-19T22:11:09.952Z",
      "clientState":"secretClientValue",
      "changeType":"created",
      "resource":"users/{user_guid}@<tenant_guid>/messages/{long_id_string}",
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

<span data-ttu-id="20d04-235">请注意，`value` 字段是一个对象数组。</span><span class="sxs-lookup"><span data-stu-id="20d04-235">Note the `value` field is an array of objects.</span></span> <span data-ttu-id="20d04-236">如果有很多排队的通知，Microsoft Graph 可能会在单个请求中发送多个项目。</span><span class="sxs-lookup"><span data-stu-id="20d04-236">When there are many queued notifications, Microsoft Graph may send multiple items in a single request.</span></span> <span data-ttu-id="20d04-237">来自不同订阅的通知可以包含在同一通知请求中。</span><span class="sxs-lookup"><span data-stu-id="20d04-237">Notifications from different subscriptions can be included in the same notification request.</span></span>

### <a name="processing-the-notification"></a><span data-ttu-id="20d04-238">处理通知</span><span class="sxs-lookup"><span data-stu-id="20d04-238">Processing the notification</span></span>

<span data-ttu-id="20d04-239">应处理你的应用收到的每个通知。</span><span class="sxs-lookup"><span data-stu-id="20d04-239">Each notification received by your app should be processed.</span></span> <span data-ttu-id="20d04-240">应用程序必须至少执行以下任务来处理通知：</span><span class="sxs-lookup"><span data-stu-id="20d04-240">The following are the minimum tasks that your app must perform to process a notification:</span></span>

1. <span data-ttu-id="20d04-241">验证 `clientState` 属性。</span><span class="sxs-lookup"><span data-stu-id="20d04-241">Validate the `clientState` property.</span></span> <span data-ttu-id="20d04-242">它必须与最初使用订阅创建请求提交的值匹配。</span><span class="sxs-lookup"><span data-stu-id="20d04-242">It must match the value originally submitted with the subscription creation request.</span></span>

    > <span data-ttu-id="20d04-243">**注意：** 如果不符合这个条件，无需将其视为有效通知。</span><span class="sxs-lookup"><span data-stu-id="20d04-243">**Note:** If this isn't true, you should not consider this a valid notification.</span></span> <span data-ttu-id="20d04-244">通知可能不是来自 Microsoft Graph，并且可能是由未授权操作者发送的。</span><span class="sxs-lookup"><span data-stu-id="20d04-244">It is possible that the notification has not originated from Microsoft Graph and may have been sent by a rogue actor.</span></span> <span data-ttu-id="20d04-245">还应调查通知来自何处并采取适当的措施。</span><span class="sxs-lookup"><span data-stu-id="20d04-245">You should also investigate where the notification comes from and take appropriate action.</span></span>

1. <span data-ttu-id="20d04-246">基于业务逻辑更新应用程序。</span><span class="sxs-lookup"><span data-stu-id="20d04-246">Update your application based on your business logic.</span></span>

1. <span data-ttu-id="20d04-247">将响应中的 `202 - Accepted` 状态代码发送到 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="20d04-247">Send a `202 - Accepted` status code in your response to Microsoft Graph.</span></span> <span data-ttu-id="20d04-248">如果 Microsoft Graph 没有收到 2xx 类代码，它将重试多次发送通知。</span><span class="sxs-lookup"><span data-stu-id="20d04-248">If Microsoft Graph doesn't receive a 2xx class code, it will retry the notification a number of times.</span></span>

    > <span data-ttu-id="20d04-249">**注意：** 即使 `clientState` 属性与订阅请求提交的属性不匹配，也应发送 `202 - Accepted` 状态代码。</span><span class="sxs-lookup"><span data-stu-id="20d04-249">**Note:** You should send a `202 - Accepted` status code even if the `clientState` property doesn't match the one submitted with the subscription request.</span></span> <span data-ttu-id="20d04-250">这是一个很好的做法，因为它可以防止潜在的未授权操作者发现你可能不信任他们的通知，并且可能使用该信息来猜测 `clientState` 属性的值。</span><span class="sxs-lookup"><span data-stu-id="20d04-250">This is a good practice as it prevents a potential rogue actor from discovering the fact that you may not trust their notifications, and perhaps using that information to guess the value of the `clientState` property.</span></span>

<span data-ttu-id="20d04-251">对请求中的其他通知重复该过程。</span><span class="sxs-lookup"><span data-stu-id="20d04-251">Repeat for other notifications in the request.</span></span>

## <a name="code-samples"></a><span data-ttu-id="20d04-252">代码示例</span><span class="sxs-lookup"><span data-stu-id="20d04-252">Code samples</span></span>

<span data-ttu-id="20d04-253">可在 GitHub 上获取以下代码示例。</span><span class="sxs-lookup"><span data-stu-id="20d04-253">The following code samples are available on GitHub.</span></span>

- [<span data-ttu-id="20d04-254">面向 Node.js 的 Microsoft Graph Webhooks 示例</span><span class="sxs-lookup"><span data-stu-id="20d04-254">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
- [<span data-ttu-id="20d04-255">面向 ASP.NET 的 Microsoft Graph Webhooks 示例</span><span class="sxs-lookup"><span data-stu-id="20d04-255">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)
- [<span data-ttu-id="20d04-256">使用 WebJobs SDK 的 Microsoft Graph 用户 Webhooks 示例</span><span class="sxs-lookup"><span data-stu-id="20d04-256">Microsoft Graph User Webhooks Sample using WebJobs SDK</span></span>](https://github.com/microsoftgraph/webjobs-webhooks-sample)

## <a name="see-also"></a><span data-ttu-id="20d04-257">另请参阅</span><span class="sxs-lookup"><span data-stu-id="20d04-257">See also</span></span>

- [<span data-ttu-id="20d04-258">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="20d04-258">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="20d04-259">获取订阅</span><span class="sxs-lookup"><span data-stu-id="20d04-259">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="20d04-260">创建订阅</span><span class="sxs-lookup"><span data-stu-id="20d04-260">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)

[contact]: /graph/api/resources/contact?view=graph-rest-1.0
[conversation]: /graph/api/resources/conversation?view=graph-rest-1.0
[drive]: /graph/api/resources/drive?view=graph-rest-1.0
[event]: /graph/api/resources/event?view=graph-rest-1.0
[message]: /graph/api/resources/message?view=graph-rest-1.0
