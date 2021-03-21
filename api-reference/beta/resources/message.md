---
title: 邮件资源类型
description: 邮箱文件夹中的邮件。
author: abheek-das
localization_priority: Priority
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: a74d4fb6411c1684528b6b36315782bb52373b19
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960409"
---
# <a name="message-resource-type"></a>邮件资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

邮箱文件夹中的邮件。

从 Exchange Online 邮箱发送的单个电子邮件的 **toRecipients**、**ccRecipients** 和 **bccRecipients** 属性包含的最大收件人数为 500。 有关详细信息，请参阅[发送限制](/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#sending-limits)。

该资源支持：

- 将你自己的数据添加为自定义 Internet 邮件头。 仅在创建邮件时添加自定义邮件头，并以“x-”开头命名。 邮件发送后，便无法修改邮件头。 若要获取邮件头，请在[获取邮件](../api/message-get.md)操作中应用 `$select` 查询参数。
- 将你自己的数据作为[扩展](/graph/extensibility-overview)添加到自定义属性。
- 订阅[更改通知](/graph/webhooks)。
- 通过提供 [delta](../api/message-delta.md) 函数，使用 [delta 查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
    "attachments",
    "extensions",
    "singleValueExtendedProperties",
    "multiValueExtendedProperties",
    "mentions",

    "internetMessageHeaders"
  ],
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
  "conversationIndex": "String (binary)",
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
  "mentionsPreview": {"@odata.type": "microsoft.graph.mentionsPreview"},
  "parentFolderId": "string",
  "receivedDateTime": "String (timestamp)",
  "replyTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "sender": {"@odata.type": "microsoft.graph.recipient"},
  "sentDateTime": "String (timestamp)",
  "subject": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "uniqueBody": {"@odata.type": "microsoft.graph.itemBody"},
  "unsubscribeData": "string",
  "unsubscribeEnabled": true,
  "webLink": "string",

  "attachments": [{"@odata.type": "microsoft.graph.attachment"}],
  "extensions": [{"@odata.type": "microsoft.graph.extension"}],
  "mentions": [{"@odata.type": "microsoft.graph.mention"}],
  "multiValueExtendedProperties": [{"@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty"}],
  "singleValueExtendedProperties": [{"@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty"}]
}

```

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------|:-----|:------------|
|bccRecipients|[recipient](recipient.md) collection|邮件的密件抄送收件人。|
|body|[itemBody](itembody.md)|邮件的正文。 可以是 HTML 格式或文本格式。 查看有关[邮件正文中的安全 HTML](/graph/outlook-create-send-messages#reading-messages-with-control-over-the-body-format-returned)的信息。|
|bodyPreview|String|邮件正文中的前 255 个字符。 文本格式。 如果消息包含 [mention](mention.md) 实例，该属性也包含这些提及内容的串联。 |
|类别|String collection|与邮件关联的类别。 每个类别对应于为用户定义的 [outlookCategory](outlookcategory.md) 的 **displayName** 属性。 |
|ccRecipients|[recipient](recipient.md) collection|邮件的抄送收件人。|
|changeKey|String|邮件的版本。|
|conversationId|String|电子邮件所属对话的 ID。|
|conversationIndex|Edm.Binary|指出消息在对话中的位置。|
|createdDateTime|DateTimeOffset|创建邮件的日期和时间。 <br><br> 日期和时间信息采用 ISO 8601 格式，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|flag|[followupFlag](followupflag.md)|指示邮件的状态、开始日期、截止日期或完成日期的标志值。|
|发件人|[recipient](recipient.md)|发送邮件邮箱的所有者。 在多数情况中，此数值与“**发件人**”属性相同，但共享或委派情景除外。 值必须对应于使用的实际邮箱。 查看更多有关为邮件[设置 from 和 sender 属性](/graph/outlook-create-send-messages#setting-the-from-and-sender-properties)的信息。|
|hasAttachments|Boolean|指明邮件是否包含附件。此属性不涉及内联附件。因此，如果邮件仅包含内联附件，此属性为 false。若要验证是否存在内联附件，请分析 **body** 属性，以确定是否有 `src` 属性（例如，`<IMG src="cid:image001.jpg@01D26CD8.6C05F070">`）。 |
|id|String| 邮件的唯一标识符。 [!INCLUDE [outlook-beta-id](../../includes/outlook-beta-id.md)] 只读。 |
|importance|importance| 邮件的重要性。 可能的值为： `low`、 `normal`和 `high`。|
|inferenceClassification|inferenceClassificationType| 根据推导出的相关性或重要性或显式替代，对用户邮件的分类。可能的值是：`focused`、`other`。|
|internetMessageHeaders | [internetMessageHeader](internetmessageheader.md) 集合 | 由 [RFC5322](https://www.ietf.org/rfc/rfc5322.txt) 定义的邮件头集合。 该集合包括指示邮件从发件人发送到收件人所采用的网络路径的邮件头。 还可以包含保存邮件应用数据的自定义邮件头。 <br><br> 仅在应用 `$select` 查询选项时返回。 只读。|
|internetMessageId | String | 邮件 ID 采用 [RFC5322](https://www.ietf.org/rfc/rfc5322.txt) 指定的格式。 仅当 **isDraft** 为 true 时才更更新。|
|isDeliveryReceiptRequested|Boolean|指示是否需要发送邮件已读回执。|
|isDraft|Boolean|指示邮件是否为草稿。如果尚未发送，则此邮件是一封草稿。|
|isRead|Boolean|指示是否已阅读该邮件。|
|isReadReceiptRequested|Boolean|指示是否需要发送邮件已读回执。|
|lastModifiedDateTime|DateTimeOffset|上次更改邮件的日期和时间。 <br><br> 日期和时间信息采用 ISO 8601 格式，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|mentionsPreview|[mentionsPreview](mentionspreview.md)|邮件中的提及的相关信息。处理 `GET` /messages 请求时，服务器会设置此属性并默认将其包含在响应中。若邮件中无提及，则服务器返回 NULL。可选。 |
|parentFolderId|String|邮件的父 MailFolder 的唯一标识符。|
|receivedDateTime|DateTimeOffset|收到邮件的日期和时间。 <br><br> 日期和时间信息采用 ISO 8601 格式，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|replyTo|[recipient](recipient.md) collection|在答复时使用的电子邮件地址。|
|sender|[recipient](recipient.md)|实际用于生成邮件的帐户。 大多数情况下，此值与“**from**”属性相同。 从[共享邮箱](/exchange/collaboration/shared-mailboxes/shared-mailboxes)发送邮件时，可以将此属性设置为其他值，[对于共享日历，或设置为代理人](/graph/outlook-share-delegate-calendar.md)。 在任何情况下，此值必须对应于使用的实际邮箱。 查看更多有关为邮件[设置 from 和 sender 属性](/graph/outlook-create-send-messages#setting-the-from-and-sender-properties)的信息。|
|sentDateTime|DateTimeOffset|发送邮件的日期和时间。 <br><br> 日期和时间信息采用 ISO 8601 格式，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|subject|String|邮件的主题。|
|toRecipients|[recipient](recipient.md) collection|邮件的收件人。|
|uniqueBody|[itemBody](itembody.md)|对于当前邮件独一无二的邮件正文部分。**uniqueBody** 默认不返回，但可以使用 `?$select=uniqueBody` 查询为给定邮件检索它。可以是 HTML 格式或文本格式。|
|unsubscribeData|String|从 List-Unsubscribe 标头中解析的有效条目。若 UnsubscribeEnabled 属性为 true，则这是 List-Unsubscribe 标头中的邮件命令的数据。|
|unsubscribeEnabled|Boolean|指示邮件是否已启用取消订阅。若 list-Unsubscribe 标头符合 rfc-2369，则其值为 True。|
|webLink|String|要在 Outlook 网页版中打开邮件的 URL。<br><br>可以将 ispopout 参数附加到此 URL 的末尾以更改邮件的显示方式。 如果 ispopout 不存在或设置为 1，则邮件显示在弹出窗口中。 如果 ispopout 设置为 0，则浏览器将在 Outlook 网页版的审阅窗格中显示邮件。<br><br>如果通过 Outlook 网页版登录邮箱，该邮件将在浏览器中打开。 如果尚未使用浏览器登录，系统将提示你登录。<br><br>无法从 iFrame 中访问此 URL。|

## <a name="relationships"></a>关系

| 关系 | 类型 |说明|
|:---------------|:--------|:----------|
|attachments|[附件](attachment.md) 集合|邮件的 [fileAttachment](fileattachment.md) 和 [itemAttachment](itemattachment.md) 附件。|
|extensions|[Extension](extension.md) 集合| 为邮件定义的开放扩展集合。 可为空。|
|提及|[mention](mention.md) 集合 | 邮件中的提及集合，按 **createdDateTime** 由最新到最旧排序。默认情况下，`GET` /messages 不会返回此属性，在该属性上应用 `$expand` 时除外。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合| 为邮件定义的多值扩展属性的集合。 可为空。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| 为邮件定义的单值扩展属性的集合。可为空。|

## <a name="methods"></a>方法

| 方法 | 返回类型 |说明|
|:-------|:------------|:----------|
|[列出邮件](../api/user-list-messages.md) |[邮件](message.md)集合 | 获取已登录用户的邮箱中的所有邮件（包括“已删除邮件”和“待筛选邮件”文件夹）。 |
|[创建邮件](../api/user-post-messages.md) | [邮件](message.md) | 创建新邮件的草稿。 |
|[获取邮件](../api/message-get.md) | [邮件](message.md) |读取 message 对象的属性和关系。|
|[更新](../api/message-update.md) | [邮件](message.md) |更新 message 对象。 |
|[删除](../api/message-delete.md) | 无 |删除 message 对象。 |
|[复制](../api/message-copy.md)|[邮件](message.md)|将邮件复制到文件夹。|
|[createForward](../api/message-createforward.md)|[Message](message.md)|创建转发邮件草稿以全部在一个 createForward 调用中添加注释或更新任意邮件属性。然后，你可以更新或发送草稿。|
|[createReply](../api/message-createreply.md)|[Message](message.md)|创建回复邮件草稿以全部在一个 createReply 调用中添加注释或更新任意邮件属性。然后，你可以更新或发送草稿。|
|[createReplyAll](../api/message-createreplyall.md)|[Message](message.md)|创建回复全部邮件草稿以全部在一个 createReplyAll 调用中添加注释或更新任意邮件属性。然后，你可以更新或发送草稿。|
|[删除](../api/message-delta.md)|[邮件](message.md)集合| 获取指定文件夹中已添加、删除或更新的邮件集。|
|[转发](../api/message-forward.md)|无|全部在一个 **forward** 调用中转发邮件、添加注释或修改任意可更新的属性。然后邮件保存在已发送邮件文件夹中。|
|[移动](../api/message-move.md)|[邮件](message.md)|将邮件移动到文件夹。该操作会在目标文件夹中创建邮件的新副本。|
|[回复](../api/message-reply.md)|无|全部在一个 **reply** 调用中回复邮件的发件人、添加注释或修改任意可更新的属性。然后邮件保存在已发送邮件文件夹中。|
|[全部回复](../api/message-replyall.md)|无|通过指定注释和修改回复的任意可更新属性来回复邮件的所有收件人，全部通过使用 **replyAll** 方法实现。然后邮件保存在已发送邮件文件夹中。|
|[发送](../api/message-send.md)|无|发送以前创建的邮件草稿。然后邮件保存在已发送邮件文件夹中。|
|[取消订阅](../api/message-unsubscribe.md)|无|使用 List-Unsubscribe 标头中的第一个 mailto 命令中指定的数据和地址发送邮件。|
|**附件**| | |
|[列出附件](../api/message-list-attachments.md) |[Attachment](attachment.md) 集合| 获取邮件的所有附件。|
|[添加附件](../api/message-post-attachments.md) |[Attachment](attachment.md)| 通过发布到附件集合，向邮件添加新附件。|
|**开放扩展**| | |
|[创建开放扩展](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| 创建开放扩展，并将自定义属性添加到新资源或现有资源。|
|[获取开放扩展](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md) 集合| 获取扩展名称标识的开放扩展。|
|**架构扩展**| | |
|[添加架构扩展值](/graph/extensibility-schema-groups) || 创建架构扩展定义，然后使用它向资源添加自定义键入数据。|
|**扩展属性**| | |
|[创建单值扩展属性](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[邮件](message.md)  |在新建或现有的邮件中创建一个或多个单值扩展属性。   |
|[获取具有单值扩展属性的邮件](../api/singlevaluelegacyextendedproperty-get.md)  | [邮件](message.md) | 通过使用 `$expand` 或 `$filter` 获取包含单值扩展属性的邮件。 |
|[创建多值扩展属性](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [邮件](message.md) | 在新建或现有的邮件中创建一个或多个多值扩展属性。  |
|[获取具有多值扩展属性的邮件](../api/multivaluelegacyextendedproperty-get.md)  | [邮件](message.md) | 使用 `$expand` 获取包含一个多值扩展属性的邮件。 |

## <a name="see-also"></a>另请参阅

- [获取邮箱设置](../api/user-get-mailboxsettings.md)
- [更新邮箱设置](../api/user-update-mailboxsettings.md)
- [使用增量查询跟踪 Microsoft Graph 数据更改](/graph/delta-query-overview)
- [获取文件夹中邮件的增量更改](/graph/delta-query-messages)
- [使用扩展向资源添加自定义数据](/graph/extensibility-overview)
- [使用开放扩展向用户添加自定义数据](/graph/extensibility-open-users)
- [使用架构扩展向组添加自定义数据](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}



