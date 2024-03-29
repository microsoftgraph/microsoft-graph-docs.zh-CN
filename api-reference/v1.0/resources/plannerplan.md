---
title: plannerPlan 资源类型
description: '**plannerPlan** 资源表示 Microsoft 365 中的计划。计划可以由组所有，并包含 plannerTasks 集合。它也可以拥有 plannerBuckets 集合。每个计划对象都具有可以包含该计划的更多信息的详细信息对象。有关组、计划和任务之间的关系的详细信息，请参阅“Planner”。'
ms.localizationpriority: high
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: d25c85d8cf63ff018a521b86822d8d2380d65ebb
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819711"
---
# <a name="plannerplan-resource-type"></a>plannerPlan 资源类型

命名空间：microsoft.graph

**plannerPlan** 资源表示 Microsoft 365 中的计划。计划可以由 [组](group.md)所有，并包含 [plannerTasks](plannertask.md) 集合。它也可以拥有 [plannerBuckets](plannerbucket.md) 集合。每个计划对象都具有可以包含该计划的更多信息的 [详细信息](plannerplandetails.md)对象。有关组、计划和任务之间的关系的详细信息，请参阅 [Planner](planner-overview.md)。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Get plannerPlan](../api/plannerplan-get.md) | [plannerPlan](plannerplan.md) |读取 **plannerPlan** 对象的属性和关系。|
|[List buckets](../api/plannerplan-list-buckets.md) |[plannerBucket](plannerbucket.md) collection| 获取 **plannerBucket** 对象集合。|
|[List tasks](../api/plannerplan-list-tasks.md) |[plannerTask](plannertask.md) collection| 获取 **plannerTask** 对象集合。|
|[Update](../api/plannerplan-update.md) | [plannerPlan](plannerplan.md) |更新 **plannerPlan** 对象。 |
|[删除](../api/plannerplan-delete.md) | 无 | 删除 **plannerPlan** 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|容器|[plannerPlanContainer](../resources/plannerplancontainer.md)|标识计划的容器。 设置后，此属性无法更新。 必填。|
|createdBy|[identitySet](identityset.md)|只读。创建计划的用户。|
|createdDateTime|DateTimeOffset|只读。创建计划的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。例如，UTC 时间 2014 年 1 月 1 日午夜将表示为 `2014-01-01T00:00:00Z`|
|id|String| 只读。计划的 ID。长度为 28 个字符，区分大小写。[格式验证](planner-identifiers-disclaimer.md)在服务上完成。|
|title|String|必填。计划的标题|
|所有者（已弃用） |字符串| 请改用 **container** 属性。 拥有计划的[组](group.md)的 ID。 设置后，此属性无法更新。 如果计划的容器不是组，则此属性将不会返回有效的组 ID。|

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
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlan"
}-->

```json
{
  "container": {
    "@odata.type": "microsoft.graph.plannerPlanContainer",
    "containerId": "String",
    "type": "String",
    "url": "String"
  },
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "title": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

