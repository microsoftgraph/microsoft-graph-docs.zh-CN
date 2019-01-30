---
title: 图表资源类型
description: 表示工作簿中的 chart 对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4bc0ad0d31981e7e84241519e92569ab25c2cf18
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643232"
---
# <a name="chart-resource-type"></a>图表资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示工作簿中的 chart 对象。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取图表](../api/chart-get.md) | [Chart](chart.md) |读取 chart 对象的属性和关系。|
|[创建 ChartSeries](../api/chart-post-series.md) |[ChartSeries](chartseries.md)| 通过发布到序列集合创建新的 ChartSeries。|
|[创建系列](../api/chart-list-series.md) |[ChartSeries](chartseries.md) 集合| 获取 ChartSeries 对象集合。|
|[更新](../api/chart-update.md) | [Chart](chart.md)   |更新 Chart 对象。 |
|[Image](../api/chart-image.md)|图像 base64 编码字符串|通过缩放图表适应指定的尺寸，将图表呈现为 base64 编码的图像。|
|[删除](../api/chart-delete.md)|无|删除 chart 对象。|
|[Setdata](../api/chart-setdata.md)|无|重置图表的源数据。|
|[Setposition](../api/chart-setposition.md)|无|相对于工作表上的单元格放置图表。|
|[List](../api/chart-list.md) | [图表](chart.md) 集合 |获取 chart 对象集合。 |
|[Itemat](../api/chartcollection-itemat.md)|[Chart](chart.md)|按图表在集合中的位置获取此对象。|
|[Add](../api/chartcollection-add.md)|[Chart](chart.md)|创建新图表。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|height|double|表示 chart 对象的高度，以磅值表示。|
|id|string|根据其在集合中的位置获取图表。只读。|
|left|double|从图表左侧到工作表原点的距离，以磅值表示。|
|name|string|表示 chart 对象的名称。|
|top|double|表示从对象左边界至第 1 行顶部（在工作表上）或图表区域顶部（在图表上）的距离，以磅值表示。|
|width|double|表示 chart 对象的宽度，以磅值表示。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|axes|[ChartAxes](chartaxes.md)|表示图表坐标轴。只读。|
|dataLabels|[ChartDataLabels](chartdatalabels.md)|表示图表上的数据标签。只读。|
|format|[ChartAreaFormat](chartareaformat.md)|封装图表区域的格式属性。只读。|
|legend|[ChartLegend](chartlegend.md)|表示图表的图例。只读。|
|series|[ChartSeries](chartseries.md) 集合|表示单个系列或图表中的系列集合。只读。|
|title|[ChartTitle](charttitle.md)|表示指定图表的标题，包括标题的文本、可见性、位置和格式。只读。|
|worksheet|[工作表](worksheet.md)|包含当前图表的工作表。只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chart"
}-->

```json
{
  "height": 1024,
  "id": "string",
  "left": 1024,
  "name": "string",
  "top": 1024,
  "width": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Chart resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chart.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
