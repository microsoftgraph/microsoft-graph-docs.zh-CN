---
title: ChartDataLabels 资源类型
description: 表示图表点上的所有数据标签的集合。
author: lumine2008
ms.localizationpriority: medium
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 4a705e27893b0bb2f873fa09e3a07e705aab0823
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59049709"
---
# <a name="chartdatalabels-resource-type"></a>ChartDataLabels 资源类型

命名空间：microsoft.graph

表示图表点上的所有数据标签的集合。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 ChartDataLabels](../api/chartdatalabels-get.md) | [WorkbookChartDataLabels](chartdatalabels.md) |读取 chartDataLabels 对象的属性和关系。|
|[更新](../api/chartdatalabels-update.md) | [WorkbookChartDataLabels](chartdatalabels.md) |更新 ChartDataLabels 对象 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|position|string|表示数据标签的位置的 DataLabelPosition 值。 可能的值包括 `None` `Center` `InsideEnd` `InsideBase` `OutsideEnd` `Left` ：、、、、、、、、。 `Right` `Top` `Bottom` `BestFit` `Callout`|
|Separator|string|表示用于图表中数据标签的分隔符的字符串。|
|showBubbleSize|布尔|表示数据标签气泡大小是否可见的布尔值。|
|showCategoryName|布尔|表示数据标签类别名称是否可见的布尔值。|
|showLegendKey|布尔|表示数据标签图例标示是否可见的布尔值。|
|showPercentage|布尔|表示数据标签百分比是否可见的布尔值。|
|showSeriesName|布尔|表示数据标签系列名称是否可见的布尔值。|
|showValue|布尔|表示数据标签值是否可见的布尔值。|

## <a name="relationships"></a>关系
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

