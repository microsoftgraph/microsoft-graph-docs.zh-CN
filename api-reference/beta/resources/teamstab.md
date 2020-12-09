---
title: teamsTab 资源类型
description: 'TeamsTab 是一个固定在团队中的频道 (附加) 的选项卡。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fa675992401c8953b5611739ba69cb0d5688f833
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49606949"
---
# <a name="teamstab-resource-type"></a>teamsTab 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

TeamsTab 是一个固定在[团队](team.md)中的[频道](channel.md) (附加) 的[选项卡](../resources/teamstab.md)。 

## <a name="methods"></a>方法

| 方法       | 返回类型  |Description|
|:---------------|:--------|:----------|
|[通道中的列表选项卡](../api/channel-list-tabs.md) | [teamsTab](teamstab.md) | 固定到频道的列表选项卡。|
|[通道中的获取选项卡](../api/channel-get-tabs.md) | [teamsTab](teamstab.md) | 获取固定到频道的特定选项卡。|
|[将选项卡添加到频道](../api/channel-post-tabs.md) | [teamsTab](teamstab.md) | 将选项卡 (插) 到频道。|
|[通道中的 "更新" 选项卡](../api/channel-patch-tabs.md) | [teamsTab](teamstab.md) | 更新通道中的选项卡的属性。|
|[从频道中删除选项卡](../api/channel-delete-tabs.md) | 无 | 从频道) 选项卡中删除 ("取消固定"。|
|[聊天中的列表选项卡](../api/chat-list-tabs.md) | [teamsTab](teamstab.md) | 固定到聊天的列表选项卡。|
|[聊天中的 "获取" 选项卡](../api/chat-get-tabs.md) | [teamsTab](teamstab.md) | 获取固定到聊天的特定选项卡。|
|[将选项卡添加到聊天](../api/chat-post-tabs.md) | [teamsTab](teamstab.md) | 向聊天添加 (pin) 选项卡。|
|[聊天中的更新选项卡](../api/chat-patch-tabs.md) | [teamsTab](teamstab.md) | 更新聊天中的选项卡的属性。|
|[从聊天中删除选项卡](../api/chat-delete-tabs.md) | 无 | ) 聊天中的选项卡删除 (的 "取消固定"。|



## <a name="properties"></a>属性

|属性|类型|说明|
|:---------------|:--------|:----------|
|  id              |   string                  |  唯一标识 "通道" 选项卡的特定实例的标识符。只读。     |
|  displayName            |   string                  |  选项卡的名称。     |
|  名称 (弃用)       |   string                  |  选项卡的名称。     |
|  teamsAppId (弃用) |   string             |  选项卡的应用程序定义标识符。创建选项卡后，不能更改此值。 由于此属性已弃用，因此我们建议扩展 **teamsApp** 以检索链接到该选项卡的应用程序。 |
|  sortOrderIndex  |   string                  |  用于对选项卡进行排序的顺序的索引。     |
|  webUrl          |   string                  |  选项卡实例的深层链接 URL。 只读。     |
|  configuration        |   [teamsTabConfiguration](teamstabconfiguration.md) |  应用于选项卡的自定义设置的容器。仅在设置此属性后，才会认为选项卡已配置。     |

## <a name="relationships"></a>关系

| 关系 | 类型   | Description |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md) | 链接到该选项卡的应用程序。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。


<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.teamsTab"
}-->

```json
{
  "id": "string",
  "displayName": "string",
  "teamsAppId": "string",
  "sortOrderIndex": "string",
  "webUrl": "string",
  "configuration": "teamsTabConfiguration",
  "name": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsTab resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

## <a name="see-also"></a>另请参阅

[配置内置选项卡类型](/graph/teams-configuring-builtin-tabs)


