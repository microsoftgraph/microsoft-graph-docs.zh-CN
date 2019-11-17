---
title: chatMessage 资源类型
description: 表示渠道或聊天实体内的单个聊天消息。 聊天消息可以是一个根聊天消息，也可以是由聊天消息中的**replyToId**属性定义的线程的一部分。
doc_type: resourcePageType
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: 0d11230402d95009e414c16962a2eb9b5dce1f58
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333363"
---
# <a name="chatmessage-resource-type"></a>chatMessage 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [渠道](channel.md)或[聊天](chat.md)中的单个聊天信息。 聊天消息可以是一个根聊天消息，也可以是由聊天消息中的**replyToId**属性定义的答复线程的一部分。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出频道了 chatmessage](../api/channel-list-messages.md) | [chatMessage](chatmessage.md) 集合 | 频道中所有根聊天邮件的列表。|
|[在频道 delta 中获取 Chatmessages 集合](../api/chatmessage-delta.md)  | [chatMessage](../resources/chatmessage.md) | 获取频道中的增量聊天消息。 |
|[获取频道了 chatmessage](../api/channel-get-message.md) | [chatMessage](chatmessage.md) | 从频道中获取单个根聊天消息。|
|[列出对了 chatmessage 的答复](../api/channel-list-messagereplies.md) | [chatMessage](chatmessage.md) 集合| 频道中对聊天消息的所有回复的列表。|
|[获取对了 chatmessage 的答复](../api/channel-get-messagereply.md) | [chatMessage](chatmessage.md)| 获取频道中的聊天消息的单个答复。|
|[在频道中创建了 chatmessage](../api/channel-post-messages.md) | [chatMessage](chatmessage.md)| 在频道中创建新的顶级聊天邮件。|
|[答复频道中的了 chatmessage](../api/channel-post-messagereply.md) | [chatMessage](chatmessage.md)| 在频道中答复现有聊天邮件。|
|[在聊天中创建了 chatmessage](../api/chat-post-messages.md) | [chatMessage](chatmessage.md)| 在现有的1:1 或组聊天对话中发送聊天消息。|
|[在聊天中列出 Chatmessages 集合](../api/chatmessage-list.md)  | [chatMessage](../resources/chatmessage.md) | 列出1:1 或组聊天中的聊天消息。 |
|[在聊天中获取了 chatmessage](../api/chatmessage-get.md)  | [chatMessage](../resources/chatmessage.md) | 在聊天中获取单个聊天消息。 |
|[列出所有已承载的内容](../api/chatmessage-list-chatmessagehostedcontents.md) | [chatMessageHostedContent](../resources/chatmessagehostedcontent.md)集合| 获取聊天消息中的所有托管内容。|
|[获取托管内容](../api/chatmessagehostedcontent-get.md) | [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) | 从聊天消息中获取托管的内容。|

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|id|String| 只读。 邮件的唯一 Id。|
|replyToId| string | 只读。 线程的父聊天消息或根聊天消息的 Id。 （仅适用于频道中不聊天的聊天邮件） |
|from|[identitySet](identityset.md)| 只读。 聊天消息发件人的详细信息。|
|etag| string | 只读。 聊天消息的版本号。 |
|messageType|chatMessageType|聊天消息的类型。 可能的值是： `message`。|
|createdDateTime|dateTimeOffset|只读。 在聊天消息创建时的时间戳。|
|lastModifiedDateTime|dateTimeOffset|只读。 在创建或编辑聊天消息时的时间戳，包括答复的时间（如果是频道中的根聊天邮件）或添加或删除了反应。 |
|deletedDateTime|dateTimeOffset|只读。 删除聊天邮件的时间戳，如果未删除，则为 null。 |
|subject|string| 聊天消息的主题，以纯文本形式。|
|body|[itemBody](itembody.md)|聊天消息内容的纯文本/HTML 表示形式。 表示形式由正文中的 contentType 进行指定。 如果聊天消息包含[chatMessageMention](chatmessagemention.md)，则该内容始终为 HTML。 |
|摘要|string| 可用于推送通知和摘要视图或回退视图的聊天消息的摘要文本。 仅适用于频道聊天消息，而不是聊天中的聊天消息。 |
|附件|[chatMessageAttachment](chatmessageattachment.md) 集合 |附加文件。 附件目前是只读的 – 不支持发送附件。 |
|提及|[chatMessageMention](chatmessagemention.md) 集合| 聊天消息中提及的实体列表。 当前支持用户、机器人、团队、渠道。|
|重要性| chatMessageImportance | 聊天消息的重要性。 可能的值包括 `normal`、`high`、`urgent`。|
|反应| [chatMessageReaction](chatmessagereaction.md) 集合 | 此聊天消息的反应（例如，如）。|
|区域设置|string|客户端的聊天消息的区域设置。|

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
  "deletedDateTime": "string (timestamp)",
  "subject": "string",
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "summary": "string",
  "attachments": [{"@odata.type": "microsoft.graph.chatMessageAttachment"}],
  "mentions": [{"@odata.type": "microsoft.graph.chatMessageMention"}],
  "importance": "string",
  "policyViolation": "string",
  "reactions": [{"@odata.type": "microsoft.graph.chatMessageReaction"}],
  "locale": "string",
  "deleted": true
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
  "suppressions": []
}
-->
