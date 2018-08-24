# <a name="create-subscription"></a>创建订阅

订阅侦听器应用程序，以在 Microsoft Graph 中的数据发生更改时接收通知。

## <a name="permissions"></a>权限

创建订阅需要读取资源范围。例如，若要获取通知消息，应用需要 `Mail.Read` 权限。下表列出了对各个资源所需权限的建议。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。

| 资源类型/项        | 权限          |
|-----------------------------|---------------------|
| 联系人                    | Contacts.Read       |
| 对话               | Group.Read.All      |
| 事件                      | Calendars.Read      |
| 消息                    | Mail.Read           |
| 组                      | Group.Read.All      |
| 用户                       | User.Read.All       |
| 驱动器（用户的 OneDrive）    | Files.ReadWrite     |
| 驱动器（SharePoint 共享的内容和驱动器） | Files.ReadWrite.All |

 > **注意：**/v1.0 端点允许资源最多的应用程序权限。 应用程序权限不支持组中的对话和 OneDrive 驱动器根项目。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a>请求标头

| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | 字符串  | Bearer {token}。必需。 |

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [subscription](../resources/subscription.md) 对象。

## <a name="example"></a>示例

##### <a name="request"></a>请求

以下是用户收到新邮件时请求发送通知的示例。
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

在请求正文中，提供[订阅](../resources/subscription.md)对象的 JSON 表示。
`clientState`字段为选填。

##### <a name="resources-examples"></a>资源示例

订阅资源属性的有效值如下：

| 资源类型 | 示例 |
|:------ |:----- |
|邮件|me/mailfolders('inbox')/messages<br />me/messages|
|联系人|me/contacts|
|日历|me/events|
|用户|users|
|组|组|
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

## <a name="notification-endpoint-validation"></a>通知端点验证

订阅通知端点（在 `notificationUrl` 属性中指定）必须能够响应验证请求，如同[设置用户数据更改的通知](../../../concepts/webhooks.md#notification-endpoint-validation)所述。 如果验证失败，创建订阅的请求将返回一个 400 错误请求错误。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
