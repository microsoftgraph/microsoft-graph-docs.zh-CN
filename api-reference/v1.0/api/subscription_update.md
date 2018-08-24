# <a name="update-subscription"></a>更新订阅

通过延长到期时间续订订阅。

超过资源类型确定的时间长度后订阅过期。 为了避免遗漏通知，应用程序应在订阅到期日之前续订订阅。 请参阅[订阅](../resources/subscription.md)，了解每个资源类型的最长订阅时间。

## <a name="permissions"></a>权限

下表列出了对各个资源所需权限的建议。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。

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

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a>请求标头

| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| 授权  | 字符串  | Bearer {token}。必需。 |

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象。

## <a name="example"></a>示例

##### <a name="request"></a>请求

下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```

##### <a name="response"></a>响应

下面是一个响应示例。
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType":"created,updated",
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
