---
title: plannerPlan 资源类型
description: '**PlannerPlan**资源表示 Office 365 中的计划。 规划组可以拥有和包含 plannerTasks 的集合。 它还可以具有 plannerBuckets 的集合。 每个计划对象都可以包含有关计划的详细信息的详细信息对象。 有关组、 计划和任务之间的关系的详细信息，请参阅计划程序。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: f37f6ea08f2951256e2d7f94cf9abad7e8ac60b2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529549"
---
# <a name="plannerplan-resource-type"></a>plannerPlan 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**PlannerPlan**资源表示 Office 365 中的计划。 规划[组](group.md)可以拥有和包含[plannerTasks](plannertask.md)的集合。 它还可以具有的[plannerBuckets](plannerbucket.md)集合。 每个计划对象都可以包含有关计划的详细信息的[详细信息](plannerplandetails.md)对象。 有关组、 计划和任务之间的关系的详细信息，请参阅[计划程序](planner-overview.md)。



## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|Get plannerPlan | [plannerPlan](plannerplan.md) |读取 plannerPlan 对象的属性和关系。|
|列出存储桶 |[plannerBucket](plannerbucket.md) collection| 获取 plannerBucket 对象集合。|
|[List tasks](../api/plannerplan-list-tasks.md) |[plannerTask](plannertask.md) collection| 获取 **plannerTask** 对象集合。|
|[Update](../api/plannerplan-update.md) | [plannerPlan](plannerplan.md) |更新 plannerPlan 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|createdDateTime|DateTimeOffset|只读。创建计划的日期和时间时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|id|String| 只读。 在计划的 ID。 它是 28 字符长度和区分大小写。 服务上执行[格式验证](tasks-identifiers-disclaimer.md)。|
|owner|String|拥有计划的[组](group.md)ID。 此字段可以设置之前，必须存在有效的组。 设置后，无法更新此属性。|
|title|String|必填。计划的标题|
|createdBy|[identitySet](identityset.md)|只读。创建计划的用户。|
|上下文|[plannerPlanContextCollection](plannerplancontextcollection.md)| 只读。 使用此计划的其他用户体验表示为[plannerPlanContext](plannerplancontext.md)条目。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|buckets|[plannerBucket](plannerbucket.md) collection| 只读。可为 Null。计划中的存储桶集合。|
|详细信息|[plannerPlanDetails](plannerplandetails.md)| 只读。可为 NULL。关于计划的其他详细信息。|
|tasks|[plannerTask](plannertask.md) collection| 只读。可为 Null。计划中的任务集合。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlan"
}-->

```json
{
  "contexts": {
    "48#19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype": {
        "@odata.type": "#microsoft.graph.plannerPlanContext",
        "associationType": "Board",
        "createdDateTime": "2015-10-14T00:57:28.4698344Z",
        "displayNameSegments": [
            "Finance Team",
            "Budget Plans"
        ],
        "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
    }
  },
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "owner": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplan.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
