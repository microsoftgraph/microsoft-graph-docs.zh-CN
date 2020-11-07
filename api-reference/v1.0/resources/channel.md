---
title: 频道资源类型
description: '频道是的团队中的 chatMessages 集合。 '
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 59a6b111c08b6bfb408b1f28b4db343843ed12ad
ms.sourcegitcommit: 22d99624036ceaeb1b612538d5196faaa743881f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2020
ms.locfileid: "48932582"
---
# <a name="channel-resource-type"></a>频道资源类型

命名空间：microsoft.graph

[Teams](../resources/team.md) are made up of channels, which are the conversations you have with your teammates. Each channel is dedicated to a specific topic, department, or project. Channels are where the work actually gets done - where text, audio, and video conversations open to the whole team happen, where files are shared, and where tabs are added.

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出频道](../api/channel-list.md) | [频道](channel.md)集合 | 获取此团队中的频道列表。|
|[创建频道](../api/channel-post.md) | [频道](channel.md) | 通过包含显示名称和描述来新建频道。|
|[获取频道](../api/channel-get.md) | [频道](channel.md) | 读取频道的属性和关系。|
|[更新频道](../api/channel-patch.md) | [频道](channel.md) | 更新频道属性。|
|[删除频道](../api/channel-delete.md) | 无 | 删除通道。|
|[获取消息 Delta](../api/chatmessage-delta.md)  | [chatMessage](../resources/chatmessage.md) | 获取频道中的增量消息。 |
|[列出频道消息](../api/channel-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | 获取频道中的消息 |
|[列出频道成员](../api/conversationmember-list.md)| [conversationMember](conversationmember.md) 集合| 列出频道的成员。 |
|[获取频道成员](../api/conversationmember-get.md)| [conversationMember](conversationmember.md)| 获取频道的成员。 |
|[添加频道成员](../api/conversationmember-add.md) | [conversationMember](conversationmember.md)| Add a member to a channel. Only supported for `channelType` of `private`.|
|[更新频道成员](../api/conversationmember-update.md) | [conversationMember](conversationmember.md)| Update a member of a channel. Only supported for `channelType` of `private`.|
|[删除频道成员](../api/conversationmember-delete.md) | [conversationMember](conversationmember.md)| Delete a member of a channel. Only supported for `channelType` of `private`.|
|[在频道中创建 chatMessage](../api/channel-post-message.md) | [chatMessage](../resources/chatmessage.md) | 向频道发送消息。 |
|[在频道中创建 chatMessage 回复](../api/channel-post-messagereply.md) | [chatMessage](../resources/chatmessage.md) | 在频道中回复消息。|
|[获取文件文件夹](../api/driveitem-get.md)| [driveItem](driveitem.md) | 检索用于存储频道文件的 SharePoint 文件夹的详细信息。 |
|[列出选项卡](../api/teamstab-list.md) | [teamsTab](teamstab.md) | 列出固定到频道的选项卡。|

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|说明|String|频道的可选文本描述。|
|displayName|String|在 Microsoft Teams 中呈现在用户面前的频道名称。|
|id|String|The channel's unique identifier. Read-only.|
|isFavoriteByDefault|Boolean|Indicates whether the channel should automatically be marked 'favorite' for all members of the team. Can only be set programmatically with [Create team](../api/team-post.md). Default: `false`.|
|email|String| The email address for sending messages to the channel. Read-only.|
|webUrl|String|A hyperlink that will go to the channel in Microsoft Teams. This is the URL that you get when you right-click a channel in Microsoft Teams and select Get link to channel. This URL should be treated as an opaque blob, and not parsed. Read-only.|
|createdDateTime|dateTimeOffset|Read only. Timestamp at which the channel was created.|

## <a name="relationships"></a>关系

| 关系 | 类型 |说明|
|:---------------|:--------|:----------|
|messages|[chatMessage](chatmessage.md) 集合|A collection of all the messages in the channel. A navigation property. Nullable.|
|选项卡|[teamsTab](../resources/teamstab.md) 集合|A collection of all the tabs in the channel. A navigation property.|
|[filesFolder](../api/channel-get-filesfolder.md)|[driveItem](driveitem.md)|用于存储频道文件的位置的元数据。|
|operations|[teamsAsyncOperation](teamsasyncoperation.md) 集合| 在此团队中运行过或正在运行的异步操作。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messages"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "isFavoriteByDefault": true,
  "email": "string",
  "webUrl": "string",
  "createdDateTime": "string (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
