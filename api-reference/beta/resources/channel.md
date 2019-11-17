---
title: 频道资源类型
description: '频道是的团队中的 chatMessages 集合。 '
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cdcb7f10d068372c167f65a7868672a7cb669107
ms.sourcegitcommit: cca4f96414aededa03bb45e07e19bb20b7327563
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2019
ms.locfileid: "36677125"
---
# <a name="channel-resource-type"></a>频道资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Teams](../resources/team.md) 由频道组成，是你与团队成员的对话。 每个频道专用于特定主题、部门或项目。 频道是工作实际完成的地方 - 对整个团队开放的文本、音频和视频对话的位置、共享文件的位置以及添加标签的位置。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出频道](../api/channel-list.md) | [频道](channel.md)集合 | 获取此团队中的频道列表。|
|[创建频道](../api/channel-post.md) | [频道](channel.md) | 通过包含显示名称和描述来新建频道。|
|[获取频道](../api/channel-get.md) | [频道](channel.md) | 读取频道的属性和关系。|
|[更新频道](../api/channel-patch.md) | [频道](channel.md) | 更新频道属性。|
|[删除频道](../api/channel-delete.md) | 无 | 删除频道。|
|[获取消息 Delta](../api/chatmessage-delta.md)  | [chatMessage](../resources/chatmessage.md) | 获取频道中的增量消息。 |
|[列出频道消息](../api/channel-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | 获取频道中的消息 |
|[列出频道成员](../api/conversationmember-list.md)| [conversationMember](conversationmember.md) 集合| 列出频道的成员。 |
|[获取频道成员](../api/conversationmember-get.md)| [conversationMember](conversationmember.md)| 获取频道的成员。 |
|[添加频道成员](../api/conversationmember-add.md) | [conversationMember](conversationmember.md)| 向频道添加成员。 仅支持用于 `private` 的 `channelType`。|
|[更新频道成员](../api/conversationmember-update.md) | [conversationMember](conversationmember.md)| 更新聊天成员。 仅支持用于 `private` 的 `channelType`。|
|[删除频道成员](../api/conversationmember-delete.md) | [conversationMember](conversationmember.md)| 删除频道的成员。 仅支持用于 `private` 的 `channelType`。|
|[在频道中创建 chatMessage](../api/channel-post-messages.md) | [chatMessage](../resources/chatmessage.md) | 向频道发送消息。 |
|[在频道中创建 chatMessage 回复](../api/channel-post-messagereply.md) | [chatMessage](../resources/chatmessage.md) | 在频道中回复消息。|
|[列出选项卡](../api/teamstab-list.md) | [teamsTab](teamstab.md) | 列出固定到频道的选项卡。|
|[获取选项卡](../api/teamstab-get.md) | [teamsTab](teamstab.md) | 读取固定到频道的选项卡。|
|[添加选项卡](../api/teamstab-add.md) | [teamsTab](teamstab.md) | 将选项卡添加（固定）到频道。|
|[删除选项卡](../api/teamstab-delete.md) | 无 | 将选项卡添加（固定）到频道。|
|[更新选项卡](../api/teamstab-update.md) | [teamsTab](teamstab.md) | 更新选项卡属性。|

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|说明|String|频道的可选文本描述。|
|displayName|String|在 Microsoft Teams 中呈现在用户面前的频道名称。|
|id|String|频道的唯一标识符。 只读。|
|isFavoriteByDefault|Boolean|指示是否应对团队的所有成员将频道自动标记到“收藏夹”。 默认值：`false`。|
|email|String| 用于向频道发送邮件的电子邮件地址。 只读。|
|webUrl|String|将转到 Microsoft Teams 中的频道的超链接。 在 Microsoft Teams 中右键单击某个频道并选择“获取频道链接”即可获得此 URL。 应将此 URL 视为不透明的 blob，而不对其进行解析。 只读。|
|membershipType|[channelMembershipType](../resources/enums.md#channelmembershiptype-values)|频道的类型。 可在创建期间设置，但不可更改。 默认：标准。|

## <a name="relationships"></a>关系

| 关系 | 类型 |说明|
|:---------------|:--------|:----------|
|messages|[chatMessage](chatmessage.md) 集合|频道中的所有消息集合。 一种导航属性。 可为空。 此 API 目前仅支持读取消息，但最终也会支持写入消息。|
|选项卡|[teamsTab](../resources/teamstab.md) 集合|频道中的所有选项卡集合。 一种导航属性。|
|成员|[conversationMember](conversationmember.md) 集合|与频道关联的成员资格记录的集合。|

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
  "membershipType": "channelMembershipType"
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
