---
title: plannerPlan 资源类型
description: '**PlannerPlan**资源表示 Microsoft 365 中的计划。 计划可以由组所有，并包含 plannerTasks 集合。 其也可以有 plannerBuckets 集合。 每个计划对象具有可以包含此计划的更多信息的 details 对象。 有关组、计划和任务之间的关系的详细信息，请参阅“Planner”。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: e1dfc5e7c51bdb902b4c2c5f16c90eeb6b1e7771
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898252"
---
# <a name="plannerplan-resource-type"></a>plannerPlan 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**PlannerPlan**资源表示 Microsoft 365 中的计划。 计划可以由[组](group.md)所有，并包含 [plannerTasks](plannertask.md) 集合。 其也可以有 [plannerBuckets](plannerbucket.md) 集合。 每个计划对象具有可以包含此计划的更多信息的 [details](plannerplandetails.md) 对象。 有关组、计划和任务之间的关系的详细信息，请参阅 [Planner](planner-overview.md)。



## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Get plannerPlan](../api/plannerplan-get.md) | [plannerPlan](plannerplan.md) |读取 **plannerPlan** 对象的属性和关系。|
|[List buckets](../api/plannerplan-list-buckets.md) |[plannerBucket](plannerbucket.md) collection| 获取 **plannerBucket** 对象集合。|
|[List tasks](../api/plannerplan-list-tasks.md) |[plannerTask](plannertask.md) collection| 获取 **plannerTask** 对象集合。|
|[Update](../api/plannerplan-update.md) | [plannerPlan](plannerplan.md) |更新 **plannerPlan** 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|createdDateTime|DateTimeOffset|Read-only. Date and time at which the plan is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|id|String| 只读。 计划的 ID。 长度为 28 个字符，区分大小写。 [格式验证](tasks-identifiers-disclaimer.md)在服务上完成。|
|Owner|String|拥有计划的[组](group.md)的 ID。 必须存在有效的组才能设置此字段。 设置后，此属性无法更新。|
|title|String|必填。 计划的标题|
|createdBy|[identitySet](identityset.md)|只读。 创建计划的用户。|
|上下文|[plannerPlanContextCollection](plannerplancontextcollection.md)| 只读。 使用此计划的其他用户体验，表示为[plannerPlanContext](plannerplancontext.md)条目。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|buckets|[plannerBucket](plannerbucket.md) collection| Read-only. Nullable. Collection of buckets in the plan.|
|详细信息|[plannerPlanDetails](plannerplandetails.md)| 只读。 可为 NULL。 关于计划的其他详细信息。|
|tasks|[plannerTask](plannertask.md) collection| 只读。 可为 Null。 计划中的任务集合。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
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
  "suppressions": []
}
-->
