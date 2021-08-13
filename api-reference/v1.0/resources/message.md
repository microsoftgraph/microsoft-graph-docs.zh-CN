---
title: 邮件资源类型
description: mailFolder 中的邮件。
author: abheek-das
localization_priority: Priority
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 172156bf63c045370e58c63a8933bcf3575a522408868d658a01683a67e1c0e7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237642"
---
# <a name="message-resource-type"></a>邮件资源类型

命名空间：microsoft.graph

mailFolder 中的邮件。

从 Exchange Online 邮箱发送的单个电子邮件的 **toRecipients**、**ccRecipients** 和 **bccRecipients** 属性包含的最大收件人数为 500。 有关详细信息，请参阅[发送限制](/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#sending-limits)。

该资源支持：

- 将你自己的数据添加为自定义 Internet 邮件头。 仅在创建邮件时添加自定义邮件头，并以“x-”开头命名。 邮件发送后，便无法修改邮件头。 若要获取邮件头，请在[获取邮件](../api/message-get.md)操作中应用 `$select` 查询参数。
- 将你自己的数据作为[扩展](/graph/extensibility-overview)添加到自定义属性。
- 订阅[更改通知](/graph/webhooks)。
- 通过提供 [delta](../api/message-delta.md) 函数，使用 [delta 查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出邮件](../api/user-list-messages.md) |[邮件](message.md)集合 | 获取已登录用户的邮箱中的所有邮件（包括“已删除邮件”和“待筛选邮件”文件夹）。 |
|[创建邮件](../api/user-post-messages.md) | [邮件](message.md) | [创建](../api/user-post-messages.md#request-1) 新邮件的草稿。 |
|[获取邮件](../api/message-get.md) | [邮件](message.md) |读取 message 对象的属性和关系。|
|[更新](../api/message-update.md) | [邮件](message.md) |更新 message 对象。|
|[删除](../api/message-delete.md) | 无 |删除 message 对象。 |
|[复制](../api/message-copy.md)|[邮件](message.md)|将邮件复制到文件夹。|
|[createForward](../api/message-createforward.md)|[邮件](message.md)|创建转发邮件的草稿。然后，你可以 [更新](../api/message-update.md) 或 [发送](../api/message-send.md) 草稿。|
|[createReply](../api/message-createreply.md)|[邮件](message.md)|创建回复邮件的草稿。然后，你可以 [更新](../api/message-update.md) 或 [发送](../api/message-send.md) 草稿。|
|[createReplyAll](../api/message-createreplyall.md)|[邮件](message.md)|创建全部答复邮件的草稿。然后，你可以 [更新](../api/message-update.md) 或 [发送](../api/message-send.md) 草稿。|
|[delta](../api/message-delta.md)|[邮件](message.md)集合| 获取指定文件夹中已添加、删除或更新的邮件集。|
|[转发](../api/message-forward.md)|无|转发邮件。然后邮件保存在已发送邮件文件夹中。|
|[移动](../api/message-move.md)|[邮件](message.md)|将邮件移动到文件夹。该操作会在目标文件夹中创建邮件的新副本。|
|[回复](../api/message-reply.md)|无|答复邮件发件人然后邮件保存在已发送邮件文件夹中。|
|[replyAll](../api/message-replyall.md)|无|答复邮件的所有收件人。然后邮件保存在已发送邮件文件夹中。|
|[发送](../api/message-send.md)|无|发送以前创建的邮件草稿。然后邮件保存在已发送邮件文件夹中。|
|**附件**| | |
|[列出附件](../api/message-list-attachments.md) |[附件](attachment.md) 集合| 获取邮件的所有附件。|
|[Add attachment](../api/message-post-attachments.md) |[Attachment](attachment.md)| 通过发布到附件集合，向邮件添加新附件。|
|**开放扩展**| | |
|[创建开放扩展](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| 创建开放扩展，并在新建或现有的资源实例中添加自定义属性。|
|[获取开放扩展](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md) 集合| 获取通过名称或完全限定的名称识别的一个或多个开放扩展对象。|
|**架构扩展**| | |
|[添加架构扩展值](/graph/extensibility-schema-groups) || 创建架构扩展定义，然后使用它向资源添加自定义键入数据。|
|**扩展属性**| | |
|[创建单值扩展属性](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[邮件](message.md)  |在新建或现有的邮件中创建一个或多个单值扩展属性。   |
|[获取具有单值扩展属性的邮件](../api/singlevaluelegacyextendedproperty-get.md)  | [邮件](message.md) | 通过使用 `$expand` 或 `$filter` 获取包含单值扩展属性的邮件。 |
|[创建多值扩展属性](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [邮件](message.md) | 在新建或现有的邮件中创建一个或多个多值扩展属性。  |
|[获取具有多值扩展属性的邮件](../api/multivaluelegacyextendedproperty-get.md)  | [邮件](message.md) | 使用 `$expand` 获取包含一个多值扩展属性的邮件。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|bccRecipients|[recipient](recipient.md) collection|邮件的密件抄送收件人。|
|body|[itemBody](itembody.md)|邮件的正文。 可以是 HTML 格式或文本格式。 查看有关[邮件正文中的安全 HTML](/graph/outlook-create-send-messages#reading-messages-with-control-over-the-body-format-returned)的信息。|
|bodyPreview|字符串|邮件正文中的前 255 个字符。文本格式。|
|categories|String collection|与邮件关联的类别。|
|ccRecipients|[recipient](recipient.md) collection|邮件的抄送收件人。|
|changeKey|String|邮件的版本。|
|conversationId|String|电子邮件所属对话的 ID。|
|conversationIndex|Edm.Binary|指出消息在对话中的位置。|
|createdDateTime|DateTimeOffset|创建邮件的日期和时间。 <br><br> 日期和时间信息采用 ISO 8601 格式，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|flag|[followupFlag](followupflag.md)|指示邮件的状态、开始日期、截止日期或完成日期的标志值。|
|发件人|[recipient](recipient.md)|发送邮件邮箱的所有者。 在多数情况中，此数值与“**发件人**”属性相同，但共享或委派情景除外。 值必须对应于使用的实际邮箱。 查看更多有关为邮件[设置 from 和 sender 属性](/graph/outlook-create-send-messages#setting-the-from-and-sender-properties)的信息。|
|hasAttachments|Boolean|指明邮件是否包含附件。此属性不涉及内联附件。因此，如果邮件仅包含内联附件，此属性为 false。若要验证是否存在内联附件，请分析 **body** 属性，以确定是否有 `src` 属性（例如，`<IMG src="cid:image001.jpg@01D26CD8.6C05F070">`）。|
|id|String|邮件的唯一标识符（请注意，此值可能会随着邮件移动或更改而更改）|
|importance|importance| 邮件的重要性。 可能的值为： `low`、 `normal`和 `high`。|
|inferenceClassification | inferenceClassificationType | 根据推导出的相关性或重要性或根据显式重写，对用户邮件的分类。 可能的值为：`focused` 或 `other`。 |
|internetMessageHeaders | [internetMessageHeader](internetmessageheader.md) 集合 | 由 [RFC5322](https://www.ietf.org/rfc/rfc5322.txt) 定义的邮件头集合。 该集合包括指示邮件从发件人发送到收件人所采用的网络路径的邮件头。 还可以包含保存邮件应用数据的自定义邮件头。 <br><br> 仅在应用 `$select` 查询选项时返回。 只读。 |
|internetMessageId |String |由 [RFC2822](https://www.ietf.org/rfc/rfc2822.txt) 指定格式的邮件 ID。 |
|isDeliveryReceiptRequested|Boolean|指示是否需要发送邮件已读回执。|
|isDraft|Boolean|指示邮件是否为草稿。如果尚未发送，则此邮件是一封草稿。|
|isRead|Boolean|指示是否已阅读该邮件。|
|isReadReceiptRequested|Boolean|指示是否需要发送邮件已读回执。|
|lastModifiedDateTime|DateTimeOffset|上次更改邮件的日期和时间。 <br><br> 日期和时间信息采用 ISO 8601 格式，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|parentFolderId|String|邮件的父 MailFolder 的唯一标识符。|
|receivedDateTime|DateTimeOffset|收到邮件的日期和时间。 <br><br> 日期和时间信息采用 ISO 8601 格式，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|replyTo|[recipient](recipient.md) collection|在答复时使用的电子邮件地址。|
|sender|[recipient](recipient.md)|实际用于生成邮件的帐户。 大多数情况下，此值与“**from**”属性相同。 从[共享邮箱](/exchange/collaboration/shared-mailboxes/shared-mailboxes)发送邮件时，可以将此属性设置为其他值，[对于共享日历，或设置为代理人](/graph/outlook-share-delegate-calendar.md)。 在任何情况下，此值必须对应于使用的实际邮箱。 查看更多有关为邮件[设置 from 和 sender 属性](/graph/outlook-create-send-messages#setting-the-from-and-sender-properties)的信息。|
|sentDateTime|DateTimeOffset|发送邮件的日期和时间。 <br><br> 日期和时间信息采用 ISO 8601 格式，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|subject|String|邮件的主题。|
|toRecipients|[recipient](recipient.md) collection|邮件的收件人。|
|uniqueBody|[itemBody](itembody.md)|对于当前邮件独一无二的邮件正文部分。**uniqueBody** 默认不返回，但可以使用 `?$select=uniqueBody` 查询为给定邮件检索它。可以是 HTML 格式或文本格式。|
|webLink|String|要在 Outlook 网页版中打开邮件的 URL。<br><br>可以将 ispopout 参数附加到此 URL 的末尾以更改邮件的显示方式。 如果 ispopout 不存在或设置为 1，则邮件显示在弹出窗口中。 如果 ispopout 设置为 0，则浏览器将在 Outlook 网页版的审阅窗格中显示邮件。<br><br>如果通过 Outlook 网页版登录邮箱，该邮件将在浏览器中打开。 如果尚未使用浏览器登录，系统将提示你登录。<br><br>无法从 iFrame 中访问此 URL。|


## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|attachments|[附件](attachment.md)集合|邮件的 [fileAttachment](fileattachment.md) 和 [itemAttachment](itemattachment.md) 附件。|
|extensions|[扩展](extension.md)集合|为邮件定义的开放扩展集合。可为空。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合| 为邮件定义的多值扩展属性的集合。只读。可为空。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| 为邮件定义的单值扩展属性的集合。可为空。|

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
    "multiValueExtendedProperties",

    "internetMessageHeaders"
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

- [获取邮箱设置](../api/user-get-mailboxsettings.md)
- [更新邮箱设置](../api/user-update-mailboxsettings.md)
- [使用增量查询跟踪 Microsoft Graph 数据更改](/graph/delta-query-overview)
- [获取文件夹中邮件的增量更改](/graph/delta-query-messages)
- [使用扩展向资源添加自定义数据](/graph/extensibility-overview)
- [使用开放扩展向用户添加自定义数据](/graph/extensibility-open-users)
- [使用架构扩展向组添加自定义数据](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

