# <a name="create-subscription"></a>创建订阅

订阅侦听器应用程序，以在 Microsoft Graph 中的数据发生更改时接收通知。
## <a name="prerequisites"></a>先决条件
创建订阅需要读取资源范围。例如，若要获取通知消息，应用需要 `Mail.Read` 权限。下表列出了对各个资源所需权限的建议。

| 资源类型/项        | 范围               |
|-----------------------------|---------------------|
| Contacts                    | Contacts.Read       |
| Conversations               | Group.Read.All      |
| Events                      | Calendars.Read      |
| Messages                    | Mail.Read           |
| Drive（用户的 OneDrive）    | Files.ReadWrite     |
| Drives（Sharepoint 共享内容和驱动器） | Files.ReadWrite.All |

 ***注意：***借助 /v1.0 终结点，大多数资源都支持应用程序权限。组中的对话和 OneDrive 驱动器根项不支持应用程序权限。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions

```

## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201, Created` 响应代码和 [subscription](../resources/subscription.md) 对象。

## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是在用户收到新邮件时请求发送通知的示例。
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
在请求正文中，提供 [subscription](../resources/subscription.md) 对象的 JSON 表示形式。*ClientState* 字段是可选的。

##### <a name="resources-examples"></a>资源示例
订阅资源属性的有效值如下：

| 资源类型 | 示例 |
|:------ |:----- |
|邮件|me/mailfolders('inbox')/messages<br />me/messages|
|联系人|me/contacts|
|日历|me/events|
|对话|groups('*{id}*')/conversations|
|驱动器|me/drive/root|

##### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
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
## <a name="subscription-validation"></a>订阅验证
为了避免错误订阅将通知定向到任意 URL，订阅通知终结点必须能够响应验证请求。在处理 `POST` 到 `/subscriptions` 终结点的过程中，Microsoft Graph 按照以下格式将 `POST` 请求发送回 `notificationUrl`： 
```http
POST https://webhook.azurewebsites.net/api/send/myNotifyClient?validationToken=<token>
```
通知终结点必须在 10 秒钟内发送 200 响应（将值 `<token>` 作为其正文，且内容类型为 `text/plain`，如下所示），否则将放弃创建请求。
```http
HTTP/1.1 200 OK
Content-type: text/plain
Content-length: 7
<token>
```
## <a name="notification-payload"></a>通知负载
订阅资源更改时，Webhooks 设备使用以下负载将通知发送到通知 URL。通知终结点必须在 30 秒内发送无响应正文的 200 或 204 响应，否则将以呈指数级增加的时间间隔重新尝试通知。始终花费 30 秒或更长时间的服务可能会被阻止，且收到的通知集将减少。

服务可能还会返回通知中的 422 响应，在这种情况下，订阅将被自动删除并且通知流会停止。

根据订阅资源，其他 resourceData 字段可能会提供其他信息。

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
接收来自驱动器订阅的通知时，resourceData 将为 null，并且应调用 [delta](item_delta.md) API 以确定已经发生的更改。下面是一个驱动器通知示例：
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
