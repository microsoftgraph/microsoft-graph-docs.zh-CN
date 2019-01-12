---
title: ChartDataLabelFormat 资源类型
description: 封装图表数据表的格式属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 645267fd595a4b8e83090d9d6b2179e8c6112a78
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951990"
---
# <a name="chartdatalabelformat-resource-type"></a>ChartDataLabelFormat 资源类型

封装图表数据表的格式属性。


## <a name="methods"></a>方法
无

## <a name="properties"></a>属性
无

## <a name="relationships"></a>Relationships
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|fill|[WorkbookChartFill](chartfill.md)|表示当前图表数据标签的填充格式。只读。|
|font|[WorkbookChartFont](chartfont.md)|表示图表数据标签的字体属性（字体名称、字体大小、颜色等）。只读。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartDataLabelFormat"
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
  "description": "ChartDataLabelFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
