---
title: ChartDataLabels 资源类型
description: 表示图表点上的所有数据标签的集合。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 48d6cb0d35e82fc0117a24aad1c5e171bc869870
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961414"
---
# <a name="chartdatalabels-resource-type"></a>ChartDataLabels 资源类型

表示图表点上的所有数据标签的集合。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 ChartDataLabels](../api/chartdatalabels-get.md) | [WorkbookChartDataLabels](chartdatalabels.md) |读取 chartDataLabels 对象的属性和关系。|
|[Update](../api/chartdatalabels-update.md) | [WorkbookChartDataLabels](chartdatalabels.md) |更新 ChartDataLabels 对象 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|position|string|DataLabelPosition 值，它代表数据标签的位置。 可能的值为： `None`， `Center`， `InsideEnd`， `InsideBase`， `OutsideEnd`， `Left`， `Right`， `Top`， `Bottom`， `BestFit`， `Callout`。|
|separator|string|表示用于图表中数据标签的分隔符的字符串。|
|showBubbleSize|boolean|表示数据标签气泡大小是否可见的布尔值。|
|showCategoryName|boolean|表示数据标签类别名称是否可见的布尔值。|
|showLegendKey|boolean|表示数据标签图例标示是否可见的布尔值。|
|showPercentage|boolean|表示数据标签百分比是否可见的布尔值。|
|showSeriesName|boolean|表示数据标签系列名称是否可见的布尔值。|
|showValue|boolean|表示数据标签值是否可见的布尔值。|

## <a name="relationships"></a>Relationships
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|format|[WorkbookChartDataLabelFormat](chartdatalabelformat.md)|表示图表数据标签的格式，包括填充和字体格式。只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartDataLabels"
}-->

```json
{
  "position": "string",
  "separator": "string",
  "showBubbleSize": true,
  "showCategoryName": true,
  "showLegendKey": true,
  "showPercentage": true,
  "showSeriesName": true,
  "showValue": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartDataLabels resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
