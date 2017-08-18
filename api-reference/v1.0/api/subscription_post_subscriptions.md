# <a name="create-subscription"></a><span data-ttu-id="b25fe-101">创建订阅</span><span class="sxs-lookup"><span data-stu-id="b25fe-101">Create subscription</span></span>

<span data-ttu-id="b25fe-102">订阅侦听器应用程序，以在 Microsoft Graph 中的数据发生更改时接收通知。</span><span class="sxs-lookup"><span data-stu-id="b25fe-102">Subscribes a listener application to receive notifications when data on the Microsoft Graph changes.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b25fe-103">先决条件</span><span class="sxs-lookup"><span data-stu-id="b25fe-103">Prerequisites</span></span>
<span data-ttu-id="b25fe-p101">创建订阅需要读取资源范围。例如，若要获取通知消息，应用需要 `Mail.Read` 权限。下表列出了对各个资源所需权限的建议。</span><span class="sxs-lookup"><span data-stu-id="b25fe-p101">Creating a subscription requires read scope to the resource. For example, to get notifications messages, your app needs the `Mail.Read` permission. The following table lists the suggested permission needed for each resource.</span></span>

| <span data-ttu-id="b25fe-107">资源类型/项</span><span class="sxs-lookup"><span data-stu-id="b25fe-107">Resource type / Item</span></span>        | <span data-ttu-id="b25fe-108">范围</span><span class="sxs-lookup"><span data-stu-id="b25fe-108">Scope</span></span>               |
|-----------------------------|---------------------|
| <span data-ttu-id="b25fe-109">Contacts</span><span class="sxs-lookup"><span data-stu-id="b25fe-109">Contacts</span></span>                    | <span data-ttu-id="b25fe-110">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="b25fe-110">Contacts.Read</span></span>       |
| <span data-ttu-id="b25fe-111">Conversations</span><span class="sxs-lookup"><span data-stu-id="b25fe-111">Conversations</span></span>               | <span data-ttu-id="b25fe-112">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b25fe-112">Group.Read.All</span></span>      |
| <span data-ttu-id="b25fe-113">Events</span><span class="sxs-lookup"><span data-stu-id="b25fe-113">Events</span></span>                      | <span data-ttu-id="b25fe-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b25fe-114">Calendars.Read</span></span>      |
| <span data-ttu-id="b25fe-115">Messages</span><span class="sxs-lookup"><span data-stu-id="b25fe-115">Messages</span></span>                    | <span data-ttu-id="b25fe-116">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b25fe-116">Mail.Read</span></span>           |
| <span data-ttu-id="b25fe-117">Drive（用户的 OneDrive）</span><span class="sxs-lookup"><span data-stu-id="b25fe-117">Drive  (User's OneDrive)</span></span>    | <span data-ttu-id="b25fe-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b25fe-118">Files.ReadWrite</span></span>     |
| <span data-ttu-id="b25fe-119">Drives（Sharepoint 共享内容和驱动器）</span><span class="sxs-lookup"><span data-stu-id="b25fe-119">Drives (Sharepoint shared content and drives)</span></span> | <span data-ttu-id="b25fe-120">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b25fe-120">Files.ReadWrite.All</span></span> |

 <span data-ttu-id="b25fe-p102">***注意：***借助 /v1.0 终结点，大多数资源都支持应用程序权限。组中的对话和 OneDrive 驱动器根项不支持应用程序权限。</span><span class="sxs-lookup"><span data-stu-id="b25fe-p102">One of the following scopes, depending on the target resource, are required to execute this API: Mail.Read, Calendars.Read, Contacts.Read, Group.Read.All, Files.ReadWrite or Files.ReadWrite.All. ***Note:*** The /v1.0 endpoint allows Application permissions for most resources. Conversations in a Group and OneDrive drive root items are not supported with Application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="b25fe-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b25fe-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions

```

## <a name="request-headers"></a><span data-ttu-id="b25fe-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="b25fe-124">Request headers</span></span>
| <span data-ttu-id="b25fe-125">名称</span><span class="sxs-lookup"><span data-stu-id="b25fe-125">Name</span></span>       | <span data-ttu-id="b25fe-126">类型</span><span class="sxs-lookup"><span data-stu-id="b25fe-126">Type</span></span> | <span data-ttu-id="b25fe-127">说明</span><span class="sxs-lookup"><span data-stu-id="b25fe-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b25fe-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="b25fe-128">Authorization</span></span>  | <span data-ttu-id="b25fe-129">string</span><span class="sxs-lookup"><span data-stu-id="b25fe-129">string</span></span>  | <span data-ttu-id="b25fe-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b25fe-p103">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b25fe-132">响应</span><span class="sxs-lookup"><span data-stu-id="b25fe-132">Response</span></span>

<span data-ttu-id="b25fe-133">如果成功，此方法在响应正文中返回 `201, Created` 响应代码和 [subscription](../resources/subscription.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b25fe-133">If successful, this method returns `201, Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b25fe-134">示例</span><span class="sxs-lookup"><span data-stu-id="b25fe-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b25fe-135">请求</span><span class="sxs-lookup"><span data-stu-id="b25fe-135">Request</span></span>
<span data-ttu-id="b25fe-136">下面是在用户收到新邮件时请求发送通知的示例。</span><span class="sxs-lookup"><span data-stu-id="b25fe-136">Here is an example of the request to send a notification when the user receives a new mail.</span></span>
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
   "clientState": "subscription-identifier"
}
```
<span data-ttu-id="b25fe-p104">在请求正文中，提供 [subscription](../resources/subscription.md) 对象的 JSON 表示形式。*ClientState* 字段是可选的。</span><span class="sxs-lookup"><span data-stu-id="b25fe-p104">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object. The *clientState* field is optional.</span></span>

##### <a name="resources-examples"></a><span data-ttu-id="b25fe-139">资源示例</span><span class="sxs-lookup"><span data-stu-id="b25fe-139">Resources examples</span></span>
<span data-ttu-id="b25fe-140">订阅资源属性的有效值如下：</span><span class="sxs-lookup"><span data-stu-id="b25fe-140">The following are valid values for the resource property of the subscription:</span></span>

| <span data-ttu-id="b25fe-141">资源类型</span><span class="sxs-lookup"><span data-stu-id="b25fe-141">Resource type</span></span> | <span data-ttu-id="b25fe-142">示例</span><span class="sxs-lookup"><span data-stu-id="b25fe-142">Examples</span></span> |
|:------ |:----- |
|<span data-ttu-id="b25fe-143">邮件</span><span class="sxs-lookup"><span data-stu-id="b25fe-143">Mail</span></span>|<span data-ttu-id="b25fe-144">me/mailfolders('inbox')/messages</span><span class="sxs-lookup"><span data-stu-id="b25fe-144">me/mailfolders('inbox')/messages</span></span><br /><span data-ttu-id="b25fe-145">me/messages</span><span class="sxs-lookup"><span data-stu-id="b25fe-145">me/messages</span></span>|
|<span data-ttu-id="b25fe-146">联系人</span><span class="sxs-lookup"><span data-stu-id="b25fe-146">Contacts</span></span>|<span data-ttu-id="b25fe-147">me/contacts</span><span class="sxs-lookup"><span data-stu-id="b25fe-147">me/contacts</span></span>|
|<span data-ttu-id="b25fe-148">日历</span><span class="sxs-lookup"><span data-stu-id="b25fe-148">Calendars</span></span>|<span data-ttu-id="b25fe-149">me/events</span><span class="sxs-lookup"><span data-stu-id="b25fe-149">me/events</span></span>|
|<span data-ttu-id="b25fe-150">对话</span><span class="sxs-lookup"><span data-stu-id="b25fe-150">Conversations</span></span>|<span data-ttu-id="b25fe-151">groups('*{id}*')/conversations</span><span class="sxs-lookup"><span data-stu-id="b25fe-151">groups('*{id}*')/conversations</span></span>|
|<span data-ttu-id="b25fe-152">驱动器</span><span class="sxs-lookup"><span data-stu-id="b25fe-152">Drives</span></span>|<span data-ttu-id="b25fe-153">me/drive/root</span><span class="sxs-lookup"><span data-stu-id="b25fe-153">me/drive/root</span></span>|

##### <a name="response"></a><span data-ttu-id="b25fe-154">响应</span><span class="sxs-lookup"><span data-stu-id="b25fe-154">Response</span></span>
<span data-ttu-id="b25fe-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b25fe-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 201 Created

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/mailFolders('Inbox')/messages",
  "changeType":"created, updated",
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z"
}
```
## <a name="subscription-validation"></a><span data-ttu-id="b25fe-158">订阅验证</span><span class="sxs-lookup"><span data-stu-id="b25fe-158">Subscription validation</span></span>
<span data-ttu-id="b25fe-p106">为了避免错误订阅将通知定向到任意 URL，订阅通知终结点必须能够响应验证请求。在处理 `POST` 到 `/subscriptions` 终结点的过程中，Microsoft Graph 按照以下格式将 `POST` 请求发送回 `notificationUrl`：</span><span class="sxs-lookup"><span data-stu-id="b25fe-p106">In order to to avoid mistaken subscriptions directing notifications to arbitrary URLs, the subscription notification endpoint must be capable of responding to a validation request. During processing of the `POST` to the `/subscriptions` endpoint, the Microsoft Graph will send a `POST` request back to your `notificationUrl` in the following form:</span></span> 
```http
POST https://webhook.azurewebsites.net/api/send/myNotifyClient?validationToken=<token>
```
<span data-ttu-id="b25fe-161">通知终结点必须在 10 秒钟内发送 200 响应（将值 `<token>` 作为其正文，且内容类型为 `text/plain`，如下所示），否则将放弃创建请求。</span><span class="sxs-lookup"><span data-stu-id="b25fe-161">The notification endpoint must send a 200 response with the value of `<token>` as its body and a content type of `text/plain`, as shown below, within 10 seconds otherwise the creation request will be discarded.</span></span>
```http
HTTP/1.1 200 OK
Content-type: text/plain
Content-length: 7
<token>
```
## <a name="notification-payload"></a><span data-ttu-id="b25fe-162">通知负载</span><span class="sxs-lookup"><span data-stu-id="b25fe-162">Notification payload</span></span>
<span data-ttu-id="b25fe-p107">订阅资源更改时，Webhooks 设备使用以下负载将通知发送到通知 URL。通知终结点必须在 30 秒内发送无响应正文的 200 或 204 响应，否则将以呈指数级增加的时间间隔重新尝试通知。始终花费 30 秒或更长时间的服务可能会被阻止，且收到的通知集将减少。</span><span class="sxs-lookup"><span data-stu-id="b25fe-p107">When the subscribed resource changes, the webhooks facility sends a notification to your notification URL with the following payload.  The notification endpoint must send a response of 200 or 204 with no response body within 30 seconds otherwise the notification attempt will be retried at exponentially increasing intervals.  Services that consistently take 30 seconds or more may be throttled and receive a sparser notification set.</span></span>

<span data-ttu-id="b25fe-166">服务可能还会返回通知中的 422 响应，在这种情况下，订阅将被自动删除并且通知流会停止。</span><span class="sxs-lookup"><span data-stu-id="b25fe-166">Services may also return a 422 response from a notification, in which case the subscription will be automatically deleted and the stream of notifications will come to a halt.</span></span>

<span data-ttu-id="b25fe-167">根据订阅资源，其他 resourceData 字段可能会提供其他信息。</span><span class="sxs-lookup"><span data-stu-id="b25fe-167">Depending on the subscribed resource, an additional resourceData field may provide additional information.</span></span>

```http
{
   "value":[
      {
         "subscriptionId":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
         "subscriptionExpirationDateTime":"2015-11-20T18:23:45.9356913Z",
         "clientState":"subscription-identifier",
         "changeType":"Created",
         "resource":"Users/ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4/messages/AAMkADMxZmEzMDM1LTFjODQtNGVkMC04YzY3LTBjZTRlNDFjNGE4MwBGAAAAAAAr-q_ZG7oXSaqxum7oZW5RBwCoeN6SYXGLRrvRm_CYrrfQAAAAAAEMAACoeN6SYXGLRrvRm_CYrrfQAACvtMe6AAA=",
         "resourceData":{
            "@odata.type":"#Microsoft.Graph.Message",
            "@odata.id":"Users/ddfcd489-628b-7d04-b48b-20075df800e5@1717622f-1d94-c0d4-9d74-f907ad6677b4/messages/AAMkADMxZmEzMDM1LTFjODQtNGVkMC04YzY3LTBjZTRlNDFjNGE4MwBGAAAAAAAr-q_ZG7oXSaqxum7oZW5RBwCoeN6SYXGLRrvRm_CYrrfQAAAAAAEMAACoeN6SYXGLRrvRm_CYrrfQAACvtMe6AAA=",
            "@odata.etag":"W/\"CQAAABYAAACoeN6SYXGLRrvRm+CYrrfQAACvvGdb\"",
            "Id":"AAMkADMxZmEzMDM1LTFjODQtNGVkMC04YzY3LTBjZTRlNDFjNGE4MwBGAAAAAAAr-q_ZG7oXSaqxum7oZW5RBwCoeN6SYXGLRrvRm_CYrrfQAAAAAAEMAACoeN6SYXGLRrvRm_CYrrfQAACvtMe6AAA="
         }
      }
   ]
}
```
<span data-ttu-id="b25fe-p108">接收来自驱动器订阅的通知时，resourceData 将为 null，并且应调用 [delta](item_delta.md) API 以确定已经发生的更改。下面是一个驱动器通知示例：</span><span class="sxs-lookup"><span data-stu-id="b25fe-p108">When receiving notifications from Drive subscriptions the resourceData will be null and the [delta](item_delta.md) API should be called to determine the changes that have occured. Here is an example of a Drive notification:</span></span>
```http
{
  "subscriptionId": "aa269f87-2a92-4cff-a43e-2771878c3727",
  "clientState": "My client state",
  "changeType": "updated",
  "resource": "me/drive/root",
  "subscriptionExpirationDateTime": "2016-08-26T23:08:37.00+00:00",
  "resourceData": null
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
