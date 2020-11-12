---
title: chatMessage 资源类型
description: 代表 "频道" 或 "聊天" 实体中的单个聊天消息。 聊天消息可以是一个根聊天消息，也可以是由聊天消息中的 **replyToId** 属性定义的线程的一部分。
doc_type: resourcePageType
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: bfaee36a21ee1f44781ea8ae7fed84b205ac90b4
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000637"
---
# <a name="chatmessage-resource-type"></a>chatMessage 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [渠道](channel.md)或[聊天](chat.md)中的单个聊天信息。 该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。

> **注意** ：此资源支持订阅使用 [更改通知](../resources/webhooks.md) (创建、更新和删除) 所做的更改。 这允许呼叫者实时订阅和获取更改。 有关详细信息，请参阅 [获取邮件通知](/graph/teams-changenotifications-chatMessage)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|**通道邮件**| | |
|[列出频道了 chatmessage](../api/channel-list-messages.md) | [chatMessage](chatmessage.md) 集合 | 频道中所有根聊天邮件的列表。|
|[在频道 delta 中获取 Chatmessages 集合](../api/chatmessage-delta.md)  | [chatMessage](../resources/chatmessage.md) | 获取通道中的增量聊天消息。 |
|[为新的频道消息创建订阅](../api/subscription-post-subscriptions.md) | [订阅](subscription.md) | 收听新的和编辑的频道消息以及对它们的反应。 |
|[获取频道了 chatmessage](../api/channel-get-message.md) | [chatMessage](chatmessage.md) | 从频道中获取单个根聊天消息。|
|[在频道或聊天中创建了 chatmessage](../api/chatmessage-post.md) | [chatMessage](chatmessage.md)| 在频道中创建新的顶级聊天邮件。|
|[更新了 chatmessage](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| 更新聊天邮件的 **policyViolation** 属性。|
|**频道邮件答复**| | |
|[列出对了 chatmessage 的答复](../api/channel-list-messagereplies.md) | [chatMessage](chatmessage.md) 集合| 频道中对聊天消息的所有回复的列表。|
|[获取对了 chatmessage 的答复](../api/channel-get-messagereply.md) | [chatMessage](chatmessage.md)| 获取频道中的聊天消息的单个答复。|
|[答复频道中的了 chatmessage](../api/channel-post-messagereply.md) | [chatMessage](chatmessage.md)| 在频道中答复现有聊天邮件。|
|[更新了 chatmessage](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| 更新聊天邮件的 **policyViolation** 属性。|
|**1:1 和分组聊天消息**| | |
|[在聊天中获取了 chatmessage](../api/chat-get-message.md)  | [chatMessage](../resources/chatmessage.md) | 在聊天中获取单个聊天消息。 |
|[在聊天中列出 Chatmessages 集合](../api/chat-list-message.md)  | [chatMessage](../resources/chatmessage.md) | 列出1:1 或组聊天中的聊天消息。 |
|[创建新聊天邮件的订阅](../api/subscription-post-subscriptions.md) | [订阅](subscription.md) | 收听新的和已编辑的聊天消息以及对它们的反应。 |
|[在聊天中创建了 chatmessage](../api/chat-post-message.md) | [chatMessage](chatmessage.md)| 在现有的1:1 或组聊天对话中发送聊天消息。|
|[更新了 chatmessage](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| 更新聊天邮件的 **policyViolation** 属性。|
|**托管内容**| | |
|[列出所有已承载的内容](../api/chatmessage-list-chatmessagehostedcontents.md) | [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) 集合| 获取聊天消息中的所有托管内容。|
|[获取托管内容](../api/chatmessagehostedcontent-get.md) | [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) | 从聊天消息中获取托管的内容。|


## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|id|字符串| 只读。 消息的唯一 ID。|
|replyToId| string | 只读。 线程的父聊天消息或根聊天消息的 ID。  (仅适用于频道中的聊天消息，而不是聊天。 )  |
|from|[identitySet](identityset.md)| 只读。 聊天消息发件人的详细信息。|
|etag| string | 只读。 聊天消息的版本号。 |
|messageType|string|聊天消息的类型。 可能的值是： `message` 。|
|createdDateTime|dateTimeOffset|只读。 在聊天消息创建时的时间戳。|
|lastModifiedDateTime|dateTimeOffset|只读。  (初始设置) 或修改，包括添加或删除反应时）中创建聊天邮件时的时间戳。 |
|lastEditedDateTime|dateTimeOffset|只读。 在对聊天消息进行编辑时的时间戳。 触发团队 UI 中的 "编辑" 标志。 如果未进行任何编辑，则该值为 `null` 。|
|deletedDateTime|dateTimeOffset|只读。 删除聊天邮件的时间戳，如果未删除，则为 null。 |
|subject|string| 聊天消息的主题，以纯文本形式。|
|body|[itemBody](itembody.md)|聊天消息内容的纯文本/HTML 表示形式。 表示形式由正文中的 contentType 进行指定。 如果聊天消息包含 [chatMessageMention](chatmessagemention.md)，则该内容始终为 HTML。 |
|摘要|string| 可用于推送通知和摘要视图或回退视图的聊天消息的摘要文本。 仅适用于频道聊天消息，而不是聊天中的聊天消息。 |
|附件|[chatMessageAttachment](chatmessageattachment.md) 集合 |附加文件。 附件目前是只读的 – 不支持发送附件。 |
|提及|[chatMessageMention](chatmessagemention.md) 集合| 聊天消息中提及的实体列表。 当前支持用户、机器人、团队、渠道。|
|重要性|string | 聊天消息的重要性。 可能的值包括 `normal`、`high`、`urgent`。|
|反应| [chatMessageReaction](./chatmessagereaction.md) 集合 | 此聊天消息的反应 (例如，如) 。|
|区域设置|string|客户端的聊天消息的区域设置。|
| policyViolation | [chatMessagePolicyViolation](../resources/chatmessagepolicyviolation.md) |定义由数据丢失防护 (DLP) 应用程序设置的策略违规属性。|

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
  "reactions": [{"@odata.type": "microsoft.graph.chatMessageReaction"}],
  "locale": "string",
  "policyViolation": {"@odata.type": "microsoft.graph.chatMessagePolicyViolation"},
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
