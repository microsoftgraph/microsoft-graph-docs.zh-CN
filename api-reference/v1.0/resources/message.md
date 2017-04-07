# <a name="message-resource-type"></a>邮件资源类型

mailFolder 中的邮件。

通过该资源可以使用[扩展](../../../concepts/extensibility_overview.md)将自己的数据添加到自定义属性。


## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出邮件](../api/user_list_messages.md) |[邮件](message.md)集合 | 获取已登录用户的邮箱中的所有邮件（包括“已删除邮件”和“待筛选邮件”文件夹）。 |
|[创建邮件](../api/user_post_messages.md) | [邮件](message.md) | [创建](../api/user_post_messages.md#request-1) 新邮件的草稿。 |
|[获取邮件](../api/message_get.md) | [邮件](message.md) |读取 message 对象的属性和关系。|
|[更新](../api/message_update.md) | [邮件](message.md) |更新 message 对象。|
|[删除](../api/message_delete.md) | 无 |删除 message 对象。 |
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
|[列出附件](../api/message_list_attachments.md) |[附件](attachment.md) 集合| 获取邮件的所有附件。|
|[Add attachment](../api/message_post_attachments.md) |[Attachment](attachment.md)| 通过发布到附件集合，向邮件添加新附件。|
|**开放扩展**| | |
|[创建开放扩展](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| 创建开放扩展，并在新建或现有的资源实例中添加自定义属性。|
|[获取开放扩展](../api/opentypeextension_get.md) |[openTypeExtension](opentypeextension.md) 集合| 获取通过名称或完全限定的名称识别的一个或多个开放扩展对象。|
|**扩展属性**| | |
|[创建单值扩展属性](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[邮件](message.md)  |在新建或现有的邮件中创建一个或多个单值扩展属性。   |
|[获取具有单值扩展属性的邮件](../api/singlevaluelegacyextendedproperty_get.md)  | [邮件](message.md) | 通过使用 `$expand` 或 `$filter` 获取包含单值扩展属性的邮件。 |
|[创建多值扩展属性](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [邮件](message.md) | 在新建或现有的邮件中创建一个或多个多值扩展属性。  |
|[获取具有多值扩展属性的邮件](../api/multivaluelegacyextendedproperty_get.md)  | [邮件](message.md) | 使用 `$expand` 获取包含一个多值扩展属性的邮件。 |


## <a name="properties"></a>属性
| 属性       | 类型    |说明|
|:---------------|:--------|:----------|
|bccRecipients|[recipient](recipient.md) collection|邮件的密件抄送收件人。|
|body|[itemBody](itembody.md)|邮件的正文。|
|bodyPreview|String|邮件正文中的前 255 个字符。|
|categories|String collection|与邮件关联的类别。|
|ccRecipients|[recipient](recipient.md) collection|邮件的抄送收件人。|
|changeKey|String|邮件的版本。|
|conversationId|String|电子邮件所属的对话的 ID。|
|createdDateTime|DateTimeOffset|创建邮件的日期和时间。|
|from|[recipient](recipient.md)|邮箱所有者和邮件发件人。|
|hasAttachments|Boolean|指示邮件是否包含附件。|
|id|String|邮件的唯一标识符（请注意，此值可能会随着邮件移动或更改而更改）|
|importance|String| 邮件的重要性：`Low`、`Normal`、`High`。|
|inferenceClassification | String | 根据推导出的相关性或重要性或显式替代，对用户邮件的分类。可能的值是：`focused` 或 `other`。 |
|internetMessageId |String |由 [RFC2822](http://www.ietf.org/rfc/rfc2822.txt) 指定格式的邮件 ID。 |
|isDeliveryReceiptRequested|Boolean|指示是否需要发送邮件已读回执。|
|isDraft|Boolean|指示邮件是否为草稿。如果尚未发送，则此邮件是一封草稿。|
|isRead|Boolean|指示是否已阅读该邮件。|
|isReadReceiptRequested|Boolean|指示是否需要发送邮件已读回执。|
|lastModifiedDateTime|DateTimeOffset|上次更改邮件的日期和时间。|
|parentFolderId|String|邮件的父 MailFolder 的唯一标识符。|
|receivedDateTime|DateTimeOffset|收到邮件的日期和时间。|
|replyTo|[recipient](recipient.md) collection|在答复时使用的电子邮件地址。|
|sender|[recipient](recipient.md)|实际用于生成邮件的帐户。|
|sentDateTime|DateTimeOffset|发送邮件的日期和时间。|
|subject|String|邮件的主题。|
|toRecipients|[recipient](recipient.md) collection|邮件的收件人。|
|uniqueBody|[itemBody](itembody.md)|对于当前邮件独一无二的邮件正文部分。uniqueBody 默认不提供，但可以使用 ?$select=uniqueBody 为指定邮件检索它。|
|webLink|String|要在 Outlook Web App 中打开邮件的 URL。<br><br>可以将 ispopout 参数附加到此 URL 的末尾以更改邮件的显示方式。如果 ispopout 不存在或设置为 1，则邮件显示在弹出窗口中。如果 ispopout 设置为 0，则浏览器将在 Outlook Web App 审阅窗格中显示邮件。<br><br>如果通过 Outlook Web App 登录邮箱，该邮件将在浏览器中打开。如果尚未使用浏览器登录，系统将提示你登录。<br><br>可以从 iFrame 中访问此 URL。|

**从 Body 属性中删除脚本**

邮件正文可以是 HTML 或文本。如果正文是 HTML 格式，默认情况下，在 REST 响应中返回正文内容之前，将删除嵌入 Body 属性中的任意具有潜在不安全性的 HTML（例如 JavaScript）。若要获取整个原始 HTML 内容，请包括以下 HTTP 请求标头：
```
Prefer: outlook.allow-unsafe-html
```

**设置 From 和 Sender 属性**

撰写邮件时，在大多数情况下，From 和 Sender 属性表示同一个已登录用户，除非其中一个属性已更新，如以下情况中所述：

- 如果 Exchange 管理员已将邮箱的 **SendAs** 权限分配给其他一些用户，则可以更改 **From** 属性。通过在 Azure 管理门户选择邮箱所有者的**邮箱权限**，或通过使用 Exchange 管理中心或 Windows PowerShell Add-ADPermission cmdlet，管理员可以更改此属性。然后，可以通过编程方式将 **From** 属性设置为其中一个拥有邮箱的 **SendAs** 权限的用户。
- 如果邮箱所有者已委派一个或多个用户能够从该邮箱发送邮件，则可以更改 **Sender** 属性。可以在 Outlook 中委派邮箱所有者。当代理代表邮箱所有者发送邮件时，**Sender** 属性设置为代理的帐户，**from** 属性仍保持为邮箱所有者。可以通过编程方式将 **Sender** 属性设置为拥有邮箱代理权限的用户。

## <a name="relationships"></a>Relationships
| 关系 | 类型    |说明|
|:---------------|:--------|:----------|
|attachments|[附件](attachment.md)集合|邮件的 [fileAttachment](fileattachment.md) 和 [itemAttachment](itemattachment.md) 附件。|
|extensions|[扩展](extension.md)集合|为邮件定义的开放扩展集合。只读。可为 Null。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合| 为邮件定义的多值扩展属性的集合。只读。可为 Null。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| 为邮件定义的单值扩展属性的集合。只读。可为 Null。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "extensions",
    "singleValueExtendedProperties",
    "multiValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.message"
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
  "inferenceClassification": "String",
  "internetMessageId": "String",
  "isDeliveryReceiptRequested": true,
  "isDraft": true,
  "isRead": true,
  "isReadReceiptRequested": true,
  "lastModifiedDateTime": "String (timestamp)",
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

## <a name="see-also"></a>另请参阅

- [获取邮箱设置](../api/user_get_mailboxsettings.md) 
- [更新邮箱设置](../api/user_update_mailboxsettings.md)
- [使用扩展向资源添加自定义数据](../../../concepts/extensibility_overview.md)
- [使用开放扩展向用户添加自定义数据（预览）](../../../concepts/extensibility_open_users.md)
- [使用架构扩展向组添加自定义数据（预览）](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
