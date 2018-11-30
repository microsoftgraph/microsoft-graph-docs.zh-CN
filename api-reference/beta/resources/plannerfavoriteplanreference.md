---
title: plannerFavoritePlanReference 资源类型
description: '**PlannerFavoritePlanReference**资源类型代表对由用户标记为收藏 plannerPlan 的引用。 '
ms.openlocfilehash: bd399572dfce54ee7e46da6af60eb661484519de
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043342"
---
# <a name="plannerfavoriteplanreference-resource-type"></a>plannerFavoritePlanReference 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

**PlannerFavoritePlanReference**资源类型代表对由用户标记为收藏[plannerPlan](plannerplan.md)的引用。 客户端应注意**plannerFavoritePlanReference**条目可以引用**plannerPlans**的被删除，用户不再可以访问，或已更新具有不同的标题。

我们建议客户端差异时通知用户，并保持最新条目。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|orderHint|字符串|用于为列表视图中的此类型项目排序的提示。此格式在[使用规划器中的排序提示](planner-order-hint-format.md)定义中。|
|planTitle|字符串|用户将其标记为收藏时计划的标题。|


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
<!-- {
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
