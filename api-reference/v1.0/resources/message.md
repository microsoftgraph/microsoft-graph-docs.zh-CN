# <a name="message-resource-type"></a>邮件资源类型

mailFolder 中的邮件。

该资源支持：

- 添加您自己的数据作为自定义 Internet 邮件标头。 仅当创建邮件时添加自定义标头，并以开头字母为 "x-" 的方式对其进行命名。 一旦已发送邮件，您无法修改标头。 若要获取的邮件标头，请在[获取邮件](../api/message_get.md)操作中应用 `$select` 查询参数。
- 在[扩展](../../../concepts/extensibility_overview.md)中添加您自己的数据作为自定义属性。
- 通过提供 [delta](../api/message_delta.md) 函数使用[增量查询](../../../concepts/delta_query_overview.md)跟踪增量添加、删除和更新。

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
|[delta](../api/message_delta.md)|[邮件](message.md)集合| 获取指定文件夹中已添加、删除或更新的邮件集。|
|[转发](../api/message_forward.md)|无|转发邮件。然后邮件保存在已发送邮件文件夹中。|
|[移动](../api/message_move.md)|[邮件](message.md)|将邮件移动到文件夹。该操作会在目标文件夹中创建邮件的新副本。|
|[回复](../api/message_reply.md)|无|答复邮件发件人然后邮件保存在已发送邮件文件夹中。|
|[replyAll](../api/message_replyall.md)|无|答复邮件的所有收件人。然后邮件保存在已发送邮件文件夹中。|
|[发送](../api/message_send.md)|无|发送以前创建的邮件草稿。然后邮件保存在已发送邮件文件夹中。|
|**附件**| | |
|[列出附件](../api/message_list_attachments.md) |[附件](attachment.md) 集合| 获取邮件的所有附件。|
|[添加附件](../api/message_post_attachments.md) |[附件](attachment.md)| 通过发布到附件集合，向邮件添加新附件。|
|**开放扩展**| | |
|[创建开放扩展](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| 创建开放扩展，并在新建或现有的资源实例中添加自定义属性。|
|[获取开放扩展](../api/opentypeextension_get.md) |[openTypeExtension](opentypeextension.md) 集合| 获取通过名称或完全限定的名称识别的一个或多个开放扩展对象。|
|**架构扩展**| | |
|[添加架构扩展值](../../../concepts/extensibility_schema_groups.md) || 创建架构扩展定义，然后使用它向资源添加自定义键入数据。|
|**扩展属性**| | |
|[创建单值扩展属性](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[邮件](message.md)  |在新建或现有的邮件中创建一个或多个单值扩展属性。   |
|[获取具有单值扩展属性的邮件](../api/singlevaluelegacyextendedproperty_get.md)  | [邮件](message.md) | 通过使用 `$expand` 或 `$filter` 获取包含单值扩展属性的邮件。 |
|[创建多值扩展属性](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [邮件](message.md) | 在新建或现有的邮件中创建一个或多个多值扩展属性。  |
|[获取具有多值扩展属性的邮件](../api/multivaluelegacyextendedproperty_get.md)  | [邮件](message.md) | 使用 `$expand` 获取包含一个多值扩展属性的邮件。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|bccRecipients|[收件人](recipient.md)集合|邮件的密件抄送收件人。|
|body|[itemBody](itembody.md)|邮件的正文。可以是 HTML 格式或文本格式。|
|bodyPreview|字符串|邮件正文中的前 255 个字符。文本格式。|
|categories|字符串集合|与邮件关联的类别。|
|ccRecipients|[收件人](recipient.md)集合|邮件的抄送收件人。|
|changeKey|字符串|邮件的版本。|
|conversationId|字符串|电子邮件所属的对话的 ID。|
|createdDateTime|DateTimeOffset|创建邮件的日期和时间。|
|flag|[followupFlag](followupflag.md)|指示状态、开始日期、截止日期或邮件的完成日期的标记值。|
|发件人|[recipient](recipient.md)|邮箱所有者和邮件发件人。 值必须与实际使用的邮箱对应。|
|hasAttachments|布尔|指明邮件是否包含附件。此属性不涉及内联附件。因此，如果邮件仅包含内联附件，此属性为 false。若要验证是否存在内联附件，请分析 **body** 属性，以确定是否有 `src` 属性（例如，`<IMG src="cid:image001.jpg@01D26CD8.6C05F070">`）。|
|id|字符串|邮件的唯一标识符（请注意，此值可能会随着邮件移动或更改而更改）|
|importance|importance| 邮件的重要性：`Low`、`Normal`、`High`。|
|inferenceClassification | InferenceClassificationType | 根据推导出的相关性或重要性或显式替代，对用户邮件的分类。 可能的值包括 `focused` 或 `other`。 |
|internetMessageHeaders | [internetMessageHeader](internetmessageheader.md) 集合 | 由 [RFC5322](https://www.ietf.org/rfc/rfc5322.txt) 定义的邮件标头的集合。 集合包括指示邮件由发件人到达收件人所采用的网络路径的邮件标头。 它还可以包含保留邮件应用程序数据的自定义邮件标头。 |
|internetMessageId |字符串 |由 [RFC2822](http://www.ietf.org/rfc/rfc2822.txt) 指定格式的邮件 ID。 |
|isDeliveryReceiptRequested|布尔|指示是否需要发送邮件已读回执。|
|isDraft|布尔|指示邮件是否为草稿。如果尚未发送，则此邮件是一封草稿。|
|isRead|布尔|指示是否已阅读该邮件。|
|isReadReceiptRequested|布尔|指示是否需要发送邮件已读回执。|
|lastModifiedDateTime|DateTimeOffset|上次更改邮件的日期和时间。|
|parentFolderId|字符串|邮件的父 MailFolder 的唯一标识符。|
|receivedDateTime|DateTimeOffset|收到邮件的日期和时间。|
|replyTo|[收件人](recipient.md)集合|在答复时使用的电子邮件地址。|
|sender|[recipient](recipient.md)|实际用于生成邮件的帐户。 在多数情况下，此值将与 **from** 属性相同。 从 [共享的邮箱](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)发送邮件或作为[委派](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926)发送邮件时，您可以将该属性设置为不同的值。 在任何情况下，值必须与实际使用的邮箱对应。|
|sentDateTime|DateTimeOffset|发送邮件的日期和时间。|
|subject|字符串|邮件的主题。|
|toRecipients|[收件人](recipient.md)集合|邮件的收件人。|
|uniqueBody|[itemBody](itembody.md)|对于当前邮件独一无二的邮件正文部分。**uniqueBody** 默认不返回，但可以使用 `?$select=uniqueBody` 查询为给定邮件检索它。可以是 HTML 格式或文本格式。|
|webLink|字符串|要在 Outlook Web App 中打开邮件的 URL。<br><br>可以将 ispopout 参数附加到此 URL 的末尾以更改邮件的显示方式。如果 ispopout 不存在或设置为 1，则邮件显示在弹出窗口中。如果 ispopout 设置为 0，则浏览器将在 Outlook Web App 审阅窗格中显示邮件。<br><br>如果通过 Outlook Web App 登录邮箱，该邮件将在浏览器中打开。如果尚未使用浏览器登录，系统将提示你登录。<br><br>可以从 iFrame 中访问此 URL。|

**从 body 属性中删除脚本**

邮件正文可以是 HTML 或文本格式。如果正文是 HTML 格式，默认情况下，在 REST 响应中返回正文内容之前，将删除嵌入 **body** 属性中的任意具有潜在不安全性的 HTML（例如 JavaScript）。若要获取整个原始 HTML 内容，请包括以下 HTTP 请求标头：
```
Prefer: outlook.allow-unsafe-html
```

**设置 from 和 sender 属性**

撰写邮件时，在大多数情况下，From 和 Sender 属性表示同一个已登录用户，除非其中一个属性已更新，如以下情况中所述：

- 如果 Exchange 管理员已将邮箱的 **sendAs** 权限分配给其他一些用户，可以更改 **from** 属性。为此，管理员可以在 Azure 门户中选择邮箱所有者的**邮箱权限**，也可以使用 Exchange 管理中心或 Windows PowerShell Add-ADPermission cmdlet。然后，可以编程方式将 **from** 属性设置为，对相应邮箱拥有 **sendAs** 权限的用户之一。
- 如果邮箱所有者已委派一个或多个用户能够从该邮箱发送邮件，则可以更改 **sender** 属性。可以在 Outlook 中委派邮箱所有者。当代理代表邮箱所有者发送邮件时，**sender** 属性设置为代理的帐户，**from** 属性仍保持为邮箱所有者。可以通过编程方式将 **sender** 属性设置为拥有邮箱代理权限的用户。

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|attachments|[附件](attachment.md)集合|邮件的 [fileAttachment](fileattachment.md) 和 [itemAttachment](itemattachment.md) 附件。|
|extensions|[扩展](extension.md)集合|为邮件定义的开放扩展集合。只读。可为 Null。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合| 为邮件定义的多值扩展属性的集合。只读。可为 Null。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) 集合| 为邮件定义的单值扩展属性的集合。只读。可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.outlookItem",
  "openType": true,
  "optionalProperties": [
    "attachments",
    "extensions",
    "singleValueExtendedProperties",
    "multiValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.message",
  "@odata.annotations": [
    {
      "property": "attachments",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "extensions",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    }
  ]
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
  "flag": {"@odata.type": "microsoft.graph.followupFlag"},
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "String",
  "inferenceClassification": "String",
  "internetMessageHeaders": [{"@odata.type": "microsoft.graph.internetMessageHeader"}],
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
  "webLink": "string",

  "attachments": [{"@odata.type": "microsoft.graph.attachment"}],
  "extensions": [{"@odata.type": "microsoft.graph.extension"}],
  "multiValueExtendedProperties": [{"@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty"}],
  "singleValueExtendedProperties": [{"@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty"}]
}

```

## <a name="see-also"></a>另请参阅

- [获取邮箱设置](../api/user_get_mailboxsettings.md) 
- [更新邮箱设置](../api/user_update_mailboxsettings.md)
- [使用增量查询跟踪 Microsoft Graph 数据更改](../../../concepts/delta_query_overview.md)
- [获取文件夹中邮件的增量更改](../../../concepts/delta_query_messages.md)
- [使用扩展向资源添加自定义数据](../../../concepts/extensibility_overview.md)
- [使用开放扩展向用户添加自定义数据](../../../concepts/extensibility_open_users.md)
- [使用架构扩展向组添加自定义数据](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
