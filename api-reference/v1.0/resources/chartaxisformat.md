---
title: ChartAxisFormat 资源类型
description: 封装图表坐标轴的格式属性。
ms.openlocfilehash: 38679d8f6d70c336f17aa5c17c9a20e80204cfb2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011742"
---
# <a name="chartaxisformat-resource-type"></a>ChartAxisFormat 资源类型

封装图表坐标轴的格式属性。


## <a name="methods"></a>方法
无
## <a name="properties"></a>属性
无

## <a name="relationships"></a>Relationships
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|font|[WorkbookChartFont](chartfont.md)|表示图表坐标轴元素的字体属性（字体名称、字体大小、颜色等）。只读。|
|line|[WorkbookChartLineFormat](chartlineformat.md)|表示图表线条格式。只读。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"},
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->