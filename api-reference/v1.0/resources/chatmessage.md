---
title: chatMessage 资源类型
description: 表示渠道或聊天实体内的单个聊天消息。 聊天消息可以是一个根聊天消息，也可以是由聊天消息中的 **replyToId** 属性定义的线程的一部分。
doc_type: resourcePageType
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: a3d994379b3b15170ff490433827eda79c18d4f7
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2020
ms.locfileid: "48849191"
---
# <a name="chatmessage-resource-type"></a>chatMessage 资源类型

命名空间：microsoft.graph

代表 beta) [研讨](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true)中的[频道](./channel.md)或 (内的单个聊天邮件。 聊天消息可以是一个根聊天消息，也可以是由聊天消息中的 **replyToId** 属性定义的答复线程的一部分。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|**通道邮件**| | |
|[列出频道了 chatmessage](../api/channel-list-messages.md) | [chatMessage](chatmessage.md) 集合 | 频道中所有根聊天邮件的列表。|
|[在频道 delta 中获取 Chatmessages 集合](../api/chatmessage-delta.md)  | [chatMessage](../resources/chatmessage.md) | 获取通道中的增量聊天消息。 |
|[为新的频道消息创建订阅](../api/subscription-post-subscriptions.md) | [订阅](subscription.md) | 收听新的和编辑的频道消息以及对它们的反应。 |
|[获取频道了 chatmessage](../api/channel-get-message.md) | [chatMessage](chatmessage.md) | 从频道中获取单个根聊天消息。|
|[在频道中创建 chatMessage](../api/channel-post-messages.md) | [chatMessage](../resources/chatmessage.md) | 向频道发送消息。 |
|[更新了 chatmessage](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| 更新聊天邮件的 **policyViolation** 属性。|
|**频道邮件答复**| | |
|[列出对了 chatmessage 的答复](../api/channel-list-messagereplies.md) | [chatMessage](chatmessage.md) 集合| 频道中对聊天消息的所有回复的列表。|
|[获取对了 chatmessage 的答复](../api/channel-get-messagereply.md) | [chatMessage](chatmessage.md)| 获取频道中的聊天消息的单个答复。|
|[答复频道中的了 chatmessage](../api/channel-post-messagereply.md) | [chatMessage](chatmessage.md)| 在频道中答复现有聊天邮件。|
|[更新了 chatmessage](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| 更新聊天邮件的 **policyViolation** 属性。|

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|id|String| 只读。 邮件的唯一 Id。|
|replyToId| string | 只读。 线程的父聊天消息或根聊天消息的 Id。  (仅适用于频道中不聊天的聊天消息)  |
|from|[identitySet](identityset.md)| 只读。 聊天消息发件人的详细信息。|
|etag| string | 只读。 聊天消息的版本号。 |
|messageType|string|聊天消息的类型。 可能的值是： `message` 。|
|createdDateTime|dateTimeOffset|只读。 在聊天消息创建时的时间戳。|
|lastModifiedDateTime|dateTimeOffset|只读。 在 (初始设置) 或编辑时（包括添加或删除反应时）创建聊天邮件时的时间戳。 |
|lastEditedDateTime|dateTimeOffset|只读。 在对聊天消息进行编辑时的时间戳。 触发 Microsoft 团队 UI 中的 "编辑" 标志。 如果未进行任何编辑，则该值为 `null` 。|
|deletedDateTime|dateTimeOffset|只读。 删除聊天邮件的时间戳，如果未删除，则为 null。 |
|subject|string| 聊天消息的主题，以纯文本形式。|
|body|[itemBody](itembody.md)|聊天消息内容的纯文本/HTML 表示形式。 表示形式由正文中的 contentType 进行指定。 如果聊天消息包含 [chatMessageMention](chatmessagemention.md)，则该内容始终为 HTML。 |
|摘要|string| 可用于推送通知和摘要视图或回退视图的聊天消息的摘要文本。 仅适用于频道聊天消息，而不是聊天中的聊天消息。 |
|附件|[chatMessageAttachment](chatmessageattachment.md) 集合 |附加文件。 附件目前是只读的 – 不支持发送附件。 |
|提及|[chatMessageMention](chatmessagemention.md) 集合| 聊天消息中提及的实体列表。 当前支持用户、机器人、团队、渠道。|
|重要性| string | 聊天消息的重要性。 可能的值包括 `normal`、`high`、`urgent`。|
| policyViolation | [chatMessagePolicyViolation](../resources/chatmessagepolicyviolation.md) |定义由数据丢失防护 (DLP) 应用程序设置的策略违规属性。|
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
    "mentions",
    "subject",
    "summary",
    "policyViolation",
    "locale"
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
  "policyViolation": {"@odata.type": "microsoft.graph.chatMessagePolicyViolation"},
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
  "suppressions": []
}
-->
