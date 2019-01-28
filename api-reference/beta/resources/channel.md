---
title: 频道资源类型
description: '频道是的团队中的 chatMessages 集合。 '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 73775cb446e9cd90eaf31ade28f25638465c884e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511000"
---
# <a name="channel-resource-type"></a>频道资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

频道是的[团队](../resources/team.md)中的 [chatMessages](chatmessage.md) 集合。 频道表示团队内部的某个主题，因此是讨论的逻辑隔离。 示例可以是“星期五团队午餐”和“体系结构讨论”频道。


## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出频道](../api/channel-list.md) | [频道](channel.md)集合 | 获取此团队中的频道列表。|
|[创建频道](../api/channel-post.md) | [频道](channel.md) | 通过包含显示名称和描述来新建频道。|
|[获取频道](../api/channel-get.md) | [频道](channel.md) | 读取频道的属性和关系。|
|[更新频道](../api/channel-patch.md) | [频道](channel.md) | 更新频道属性。|
|[删除频道](../api/channel-delete.md) | 无 | 删除通道。|
|[列出频道消息](../api/channel-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | 获取频道中的消息 |
|[创建聊天线程](../api/channel-post-chatthreads.md) | [chatThread](chatthread.md) 集合| 在指定频道中创建聊天线程。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|说明|String|频道的可选文本描述。|
|displayName|String|在 Microsoft Teams 中呈现在用户面前的频道名称。|
|id|String|频道的唯一标识符。 只读。|
|isFavoriteByDefault|Boolean|频道是否对团队所有成员标记为“收藏夹”。 默认值：`false`。|
|电子邮件|Boolean| 用于向频道发送邮件的电子邮件地址。 只读。|
|webUrl|String|导航至 Microsoft Teams 中的频道的超链接。 在 Microsoft Teams 中右键单击某个频道并选择“获取频道链接”即可获得此 URL。 应将此 URL 视为不透明的 blob，而不对其进行解析。 只读。|


## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|messages|[chatMessage](chatmessage.md) 集合|频道中的所有消息集合。 一种导航属性。 可为空。 此 API 目前仅支持读取消息，但最终也会支持写入消息。|
|chatThreads|[chatThread](chatthread.md) 集合|（这将会分阶段推出，以支持消息属性）chatThreads 支持新建消息，但不支持读取消息。 ChatThreads 是一种导航属性，可为空。|
|选项卡|[teamsTab](../resources/teamstab.md) 集合|频道中的所有选项卡集合。 一种导航属性。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "chatthreads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
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
  "suppressions": [
    "Error: /api-reference/beta/resources/channel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
