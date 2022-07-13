---
title: chatMessage 资源类型
description: 表示频道或聊天实体中的单个聊天消息。 聊天消息可以是根聊天消息或由聊天消息中的 **replyToId** 属性定义的线程的一部分。
doc_type: resourcePageType
ms.localizationpriority: medium
author: RamjotSingh
ms.prod: microsoft-teams
ms.openlocfilehash: d02f67363c11f9e70419ebc8f4dee376e23dba06
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2022
ms.locfileid: "66768320"
---
# <a name="chatmessage-resource-type"></a>chatMessage 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [渠道](channel.md)或[聊天](chat.md)中的单个聊天信息。 该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。

> **注意**：此资源支持使用 [更改通知](../resources/webhooks.md)订阅更改 (创建、更新和删除) 。 这使呼叫方可以实时订阅和获取更改。 有关详细信息，请参阅[获取消息通知](/graph/teams-changenotifications-chatMessage)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|**频道消息**| | |
|[在通道中列出消息](../api/channel-list-messages.md) | [chatMessage](chatmessage.md) 集合 | 通道中所有根消息的列表。|
|[获取通道中消息的增量](../api/chatmessage-delta.md)  | [chatMessage](../resources/chatmessage.md) | 获取频道中的增量消息。 |
|[创建新频道消息的订阅](../api/subscription-post-subscriptions.md) | [订阅](subscription.md) | 侦听新的、编辑的和已删除的消息，以及对它们的反应。 |
|[在频道中获取消息](../api/chatmessage-get.md) | [chatMessage](chatmessage.md) | 获取通道中的单个根消息。|
|[在通道中发送消息](../api/chatmessage-post.md) | [chatMessage](chatmessage.md)| 在通道中创建新的根消息。|
|[在通道中更新消息](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| 更新聊天消息的 **policyViolation** 属性。|
|[删除通道中的消息](../api/chatmessage-softdelete.md)|[chatMessage](chatmessage.md)| 删除频道中的消息。|
|[撤消通道中邮件的删除](../api/chatmessage-undoSoftdelete.md)|[chatMessage](chatmessage.md)| 取消删除频道中的消息。|
|**频道消息回复**| | |
|[列出对邮件的答复](../api/chatmessage-list-replies.md) | [chatMessage](chatmessage.md) 集合| 频道中对聊天消息的所有答复的列表。|
|[在频道中获取回复消息](../api/chatmessage-get.md) | [chatMessage](chatmessage.md) | 在频道中获取一条回复消息。|
|[在频道中回复消息](../api/chatmessage-post-replies.md) | [chatMessage](chatmessage.md)| 回复频道中的现有聊天消息。|
|[更新回复消息](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| 更新聊天消息的 **policyViolation** 属性。|
|[删除频道中的回复消息](../api/chatmessage-softdelete.md)|[chatMessage](chatmessage.md)| 删除频道中的单个回复消息。|
|[撤消通道中回复消息的删除](../api/chatmessage-undoSoftdelete.md)|[chatMessage](chatmessage.md)| 取消删除频道中的单个回复消息。
|**聊天消息**| | |
|[列出聊天中的消息](../api/chat-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | 列出聊天中的聊天消息。 |
|[获取聊天中的消息](../api/chatmessage-get.md)  | [chatMessage](../resources/chatmessage.md) | 在聊天中获取一条聊天消息。 |
|[为用户在所有聊天中获取消息](../api/chats-getallmessages.md)| [聊天](chat.md) 集合| 从用户参与的所有聊天中获取消息，包括 1：1 聊天、群聊和会议聊天。 |
|[获取所有频道消息](../api/channel-getallmessages.md)|[channel](channel.md) 集合 | 获取用户参与的所有频道中的所有消息。 |
|[创建新聊天消息的订阅](../api/subscription-post-subscriptions.md) | [订阅](subscription.md) | 侦听新的、编辑的和已删除的聊天消息，以及对它们的反应。 |
|[在聊天中发送消息](../api/chat-post-messages.md) | [chatMessage](chatmessage.md)| 在现有 1：1 或群组聊天对话中发送聊天消息。|
|[在聊天中更新消息](../api/chatmessage-update.md)|[chatMessage](chatmessage.md)| 更新聊天消息的 **policyViolation** 属性。|
|[删除聊天中的消息](../api/chatmessage-softdelete.md)|[chatMessage](chatmessage.md)| 删除聊天消息。|
|[撤消聊天中邮件的删除](../api/chatmessage-undoSoftdelete.md)|[chatMessage](chatmessage.md)| 在聊天中取消删除消息。|
|**托管内容**| | |
|[列出所有托管内容](../api/chatmessage-list-hostedcontents.md) | [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) 集合| 获取与消息关联的所有托管内容。|
|[获取托管内容](../api/chatmessagehostedcontent-get.md) | [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) | 获取邮件的托管内容 (及其字节) 。|

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|attachments|[chatMessageAttachment](chatmessageattachment.md) 集合 |对文件、选项卡、会议等附加对象的引用。|
|body|[itemBody](itembody.md)|聊天消息内容的纯文本/HTML 表示形式。 表示形式由正文中的 contentType 进行指定。 如果聊天消息包含 [chatMessageMention](chatmessagemention.md)，则内容始终采用 HTML。 |
|channelIdentity|[channelIdentity](channelidentity.md)|如果消息是在通道中发送的，则表示通道的标识。|
|chatId|string|如果消息是在 **聊天** 中发送的，则表示 **聊天** 的标识。|
|createdDateTime|dateTimeOffset|创建聊天消息的时间戳。|
|deletedDateTime|dateTimeOffset|只读。 删除聊天消息的时间戳，如果未删除，则为 null。 |
|etag| string | 只读。 聊天消息的版本号。 |
|eventDetail|[eventMessageDetail](../resources/eventmessagedetail.md)|只读。  如果存在，则表示 **聊天**、 **频道** 或 **团队** 中发生的事件的详细信息，例如添加新成员。 对于事件消息， **messageType** 属性将设置为 `systemEventMessage`。|
|起始数量|[chatMessageFromIdentitySet](chatmessagefromidentityset.md)| 聊天消息的发件人详细信息。 只能在 [迁移](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)期间设置。|
|id|String| 只读。 消息的唯一 ID。|
|importance|string | 聊天消息的重要性。 可能的值包括 `normal`、`high`、`urgent`。|
|lastEditedDateTime|dateTimeOffset|只读。 对聊天消息进行编辑时的时间戳。 在 Teams UI 中触发“编辑”标志。 如果未进行任何编辑，则值为 `null`。|
|lastModifiedDateTime|dateTimeOffset|只读。 创建聊天消息时的时间戳 (初始设置) 或修改，包括添加或删除反应的时间。 |
|区域设置|string|客户端设置的聊天消息的区域设置。 始终设置为 `en-us`。|
|提及|[chatMessageMention](chatmessagemention.md) 集合| 聊天消息中提到的实体列表。 支持的实体包括：用户、机器人、团队、频道和标记。|
|messageType|chatMessageType|聊天消息的类型。 可能的值包括 `message`、`chatEvent`、`typing`、`unknownFutureValue`、`systemEventMessage`。 请注意，必须使用 `Prefer: include-unknown-enum-members` 请求标头获取此 [可进化枚举](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations) 中的以下值: `systemEventMessage`。|
|onBehalfOf|[chatMessageFromIdentitySet](chatmessagefromidentityset.md)| [机器人](/microsoftteams/platform/messaging-extensions/how-to/action-commands/respond-to-task-module-submit?tabs=dotnet%2Cdotnet-1#user-attribution-for-bots-messages)代表用户发送消息时消息的用户归属。|
|policyViolation | [chatMessagePolicyViolation](chatmessagepolicyviolation.md) |定义由数据丢失防护设置的策略冲突的属性 (DLP) 应用程序。|
|反应| [chatMessageReaction](chatmessagereaction.md) 集合 | 此聊天消息的反应 (如) 。|
|replyToId| string | 只读。 线程的父聊天消息或根聊天消息的 ID。  (仅适用于频道中的聊天消息，而不适用于聊天。)  |
|subject|string| 聊天消息的主题，用纯文本表示。|
|摘要|string| 可用于推送通知和摘要视图或回退视图的聊天消息的摘要文本。 仅适用于频道聊天消息，而不适用于聊天中的聊天消息。 |
|webUrl|string|只读。 链接到 Microsoft Teams 中的消息。|

## <a name="relationships"></a>关系

| 关系   | 类型    | 说明 |
|:---------------|:--------|:----------|
|答复|[chatMessage](chatmessage.md)| 针对指定消息的答复。 支持 `$expand` 通道消息。 |
|hostedContents|[chatMessageHostedContent](chatmessagehostedcontent.md)| Microsoft Teams 托管的消息中的内容 -例如，图像或代码片段。 |

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
