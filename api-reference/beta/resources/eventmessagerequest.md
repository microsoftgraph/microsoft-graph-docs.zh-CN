---
title: eventMessageRequest 资源类型
description: 表示会议请求的邮件。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 3d691b814517a6180a42ecd13954e019cc75be8b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973586"
---
# <a name="eventmessagerequest-resource-type"></a>eventMessageRequest 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示会议请求的邮件。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [
    "attachments",
    "event",
    "extensions",
    "previousLocation",
    "previousStartDateTime",
    "previousEndDateTime"
  ],
  "@odata.type": "microsoft.graph.eventMessageRequest"
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
  "endDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "String",
  "inferenceClassification": "String",
  "isDeliveryReceiptRequested": true,
  "isDraft": true,
  "isOutOfDate": "Boolean",
  "isRead": true,
  "isReadReceiptRequested": true,
  "lastModifiedDateTime": "String (timestamp)",
  "location": {"@odata.type": "microsoft.graph.location"},
  "meetingMessageType": "microsoft.graph.meetingMessageType",
  "parentFolderId": "string",
  "previousEndDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "previousLocation": {"@odata.type": "microsoft.graph.location"},
  "previousStartDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "receivedDateTime": "String (timestamp)",
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "replyTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "sender": {"@odata.type": "microsoft.graph.recipient"},
  "sentDateTime": "String (timestamp)",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "subject": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "type": "string",
  "uniqueBody": {"@odata.type": "microsoft.graph.itemBody"},
  "webLink": "string"
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|bccRecipients|[recipient](recipient.md) collection|邮件的密件抄送收件人。|
|body|[itemBody](itembody.md)|邮件的正文。|
|bodyPreview|String|邮件正文中的前 255 个字符。|
|categories|String collection|与邮件关联的类别。|
|ccRecipients|[recipient](recipient.md) collection|邮件的抄送收件人。|
|changeKey|字符串|邮件的版本。|
|conversationId|String|电子邮件所属的对话的 ID。|
|createdDateTime|DateTimeOffset|创建邮件的日期和时间。|
|endDateTime|[DateTimeTimeZone](datetimetimezone.md)|请求的会议的结束时间。|
|发件人|[recipient](recipient.md)|邮箱所有者和邮件发件人。|
|hasAttachments|Boolean|指示邮件是否包含附件。|
|id|字串符号|只读。|
|importance|String| 邮件的重要性：`Low`、`Normal`、`High`。|
|inferenceClassification|String| 可取值为：`Focused`、`Other`。|
|isDeliveryReceiptRequested|Boolean|指示是否需要发送邮件已读回执。|
|isDraft|Boolean|指示邮件是否为草稿。如果尚未发送，则此邮件是一封草稿。|
|isOutOfDate|Boolean|指示此会议请求是否已由较新的请求发出。|
|isRead|Boolean|指示是否已阅读该邮件。|
|isReadReceiptRequested|Boolean|指示是否需要发送邮件已读回执。|
|lastModifiedDateTime|DateTimeOffset|上次更改邮件的日期和时间。|
|位置|[位置](location.md)|请求的会议的位置。|
|meetingMessageType|String| 事件消息的类型：`none`、`meetingRequest`、`meetingCancelled`、`meetingAccepted`、`meetingTentativelyAccepted`、`meetingDeclined`。|
|parentFolderId|String|邮件的父 MailFolder 的唯一标识符。|
|previousEndDateTime|[DateTimeTimeZone](datetimetimezone.md)|请求的会议的上一次结束时间。|
|previousLocation|[Location](location.md)|所请求会议的上一个位置。|
|previousStartDateTime|[DateTimeTimeZone](datetimetimezone.md)|请求的会议的上一次开始时间。|
|receivedDateTime|DateTimeOffset|收到邮件的日期和时间。|
|recurrence|[PatternedRecurrence](patternedrecurrence.md)|请求的会议的定期模式。|
|replyTo|[recipient](recipient.md) collection|在答复时使用的电子邮件地址。|
|sender|[recipient](recipient.md)|实际用于生成邮件的帐户。|
|sentDateTime|DateTimeOffset|发送邮件的日期和时间。|
|startDateTime|[DateTimeTimeZone](datetimetimezone.md)|请求的会议的开始时间。|
|subject|String|邮件的主题。|
|toRecipients|[recipient](recipient.md) collection|邮件的收件人。|
|type|String|所需会议的类型: `singleInstance`、 `occurence`、 `exception`、 `seriesMaster`。|
|uniqueBody|[itemBody](itembody.md)|当前邮件专用的邮件正文部分。|
|webLink|String|要在 Outlook Web App 中打开邮件的 URL。<br><br>可以将 ispopout 参数附加到此 URL 的末尾以更改邮件的显示方式。如果 ispopout 不存在或设置为 1，则邮件显示在弹出窗口中。如果 ispopout 设置为 0，则浏览器将在 Outlook Web App 审阅窗格中显示邮件。<br><br>如果通过 Outlook Web App 登录邮箱，该邮件将在浏览器中打开。如果尚未使用浏览器登录，系统将提示你登录。<br><br>可以从 iFrame 中访问此 URL。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|attachments|[附件](attachment.md) 集合| 只读。可为 Null。|
|event|[事件](event.md)| 与事件消息相关联的事件。对于与会者或会议室资源，假定已将日历助理设为在会议请求事件消息到达时自动更新包含事件的日历。导航属性。只读。|
|extensions|[扩展](extension.md)集合| 只读。 可为 Null。|

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 eventMessage](../api/eventmessage-get.md) | [eventMessage](eventmessage.md) |读取 eventmessage 对象的属性和关系。|
|[创建附件](../api/eventmessage-post-attachments.md) |[附件](attachment.md)| 通过发布到附件集合创建新附件。|
|[列出附件](../api/eventmessage-list-attachments.md) |[Attachment](attachment.md) 集合| 获取附件对象集合。|
|[更新](../api/eventmessage-update.md) | [eventMessage](eventmessage.md)  |更新 eventMessage 对象。 |
|[删除](../api/eventmessage-delete.md) | None |更新 eventMessage 对象。 |
|[复制](../api/message-copy.md)|[邮件](message.md)||
|[createForward](../api/message-createforward.md)|[Message](message.md)||
|[createReply](../api/message-createreply.md)|[邮件](message.md)||
|[createReplyAll](../api/message-createreplyall.md)|[Message](message.md)||
|[转发](../api/message-forward.md)|无|转发邮件。 然后邮件保存在已发送邮件文件夹中。|
|[移动](../api/message-move.md)|[邮件](message.md)|将邮件移动到 mailFolder。|
|[回复](../api/message-reply.md)|无|Replys 到邮件的发件人。 然后邮件保存在已发送邮件文件夹中。|
|[全部回复](../api/message-replyall.md)|无|答复邮件的所有收件人。然后邮件保存在已发送邮件文件夹中。|
|[发送](../api/message-send.md)|无|发送以前创建的邮件草稿。然后邮件保存在已发送邮件文件夹中。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "eventMessageRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
