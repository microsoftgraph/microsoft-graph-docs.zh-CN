---
title: workbookChartDataLabels 资源类型
description: 表示图表点上的所有数据标签的集合。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 28dc0d70f057569cd240770e15964b13c7982bae
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979283"
---
# <a name="workbookchartdatalabels-resource-type"></a>workbookChartDataLabels 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示图表点上的所有数据标签的集合。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 workbookChartDataLabels](../api/chartdatalabels-get.md) | [workbookChartDataLabels](workbookchartdatalabels.md) |读取 chartDataLabels 对象的属性和关系。|
|[更新](../api/chartdatalabels-update.md) | [workbookChartDataLabels](workbookchartdatalabels.md) |更新 ChartDataLabels 对象 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|position|string|表示数据标签的位置的 DataLabelPosition 值。 可能的值为：、、、、、、、、、、 `None` `Center` `InsideEnd` `InsideBase` `OutsideEnd` `Left` `Right` `Top` `Bottom` `BestFit` `Callout` 。|
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
|format|[workbookChartDataLabelFormat](workbookchartdatalabelformat.md)|表示图表数据标签的格式，包括填充和字体格式。 只读。|

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
<!--
{
  "type": "#page.annotation",
  "description": "workbookChartDataLabels resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


