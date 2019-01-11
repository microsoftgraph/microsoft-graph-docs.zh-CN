---
title: ChartAreaFormat 资源类型
description: 封装整个图表区域的格式属性。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 79867ff3519467279abcb4b9684b713964eb8f98
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838169"
---
# <a name="chartareaformat-resource-type"></a>ChartAreaFormat 资源类型

封装整个图表区域的格式属性。


## <a name="methods"></a>方法
无

## <a name="properties"></a>属性
无

## <a name="relationships"></a>Relationships
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|fill|[WorkbookChartFill](chartfill.md)|表示对象的填充格式，包括背景格式信息。只读。|
|font|[WorkbookChartFont](chartfont.md)|表示当前对象的字体属性（字体名称、字体大小、颜色等）。只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAreaFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAreaFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
