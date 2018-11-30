---
title: chatMessage 资源类型
description: 代表单个聊天消息中的通道或聊天实体。 消息能为根邮件或由**replyToId**属性在消息中定义的线程的一部分。
ms.openlocfilehash: 1fba27567d5a1c80a36a5758925ec427735504cf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041602"
---
# <a name="chatmessage-resource-type"></a>chatMessage 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

代表单个聊天消息中的[通道](channel.md)或聊天实体。 消息能为根邮件或由**replyToId**属性在消息中定义的线程的一部分。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列表通道消息](../api/channel-list-messages.md) | [chatmessage](chatmessage.md)集合 | 在通道中获取的所有根邮件的列表。|
|[Get 频道消息](../api/channel-get-message.md) | [chatmessage](chatmessage.md) | 从通道中获取单个根消息。|
|[列表回复到一条消息](../api/channel-list-messagereplies.md) | [chatmessage](chatmessage.md)集合| 在通道中获取所有回复到一条消息的列表。|
|[获取邮件答复](../api/channel-get-messagereply.md) | [chatmessage](chatmessage.md)| 在通道中获取单个邮件答复。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 只读。 邮件的唯一 ID。|
|replyToId| string | 父消息/根邮件的主题的 id |
|发件人|[identitySet](identityset.md)| 发件人的邮件的详细信息|
|etag| string | 邮件的版本号 |
|messageType|字符串|支持的邮件，当前的类型的值为： 消息，chatEvent，键入|
|createdDateTime|dateTimeOffset|只读。 创建邮件时的时间戳|
|lastModifiedDateTime|dateTimeOffset|只读。 时间戳的邮件时编辑更新|
|被|boolean|如果已软删除一条消息，表示|
|deletedDateTime|dateTimeOffset|只读。 邮件已被删除的时间戳 |
|subject|string|邮件主题行。 可选|
|body|[itemBody](itembody.md)|纯文本/HTML 表示形式的消息内容。 返回纯文本默认情况下应用程序可以查询参数的一部分选择 HTML|
|摘要|string|摘要无法用于推送通知和摘要视图或秋季后视图的消息文本|
|提及|[chatMessageMention](chatmention.md)集合| 消息中提到的实体的列表。 当前支持用户、 自动程序、 团队和通道|
|importance| string | 邮件的重要性： 普通、 高|
|反应的方式| [chatMessageReaction](chatreaction.md)集合 | 此消息的反应的方式 （例如，如）|
|区域设置|string|设置由客户端消息的区域设置|
|attachments|[chatMessageAttachment](chatattachment.md)集合 |附加的文件|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "isDeleted",
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
<!-- {
  "type": "#page.annotation",
  "description": "chat message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
