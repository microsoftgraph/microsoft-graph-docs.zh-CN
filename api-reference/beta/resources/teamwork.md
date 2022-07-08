---
title: teamwork 资源类型
description: 可供组织使用的 Microsoft Teams 功能范围的容器。
author: charlieforce
ms.localizationpriority: medium
ms.prod: teamwork
doc_type: resourcePageType
ms.openlocfilehash: 3c5282ff44f2ae56d40e666548e222ccfb6e13f4
ms.sourcegitcommit: c168f2cb95b4863080a84cc199a7b878fb5eeb8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2022
ms.locfileid: "66690010"
---
# <a name="teamwork-resource-type"></a>teamwork 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

可供组织使用的 Microsoft Teams 功能范围的容器。 

继承自 [entity](../resources/entity.md)。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deletedTeams](../api/teamwork-list-deletedteams.md)|[deletedTeam](../resources/deletedteam.md) 集合|获取 [deletedTeam](../resources/deletedteam.md) 对象及其属性的列表。|
|[列出 teamTemplates](../api/teamwork-list-teamtemplates.md)|[teamTemplate](../resources/teamtemplate.md) 集合|获取可用于租户的 [teamTemplate](../resources/teamtemplate.md) 对象的列表。 |

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String| 唯一标识符。 继承自 [entity](../resources/entity.md)。|

## <a name="relationships"></a>关系
| 关系 | 类型 | 说明 |
|:---------------|:--------|:----------|
|deletedTeams|[deletedTeam](../resources/deletedteam.md) 集合| 已删除团队的集合。|
|设备|[teamworkDevice](../resources/teamworkdevice.md) 集合|为租户预配的 Teams 设备。|
|teamsAppSettings|[teamsAppSettings](../resources/teamsappsettings.md)|表示租户中所有 [Teams 应用](teamsapp.md) 的租户范围设置。|
|teamTemplates|[teamtemplate](../resources/teamtemplate.md) 集合| 与团队关联的模板。|
|workforceIntegration|[workforceIntegration](../resources/workforceintegration.md) 集合| 工作人员与班次的集成。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamwork",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
    "@odata.type": "#microsoft.graph.teamwork",
    "id": "String (identifier)"
}
```

## <a name="see-also"></a>另请参阅

- [userTeamwork 资源类型](userteamwork.md)

