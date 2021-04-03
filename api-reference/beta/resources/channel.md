---
title: 频道资源类型
description: '频道是的团队中的 chatMessages 集合。 '
author: laujan
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ad1c2da7d5c9656796e8f70bdc74d4444ffd1188
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582639"
---
# <a name="channel-resource-type"></a>频道资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Teams](../resources/team.md) 由频道组成，是你与团队成员的对话。 每个频道专用于特定主题、部门或项目。 频道是工作实际完成的地方 - 对整个团队开放的文本、音频和视频对话的位置、共享文件的位置以及添加标签的位置。

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
|[获取所有频道消息](../api/channel-getallmessages.md)|[channel](channel.md) 集合 | 获取用户参与的所有频道中的所有消息。 |
|[创建频道消息发布](../api/channel-post-messages.md) | [chatMessage](../resources/chatmessage.md) | 向频道发送消息。 |
|[创建回复频道消息发布](../api/chatmessage-post-replies.md) | [chatMessage](../resources/chatmessage.md) | 在频道中回复消息。|
|[获取文件文件夹](../api/channel-get-filesfolder.md)| [driveItem](driveitem.md) | 检索用于存储频道文件的 SharePoint 文件夹的详细信息。 |
|[列出选项卡](../api/channel-list-tabs.md) | [teamsTab](teamstab.md) | 列出固定到频道的选项卡。|
|[列出频道成员](../api/channel-list-members.md) | [conversationMember](conversationmember.md) 集合 | 获取频道中的成员列表。|
|[添加频道成员](../api/channel-post-members.md) | [conversationMember](conversationmember.md) | 向频道添加成员。 仅支持 membershipType 为 `private` 的 `channel`。|
|[获取频道成员](../api/channel-get-members.md) | [conversationMember](conversationmember.md) 集合 | 获取频道中的成员。|
|[更新频道成员角色](../api/channel-update-members.md) | [conversationMember](conversationmember.md) | 更新频道成员的属性。 仅支持 membershipType 为 `private` 的频道。|
|[删除频道成员](../api/channel-delete-members.md) | 无 | 从频道中删除一个成员。 仅支持用于 `private` 的 `channelType`。|
|[完成迁移](../api/channel-completemigration.md)|[频道](channel.md)| 删除频道中的迁移模式，让用户可在频道中发布和阅读消息。|
|[列出频道中的选项卡](../api/channel-list-tabs.md) | [teamsTab](teamstab.md) | 列出固定到频道的选项卡。|
|[将选项卡添加到频道](../api/channel-post-tabs.md) | [teamsTab](teamstab.md) | 将选项卡添加（固定）到频道。|
|[获取频道中的选项卡](../api/channel-get-tabs.md) | [teamsTab](teamstab.md) | 获取固定到频道的特定选项卡。|
|[更新频道中的选项卡](../api/channel-patch-tabs.md) | [teamsTab](teamstab.md) | 更新频道中的选项卡的属性。|
|[从频道中删除选项卡](../api/channel-delete-tabs.md) | 无 | 从频道中删除（取消固定）选项卡。|


## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|说明|String|频道的可选文本描述。|
|displayName|String|在 Microsoft Teams 中呈现在用户面前的频道名称。|
|id|String|频道的唯一标识符。 只读。|
|isFavoriteByDefault|Boolean|指示是否应对团队的所有成员将频道自动标记到“收藏夹”。 仅可使用“[创建团队](../api/team-post.md)”以编程方式设置。 默认值：`false`。|
|email|String| 用于向频道发送邮件的电子邮件地址。 只读。|
|webUrl|String|将转到 Microsoft Teams 中的频道的超链接。 在 Microsoft Teams 中右键单击某个频道并选择“获取频道链接”即可获得此 URL。 应将此 URL 视为不透明的 blob，而不对其进行解析。 只读。|
|membershipType|[channelMembershipType](../resources/enums.md#channelmembershiptype-values)|频道的类型。 可在创建期间设置，但不可更改。 默认：标准。|
|createdDateTime|dateTimeOffset|只读。 创建频道的时间戳。|
|moderationSettings|[channelModerationSettings](../resources/channelmoderationsettings.md)|配置频道审核，以控制谁能在此频道中发起新帖子并回复帖子的设置。|

### <a name="instance-attributes"></a>实例属性

实例属性是具有特殊行为的属性。这些属性是临时的，并且 a) 定义服务应执行的行为或 b) 提供短期的属性值，例如过期项目的下载 URL。

| 属性名称| 类型   | 说明
|:-----------------------|:-------|:-------------------------|
|@microsoft. graph channelCreationMode|string|指示频道处于迁移状态，并且当前正用于迁移目的。 它接受一个值：`migration`。|

> **注意**：`channelCreationMode` 是采用值 `migration`的枚举。

有关 POST 请求示例，请参阅[请求（在迁移状态下创建频道）](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams#request-create-a-team-in-migration-state)。

## <a name="relationships"></a>关系

| 关系 | 类型 |说明|
|:---------------|:--------|:----------|
|messages|[chatMessage](chatmessage.md) 集合|频道中的所有消息集合。 一种导航属性。 可为 NULL。|
|选项卡|[teamsTab](../resources/teamstab.md) 集合|频道中的所有选项卡集合。 一种导航属性。|
|成员|[conversationMember](conversationmember.md) 集合|与频道关联的成员资格记录的集合。|
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
  "membershipType": "channelMembershipType",
  "createdDateTime": "string (timestamp)",
  "moderationSettings": "channelModerationSettings"
    
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
