---
title: plannerPlanContextDetails 资源类型
description: '**PlannerPlanContextDetails**资源包含有关 plannerPlanContext 的其他信息。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 9d4bf7d0a5c2149f826097eedc350e81eb32bf70
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009018"
---
# <a name="plannerplancontextdetails-resource-type"></a>plannerPlanContextDetails 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**PlannerPlanContextDetails**资源包含有关[plannerPlanContext](plannerplancontext.md)的其他信息。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|url|String|由关联的[plannerPlanContext](plannerplancontext.md)表示的用户体验的 URL。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContextDetails"
}-->

```json
{
  "url": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
