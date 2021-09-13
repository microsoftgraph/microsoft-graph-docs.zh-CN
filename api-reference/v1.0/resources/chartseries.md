---
title: ChartSeries 资源类型
description: 代表图表上的系列。
author: lumine2008
ms.localizationpriority: medium
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 7e3b9ceac73f724ef520f1fdfc22f01c636d1f51
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109463"
---
# <a name="chartseries-resource-type"></a>ChartSeries 资源类型

命名空间：microsoft.graph

代表图表上的系列。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 ChartSeries](../api/chartseries-get.md) | [WorkbookChartSeries](chartseries.md) |读取 chartSeries 对象的属性和关系。|
|[创建 ChartPoints](../api/chartseries-post-points.md) |[ChartPoints](chartpoint.md)| 通过发布到点集合创建新的 ChartPoints。|
|[列出 points](../api/chartseries-list-points.md) |[ChartPoints](chartpoint.md) 集合| 获取 ChartPoints 对象集合。|
|[更新](../api/chartseries-update.md) | [WorkbookChartSeries](chartseries.md) |更新 ChartSeries 对象。 |
|[列出](../api/chartseries-list.md) | [WorkbookChartSeries](chartseries.md) 集合 |获取 chartSeries 对象集合。 |
|[ItemAt](../api/chartseriescollection-itemat.md)|[WorkbookChartSeries](chartseries.md)|根据其在集合中的位置检索系列|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|name|string|表示图表中某个系列的名称。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|format|[WorkbookChartSeriesFormat](chartseriesformat.md)|表示图表系列的格式，包括填充和线条格式。只读。|
|points|[WorkbookChartPoint](chartpoint.md) 集合|表示系列中所有数据点的集合。只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartSeries"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeries resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

