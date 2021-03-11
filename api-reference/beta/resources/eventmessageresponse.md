---
title: eventMessageResponse 资源类型
description: 一条消息，表示对会议组织者邮箱中的会议请求的响应。
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 40c5ea3956d15a9016361d64b1e27b84e9a30e94
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721864"
---
# <a name="eventmessageresponse-resource-type"></a>eventMessageResponse 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

一条消息，表示对会议组织者邮箱中的会议请求的响应。

派生自 [eventMessage](eventmessage.md)。 

接收 **responseType** 设置为 or 且包含 proposedNewTime 属性的 **eventMessageResponse** 的组织者可以选择 `tentativelyAccepted` `declined` 接受建议。  为此，首先，使用 **eventMessageResponse** 的事件导航属性访问相应的事件，如以下示例 [所示](../api/eventmessage-get.md#example-2)。  然后将 [关联的](../api/event-update.md) 事件更新为建议的时间。

若要详细了解如何建议时间，以及如何接收和接受新时间建议，请参阅["建议新的会议时间"。](/graph/outlook-calendar-meeting-proposals)

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
|[获取 eventMessage](../api/eventmessage-get.md) | [eventMessage](eventmessage.md) |读取 eventmessage 对象的属性和关系。|
|[更新](../api/eventmessage-update.md) | [eventMessage](eventmessage.md)  |更新 eventMessage 对象。|
|[删除](../api/eventmessage-delete.md) | 无 |更新 eventMessage 对象。|
|[copy](../api/message-copy.md)|[message](message.md)|将邮件复制到文件夹。|
|[createForward](../api/message-createforward.md)|[message](message.md)|创建转发邮件的草稿。然后，你可以 [更新](../api/message-update.md) 或 [发送](../api/message-send.md) 草稿。|
|[createReply](../api/message-createreply.md)|[message](message.md)|创建回复邮件的草稿。然后，你可以 [更新](../api/message-update.md) 或 [发送](../api/message-send.md) 草稿。|
|[createReplyAll](../api/message-createreplyall.md)|[message](message.md)|创建全部答复邮件的草稿。然后，可以[更新](../api/message-update.md)或[发送](../api/message-send.md)草稿。|
|[转发](../api/message-forward.md)|无|转发邮件。然后邮件保存在已发送邮件文件夹中。|
|[移动](../api/message-move.md)|[message](message.md)|将邮件移到文件夹。此操作会在目标文件夹中新建邮件副本。|
|[回复](../api/message-reply.md)|无|答复邮件发件人然后邮件保存在已发送邮件文件夹中。|
|[replyAll](../api/message-replyall.md)|无|答复邮件的所有收件人。然后邮件保存在已发送邮件文件夹中。|
|[发送](../api/message-send.md)|无|发送以前创建的邮件草稿。然后邮件保存在已发送邮件文件夹中。|
|[取消订阅](../api/message-unsubscribe.md)|无|使用 List-Unsubscribe 标头中的第一个 mailto 命令中指定的数据和地址发送邮件。|
|**附件**| | |
|[列出附件](../api/eventmessage-list-attachments.md) |[attachment](attachment.md) 集合| 获取 eventMessage 的所有附件。|
|[Add attachment](../api/eventmessage-post-attachments.md) |[attachment](attachment.md)| 通过发布到附件集合，向 eventMessage 添加新附件。|
|**开放扩展**| | |
|[创建开放扩展](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| 创建开放扩展，并在新建或现有的资源实例中添加自定义属性。|
|[获取开放扩展](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md) 集合| 获取由名称标识的开放扩展。|
|**扩展属性**| | |
|[创建单值扩展属性](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[eventMessage](eventmessage.md)  |在新建或现有 eventMessage 中创建一个或多个单值扩展属性。   |
|[获取具有单值扩展属性的 eventMessage](../api/singlevaluelegacyextendedproperty-get.md)  | [eventMessage](eventmessage.md) | 通过使用 `$expand` 或 `$filter` 获取包含单值扩展属性的 eventMessage。 |
|[创建多值扩展属性](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [eventMessage](eventmessage.md) | 在新建或现有的 eventMessage 中创建一个或多个多值扩展属性。  |
|[获取具有多值扩展属性的 eventMessage](../api/multivaluelegacyextendedproperty-get.md)  | [eventMessage](eventmessage.md) | 使用 `$expand` 获取包含一个多值扩展属性的 eventMessage。 |


## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|bccRecipients|[recipient](recipient.md) collection|邮件的密件抄送收件人。|
|body|[itemBody](itembody.md)|邮件的正文。可以是 HTML 格式或文本格式。|
|bodyPreview|字符串|邮件正文中的前 255 个字符。文本格式。 |
|categories|String collection|与邮件关联的类别。|
|ccRecipients|[recipient](recipient.md) collection|邮件的抄送收件人。|
|changeKey|String|邮件的版本。|
|conversationId|String|电子邮件所属对话的 ID。|
|conversationIndex|Edm.Binary|电子邮件所属对话的索引。|
|createdDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|endDateTime|[dateTimeTimeZone](datetimetimezone.md)|所请求会议结束时间。|
|flag|[followupFlag](followupflag.md)|指示邮件的状态、开始日期、截止日期或完成日期的标志值。|
|发件人|[recipient](recipient.md)|发送邮件邮箱的所有者。 在多数情况中，此数值与“**发件人**”属性相同，但共享或委派情景除外。 值必须对应于使用的实际邮箱。 查看更多有关为邮件[设置 from 和 sender 属性](/graph/outlook-create-send-messages#setting-the-from-and-sender-properties)的信息。|
|hasAttachments|Boolean|指示邮件是否包含附件。|
|id|String| 邮件的唯一标识符。 [!INCLUDE [outlook-beta-id](../../includes/outlook-beta-id.md)] 只读。 |
|importance|String| 邮件的重要性：`low`、`normal`、`high`。|
|inferenceClassification|String| 可取值为：`focused`、`other`。|
|internetMessageHeaders | [internetMessageHeader](internetmessageheader.md) 集合 | 由 [RFC5322](https://www.ietf.org/rfc/rfc5322.txt) 定义的邮件头集合，它提供邮件获取的从发件人到收件人的网络路径的详细信息。 只读。|
|internetMessageId |String |邮件 ID 采用 [RFC5322](https://www.ietf.org/rfc/rfc5322.txt) 指定的格式。 |
|isAllDay |Boolean|指示事件是否持续一整天。 调整此属性还需要调整 **事件的 startDateTime** 和 **endDateTime** 属性。|
|isDelegated|布尔|如果代理可以访问此会议请求响应，则其为 True，否则为 false。 默认为 false。|
|isDeliveryReceiptRequested|Boolean|指示是否需要发送邮件已读回执。|
|isDraft|Boolean|指示邮件是否为草稿。如果尚未发送，则此邮件是一封草稿。|
|isOutOfDate|布尔|指示此会议请求是否已由最新请求过时。|
|isRead|Boolean|指示是否已阅读该邮件。|
|isReadReceiptRequested|Boolean|指示是否需要发送邮件已读回执。|
|lastModifiedDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|location|[位置](location.md)|所请求会议的位置。|
|meetingMessageType|String| 事件消息的类型：`none`、`meetingRequest`、`meetingCancelled`、`meetingAccepted`、`meetingTentativelyAccepted`、`meetingDeclined`。|
|mentionsPreview|[mentionsPreview](mentionspreview.md)|邮件中的提及的相关信息。处理 `GET` /messages 请求时，服务器会设置此属性并默认将其包含在响应中。若邮件中无提及，则服务器返回 NULL。可选。 |
|parentFolderId|String|邮件的父 MailFolder 的唯一标识符。|
|proposedNewTime|[timeSlot](timeslot.md)|被邀请者为开始和结束会议请求建议的备用日期/时间。 只读。 不可筛选。|
|receivedDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|recurrence|[patternedRecurrence](patternedrecurrence.md)|请求定期模式的组。|
|replyTo|[recipient](recipient.md) collection|在答复时使用的电子邮件地址。|
|responseType|string| 指定对会议请求的响应类型。 可取值为：`tentativelyAccepted`、`accepted`、`declined`。 对于 eventMessageResponse 类型 `none` ， `organizer` `notResponded` 和不受支持。 只读。 不可筛选。|
|sender|[recipient](recipient.md)|实际用于生成邮件的帐户。 大多数情况下，此值与“**from**”属性相同。 从[共享邮箱](/exchange/collaboration/shared-mailboxes/shared-mailboxes)发送邮件时，可以将此属性设置为其他值，[对于共享日历，或设置为代理人](/graph/outlook-share-delegate-calendar.md)。 在任何情况下，此值必须对应于使用的实际邮箱。 查看更多有关为邮件[设置 from 和 sender 属性](/graph/outlook-create-send-messages#setting-the-from-and-sender-properties)的信息。|
|sentDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|startDateTime|[dateTimeTimeZone](datetimetimezone.md)|请求的会议的开始时间。|
|subject|String|邮件的主题。|
|toRecipients|[recipient](recipient.md) collection|邮件的收件人。|
|type|String|请求的会议类型： ， `singleInstance` `occurence` ， `exception` `seriesMaster` 。|
|uniqueBody|[itemBody](itembody.md)|当前邮件专用的邮件正文部分。|
|UnsubscribeData|String|从 List-Unsubscribe 标头中解析的有效条目。若 UnsubscribeEnabled 属性为 true，则这是 List-Unsubscribe 标头中的邮件命令的数据。|
|UnsubscribeEnabled|Boolean|指示邮件是否已启用取消订阅。若 list-Unsubscribe 标头符合 rfc-2369，则其值为 True。|
|webLink|String|要在 Outlook 网页版中打开邮件的 URL。<br><br>可以将 ispopout 参数附加到此 URL 的末尾以更改邮件的显示方式。 如果 ispopout 不存在或设置为 1，则邮件显示在弹出窗口中。 如果 ispopout 设置为 0，则浏览器将在 Outlook 网页版的审阅窗格中显示邮件。<br><br>如果通过 Outlook 网页版登录邮箱，该邮件将在浏览器中打开。 如果尚未使用浏览器登录，系统将提示你登录。<br><br>无法从 iFrame 中访问此 URL。|


## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|attachments|[附件](attachment.md)集合|邮件的 [fileAttachment](fileattachment.md) [、itemAttachment](itemattachment.md)和 [referenceAttachment](referenceattachment.md) 附件的集合。 只读。 可为 NULL。|
|event|[event](event.md)| 与事件消息相关联的事件。对于与会者或会议室资源，假定已将日历助理设为在会议请求事件消息到达时自动更新包含事件的日历。导航属性。只读。|
|extensions|[扩展](extension.md)集合| 为 eventMessage 定义的开放扩展集合。只读。可为 NULL。|
|提及|[mention](mention.md) 集合 | 邮件中的提及集合，按 **createdDateTime** 由最新到最旧排序。默认情况下，`GET` /messages 不会返回此属性，在该属性上应用 `$expand` 时除外。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合| 为 eventMessage 定义的多值扩展属性的集合。只读。可为 Null。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| 为 eventMessage 定义的单值扩展属性的集合。只读。可为 Null。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.eventMessageResponse",
  "baseType": "microsoft.graph.eventMessage",
  "keyProperty": "id"
}-->

```json
{
  "bccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "bodyPreview": "String",
  "categories": ["String"],
  "ccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "changeKey": "String",
  "conversationId": "String",
  "conversationIndex": "String (binary)",
  "createdDateTime": "String (timestamp)",
  "endDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "flag": {"@odata.type": "microsoft.graph.followupFlag"},
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "String (identifier)",
  "importance": "string",
  "inferenceClassification": "string",
  "internetMessageHeaders": [{"@odata.type": "microsoft.graph.internetMessageHeader"}],
  "internetMessageId": "String",
  "isAllDay": true,
  "isDelegated": true,
  "isDeliveryReceiptRequested": true,
  "isDraft": true,
  "isOutOfDate": true,
  "isRead": true,
  "isReadReceiptRequested": true,
  "lastModifiedDateTime": "String (timestamp)",
  "location": {"@odata.type": "microsoft.graph.location"},
  "meetingMessageType": "string",
  "mentionsPreview": {"@odata.type": "microsoft.graph.mentionsPreview"},
  "parentFolderId": "String",
  "proposedNewTime": {"@odata.type": "microsoft.graph.timeSlot"},
  "receivedDateTime": "String (timestamp)",
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "replyTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "responseType": "string",
  "sender": {"@odata.type": "microsoft.graph.recipient"},
  "sentDateTime": "String (timestamp)",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "subject": "String",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "type": "string",
  "uniqueBody": {"@odata.type": "microsoft.graph.itemBody"},
  "unsubscribeData": ["String"],
  "unsubscribeEnabled": true,
  "webLink": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "eventMessageResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

