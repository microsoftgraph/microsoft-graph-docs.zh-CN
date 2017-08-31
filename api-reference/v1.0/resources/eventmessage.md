# <a name="eventmessage-resource-type"></a>eventMessage 资源类型

消息表示会议请求、会议取消消息、会议接受消息、会议暂时接受消息或会议谢绝消息。

EventMessage 通常可以在收件箱文件夹中找到，它作为事件组织者创建会议的结果或由响应会议请求的与会者邀请到达收件箱文件夹。可以使用与操作邮件相同的方式操作事件消息，只存在一些细微的差别，如下表所述。


## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取 eventMessage](../api/eventmessage_get.md) | [eventMessage](eventmessage.md) |读取 eventmessage 对象的属性和关系。|
|[更新](../api/eventmessage_update.md) | [eventMessage](eventmessage.md)  |更新 eventMessage 对象。 |
|[删除](../api/message_delete.md) | 无 |更新 eventMessage 对象。 |
|[复制](../api/message_copy.md)|[邮件](message.md)|将邮件复制到文件夹。|
|[createForward](../api/message_createforward.md)|[邮件](message.md)|创建转发邮件的草稿。然后，你可以 [更新](../api/message_update.md) 或 [发送](../api/message_send.md) 草稿。|
|[createReply](../api/message_createreply.md)|[邮件](message.md)|创建回复邮件的草稿。然后，你可以 [更新](../api/message_update.md) 或 [发送](../api/message_send.md) 草稿。|
|[createReplyAll](../api/message_createreplyall.md)|[邮件](message.md)|创建全部答复邮件的草稿。然后，你可以 [更新](../api/message_update.md) 或 [发送](../api/message_send.md) 草稿。|
|[转发](../api/message_forward.md)|无|转发邮件。然后邮件保存在已发送邮件文件夹中。|
|[移动](../api/message_move.md)|[邮件](message.md)|将邮件移动到文件夹。该操作会在目标文件夹中创建邮件的新副本。|
|[回复](../api/message_reply.md)|无|答复邮件发件人然后邮件保存在已发送邮件文件夹中。|
|[replyAll](../api/message_replyall.md)|无|答复邮件的所有收件人。然后邮件保存在已发送邮件文件夹中。|
|[发送](../api/message_send.md)|无|发送以前创建的邮件草稿。然后邮件保存在已发送邮件文件夹中。|
|**附件**| | |
|[列出附件](../api/eventmessage_list_attachments.md) |[Attachment](attachment.md) 集合| 获取 eventMessage 的所有附件。|
|[Add attachment](../api/eventmessage_post_attachments.md) |[Attachment](attachment.md)| 通过发布到附件集合，向 eventMessage 添加新附件。|
|**开放扩展**| | |
|[创建开放扩展](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| 创建开放扩展，并在新建或现有的资源实例中添加自定义属性。|
|[获取开放扩展](../api/opentypeextension_get.md) |[openTypeExtension](opentypeextension.md) 集合| 获取通过名称或完全限定的名称识别的一个或多个开放扩展对象。|
|**扩展属性**| | |
|[创建单值扩展属性](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[eventMessage](eventMessage.md)  |在新建或现有 eventMessage 中创建一个或多个单值扩展属性。   |
|[获取具有单值扩展属性的 eventMessage](../api/singlevaluelegacyextendedproperty_get.md)  | [eventMessage](eventMessage.md) | 通过使用 `$expand` 或 `$filter` 获取包含单值扩展属性的 eventMessage。 |
|[创建多值扩展属性](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [eventMessage](eventMessage.md) | 在新建或现有的 eventMessage 中创建一个或多个多值扩展属性。  |
|[获取具有多值扩展属性的 eventMessage](../api/multivaluelegacyextendedproperty_get.md)  | [eventMessage](eventMessage.md) | 使用 `$expand` 获取包含一个多值扩展属性的 eventMessage。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|bccRecipients|[recipient](recipient.md) collection|邮件的密件抄送收件人。|
|body|[itemBody](itembody.md)|邮件的正文。可以是 HTML 格式或文本格式。|
|bodyPreview|字符串|邮件正文中的前 255 个字符。文本格式。|
|categories|String collection|与邮件关联的类别。|
|ccRecipients|[recipient](recipient.md) collection|邮件的抄送收件人。|
|changeKey|String|邮件的版本。|
|conversationId|String|电子邮件所属的对话的 ID。|
|createdDateTime|DateTimeOffset|创建邮件的日期和时间。|
|from|[recipient](recipient.md)|邮箱所有者和邮件发件人。|
|hasAttachments|Boolean|指示邮件是否包含附件。|
|id|String||
|importance|String| 邮件的重要性：`Low`、`Normal`、`High`。|
|internetMessageId |String |由 [RFC2822](http://www.ietf.org/rfc/rfc2822.txt) 指定格式的邮件 ID。 |
|isDeliveryReceiptRequested|Boolean|指示是否需要发送邮件已读回执。|
|isDraft|Boolean|指示邮件是否为草稿。如果尚未发送，则此邮件是一封草稿。|
|isRead|Boolean|指示是否已阅读该邮件。|
|isReadReceiptRequested|Boolean|指示是否需要发送邮件已读回执。|
|lastModifiedDateTime|DateTimeOffset|上次更改邮件的日期和时间。|
|meetingMessageType|String| 事件消息的类型：`None`、`MeetingRequest`、`MeetingCancelled`、`MeetingAccepted`、`MeetingTenativelyAccepted`、`MeetingDeclined`。|
|parentFolderId|String|邮件的父 MailFolder 的唯一标识符。|
|receivedDateTime|DateTimeOffset|收到邮件的日期和时间。|
|replyTo|[recipient](recipient.md) collection|在答复时使用的电子邮件地址。|
|sender|[recipient](recipient.md)|实际用于生成邮件的帐户。|
|sentDateTime|DateTimeOffset|发送邮件的日期和时间。|
|subject|String|邮件的主题。|
|toRecipients|[recipient](recipient.md) collection|邮件的收件人。|
|uniqueBody|[itemBody](itembody.md)|当前邮件专用的邮件正文部分。|
|webLink|String|要在 Outlook Web App 中打开邮件的 URL。<br><br>可以将 ispopout 参数附加到此 URL 的末尾以更改邮件的显示方式。如果 ispopout 不存在或设置为 1，则邮件显示在弹出窗口中。如果 ispopout 设置为 0，则浏览器将在 Outlook Web App 审阅窗格中显示邮件。<br><br>如果通过 Outlook Web App 登录邮箱，该邮件将在浏览器中打开。如果尚未使用浏览器登录，系统将提示你登录。<br><br>可以从 iFrame 中访问此 URL。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|attachments|[附件](attachment.md) 集合| 只读。可为 Null。|
|event|[事件](event.md)| 与事件消息相关联的事件。对于与会者或会议室资源，假定已将日历助理设为在会议请求事件消息到达时自动更新包含事件的日历。导航属性。只读。|
|extensions|[扩展](extension.md)集合|为 eventMessage 定义的开放扩展集合。只读。可为 Null。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合| 为 eventMessage 定义的多值扩展属性的集合。只读。可为 Null。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) 集合| 为 eventMessage 定义的单值扩展属性的集合。只读。可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。  

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "event",
    "extensions",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "@odata.type": "microsoft.graph.eventmessage"
}-->

```json
{
  "bccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "bodyPreview": "string",
  "categories": ["string"],
  "ccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "changeKey": "string",
  "conversationId": "string",
  "createdDateTime": "String (timestamp)",
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "String",
  "internetMessageId": "String",
  "isDeliveryReceiptRequested": true,
  "isDraft": true,
  "isRead": true,
  "isReadReceiptRequested": true,
  "lastModifiedDateTime": "String (timestamp)",
  "meetingMessageType": "String",
  "parentFolderId": "string",
  "receivedDateTime": "String (timestamp)",
  "replyTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "sender": {"@odata.type": "microsoft.graph.recipient"},
  "sentDateTime": "String (timestamp)",
  "subject": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "uniqueBody": {"@odata.type": "microsoft.graph.itemBody"},
  "webLink": "string"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "eventMessage resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
