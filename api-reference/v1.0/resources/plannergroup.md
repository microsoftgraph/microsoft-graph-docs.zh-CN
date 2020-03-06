---
title: plannerGroup 资源类型
description: '**PlannerGroup**资源提供对组的 Planner 资源的访问。 它不包含任何可用属性。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: d7b495575eafbea877df79a6b8a5fb83b0ad2060
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533996"
---
# <a name="plannergroup-resource-type"></a>plannerGroup 资源类型

命名空间：microsoft.graph

**PlannerGroup**资源提供对[组](group.md)的 Planner 资源的访问。 它不包含任何可用属性。

## <a name="methods"></a>Methods

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出计划](../api/plannergroup-list-plans.md) |[plannerPlan](plannerplan.md) 集合| 获取**plannerPlan**对象集合。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|字符串| 只读。 **PlannerGroup**的标识符|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|计划|[plannerPlan](plannerplan.md) 集合| 只读。 可为空。 返回组所拥有的[plannerPlans](plannerplan.md) 。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerGroup"
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
  "description": "plannerGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
