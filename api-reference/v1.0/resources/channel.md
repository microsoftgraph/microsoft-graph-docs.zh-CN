---
title: 频道资源类型
description: '频道是的团队中的 chatMessages 集合。 '
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f9860f6d1385374258eeed11dd8db4db21ba895c
ms.sourcegitcommit: 39e48ed2d95b142ccf3f40ecc52441458f2745bf
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/06/2020
ms.locfileid: "48364397"
---
# <a name="channel-resource-type"></a>频道资源类型

命名空间：microsoft.graph

[Teams](../resources/team.md) 由频道组成，是你与团队成员的对话。 每个频道专用于特定主题、部门或项目。 频道是工作实际完成的地方 - 对整个团队开放的文本、音频和视频对话的位置、共享文件的位置以及添加标签的位置。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出频道](../api/channel-list.md) | [频道](channel.md)集合 | 获取此团队中的频道列表。|
|[创建频道](../api/channel-post.md) | [频道](channel.md) | 通过包含显示名称和描述来新建频道。|
|[获取频道](../api/channel-get.md) | [频道](channel.md) | 读取频道的属性和关系。|
|[更新频道](../api/channel-patch.md) | [频道](channel.md) | 更新频道属性。|
|[删除频道](../api/channel-delete.md) | 无 | 删除通道。|
|[列出选项卡](../api/teamstab-list.md) | [teamsTab](teamstab.md) | 列出固定到频道的选项卡。|

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|说明|String|频道的可选文本描述。|
|displayName|String|在 Microsoft Teams 中呈现在用户面前的频道名称。|
|id|String|频道的唯一标识符。 只读。|
|isFavoriteByDefault|Boolean|指示是否应对团队的所有成员将频道自动标记到“收藏夹”。 仅可使用“[创建团队](../api/team-post.md)”以编程方式设置。 默认值：`false`。|
|email|String| 用于向频道发送邮件的电子邮件地址。 只读。|
|webUrl|String|将转到 Microsoft Teams 中的频道的超链接。 在 Microsoft Teams 中右键单击某个频道并选择“获取频道链接”即可获得此 URL。 应将此 URL 视为不透明的 blob，而不对其进行解析。 只读。|
|createdDateTime|dateTimeOffset|只读。 创建频道的时间戳。|

## <a name="relationships"></a>关系

| 关系 | 类型 |说明|
|:---------------|:--------|:----------|
|messages|[chatMessage](chatmessage.md) 集合|频道中的所有消息集合。 一种导航属性。 可为 NULL。|
|选项卡|[teamsTab](../resources/teamstab.md) 集合|频道中的所有选项卡集合。 一种导航属性。|
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
