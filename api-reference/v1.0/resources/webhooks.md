# <a name="working-with-webhooks-in-microsoft-graph"></a><span data-ttu-id="91e58-101">在 Microsoft Graph 中使用 Webhooks</span><span class="sxs-lookup"><span data-stu-id="91e58-101">Working with Webhooks in Microsoft Graph</span></span>

<span data-ttu-id="91e58-p101">Microsoft Graph REST API 使用 Webhook 机制来将通知传递到客户端。客户端是用于配置自身的 URL 以接收通知的 Web 服务。客户端应用使用通知在更改时更新其状态。</span><span class="sxs-lookup"><span data-stu-id="91e58-p101">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients. A client is a web service that configures its own URL to receive notifications. Client apps use notifications to update their state upon changes.</span></span>

<span data-ttu-id="91e58-105">使用 Microsoft Graph REST API，应用可以订阅以下资源的更改：</span><span class="sxs-lookup"><span data-stu-id="91e58-105">Using the Microsoft Graph REST API, an app can subscribe to changes on the following resources:</span></span>

* <span data-ttu-id="91e58-106">邮件</span><span class="sxs-lookup"><span data-stu-id="91e58-106">Messages</span></span>
* <span data-ttu-id="91e58-107">事件</span><span class="sxs-lookup"><span data-stu-id="91e58-107">Events</span></span>
* <span data-ttu-id="91e58-108">联系人</span><span class="sxs-lookup"><span data-stu-id="91e58-108">Contacts</span></span>
* <span data-ttu-id="91e58-109">组对话</span><span class="sxs-lookup"><span data-stu-id="91e58-109">Group conversations</span></span>
* <span data-ttu-id="91e58-110">OneDrive 上共享的内容，包括与 SharePoint 网站关联的驱动器。</span><span class="sxs-lookup"><span data-stu-id="91e58-110">Content shared on OneDrive including drives associated with SharePoint sites</span></span>
* <span data-ttu-id="91e58-111">用户的个人 OneDrive 文件夹</span><span class="sxs-lookup"><span data-stu-id="91e58-111">User's personal OneDrive folders</span></span>

<span data-ttu-id="91e58-112">例如，可以创建以下特定文件夹的订阅：`me/mailfolders('inbox')/messages`</span><span class="sxs-lookup"><span data-stu-id="91e58-112">You can create a subscription to a specific folder: `me/mailfolders('inbox')/messages`</span></span>

<span data-ttu-id="91e58-113">或以下顶级资源的订阅：`me/messages`、`me/contacts`、`me/events`</span><span class="sxs-lookup"><span data-stu-id="91e58-113">Or to a top-level resource: `me/messages`</span></span>

<span data-ttu-id="91e58-114">或以下 Sharepoint / OneDrive for Business 驱动器的订阅：`/drive/root`</span><span class="sxs-lookup"><span data-stu-id="91e58-114">Or on a Sharepoint / OneDrive for Business drive: `/drive/root`</span></span>

<span data-ttu-id="91e58-115">或以下用户个人 OneDrive 的订阅：`/drives/{id}/root`
`/drives/{id}/root/subfolder`</span><span class="sxs-lookup"><span data-stu-id="91e58-115">Or on a user's personal OneDrive: `/drives/{id}/root`
`/drives/{id}/root/subfolder`</span></span>

<span data-ttu-id="91e58-p102">Microsoft Graph 接受订阅请求之后，它将通知推送到订阅中指定的 URL。然后应用程序根据其业务逻辑执行操作。例如，它获取更多数据，更新缓存和视图等。</span><span class="sxs-lookup"><span data-stu-id="91e58-p102">After Microsoft Graph accepts the subscription request, it pushes notifications to the URL specified in the subscription. The app then takes action according to its business logic. For example, it fetches more data, updates cache and views, etc.</span></span>

<span data-ttu-id="91e58-p103">应用应在过期之前续订其订阅。当前的最长过期时间为，将三天减去从创建时起的 90 分钟。需要在过期时间之前续订其订阅。否则，它们将需要新建订阅。</span><span class="sxs-lookup"><span data-stu-id="91e58-p103">Subscriptions expire. The current longest expiration time is three days minus 90 minutes (4230 in total) from the time of creation. Apps need to renew their subscriptions before the expiration time. Otherwise they'll need to create a new subscription.</span></span>

<span data-ttu-id="91e58-123">应用还可以随时取消订阅以停止接收通知。</span><span class="sxs-lookup"><span data-stu-id="91e58-123">Apps should renew their subscriptions before they expire. They can also unsubscribe at any time to stop getting notifications.</span></span>

<span data-ttu-id="91e58-p104">通常订阅操作需要拥有对资源的读取权限。例如，若要获取邮件通知，应用需要 `Mail.Read` 权限。[创建订阅](../api/subscription_post_subscriptions.md)一文列出了各个资源类型所需的权限。下表列出了将 webhook 用于特定资源类型时应用可以请求的权限类型。</span><span class="sxs-lookup"><span data-stu-id="91e58-p104">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription_post_subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span> 

| <span data-ttu-id="91e58-128">权限类型</span><span class="sxs-lookup"><span data-stu-id="91e58-128">Permission type</span></span> | <span data-ttu-id="91e58-129">v1.0 中支持的资源类型</span><span class="sxs-lookup"><span data-stu-id="91e58-129">Supported resource types in v1.0</span></span> |
|:----------------|:---------------------------------|
| <span data-ttu-id="91e58-130">委派 - 工作或学校帐户</span><span class="sxs-lookup"><span data-stu-id="91e58-130">Delegated - work or school account</span></span> | [<span data-ttu-id="91e58-131">contact](contact.md)、[conversation](conversation.md)、[drive](drive.md)、[event](event.md)、[message</span><span class="sxs-lookup"><span data-stu-id="91e58-131">contact](contact.md), [conversation](conversation.md), [drive](drive.md), [event](event.md), [message</span></span>](message.md) |
| <span data-ttu-id="91e58-132">委派 - 个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="91e58-132">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="91e58-133">无</span><span class="sxs-lookup"><span data-stu-id="91e58-133">None</span></span> |
| <span data-ttu-id="91e58-134">应用程序</span><span class="sxs-lookup"><span data-stu-id="91e58-134">Application</span></span> | [<span data-ttu-id="91e58-135">contact](contact.md)、[conversation](conversation.md)、[event](event.md)、[message</span><span class="sxs-lookup"><span data-stu-id="91e58-135">contact](contact.md), [conversation](conversation.md), [event](event.md), [message</span></span>](message.md) |

## <a name="code-samples"></a><span data-ttu-id="91e58-136">代码示例</span><span class="sxs-lookup"><span data-stu-id="91e58-136">Code samples</span></span>

<span data-ttu-id="91e58-137">可在 GitHub 上获取以下代码示例。</span><span class="sxs-lookup"><span data-stu-id="91e58-137">The following samples are available on GitHub in the OneDrive organization.</span></span>

* [<span data-ttu-id="91e58-138">面向 Node.js 的 Microsoft Graph Webhooks 示例</span><span class="sxs-lookup"><span data-stu-id="91e58-138">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
* [<span data-ttu-id="91e58-139">面向 ASP.NET 的 Microsoft Graph Webhooks 示例</span><span class="sxs-lookup"><span data-stu-id="91e58-139">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)

# <a name="creating-a-subscription"></a><span data-ttu-id="91e58-140">创建订阅</span><span class="sxs-lookup"><span data-stu-id="91e58-140">Creating a subscription</span></span>

<span data-ttu-id="91e58-p105">创建订阅是开始接收资源通知的第一步。订阅流程如下所示：</span><span class="sxs-lookup"><span data-stu-id="91e58-p105">Creating a subscription is the first step to start receiving notifications for a resource. The subscription process is as follows:</span></span>

1. <span data-ttu-id="91e58-143">客户端发送特定资源的订阅 (POST) 请求。</span><span class="sxs-lookup"><span data-stu-id="91e58-143">The client sends a subscription (POST) request for a specific resource.</span></span>
2. <span data-ttu-id="91e58-144">Microsoft Graph 验证请求。</span><span class="sxs-lookup"><span data-stu-id="91e58-144">Microsoft Graph verifies the request.</span></span>
  * <span data-ttu-id="91e58-145">如果请求有效，Microsoft Graph 将验证令牌发送到通知 URL。</span><span class="sxs-lookup"><span data-stu-id="91e58-145">If the request is valid, Microsoft Graph sends a validation token to the notification URL.</span></span>
  * <span data-ttu-id="91e58-146">如果该请求无效，Microsoft Graph 将发送包含代码和详细信息的错误响应。</span><span class="sxs-lookup"><span data-stu-id="91e58-146">If the request is invalid, Microsoft Graph sends an error response with code and details.</span></span>
3. <span data-ttu-id="91e58-147">客户端将验证令牌发送回 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="91e58-147">The client sends the validation token back to Microsoft Graph.</span></span>

<span data-ttu-id="91e58-148">客户端必须存储订阅 ID 以便将通知与相应订阅关联。</span><span class="sxs-lookup"><span data-stu-id="91e58-148">Client must store the subscription ID to correlate a notification with the corresponding subscription.</span></span>

## <a name="notification-url-validation"></a><span data-ttu-id="91e58-149">通知 URL 验证</span><span class="sxs-lookup"><span data-stu-id="91e58-149">Notification URL validation</span></span>

<span data-ttu-id="91e58-p106">Microsoft Graph 在创建订阅之前验证订阅请求中的通知 URL。验证流程如下所示：</span><span class="sxs-lookup"><span data-stu-id="91e58-p106">Microsoft Graph validates the notification URL in a subscription request before creating the subscription. The validation process occurs as follows:</span></span>

1. <span data-ttu-id="91e58-152">Microsoft Graph 将 POST 请求发送到通知 URL：</span><span class="sxs-lookup"><span data-stu-id="91e58-152">Microsoft Graph sends a POST request to the notification URL:</span></span>

  ```
  POST https://{notificationUrl}?validationToken={TokenDefinedByMicrosoftGraph}
  ClientState: {Data sent in ClientState value in subscription request (if any)}
  ```
 
2. <span data-ttu-id="91e58-153">客户端必须在 10 秒内提供具有以下特性的响应：</span><span class="sxs-lookup"><span data-stu-id="91e58-153">The client must provide a response with the following characteristics within 10 seconds:</span></span>

  * <span data-ttu-id="91e58-154">200 (OK) 状态代码。</span><span class="sxs-lookup"><span data-stu-id="91e58-154">An 200 (OK) status code.</span></span>
  * <span data-ttu-id="91e58-155">内容类型必须是 text/plain。</span><span class="sxs-lookup"><span data-stu-id="91e58-155">The content type must be text/plain.</span></span> 
  * <span data-ttu-id="91e58-156">正文必须包括 Microsoft Graph 提供的验证令牌。</span><span class="sxs-lookup"><span data-stu-id="91e58-156">The body must include the validation token provided by Microsoft Graph.</span></span>

<span data-ttu-id="91e58-157">在响应中提供验证令牌之后，客户端应放弃验证令牌。</span><span class="sxs-lookup"><span data-stu-id="91e58-157">The client should discard the validation token after providing it in the response.</span></span>

## <a name="subscription-request-example"></a><span data-ttu-id="91e58-158">订阅请求示例</span><span class="sxs-lookup"><span data-stu-id="91e58-158">Subscription request example</span></span>

```
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

<span data-ttu-id="91e58-p107">`changeType`、`notificationUrl`、`resource` 和 `expirationDateTime` 属性是必需的。如需属性定义和值，请参阅[订阅资源类型](subscription.md)。虽然不需要 `clientState`，但必须包括它才能符合我们建议的通知处理过程。</span><span class="sxs-lookup"><span data-stu-id="91e58-p107">The `changeType`, `notificationUrl`, `resource`, and `expirationDateTime` properties are required. See [subscription resource type](subscription.md) for property definitions and values. Although `clientState` is not required, you must include it to comply with our recommended notification handling process.</span></span>

<span data-ttu-id="91e58-162">如果成功，Microsoft Graph 在正文中返回 `201 Created` 代码和一个 [subscription](subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="91e58-162">If successful, Microsoft Graph returns a `201 Created` code and a [subscription](subscription.md) object in the body.</span></span>

# <a name="renewing-a-subscription"></a><span data-ttu-id="91e58-163">续订订阅</span><span class="sxs-lookup"><span data-stu-id="91e58-163">Renewing a subscription</span></span>

<span data-ttu-id="91e58-p108">客户端可以续订特定过期日期的订阅，自请求时间起长达三天。ExpirationDateTime 属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="91e58-p108">The client can renew a subscription with a specific expiration date of up to three days from the time of request. The expirationDateTime property is required.</span></span>

## <a name="subscription-renewal-example"></a><span data-ttu-id="91e58-166">订阅续订示例</span><span class="sxs-lookup"><span data-stu-id="91e58-166">Subscription renewal example</span></span>

```
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id};
Content-Type: application/json
{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

<span data-ttu-id="91e58-p109">如果成功，Microsoft Graph 在正文中返回 `200 OK` 代码和一个 [subscription](subscription.md) 对象。订阅对象包括新的 expirationDateTime 值。</span><span class="sxs-lookup"><span data-stu-id="91e58-p109">If successful, Microsoft Graph returns a `200 OK` code and a [subscription](subscription.md) object in the body. The subscription object includes the new expirationDateTime value.</span></span> 

# <a name="deleting-a-subscription"></a><span data-ttu-id="91e58-169">删除订阅</span><span class="sxs-lookup"><span data-stu-id="91e58-169">Deleting a subscription</span></span>

<span data-ttu-id="91e58-170">客户端可以通过使用其 ID 删除订阅来停止接收通知。</span><span class="sxs-lookup"><span data-stu-id="91e58-170">The client can stop receiving notifications by deleting the subscription using its ID.</span></span>

```
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

<span data-ttu-id="91e58-171">如果成功，Microsoft Graph 将返回 `204 No Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="91e58-171">If successful, Microsoft Graph returns a `204 No Content` code.</span></span>

# <a name="notifications"></a><span data-ttu-id="91e58-172">通知</span><span class="sxs-lookup"><span data-stu-id="91e58-172">Notifications</span></span>

<span data-ttu-id="91e58-p110">客户端在创建订阅后开始接收通知。资源发生更改时，Microsoft Graph 将 POST 请求发送到通知 URL。客户端只能根据指定的更改类型获取通知，例如 *created*。</span><span class="sxs-lookup"><span data-stu-id="91e58-p110">The client starts receiving notifications after creating the subscription. Microsoft Graph sends a POST request to the notification URL when changes happen to the resource. The client only gets notifications according to the specified change type, such as *created*.</span></span>

## <a name="notification-properties"></a><span data-ttu-id="91e58-176">通知属性</span><span class="sxs-lookup"><span data-stu-id="91e58-176">Notification properties</span></span>

<span data-ttu-id="91e58-177">通知对象具有以下属性：</span><span class="sxs-lookup"><span data-stu-id="91e58-177">The notification object has the following properties:</span></span>

* <span data-ttu-id="91e58-178">subscriptionId — 此通知所属的订阅的 ID。</span><span class="sxs-lookup"><span data-stu-id="91e58-178">subscriptionId - The ID for the subscription to which this notification belongs.</span></span>
* <span data-ttu-id="91e58-179">subscriptionexpirationDateTime — 订阅的过期时间。</span><span class="sxs-lookup"><span data-stu-id="91e58-179">subscriptionExpirationDateTime - The expiration time for the subscription.</span></span>
* <span data-ttu-id="91e58-180">clientState — 订阅请求中指定的 clientState 属性。</span><span class="sxs-lookup"><span data-stu-id="91e58-180">clientState - The clientState property specified in the subscription request.</span></span>
* <span data-ttu-id="91e58-p111">changeType — 引发通知的事件类型。例如，邮件接收时为 *created*，或将邮件标记为已读时为 *updated*。</span><span class="sxs-lookup"><span data-stu-id="91e58-p111">changeType - The event type that caused the notification. For example, *created* on mail receive, or *updated* on marking a message read.</span></span>
* <span data-ttu-id="91e58-183">resource — 资源相对于 `https://graph.microsoft.com` 的 URI。</span><span class="sxs-lookup"><span data-stu-id="91e58-183">resource - The URI of the resource relative to `https://graph.microsoft.com`.</span></span> 
* <span data-ttu-id="91e58-p112">resourceData — 取决于订阅资源的对象。例如，对于 Outlook 资源：</span><span class="sxs-lookup"><span data-stu-id="91e58-p112">resourceData - The object dependent on the resource being subscribed to.  For example, for Outlook resources:</span></span>
  * <span data-ttu-id="91e58-186">@odata.type — Microsoft Graph 中描述所表示对象的 OData 实体类型。</span><span class="sxs-lookup"><span data-stu-id="91e58-186">@odata.type - The OData entity type in Microsoft Graph that describes the represented object.</span></span>
  * <span data-ttu-id="91e58-187">@odata.id — 对象的 OData 标识符。</span><span class="sxs-lookup"><span data-stu-id="91e58-187">@odata.id - The OData identifier of the object.</span></span>
  * <span data-ttu-id="91e58-188">@odata.etag — 表示对象版本的 HTTP 实体标记。</span><span class="sxs-lookup"><span data-stu-id="91e58-188">@odata.etag - The HTTP entity tag that represents a version of the object.</span></span>
  * <span data-ttu-id="91e58-189">id — 对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="91e58-189">id - The identifier of the object.</span></span>


> <span data-ttu-id="91e58-p113">注意：resourceData 中提供的 Id 值在通知已排入队列时有效。一些操作（例如将邮件移到其他文件夹中）可能会导致资源 Id 发生更改。</span><span class="sxs-lookup"><span data-stu-id="91e58-p113">Note: The Id value provided in resourceData is valid at the time the notification was queued. Some actions, such as moving a message to another folder, may result in a resource's Id being changed.</span></span> 

## <a name="notification-example"></a><span data-ttu-id="91e58-192">通知示例</span><span class="sxs-lookup"><span data-stu-id="91e58-192">Notification example</span></span>

<span data-ttu-id="91e58-193">用户收到电子邮件时，Microsoft Graph 将发送如下所示的通知：</span><span class="sxs-lookup"><span data-stu-id="91e58-193">When the user receives an email, Microsoft Graph sends a notification like the following:</span></span>

```
{
  "value":[
  {
    "subscriptionId":"<subscription_guid>",
    "subscriptionExpirationDateTime":"2016-03-19T22:11:09.952Z",
    "clientState":"SecretClientState",
    "changeType":"Created",
    "resource":"Users/{user_guid}@<tenant_guid>/Messages/{long_id_string}",
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

<span data-ttu-id="91e58-p114">请注意，值对象包含一个列表。如果有很多排队的通知，Microsoft Graph 会在单个请求中发送这些通知。</span><span class="sxs-lookup"><span data-stu-id="91e58-p114">Note that the value object contains a list. If there are many queued notifications, Microsoft Graph sends them in a single request.</span></span>

## <a name="processing-the-notification"></a><span data-ttu-id="91e58-196">处理通知</span><span class="sxs-lookup"><span data-stu-id="91e58-196">Processing the notification</span></span>

<span data-ttu-id="91e58-p115">必须在应用程序开始接收通知后处理它们。应用程序必须至少执行以下任务来处理通知：</span><span class="sxs-lookup"><span data-stu-id="91e58-p115">After your application starts receiving notifications it must process them. The following are the minimum tasks that your app must perform to process a notification:</span></span>

1. <span data-ttu-id="91e58-p116">验证 `clientState` 属性。通知中的 clientState 属性必须与订阅请求提交的属性匹配。</span><span class="sxs-lookup"><span data-stu-id="91e58-p116">Validate the `clientState` property. The clientState property in the notification must match the one submitted with the subscription request.</span></span>
  > <span data-ttu-id="91e58-p117">注意：如果不符合这个条件，无需将其视为有效通知。还应调查通知来自何处并采取适当的措施。</span><span class="sxs-lookup"><span data-stu-id="91e58-p117">Note: If this isn't true, you shouldn't consider this a valid notification. You should also investigate where the notification comes from and take appropriate action.</span></span>

2. <span data-ttu-id="91e58-203">基于业务逻辑更新应用程序。</span><span class="sxs-lookup"><span data-stu-id="91e58-203">Update your application based on your business logic.</span></span>
3. <span data-ttu-id="91e58-p118">将响应中的 `202 - Accepted` 状态代码发送到 Microsoft Graph。如果 Microsoft Graph 没有收到 2xx 类代码，它将重试多次发送通知。</span><span class="sxs-lookup"><span data-stu-id="91e58-p118">Send a `202 - Accepted` status code in your response to Microsoft Graph. If Microsoft Graph doesn't receive a 2xx class code, it will retry resending the notification a number of times.</span></span>
  > <span data-ttu-id="91e58-206">即使 clientState 属性与订阅请求提交的属性不匹配，也应发送 `202 - Accepted` 状态代码。</span><span class="sxs-lookup"><span data-stu-id="91e58-206">You should send a `202 - Accepted` status code even if the clientState property doesn't match the one submitted with the subscription request.</span></span>

<span data-ttu-id="91e58-207">对请求中的其他通知重复该过程。</span><span class="sxs-lookup"><span data-stu-id="91e58-207">Repeat for other notifications in the request.</span></span>

# <a name="additional-resources"></a><span data-ttu-id="91e58-208">其他资源</span><span class="sxs-lookup"><span data-stu-id="91e58-208">Additional resources</span></span>

* [<span data-ttu-id="91e58-209">订阅资源类型</span><span class="sxs-lookup"><span data-stu-id="91e58-209">Subscription resource type</span></span>](subscription.md)
* [<span data-ttu-id="91e58-210">获取订阅</span><span class="sxs-lookup"><span data-stu-id="91e58-210">Get subscription</span></span>](../api/subscription_get.md)
* [<span data-ttu-id="91e58-211">创建订阅</span><span class="sxs-lookup"><span data-stu-id="91e58-211">Create subscription</span></span>](../api/subscription_post_subscriptions.md)
* <span data-ttu-id="91e58-212">[Microsoft Graph Webhooks Sample for Node.js](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)（面向 Node.js 的 Microsoft Graph Webhooks 示例）</span><span class="sxs-lookup"><span data-stu-id="91e58-212">[Microsoft Graph Webhooks Sample for Node.js](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)</span></span>
* <span data-ttu-id="91e58-213">[Microsoft Graph Webhooks Sample for ASP.NET](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)（面向 ASP.NET 的 Microsoft Graph Webhooks 示例）</span><span class="sxs-lookup"><span data-stu-id="91e58-213">[Microsoft Graph Webhooks Sample for ASP.NET](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)</span></span>
