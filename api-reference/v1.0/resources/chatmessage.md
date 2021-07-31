---
title: chatMessage 资源类型
description: 表示频道或聊天实体中的单个聊天消息。 聊天消息可以是根聊天消息，也可以是由聊天消息中的 **replyToId** 属性定义的线程的一部分。
doc_type: resourcePageType
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
ms.openlocfilehash: 5575b2dd1659e730f04b038a8b6372a7d5662c10
ms.sourcegitcommit: 596b3d5636f3f3e042d180ea8f039f00ebd6b38a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2021
ms.locfileid: "53665887"
---
# <a name="chatmessage-resource-type"></a>chatMessage 资源类型

命名空间：microsoft.graph

表示 [渠道](channel.md)或[聊天](chat.md)中的单个聊天信息。 该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。

> **注意**：此资源支持订阅更改 (使用更改通知创建、) 和 [删除更改](../resources/webhooks.md)。 这使呼叫方可以实时订阅和获取更改。 有关详细信息，请参阅[获取消息通知](/graph/teams-changenotifications-chatMessage)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|**频道消息**| | |
|[列出频道中的消息](../api/channel-list-messages.md) | [chatMessage](chatmessage.md) 集合 | 频道中所有根消息的列表。|
|[获取频道中消息的增量](../api/chatmessage-delta.md)  | [chatMessage](../resources/chatmessage.md) | 获取频道中的增量消息。 |
|[创建新频道消息的订阅](../api/subscription-post-subscriptions.md) | [订阅](subscription.md) | 收听新邮件、已编辑邮件和已删除邮件以及响应消息。 |
|[获取频道中的消息](../api/chatmessage-get.md) | [chatMessage](chatmessage.md) | 获取频道中的单个根消息。|
|[在频道中发送消息](../api/chatmessage-post.md) | [chatMessage](chatmessage.md)| 在频道中创建新的根消息。|
|[更新频道中的消息](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| 更新 **聊天消息的 policyViolation** 属性。|
|**频道消息回复**| | |
|[列出对邮件的答复](../api/chatmessage-list-replies.md) | [chatMessage](chatmessage.md) 集合| 频道中聊天消息的所有回复列表。|
|[获取频道中的回复消息](../api/chatmessage-get.md) | [chatMessage](chatmessage.md) | 获取频道中的单个回复消息。|
|[在频道中回复消息](../api/chatmessage-post-replies.md) | [chatMessage](chatmessage.md)| 回复频道中的现有聊天消息。|
|[更新回复邮件](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| 更新 **聊天消息的 policyViolation** 属性。|
|**聊天消息**| | |
|[列出聊天中的消息](../api/chat-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | 列出聊天中的聊天消息。 |
|[获取聊天中的消息](../api/chatmessage-get.md)  | [chatMessage](../resources/chatmessage.md) | 获取聊天中的单个聊天消息。 |
|[创建新聊天消息的订阅](../api/subscription-post-subscriptions.md) | [订阅](subscription.md) | 收听新的、编辑的和删除的聊天消息，以及这些消息的反应。 |
|[在聊天中发送消息](../api/chat-post-messages.md) | [chatMessage](chatmessage.md)| 在现有的一对一或群组聊天对话中发送聊天消息。|
|[更新聊天中的消息](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| 更新 **聊天消息的 policyViolation** 属性。|
|**托管内容**| | |
|[列出所有托管内容](../api/chatmessage-list-hostedcontents.md) | [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) 集合| 获取与邮件关联的所有托管内容。|
|[获取托管内容](../api/chatmessagehostedcontent-get.md) | [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) | 获取托管的内容 (其字节数) 消息的字节数。|


## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|id|String| 只读。 邮件的唯一 ID。|
|replyToId| string | 只读。 线程的父聊天消息或根聊天消息的 ID。  (仅适用于频道中的聊天消息，而仅适用于 chats)  |
|起始数量|[chatMessageFromIdentitySet](chatmessagefromidentityset.md)| 只读。 聊天消息的发送者的详细信息。|
|etag| string | 只读。 聊天消息的版本号。 |
|messageType|chatMessageType|聊天消息的类型。 可能的值包括 `message`、`chatEvent`、`typing`、`unknownFutureValue`。|
|createdDateTime|dateTimeOffset|创建聊天消息的时间戳。|
|lastModifiedDateTime|dateTimeOffset|只读。 创建聊天消息的时间戳 (设置) 修改，包括添加或删除回应时。 |
|lastEditedDateTime|dateTimeOffset|只读。 编辑聊天消息的时间戳。 在用户界面中触发"已编辑Teams标记。 如果未进行编辑，则值为 `null` 。|
|deletedDateTime|dateTimeOffset|只读。 删除聊天消息的时间戳;如果未删除，则返回 null。 |
|subject|string| 纯文本形式的聊天消息的主题。|
|body|[itemBody](itembody.md)|聊天消息内容的纯文本/HTML 表示形式。 表示形式由正文中的 contentType 进行指定。 如果聊天消息包含 [chatMessageMention](chatmessagemention.md)，则内容始终为 HTML 格式。 |
|摘要|string| 可用于推送通知和摘要视图或回退视图的聊天消息的摘要文本。 仅适用于频道聊天消息，不应用于聊天中的聊天消息。 |
|附件|[chatMessageAttachment](chatmessageattachment.md) 集合 |附加文件。 附件目前是只读的 – 不支持发送附件。 |
|提及|[chatMessageMention](chatmessagemention.md) 集合| 聊天消息中提到的实体列表。 当前支持用户、机器人、团队、渠道。|
|重要性|string | 聊天消息的重要性。 可能的值包括 `normal`、`high`、`urgent`。|
|反应| [chatMessageReaction](chatmessagereaction.md) 集合 | 此聊天消息的反应 (例如，如) 。|
|区域设置|string|客户端设置的聊天消息区域设置。 始终设置为 `en-us`。|
|policyViolation | [chatMessagePolicyViolation](chatmessagepolicyviolation.md) |定义 DLP 应用程序中数据丢失防护设置的策略违反 () 属性。|
|chatId|string|如果消息是在聊天中发送的，则代表聊天的标识。|
|channelIdentity|[channelIdentity](channelidentity.md)|如果消息是在频道中发送的，则代表频道的标识。|
|webUrl|string|只读。 指向邮件中Microsoft Teams。|
## <a name="relationships"></a>关系

| 关系   | 类型    | 说明 |
|:---------------|:--------|:----------|
|replies|[chatMessage](chatmessage.md)| 对指定邮件的答复。 |
|hostedContents|[chatMessageHostedContent](chatmessagehostedcontent.md)| 由用户托管的消息中Microsoft Teams例如图像或代码段。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "replyToId",
    "lastEditedDateTime",
    "deletedDateTime",
    "subject",
    "summary",
    "attachments",
    "mentions",
    "reactions",
    "policyViolation",
    "chatId",
    "channelIdentity"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessage"
}-->


```json
{
  "id": "string (identifier)",
  "replyToId": "string (identifier)",
  "from": {"@odata.type": "microsoft.graph.chatMessageFromIdentitySet"},
  "etag": "string",
  "messageType": "string",
  "createdDateTime": "string (timestamp)",
  "lastModifiedDateTime": "string (timestamp)",
  "lastEditedDateTime": "string (timestamp)",
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
  "chatId": "string",
  "channelIdentity": {"@odata.type": "microsoft.graph.channelIdentity"},
  "webUrl": "string"
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
