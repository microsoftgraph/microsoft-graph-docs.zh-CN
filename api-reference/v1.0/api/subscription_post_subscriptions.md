# <a name="create-subscription"></a><span data-ttu-id="a3fed-101">创建订阅</span><span class="sxs-lookup"><span data-stu-id="a3fed-101">Create subscription</span></span>

<span data-ttu-id="a3fed-102">订阅侦听器应用程序，以在 Microsoft Graph 中的数据发生更改时接收通知。</span><span class="sxs-lookup"><span data-stu-id="a3fed-102">Subscribes a listener application to receive notifications when data on the Microsoft Graph changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3fed-103">权限</span><span class="sxs-lookup"><span data-stu-id="a3fed-103">Permissions</span></span>

<span data-ttu-id="a3fed-p101">创建订阅需要读取资源范围。例如，若要获取通知消息，应用需要 `Mail.Read` 权限。下表列出了对各个资源所需权限的建议。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a3fed-p101">Creating a subscription requires read scope to the resource. For example, to get notifications messages, your app needs the `Mail.Read` permission. The following table lists the suggested permission needed for each resource. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="a3fed-108">资源类型/项</span><span class="sxs-lookup"><span data-stu-id="a3fed-108">Resource type / Item</span></span>        | <span data-ttu-id="a3fed-109">权限</span><span class="sxs-lookup"><span data-stu-id="a3fed-109">Permission</span></span>          |
|-----------------------------|---------------------|
| <span data-ttu-id="a3fed-110">联系人</span><span class="sxs-lookup"><span data-stu-id="a3fed-110">Contacts</span></span>                    | <span data-ttu-id="a3fed-111">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a3fed-111">Contacts.Read</span></span>       |
| <span data-ttu-id="a3fed-112">对话</span><span class="sxs-lookup"><span data-stu-id="a3fed-112">Conversations</span></span>               | <span data-ttu-id="a3fed-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3fed-113">Group.Read.All</span></span>      |
| <span data-ttu-id="a3fed-114">事件</span><span class="sxs-lookup"><span data-stu-id="a3fed-114">Events</span></span>                      | <span data-ttu-id="a3fed-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a3fed-115">Calendars.Read</span></span>      |
| <span data-ttu-id="a3fed-116">消息</span><span class="sxs-lookup"><span data-stu-id="a3fed-116">Messages</span></span>                    | <span data-ttu-id="a3fed-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a3fed-117">Mail.Read</span></span>           |
| <span data-ttu-id="a3fed-118">组</span><span class="sxs-lookup"><span data-stu-id="a3fed-118">Groups</span></span>                      | <span data-ttu-id="a3fed-119">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3fed-119">Group.Read.All</span></span>      |
| <span data-ttu-id="a3fed-120">用户</span><span class="sxs-lookup"><span data-stu-id="a3fed-120">Users</span></span>                       | <span data-ttu-id="a3fed-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3fed-121">User.Read.All</span></span>       |
| <span data-ttu-id="a3fed-122">驱动器（用户的 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="a3fed-122">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="a3fed-123">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a3fed-123">Files.ReadWrite</span></span>     |
| <span data-ttu-id="a3fed-124">驱动器（SharePoint 共享的内容和驱动器）</span><span class="sxs-lookup"><span data-stu-id="a3fed-124">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="a3fed-125">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3fed-125">Files.ReadWrite.All</span></span> |

 > <span data-ttu-id="a3fed-126">**注意：**/v1.0 端点允许资源最多的应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="a3fed-126">**Note:** The /v1.0 endpoint allows application permissions for most resources.</span></span> <span data-ttu-id="a3fed-127">应用程序权限不支持组中的对话和 OneDrive 驱动器根项目。</span><span class="sxs-lookup"><span data-stu-id="a3fed-127">Note: The /v1.0 endpoint allows Application permissions for most resources. Conversations in a Group and OneDrive drive root items are not supported with Application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="a3fed-128">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a3fed-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="a3fed-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="a3fed-129">Request headers</span></span>

| <span data-ttu-id="a3fed-130">名称</span><span class="sxs-lookup"><span data-stu-id="a3fed-130">Name</span></span>       | <span data-ttu-id="a3fed-131">类型</span><span class="sxs-lookup"><span data-stu-id="a3fed-131">Type</span></span> | <span data-ttu-id="a3fed-132">说明</span><span class="sxs-lookup"><span data-stu-id="a3fed-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a3fed-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3fed-133">Authorization</span></span>  | <span data-ttu-id="a3fed-134">字符串</span><span class="sxs-lookup"><span data-stu-id="a3fed-134">string</span></span>  | <span data-ttu-id="a3fed-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a3fed-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a3fed-137">响应</span><span class="sxs-lookup"><span data-stu-id="a3fed-137">Response</span></span>

<span data-ttu-id="a3fed-138">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a3fed-138">If successful, this method returns `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3fed-139">示例</span><span class="sxs-lookup"><span data-stu-id="a3fed-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a3fed-140">请求</span><span class="sxs-lookup"><span data-stu-id="a3fed-140">Request</span></span>

<span data-ttu-id="a3fed-141">以下是用户收到新邮件时请求发送通知的示例。</span><span class="sxs-lookup"><span data-stu-id="a3fed-141">Here is an example of the request to send a notification when the user receives a new mail.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-type: application/json

{
   "changeType": "created,updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue"
}
```

<span data-ttu-id="a3fed-142">在请求正文中，提供[订阅](../resources/subscription.md)对象的 JSON 表示。</span><span class="sxs-lookup"><span data-stu-id="a3fed-142">In the request body, supply a JSON representation of the [Contact](../resources/subscription.md) object.</span></span>
<span data-ttu-id="a3fed-143">`clientState`字段为选填。</span><span class="sxs-lookup"><span data-stu-id="a3fed-143">The `clientState` field is optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="a3fed-144">资源示例</span><span class="sxs-lookup"><span data-stu-id="a3fed-144">Resources examples</span></span>

<span data-ttu-id="a3fed-145">订阅资源属性的有效值如下：</span><span class="sxs-lookup"><span data-stu-id="a3fed-145">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="a3fed-146">资源类型</span><span class="sxs-lookup"><span data-stu-id="a3fed-146">Resource type</span></span> | <span data-ttu-id="a3fed-147">示例</span><span class="sxs-lookup"><span data-stu-id="a3fed-147">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="a3fed-148">邮件</span><span class="sxs-lookup"><span data-stu-id="a3fed-148">Mail</span></span>|<span data-ttu-id="a3fed-149">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="a3fed-149">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="a3fed-150">me/messages</span><span class="sxs-lookup"><span data-stu-id="a3fed-150">me/messages</span></span>|
|<span data-ttu-id="a3fed-151">联系人</span><span class="sxs-lookup"><span data-stu-id="a3fed-151">Contacts</span></span>|<span data-ttu-id="a3fed-152">me/contacts</span><span class="sxs-lookup"><span data-stu-id="a3fed-152">me/contacts</span></span>|
|<span data-ttu-id="a3fed-153">日历</span><span class="sxs-lookup"><span data-stu-id="a3fed-153">Calendars</span></span>|<span data-ttu-id="a3fed-154">me/events</span><span class="sxs-lookup"><span data-stu-id="a3fed-154">me/events</span></span>|
|<span data-ttu-id="a3fed-155">用户</span><span class="sxs-lookup"><span data-stu-id="a3fed-155">Users</span></span>|<span data-ttu-id="a3fed-156">users</span><span class="sxs-lookup"><span data-stu-id="a3fed-156">users</span></span>|
|<span data-ttu-id="a3fed-157">组</span><span class="sxs-lookup"><span data-stu-id="a3fed-157">Groups</span></span>|<span data-ttu-id="a3fed-158">组</span><span class="sxs-lookup"><span data-stu-id="a3fed-158">groups</span></span>|
|<span data-ttu-id="a3fed-159">对话</span><span class="sxs-lookup"><span data-stu-id="a3fed-159">Conversations</span></span>|<span data-ttu-id="a3fed-160">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="a3fed-160">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="a3fed-161">驱动器</span><span class="sxs-lookup"><span data-stu-id="a3fed-161">Drives</span></span>|<span data-ttu-id="a3fed-162">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="a3fed-162">me/drive/root</span></span>|

##### <a name="response"></a><span data-ttu-id="a3fed-163">响应</span><span class="sxs-lookup"><span data-stu-id="a3fed-163">Response</span></span>

<span data-ttu-id="a3fed-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a3fed-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 252

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions/$entity",
  "id": "7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource": "me/mailFolders('Inbox')/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType": "created,updated",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

## <a name="notification-endpoint-validation"></a><span data-ttu-id="a3fed-167">通知端点验证</span><span class="sxs-lookup"><span data-stu-id="a3fed-167">Notification endpoint validation</span></span>

<span data-ttu-id="a3fed-168">订阅通知端点（在 `notificationUrl` 属性中指定）必须能够响应验证请求，如同[设置用户数据更改的通知](../../../concepts/webhooks.md#notification-endpoint-validation)所述。</span><span class="sxs-lookup"><span data-stu-id="a3fed-168">The subscription notification endpoint (specified in the `notificationUrl` property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](../../../concepts/webhooks.md#notification-endpoint-validation).</span></span> <span data-ttu-id="a3fed-169">如果验证失败，创建订阅的请求将返回一个 400 错误请求错误。</span><span class="sxs-lookup"><span data-stu-id="a3fed-169">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
