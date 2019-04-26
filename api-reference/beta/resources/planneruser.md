---
title: plannerUser 资源类型
description: '**plannerUser**资源为用户提供对 Planner 资源的访问权限。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 1f10810f6debf2346ed12484bac8e1f4bfd2f372
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563651"
---
# <a name="planneruser-resource-type"></a>plannerUser 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**plannerUser**资源为[用户](user.md)提供对 Planner 资源的访问权限。 


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出任务](../api/planneruser-list-tasks.md) |[plannerTask](plannertask.md) 集合| 获取分配给用户的[plannerTasks](plannertask.md) 。|
|[列出 favoritePlans](../api/planneruser-list-favoriteplans.md) |[plannerPlan](plannerplan.md) 集合| 获取用户标记为收藏的[plannerPlans](plannerplan.md) 。|
|[列出 recentPlans](../api/planneruser-list-recentplans.md) |[plannerPlan](plannerplan.md) 集合| 获取用户最近查看过的[plannerPlans](plannerplan.md) 。|
|[更新](../api/planneruser-update.md) | [plannerUser](planneruser.md)| 更新**plannerUser**对象。 |


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 只读。 plannerUser 的标识符|
|favoritePlanReferences|[plannerFavoritePlanReferenceCollection](plannerfavoriteplanreferencecollection.md)| 包含对用户已标记为收藏夹的计划引用的集合。|
|recentPlanReferences|[plannerRecentPlanReferenceCollection](plannerrecentplanreferencecollection.md)| 包含对计划的引用的集合, 该用户最近在支持最近计划的应用程序中查看了这些计划。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|任务|[plannerTask](plannertask.md) 集合| 只读。 可为 Null。 返回分配给用户的[plannerTasks](plannertask.md) 。|
|favoritePlans|[plannerPlan](plannerplan.md) 集合| 只读。 可为 Null。 返回用户标记为收藏夹的[plannerPlans](plannerplan.md) 。|
|recentPlans|[plannerPlan](plannerplan.md) 集合| 只读。 可为 Null。 返回用户最近在支持最近计划的应用程序中查看的[plannerPlans](plannerplan.md) 。 |

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
