---
title: eventMessage 资源类型
description: '表示会议请求、取消或响应（可以是下列任一行为：接受、暂定接受或拒绝）的邮件。 '
ms.openlocfilehash: ab63a2d216b5ff12e88e887cb054ca3cb562620e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043203"
---
# <a name="eventmessage-resource-type"></a>eventMessage 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

表示会议请求、取消或响应（可以是下列任一行为：接受、暂定接受或拒绝）的邮件。 

**EventMessage**实体派生[邮件](message.md)，并[eventMessageRequest](eventmessagerequest.md)派生自**eventMessage**对象表示一个会议请求。 **meetingMessageType** 属性确定事件邮件类型。

如果组织者或应用发送会议请求，会议请求以 **eventMessage** 实例（其中包含 **meetingRequest** 的 **meetingMessageType**）的形式，发送到与会者收件箱中。 此外，Outlook 会自动在与会者日历中创建 **event** 实例，其中 **showAs** 属性设置为 **tentative**。 

若要获取与会者邮箱中关联事件的属性，应用可以使用 **eventMessage** 的 **event** 导航属性，如[获取事件邮件示例](../api/eventmessage-get.md#request-2)中所示。 应用程序还可以响应事件代表与会者以编程方式，通过[接受](../api/event-accept.md)、[暂时接受](../api/event-tentativelyaccept.md)或[拒绝](../api/event-decline.md)该事件。

除了会议请求中，在与会者的会议，用来取消事件管理器的结果的收件箱文件夹或由于与会者响应会议请求的组织者的收件箱中可以找到**eventMessage**实例。 应用可以对事件邮件执行操作，就像对邮件执行操作一样，但略有不同。

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
  "@odata.type": "microsoft.graph.eventMessage"
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
  "conversationIndex": "binary",
  "createdDateTime": "DateTimeOffset",
  "endDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "flag": {"@odata.type": "microsoft.graph.followupFlag"},
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "String",
  "inferenceClassification": "String",
  "internetMessageHeaders": [{"@odata.type": "microsoft.graph.internetMessageHeader"}],
  "internetMessageId": "String",
  "isAllDay": "Boolean",
  "isDeliveryReceiptRequested": true,
  "isDraft": true,
  "isOutOfDate": "Boolean",
  "isRead": true,
  "isReadReceiptRequested": true,
  "lastModifiedDateTime": "DateTimeOffset",
  "location": {"@odata.type": "microsoft.graph.location"},
  "meetingMessageType": {"@odata.type": "microsoft.graph.meetingMessageType"},
  "parentFolderId": "string",
  "receivedDateTime": "DateTimeOffset",
  "recurrence": {"@odata.type": "microsoft.graph.patternedrecurrence"},
  "replyTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "sender": {"@odata.type": "microsoft.graph.recipient"},
  "sentDateTime": "DateTimeOffset",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "subject": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "type": "string",
  "uniqueBody": {"@odata.type": "microsoft.graph.itemBody"},
  "UnsubscribeData": "string",
  "UnsubscribeEnabled": true,
  "webLink": "string"
}

```

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|bccRecipients|[recipient](recipient.md) collection|邮件的密件抄送收件人。|
|body|[itemBody](itembody.md)|邮件的正文。可以是 HTML 格式或文本格式。|
|bodyPreview|字符串|邮件正文中的前 255 个字符。文本格式。 |
|categories|String collection|与邮件关联的类别。|
|ccRecipients|[recipient](recipient.md) collection|邮件的抄送收件人。|
|changeKey|String|邮件的版本。|
|conversationId|String|电子邮件所属对话的 ID。|
|conversationIndex|Binary|电子邮件所属对话的索引。|
|createdDateTime|DateTimeOffset|创建邮件的日期和时间。|
|endDateTime|[dateTimeTimeZone](datetimetimezone.md)|请求会议结束时间。|
|标记|[followUpFlag](followupflag.md)|指示状态、开始日期、截止日期或邮件的完成日期的标记值。|
|发件人|[recipient](recipient.md)|邮箱所有者和邮件发件人。|
|hasAttachments|布尔|指示邮件是否包含附件。|
|id|String||
|importance|String| 邮件的重要性：`low`、`normal`、`high`。|
|inferenceClassification|String| 可取值为：`focused`、`other`。|
|internetMessageHeaders | [internetMessageHeader](internetmessageheader.md) 集合 | 由 [RFC5322](https://www.ietf.org/rfc/rfc5322.txt) 定义的邮件头集合，它提供邮件获取的从发件人到收件人的网络路径的详细信息。 只读。|
|internetMessageId |String |所指定的[RFC5322](https://www.ietf.org/rfc/rfc5322.txt)格式中邮件 ID。 |
|isAllDay |布尔|指示是否事件持续的整个天。 调整此属性需要调整事件以及的**开始日期时间**和**endDateTime**属性。|
|isDeliveryReceiptRequested|布尔|指示是否需要发送邮件已读回执。|
|isDraft|布尔|指示邮件是否为草稿。如果尚未发送，则此邮件是一封草稿。|
|isOutOfDate|布尔|指示是否此会议请求已过期较新的请求。|
|isRead|布尔|指示是否已阅读该邮件。|
|isReadReceiptRequested|布尔|指示是否需要发送邮件已读回执。|
|lastModifiedDateTime|DateTimeOffset|上次更改邮件的日期和时间。|
|location|[位置](location.md)|请求会议的位置。|
|meetingMessageType|String| 事件消息的类型：`none`、`meetingRequest`、`meetingCancelled`、`meetingAccepted`、`meetingTenativelyAccepted`、`meetingDeclined`。|
|parentFolderId|String|邮件的父 MailFolder 的唯一标识符。|
|receivedDateTime|DateTimeOffset|收到邮件的日期和时间。|
|recurrence|[patternedRecurrence](patternedrecurrence.md)|请求会议定期模式。|
|replyTo|[recipient](recipient.md) collection|在答复时使用的电子邮件地址。|
|sender|[recipient](recipient.md)|实际用于生成邮件的帐户。|
|sentDateTime|DateTimeOffset|发送邮件的日期和时间。|
|startDateTime|[dateTimeTimeZone](datetimetimezone.md)|请求的会议的开始时间。|
|subject|String|邮件的主题。|
|toRecipients|[recipient](recipient.md) collection|邮件的收件人。|
|type|字符串|请求会议类型： `singleInstance`， `occurence`， `exception`， `seriesMaster`。|
|uniqueBody|[itemBody](itembody.md)|当前邮件专用的邮件正文部分。|
|UnsubscribeData|String|从 List-Unsubscribe 标头中解析的有效条目。若 UnsubscribeEnabled 属性为 true，则这是 List-Unsubscribe 标头中的邮件命令的数据。|
|UnsubscribeEnabled|布尔|指示邮件是否已启用取消订阅。若 list-Unsubscribe 标头符合 rfc-2369，则其值为 True。|
|webLink|String|要在 Outlook Web App 中打开邮件的 URL。<br><br>可以将 ispopout 参数附加到此 URL 的末尾以更改邮件的显示方式。如果 ispopout 不存在或设置为 1，则邮件显示在弹出窗口中。如果 ispopout 设置为 0，则浏览器将在 Outlook Web App 审阅窗格中显示邮件。<br><br>如果通过 Outlook Web App 登录邮箱，该邮件将在浏览器中打开。如果尚未使用浏览器登录，系统将提示你登录。<br><br>可以从 iFrame 中访问此 URL。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|attachments|[附件](attachment.md) 集合|[FileAttachment](fileattachment.md)和[itemAttachment](itemattachment.md)， [referenceAttachment](referenceattachment.md)附件的邮件的集合。 只读。 可为 Null。|
|event|[event](event.md)| 与事件消息相关联的事件。对于与会者或会议室资源，假定已将日历助理设为在会议请求事件消息到达时自动更新包含事件的日历。导航属性。只读。|
|extensions|[extension](extension.md) 集合| 为 eventMessage 定义的开放扩展集合。只读。可为 NULL。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合| 为 eventMessage 定义的多值扩展属性的集合。只读。可为 Null。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| 为 eventMessage 定义的单值扩展属性的集合。只读。可为 Null。|

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取 eventMessage](../api/eventmessage-get.md) | [eventMessage](eventmessage.md) |读取 eventmessage 对象的属性和关系。|
|[更新](../api/eventmessage-update.md) | [eventMessage](eventmessage.md)  |更新 eventMessage 对象。|
|[删除](../api/eventmessage-delete.md) | 无 |更新 eventMessage 对象。|
|[copy](../api/message-copy.md)|[message](message.md)|将邮件复制到文件夹。|
|[createForward](../api/message-createforward.md)|[message](message.md)|创建转发邮件的草稿。然后，可以[更新](../api/message-update.md)或[发送](../api/message-send.md)草稿。|
|[createReply](../api/message-createreply.md)|[message](message.md)|创建回复邮件的草稿。然后，可以[更新](../api/message-update.md)或[发送](../api/message-send.md)草稿。|
|[createReplyAll](../api/message-createreplyall.md)|[message](message.md)|创建全部答复邮件的草稿。然后，可以[更新](../api/message-update.md)或[发送](../api/message-send.md)草稿。|
|[转发](../api/message-forward.md)|无|转发邮件。然后邮件保存在已发送邮件文件夹中。|
|[move](../api/message-move.md)|[message](message.md)|将邮件移到文件夹。此操作会在目标文件夹中新建邮件副本。|
|[回复](../api/message-reply.md)|无|答复邮件发件人然后邮件保存在已发送邮件文件夹中。|
|[replyAll](../api/message-replyall.md)|无|答复邮件的所有收件人。然后邮件保存在已发送邮件文件夹中。|
|[发送](../api/message-send.md)|无|发送以前创建的邮件草稿。然后邮件保存在已发送邮件文件夹中。|
|[unsubscribe](../api/message-unsubscribe.md)|无|使用 List-Unsubscribe 标头中的第一个 mailto 命令中指定的数据和地址发送邮件。|
|**Attachments**| | |
|[列出附件](../api/eventmessage-list-attachments.md) |[attachment](attachment.md) 集合| 获取 eventMessage 的所有附件。|
|[Add attachment](../api/eventmessage-post-attachments.md) |[attachment](attachment.md)| 通过发布到附件集合，向 eventMessage 添加新附件。|
|**开放扩展**| | |
|[创建开放扩展](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| 创建开放扩展，并在新建或现有的资源实例中添加自定义属性。|
|[获取开放扩展](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md) 集合| 获取打开扩展名按姓名标识。|
|**扩展属性**| | |
|[创建单值扩展属性](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[eventMessage](eventmessage.md)  |在新建或现有 eventMessage 中创建一个或多个单值扩展属性。   |
|[获取具有单值扩展属性的 eventMessage](../api/singlevaluelegacyextendedproperty-get.md)  | [eventMessage](eventmessage.md) | 通过使用 `$expand` 或 `$filter` 获取包含单值扩展属性的 eventMessage。 |
|[创建多值扩展属性](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [eventMessage](eventmessage.md) | 在新建或现有的 eventMessage 中创建一个或多个多值扩展属性。  |
|[获取具有多值扩展属性的 eventMessage](../api/multivaluelegacyextendedproperty-get.md)  | [eventMessage](eventmessage.md) | 使用 `$expand` 获取包含一个多值扩展属性的 eventMessage。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "eventMessage resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
