---
title: workbookChartDataLabelFormat 资源类型
description: 封装图表数据表的格式属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: bd60187d5bc62675b53b4a0a254afa3632e9c1d6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963995"
---
# <a name="workbookchartdatalabelformat-resource-type"></a>workbookChartDataLabelFormat 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

封装图表数据表的格式属性。


## <a name="methods"></a>方法
无

## <a name="properties"></a>属性
无

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|fill|[workbookChartFill](workbookchartfill.md)|表示当前图表数据标签的填充格式。只读。|
|font|[workbookChartFont](workbookchartfont.md)|表示图表数据标签的字体属性（字体名称、字体大小、颜色等）。 只读。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "fill",
    "font"
    ],
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartDataLabelFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
