---
title: plannerGroup 资源类型
description: '**plannerGroup** 资源提供对组 Planner 资源的访问权限。 它不包含任何可用属性。'
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 1140d22b4b2f1bb5f863c19a741d08171c5f00f7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019256"
---
# <a name="plannergroup-resource-type"></a>plannerGroup 资源类型

命名空间：microsoft.graph

**plannerGroup** 资源提供对组 的 Planner 资源 [的访问权限](group.md)。 它不包含任何可用属性。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出计划](../api/plannergroup-list-plans.md) |[plannerPlan](plannerplan.md) 集合| 获取 **plannerPlan** 对象集合。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 只读。 **plannerGroup 的标识符**|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|计划|[plannerPlan](plannerplan.md) 集合| 只读。 可为空。 返回[组所有的 plannerPlans。](plannerplan.md)|

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

