---
title: plannerUser 资源类型
description: '**PlannerUser**资源为用户提供对 Planner 资源的访问权限。 它不包含任何可用属性。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 49b8989bd8526cbe8074a386ae31e76fd195642d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447092"
---
# <a name="planneruser-resource-type"></a>plannerUser 资源类型

命名空间： microsoft. graph

**PlannerUser**资源为[用户](user.md)提供对 Planner 资源的访问权限。 它不包含任何可用属性。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出计划](../api/planneruser-list-plans.md) |[plannerPlan](plannerplan.md) 集合| 获取**plannerPlan**对象集合。|
|[List tasks](../api/planneruser-list-tasks.md) |[plannerTask](plannertask.md) 集合| 获取 **plannerTask** 对象集合。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 只读。 PlanenrUser 的标识符|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|计划|[plannerPlan](plannerplan.md) 集合| 只读。 可为 NULL。 返回分配给用户的[plannerTasks](plannertask.md) 。|
|tasks|[plannerTask](plannertask.md) collection| 只读。 可为 NULL。 返回与用户共享的[plannerPlans](plannerplan.md) 。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUser"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
