---
title: chatMessage 资源类型
description: 表示频道或聊天实体中的单个聊天消息。 聊天消息可以是根聊天消息，也可以是由聊天消息中的 **replyToId** 属性定义的线程的一部分。
doc_type: resourcePageType
ms.localizationpriority: medium
author: RamjotSingh
ms.prod: microsoft-teams
ms.openlocfilehash: 8b449c28f8283096696a6d95704de46cadaa8cfb
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61860934"
---
# <a name="chatmessage-resource-type"></a>chatMessage 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [渠道](channel.md)或[聊天](chat.md)中的单个聊天信息。 该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。

> **注意**：此资源支持订阅更改 (使用更改通知) 、更新和 [删除更改](../resources/webhooks.md)。 这使呼叫方可以实时订阅和获取更改。 有关详细信息，请参阅[获取消息通知](/graph/teams-changenotifications-chatMessage)。

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
|[为用户在所有聊天中获取消息](../api/chats-getallmessages.md)| [chat](chat.md) 集合| 从用户是参与者的所有聊天获取消息，包括一对一聊天、群聊和会议聊天。 |
|[获取所有频道消息](../api/channel-getallmessages.md)|[channel](channel.md) 集合 | 获取用户参与的所有频道中的所有消息。 |
|[创建新聊天消息的订阅](../api/subscription-post-subscriptions.md) | [订阅](subscription.md) | 收听新的、编辑的和删除的聊天消息，并响应这些消息。 |
|[在聊天中发送消息](../api/chat-post-messages.md) | [chatMessage](chatmessage.md)| 在现有的一对一或群组聊天对话中发送聊天消息。|
|[更新聊天中的消息](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| 更新 **聊天消息的 policyViolation** 属性。|
|**托管内容**| | |
|[列出所有托管内容](../api/chatmessage-list-hostedcontents.md) | [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) 集合| 获取与邮件关联的所有托管内容。|
|[获取托管内容](../api/chatmessagehostedcontent-get.md) | [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) | 获取托管的内容 (其字节数) 消息的字节数。|

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|attachments|[chatMessageAttachment](chatmessageattachment.md) 集合 |对附加对象（如文件、选项卡、会议等）的引用。|
|body|[itemBody](itembody.md)|聊天消息内容的纯文本/HTML 表示形式。 表示形式由正文中的 contentType 进行指定。 如果聊天消息包含 [chatMessageMention](chatmessagemention.md)，则内容始终为 HTML 格式。 |
|channelIdentity|[channelIdentity](channelidentity.md)|如果消息是在频道中发送的，则代表频道的标识。|
|chatId|string|如果消息是在聊天中 **发送的**，则表示聊天 **的标识**。|
|createdDateTime|dateTimeOffset|创建聊天消息的时间戳。|
|deletedDateTime|dateTimeOffset|只读。 删除聊天消息的时间戳;如果未删除，则返回 null。 |
|etag| string | 只读。 聊天消息的版本号。 |
|eventDetail|[eventMessageDetail](../resources/eventmessagedetail.md)|只读。  如果存在，表示聊天、频道或团队中发生的事件的详细信息，例如添加新成员。  对于事件消息 **，messageType** 属性将设置为 `systemEventMessage` 。|
|起始数量|[chatMessageFromIdentitySet](chatmessagefromidentityset.md)| 聊天消息的发送者的详细信息。 只能在迁移期间 [进行设置](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)。|
|id|String| 只读。 消息的唯一 ID。|
|importance|string | 聊天消息的重要性。 可能的值包括 `normal`、`high`、`urgent`。|
|lastEditedDateTime|dateTimeOffset|只读。 编辑聊天消息的时间戳。 在用户界面中触发"已编辑Teams标记。 如果未进行编辑，则值为 `null` 。|
|lastModifiedDateTime|dateTimeOffset|只读。 创建聊天消息的时间戳 (设置) 修改，包括添加或删除回应时。 |
|区域设置|string|客户端设置的聊天消息区域设置。 始终设置为 `en-us`。|
|提及|[chatMessageMention](chatmessagemention.md) 集合| 聊天消息中提到的实体列表。 支持的实体包括：user、bot、team、channel 和 tag。|
|messageType|chatMessageType|聊天消息的类型。 可能的值包括 `message`、`chatEvent`、`typing`、`unknownFutureValue`、`systemEventMessage`。 请注意，必须使用 `Prefer: include-unknown-enum-members` 请求标头获取此 [可进化枚举](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations) 中的以下值: `systemEventMessage`。|
|onBehalfOf|[chatMessageFromIdentitySet](chatmessagefromidentityset.md)| 机器人代表用户发送邮件时邮件[](/microsoftteams/platform/messaging-extensions/how-to/action-commands/respond-to-task-module-submit?tabs=dotnet%2Cdotnet-1#user-attribution-for-bots-messages)的用户属性。|
|policyViolation | [chatMessagePolicyViolation](chatmessagepolicyviolation.md) |定义 DLP 应用程序中数据丢失防护设置的策略违反 () 属性。|
|反应| [chatMessageReaction](chatmessagereaction.md) 集合 | 此聊天消息的反应 (例如，Like) 。|
|replyToId| string | 只读。 线程的父聊天消息或根聊天消息的 ID。  (仅适用于频道中的聊天消息，而仅适用于 chats)  |
|subject|string| 纯文本形式的聊天消息的主题。|
|摘要|string| 可用于推送通知和摘要视图或回退视图的聊天消息的摘要文本。 仅适用于频道聊天消息，不应用于聊天中的聊天消息。 |
|WebUrl|string|只读。 指向邮件中Microsoft Teams。|

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
  "onBehalfOf": {"@odata.type": "microsoft.graph.chatMessageFromIdentitySet"},
  "importance": "string",
  "reactions": [{"@odata.type": "microsoft.graph.chatMessageReaction"}],
  "locale": "string",
  "policyViolation": {"@odata.type": "microsoft.graph.chatMessagePolicyViolation"},
  "chatId": "string",
  "channelIdentity": {"@odata.type": "microsoft.graph.channelIdentity"},
  "webUrl": "string",
  "eventDetail": {
    "@odata.type": "microsoft.graph.eventMessageDetail"
  }
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
