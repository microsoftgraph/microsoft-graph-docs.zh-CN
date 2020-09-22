---
title: teamsTab 资源类型
description: 'TeamsTab 是一个固定在团队中的频道 (附加) 的选项卡。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5684c98f15ed039fbba36b1df517a6d7d1d5d8c9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046445"
---
# <a name="teamstab-resource-type"></a>teamsTab 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

TeamsTab 是一个固定在[团队](team.md)中的[频道](channel.md) (附加) 的[选项卡](../resources/teamstab.md)。 

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出选项卡](../api/teamstab-list.md) | [teamsTab](teamstab.md) | 列出固定到频道的选项卡。|
|[获取选项卡](../api/teamstab-get.md) | [teamsTab](teamstab.md) | 读取固定到频道的选项卡。|
|[添加选项卡](../api/teamstab-add.md) | [teamsTab](teamstab.md) | 将选项卡添加（固定）到频道。|
|[删除选项卡](../api/teamstab-delete.md) | 无 | 将选项卡添加（固定）到频道。|
|[更新选项卡](../api/teamstab-update.md) | [teamsTab](teamstab.md) | 更新选项卡属性。|


## <a name="properties"></a>属性

|属性|类型|说明|
|:---------------|:--------|:----------|
|  id              |   string                  |  唯一标识 "通道" 选项卡的特定实例的标识符。只读。     |
|  displayName            |   string                  |  选项卡的名称。     |
|  name            |   string                  |   (已弃用) 选项卡名称。     |
|  teamsAppId           |   string             |  选项卡的应用程序定义标识符。创建选项卡后，不能更改此值。     |
|  sortOrderIndex  |   string                  |  用于对选项卡进行排序的顺序的索引。     |
|  WebUrl          |   string                  |  选项卡实例的深层链接 URL。 只读。     |
|  configuration        |   [teamsTabConfiguration](teamstabconfiguration.md) |  应用于选项卡的自定义设置的容器。仅在设置此属性后，才会认为选项卡已配置。     |

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


