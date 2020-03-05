---
title: plannerFavoritePlanReference 资源类型
description: '**PlannerFavoritePlanReference**资源类型代表对已标记为用户收藏的 plannerPlan 的引用。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: d1bb7cb2ac675d558054523e38ba6bde44378568
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521739"
---
# <a name="plannerfavoriteplanreference-resource-type"></a>plannerFavoritePlanReference 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**PlannerFavoritePlanReference**资源类型代表对已标记为用户收藏的[plannerPlan](plannerplan.md)的引用。 客户端应注意， **plannerFavoritePlanReference**条目可以引用已删除的**plannerPlans** 、用户无法再访问或已使用其他标题进行更新。

我们建议客户端在存在差异时通知用户，并将这些条目保持为最新。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|orderHint|String|用于为列表视图中的此类型项目排序的提示。此格式在[使用规划器中的排序提示](planner-order-hint-format.md)定义中。|
|planTitle|String|用户将其标记为收藏时计划的标题。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerFavoritePlanReference"
}-->

```json
{
  "orderHint": "String",
  "planTitle": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
