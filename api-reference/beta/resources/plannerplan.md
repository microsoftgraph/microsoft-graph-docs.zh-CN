---
title: plannerPlan 资源类型
description: '**plannerPlan** 资源表示 Microsoft 365 中的计划。 计划可以由组所有，并包含 plannerTasks 集合。 其也可以有 plannerBuckets 集合。 每个计划对象具有可以包含此计划的更多信息的 details 对象。 有关组、计划和任务之间的关系的详细信息，请参阅“Planner”。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 4763f268628a4609ac91d0597aeb4f55a2d406ce
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720989"
---
# <a name="plannerplan-resource-type"></a>plannerPlan 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**plannerPlan** 资源表示 Microsoft 365 中的计划。 计划可以由[组](group.md)所有，并包含 [plannerTasks](plannertask.md) 集合。 其也可以有 [plannerBuckets](plannerbucket.md) 集合。 每个计划对象具有可以包含此计划的更多信息的 [details](plannerplandetails.md) 对象。 有关组、计划和任务之间的关系的详细信息，请参阅 [Planner](planner-overview.md)。



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
|容器|[plannerPlanContainer](../resources/plannerplancontainer.md)|标识计划的容器。 设置后，此属性无法更新。 必需。|
|createdDateTime|DateTimeOffset|只读。 创建计划的日期和时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|id|String| 只读。 计划的 ID。 长度为 28 个字符，区分大小写。 [格式验证](tasks-identifiers-disclaimer.md)在服务上完成。|
|title|String|必填。 计划的标题|
|createdBy|[identitySet](identityset.md)|只读。 创建计划的用户。|
|上下文|[plannerPlanContextCollection](plannerplancontextcollection.md)| 只读。 在此计划中使用的其他用户体验，表示为 [plannerPlanContext](plannerplancontext.md) 条目。|
|所有者 (已弃)  |String| 请 **改为使用容器** 属性。 拥有 [计划的](group.md) 组的 ID。 设置后，此属性无法更新。 如果计划的容器不是组，则此属性不会返回有效的组 ID。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|buckets|[plannerBucket](plannerbucket.md) collection| 计划中的存储桶集合。 只读。 可为 NULL。|
|详细信息|[plannerPlanDetails](plannerplandetails.md)| 关于计划的其他详细信息。 只读。 可为 NULL。 |
|tasks|[plannerTask](plannertask.md) collection| 计划中的任务集合。 只读。 可为 Null。 |

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
  "container": {
    "@odata.type": "microsoft.graph.plannerPlanContainer",
    "url": "String",
    "containerId": "String",
    "type": "String"
  },
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


