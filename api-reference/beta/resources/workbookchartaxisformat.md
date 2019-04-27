---
title: workbookChartAxisFormat 资源类型
description: 封装图表坐标轴的格式属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 8c152971dde5efb188cfde30c30b54a1266b44fb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348560"
---
# <a name="workbookchartaxisformat-resource-type"></a>workbookChartAxisFormat 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

封装图表坐标轴的格式属性。


## <a name="methods"></a>方法
无
## <a name="properties"></a>属性
无

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|font|[workbookChartFont](workbookchartfont.md)|表示图表坐标轴元素的字体属性（字体名称、字体大小、颜色等）。只读。|
|line|[workbookChartLineFormat](workbookchartlineformat.md)|表示图表线条格式。 只读。|


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
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxisFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
