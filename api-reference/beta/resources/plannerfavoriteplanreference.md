---
title: plannerFavoritePlanReference 资源类型
description: '**plannerFavoritePlanReference**资源类型代表对已标记为用户收藏的 plannerPlan 的引用。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 239376a9d1cb8a761cc8f479ff600519b01effcb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344492"
---
# <a name="plannerfavoriteplanreference-resource-type"></a>plannerFavoritePlanReference 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**plannerFavoritePlanReference**资源类型代表对已标记为用户收藏的[plannerPlan](plannerplan.md)的引用。 客户端应注意, **plannerFavoritePlanReference**条目可以引用已删除的**plannerPlans** 、用户无法再访问或已使用其他标题进行更新。

我们建议客户端在存在差异时通知用户, 并将这些条目保持为最新。


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
