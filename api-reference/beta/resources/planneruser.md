---
title: plannerUser 资源类型
description: '**PlannerUser**资源的用户提供对计划工具资源的访问。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 1f10810f6debf2346ed12484bac8e1f4bfd2f372
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526877"
---
# <a name="planneruser-resource-type"></a>plannerUser 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**PlannerUser**资源提供了对计划工具资源的[用户](user.md)的访问。 


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[List tasks](../api/planneruser-list-tasks.md) |[plannerTask](plannertask.md) 集合| 获取[plannerTasks](plannertask.md)分配给用户。|
|[列表 favoritePlans](../api/planneruser-list-favoriteplans.md) |[plannerPlan](plannerplan.md) 集合| 获取用户标记为 favorite [plannerPlans](plannerplan.md) 。|
|[列表 recentPlans](../api/planneruser-list-recentplans.md) |[plannerPlan](plannerplan.md) 集合| 获取由用户最近查看[plannerPlans](plannerplan.md) 。|
|[Update](../api/planneruser-update.md) | [plannerUser](planneruser.md)| 更新**plannerUser**对象。 |


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 只读。 PlannerUser 的标识符|
|favoritePlanReferences|[plannerFavoritePlanReferenceCollection](plannerfavoriteplanreferencecollection.md)| 包含对用户已标记为收藏夹的计划的引用的集合。|
|recentPlanReferences|[plannerRecentPlanReferenceCollection](plannerrecentplanreferencecollection.md)| 包含支持最新的计划的应用程序中的用户最近查看的计划对引用的集合。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|tasks|[plannerTask](plannertask.md) collection| 只读。可为 NULL。返回分配给用户的 [plannerTasks](plannertask.md)。|
|favoritePlans|[plannerPlan](plannerplan.md) 集合| 只读。 可为 NULL。 返回用户标记为收藏夹[plannerPlans](plannerplan.md) 。|
|recentPlans|[plannerPlan](plannerplan.md) 集合| 只读。 可为 NULL。 返回支持最新的计划的应用程序中的用户最近查看[plannerPlans](plannerplan.md) 。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUser"
}-->

```json
{
  "favoritePlanReferences": {"@odata.type": "microsoft.graph.plannerFavoritePlanReferenceCollection"},
  "id": "String (identifier)",
  "recentPlanReferences": {"@odata.type": "microsoft.graph.plannerRecentPlanReferenceCollection"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/planneruser.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
