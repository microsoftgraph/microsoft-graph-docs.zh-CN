---
title: chatMessage 资源类型
description: 表示渠道或聊天实体内的单个聊天消息。 该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。
localization_priority: Priority
ms.openlocfilehash: ef91281eff0cc61f992f659bd33debec03841bb4
ms.sourcegitcommit: a1f1e59ee568340bfabdb524e01cff7860bcc862
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2019
ms.locfileid: "29735577"
---
# <a name="chatmessage-resource-type"></a>chatMessage 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [渠道](channel.md)或聊天实体内的单个聊天信息。 该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出渠道消息](../api/channel-list-messages.md) | [chatmessage](chatmessage.md) 集合 | 获取渠道中的所有根消息列表。|
|[获取渠道消息](../api/channel-get-message.md) | [chatmessage](chatmessage.md) | 获取渠道中的单个根消息。|
|[列出消息回复](../api/channel-list-messagereplies.md) | [chatmessage](chatmessage.md) 集合| 获取渠道中的所有消息回复列表。|
|[获取消息回复](../api/channel-get-messagereply.md) | [chatmessage](chatmessage.md)| 获取渠道中的单个消息回复。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 只读。 消息的唯一 ID。|
|replyToId| string | 线程的父级消息/根消息的 Id |
|from|[identitySet](identityset.md)| 消息发送者的详细信息|
|etag| string | 消息的版本号 |
|messageType|String|消息类型，当前支持的值包括：message、chatEvent、Typing|
|createdDateTime|dateTimeOffset|只读。 创建消息时的时间戳|
|lastModifiedDateTime|dateTimeOffset|只读。 编辑/更新消息时的时间戳|
|deleted|布尔值|指示消息是否已被软删除|
|deletedDateTime|dateTimeOffset|只读。 删除消息时的时间戳 |
|主题|string|消息主题行。 可选|
|正文|[itemBody](itembody.md)|消息内容的纯文本/HTML 表示。 默认返回纯文本，应用程序可选择 HTML 作为查询参数的一部分|
|摘要|string|可用于推送通知的消息摘要文本和摘要视图或回退视图|
|提及|[chatMessageMention](chatmention.md) 集合| 消息中提到的实体列表。 当前支持用户、机器人、团队、渠道|
|重要性| string | 消息重要性包括：正常、高|
|反应| [chatMessageReaction](chatreaction.md) 集合 | 此消息的反应（例如，赞）|
|区域设置|string|客户设置的消息区域设置|
|附件|[chatMessageAttachment](chatattachment.md) 集合 |附加文件|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "deleted",
    "deletedDateTime",
    "attachments",
    "importance",
    "reactions",
    "mentions",
    "subject",
    "summary"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessage"
}-->

```json
{
  "id": "string (identifier)",
  "replyToId": "string (identifier)",
  "from": {"@odata.type": "microsoft.graph.identitySet"},
  "etag": "string",
  "messageType": "string",
  "createdDateTime": "string (timestamp)",
  "lastModifiedDateTime": "string (timestamp)",
  "isDeleted": "boolean",
  "deletedDateTime": "string (timestamp)",
  "subject": "string",
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "summary": "string",
  "attachments": [{"@odata.type": "microsoft.graph.chatMessageAttachment"}],
  "mentions": [{"@odata.type": "microsoft.graph.chatMessageMention"}],
  "importance": "string",
  "reactions": [{"@odata.type": "microsoft.graph.chatMessageReaction"}],
  "locale": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
