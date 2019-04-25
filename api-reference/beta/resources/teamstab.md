---
title: teamsTab 资源类型
description: 'teamsTab 是固定 (附加) 到团队中的频道的选项卡。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 207b9d1d4d27199f07ae22bd47587411f917afae
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553643"
---
# <a name="teamstab-resource-type"></a>teamsTab 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

teamsTab 是固定 (附加) 到[团队](team.md)中的[频道](channel.md)的[选项卡](../resources/teamstab.md)。 

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出选项卡](../api/teamstab-list.md) | [teamsTab](teamstab.md) | 列出固定到频道的选项卡。|
|[获取选项卡](../api/teamstab-get.md) | [teamsTab](teamstab.md) | 读取固定到通道的选项卡。|
|[添加选项卡](../api/teamstab-add.md) | [teamsTab](teamstab.md) | 将选项卡添加 (插针) 到频道。|
|[删除选项卡](../api/teamstab-delete.md) | 无 | 从频道中删除 (unpins) 选项卡。|
|[更新选项卡](../api/teamstab-update.md) | [teamsTab](teamstab.md) | 更新选项卡属性。|


## <a name="properties"></a>属性

|属性|类型|说明|
|:---------------|:--------|:----------|
|  id              |   字符串                  |  唯一标识 "通道" 选项卡的特定实例的标识符。只读。     |
|  displayName            |   string                  |  选项卡的名称。     |
|  name            |   string                  |  被选项卡的名称。     |
|  teamsAppId           |   string             |  选项卡的应用程序定义标识符。创建选项卡后, 不能更改此值。     |
|  sortOrderIndex  |   string                  |  用于对选项卡进行排序的顺序的索引。     |
|  WebUrl          |   string                  |  选项卡实例的深层链接 url。 只读。     |
|  设置        |   [teamsTabConfiguration](teamstabconfiguration.md) |  应用于选项卡的自定义设置的容器。仅在设置此属性后, 才会认为选项卡已配置。     |

## <a name="relationships"></a>关系

| 关系 | 类型   | 说明 |
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
  "configuration" : "teamsTabConfiguration"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/teamstab.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

## <a name="see-also"></a>另请参阅

[配置内置选项卡类型](/graph/teams-configuring-builtin-tabs)
