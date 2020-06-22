---
title: 频道资源类型
description: '频道是的团队中的消息集合。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8b6a0baaa684808c4d05bdcebf4be6d761d41d1b
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793582"
---
# <a name="channel-resource-type"></a>频道资源类型

命名空间：microsoft.graph

[Teams](../resources/team.md) 由频道组成，是你与团队成员的对话。 每个频道专用于特定主题、部门或项目。
频道是工作实际完成的地方 - 对整个团队开放的文本、音频和视频对话的位置、共享文件的位置以及添加标签的位置。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出频道](../api/channel-list.md) | [频道](channel.md)集合 | 获取此团队中的频道列表。|
|[创建频道](../api/channel-post.md) | [频道](channel.md) | 通过包含显示名称和描述来新建频道。|
|[获取频道](../api/channel-get.md) | [频道](channel.md) | 读取频道的属性和关系。|
|[更新频道](../api/channel-patch.md) | [频道](channel.md) | 更新频道属性。|
|[删除频道](../api/channel-delete.md) | 无 | 删除通道。|
|[列出选项卡](../api/teamstab-list.md) | [teamsTab](teamstab.md) | 列出固定到频道的选项卡。|
|[获取选项卡](../api/teamstab-get.md) | [teamsTab](teamstab.md) | 读取固定到频道的选项卡。|
|[添加选项卡](../api/teamstab-add.md) | [teamsTab](teamstab.md) | 将选项卡添加（固定）到频道。|
|[删除选项卡](../api/teamstab-delete.md) | 无 | 将选项卡添加（固定）到频道。|
|[更新选项卡](../api/teamstab-update.md) | [teamsTab](teamstab.md) | 更新选项卡属性。|

## <a name="properties"></a>属性

| 属性   | 类型 | 说明|
|:---------------|:--------|:----------|
|说明|String|频道的可选文本描述。|
|displayName|String|在 Microsoft Teams 中呈现在用户面前的频道名称。|
|email|String| 用于向频道发送邮件的电子邮件地址。 只读。|
|id|String|频道的唯一标识符。 只读。|
|webUrl|String|导航至 Microsoft Teams 中的频道的超链接。 在 Microsoft Teams 中右键单击某个频道并选择“获取频道链接”即可获得此 URL。 应将此 URL 视为不透明的 blob，而不对其进行解析。 只读。|

## <a name="relationships"></a>关系

| 关系 | 类型 | 说明|
|:---------------|:--------|:----------|
|messages|[chatMessage](./chatmessage.md) 集合|频道中的所有消息集合。 一种导航属性。 可为 NULL。|
|选项卡|[teamsTab](../resources/teamstab.md) 集合|频道中的所有选项卡集合。 一种导航属性。|
|[filesFolder](../api/channel-get-filesfolder.md)|[driveItem](driveitem.md)|用于存储频道文件的位置的元数据。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "email": "string (identifier)",
  "id": "string",
  "webUrl": "string"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
