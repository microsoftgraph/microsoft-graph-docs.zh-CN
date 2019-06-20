---
title: chatMessage 资源类型
description: 表示渠道或聊天实体内的单个聊天消息。 该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: 269041dece2ab626c5f3d0ecccbf70d62c296ede
ms.sourcegitcommit: b523648530fcc8c2a3ded35b419be8047b9fcd10
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/20/2019
ms.locfileid: "35084045"
---
# <a name="chatmessage-resource-type"></a>chatMessage 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [渠道](channel.md)或[聊天](chat.md)中的单个聊天信息。
该消息可以是根消息，也可以是消息中的 **replyToId** 属性定义的线程部分。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出渠道消息](../api/channel-list-messages.md) | [chatMessage](chatmessage.md) 集合 | 渠道中的所有根消息列表。|
|[获取渠道消息](../api/channel-get-message.md) | [chatMessage](chatmessage.md) | 获取渠道中的单个根消息。|
|[列出消息回复](../api/channel-list-messagereplies.md) | [chatMessage](chatmessage.md) 集合| 渠道中的所有消息回复列表。|
|[获取消息回复](../api/channel-get-messagereply.md) | [chatMessage](chatmessage.md)| 获取渠道中的单个消息回复。|
|[在渠道中创建 chatMessage](../api/channel-post-messages.md) | [chatMessage](chatmessage.md)| 在渠道中创建新的顶级消息。|
|[在渠道中回复消息](../api/channel-post-messagereply.md) | [chatMessage](chatmessage.md)| 在渠道中回复现有消息。|
|[列出聊天中的消息](../api/chat-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | 一对一聊天或群组聊天中的消息。 |
|[获取聊天中的消息](../api/chat-get-message.md)  | [chatMessage](../resources/chatmessage.md) | 获取聊天中的单个消息。 |
|[列出所有托管图像](../api/chatmessagehostedimage-list-hostedimages.md) | [hostedImage](../resources/chatmessagehostedimage.md) 集合| 获取消息中的所有托管图像。|
|[获取托管图像](../api/chatmessagehostedimage-get.md) | [hostedImage](../resources/chatmessagehostedimage.md) | 获取消息中的托管图像。|
|[获取托管图像字节](../api/chatmessagehostedimage-getbytes.md) | 二进制图像数据 | 获取消息中托管图像的二进制图像数据。|

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|id|String| 只读。 消息的唯一 ID。|
|replyToId| string | 只读。 线程的父级消息/根消息的 Id。 （仅适用于频道中的消息，不适用于聊天） |
|from|[identitySet](identityset.md)| 只读。 消息发送者的详细信息。|
|etag| string | 只读。 消息的版本号。 |
|messageType|chatMessageType|邮件类型。 可取值包括：`message`。|
|createdDateTime|dateTimeOffset|只读。 创建消息时的时间戳。|
|lastModifiedDateTime|dateTimeOffset|只读。 编辑/更新消息时的时间戳。|
|deletedDateTime|dateTimeOffset|只读。 删除消息时的时间戳，如果未删除则为 null。 |
|subject|string| 消息的主题（纯文本）。|
|正文|[itemBody](itembody.md)|消息内容的纯文本/HTML 表示。 表示形式由正文中的 contentType 进行指定。 如果消息包含 [chatMessageMention](chatmessagemention.md)，则内容始终采用 HTML 格式。 |
|摘要|string| 可用于推送通知的消息摘要文本和摘要视图或回退视图。 仅适用于频道消息，不适用于聊天消息。 |
|附件|[chatMessageAttachment](chatmessageattachment.md) 集合 |附加文件。 附件目前是只读的 – 不支持发送附件。 |
|提及|[chatMessageMention](chatmessagemention.md) 集合| 消息中提到的实体列表。 当前支持用户、机器人、团队、渠道。|
|importance| chatMessageImportance | 邮件的重要性。 可能的值包括 `normal`、`high`、`urgent`。|
|反应| [chatMessageReaction](chatmessagereaction.md) 集合 | 此消息的反应（例如点赞）。|
|区域设置|string|客户端设置的消息区域设置。|

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
