# <a name="update-message"></a>更新邮件

更新 message 对象的属性。
## <a name="prerequisites"></a>先决条件
要执行此 API，需要以下**范围**之一：*Mail.ReadWrite*
## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer <token>. Required. |
| Content-Type | string  | 实体正文中的数据性质。必需。 |
## <a name="request-body"></a>请求正文
在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。可写/可更新属性

| 属性       | 类型    |说明|
|:---------------|:--------|:----------|
|bccRecipients|Recipient|邮件的密件抄送收件人。仅当 IsDraft = true 时可以更新。|
|categories|String collection|与邮件关联的类别。|
|ccRecipients|收件人集合|邮件的抄送收件人。仅当 IsDraft = true 时可以更新。|
|from|Recipient|邮箱所有者和邮件发件人。仅当 IsDraft = true 时可以更新。|
|importance|String|邮件的重要性。可能的值是：`Low`、`Normal`、`High`。|
|inferenceClassification | String | 根据推导出的相关性或重要性或显式替代，对用户邮件的分类。可能的值是：`focused` 或 `other`。 |
|internetMessageId |String |由 [RFC2822](http://www.ietf.org/rfc/rfc2822.txt) 指定格式的邮件 ID。仅当 IsDraft = true 时可以更新。|
|isRead|Boolean|指示是否已阅读该邮件。|
|replyTo|Recipient collection|在答复时使用的电子邮件地址。仅当 IsDraft = true 时可以更新。|
|sender|Recipient|实际用于生成邮件的帐户。仅当 IsDraft = true 时可以更新。|
|toRecipients|Recipient collection|邮件的收件人。仅当 IsDraft = true 时可以更新。|
|正文|ItemBody|邮件的正文。仅当 IsDraft = true 时可以更新。|
|isDeliveryReceiptRequested|Boolean|指示是否需要发送邮件已读回执。|
|isReadReceiptRequested|Boolean|指示是否需要发送邮件已读回执。|
|subject|String|邮件的主题。仅当 IsDraft = true 时可以更新。|

由于**邮件**资源支持[扩展](../../../concepts/extensibility_overview.md)，因此可以使用 `PATCH` 操作在现有**邮件**实例的扩展自定义属性中添加、更新或删除自己的特定于应用的数据。

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [message](../resources/message.md) 对象。
## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "update_message"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "inferenceClassification": "other"
}
```
##### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value",
  "inferenceClassification": "other"
}
```

## <a name="see-also"></a>另请参阅

- [使用扩展向资源添加自定义数据](../../../concepts/extensibility_overview.md)
- [使用开放扩展向用户添加自定义数据（预览）](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
