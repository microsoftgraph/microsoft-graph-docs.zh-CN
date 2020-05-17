---
title: chatMessage 资源类型
description: 表示渠道或聊天实体内的单个聊天消息。 聊天消息可以是一个根聊天消息，也可以是由聊天消息中的**replyToId**属性定义的线程的一部分。
doc_type: resourcePageType
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 2030a208ed61b7137d22c29eee2743b67556c92d
ms.sourcegitcommit: 62c900af626e46439d949462f09061cc5c41d6ff
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/16/2020
ms.locfileid: "44272754"
---
# <a name="chatmessage-resource-type"></a>chatMessage 资源类型

命名空间：microsoft.graph

代表[频道](./channel.md)内或（在 beta 中）[聊天](/graph/api/resources/chat?view=graph-rest-beta)中的单个聊天邮件。 聊天消息可以是一个根聊天消息，也可以是由聊天消息中的**replyToId**属性定义的答复线程的一部分。

## <a name="methods"></a>Methods

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|**通道邮件**| | |
|[在频道中创建 chatMessage](../api/channel-post-messages.md) | [chatMessage](#chatmessage-resource-type)| 在频道中创建新的顶级聊天邮件。|
|**频道邮件答复**| | |
|[答复频道中的了 chatmessage](../api/channel-post-messagereply.md) | [chatMessage](#chatmessage-resource-type)| 在频道中答复现有聊天邮件。|

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|id|字符串| 只读。 邮件的唯一 Id。|
|replyToId| string | 只读。 线程的父聊天消息或根聊天消息的 Id。 （仅适用于通道中不聊天的聊天邮件） |
|from|[identitySet](identityset.md)| 只读。 聊天消息发件人的详细信息。|
|etag| string | 只读。 聊天消息的版本号。 |
|messageType|string|聊天消息的类型。 可能的值是： `message` 。|
|createdDateTime|dateTimeOffset|只读。 在聊天消息创建时的时间戳。|
|lastModifiedDateTime|dateTimeOffset|只读。 在创建或编辑聊天消息时的时间戳，包括答复的时间（如果是频道中的根聊天邮件）或添加或删除了反应。 |
|deletedDateTime|dateTimeOffset|只读。 删除聊天邮件的时间戳，如果未删除，则为 null。 |
|subject|string| 聊天消息的主题，以纯文本形式。|
|body|[itemBody](itembody.md)|聊天消息内容的纯文本/HTML 表示形式。 表示形式由正文中的 contentType 进行指定。 如果聊天消息包含[chatMessageMention](chatmessagemention.md)，则该内容始终为 HTML。 |
|摘要|string| 可用于推送通知和摘要视图或回退视图的聊天消息的摘要文本。 仅适用于频道聊天消息，而不是聊天中的聊天消息。 |
|附件|[chatMessageAttachment](chatmessageattachment.md) 集合 |附加文件。 附件目前是只读的 – 不支持发送附件。 |
|提及|[chatMessageMention](chatmessagemention.md) 集合| 聊天消息中提及的实体列表。 当前支持用户、机器人、团队、渠道。|
|重要性| string | 聊天消息的重要性。 可能的值包括 `normal`、`high`、`urgent`。|
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
  "locale": "string",
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
