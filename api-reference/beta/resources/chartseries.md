---
title: ChartSeries 资源类型
description: 代表图表上的系列。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 6742c30eca55426e54290ae689bfabd8e14ce70f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842628"
---
# <a name="chartseries-resource-type"></a>ChartSeries 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

代表图表上的系列。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 ChartSeries](../api/chartseries-get.md) | [ChartSeries](chartseries.md) |读取 chartSeries 对象的属性和关系。|
|[创建 ChartPoints](../api/chartseries-post-points.md) |[ChartPoints](chartpoint.md)| 通过发布到点集合创建新的 ChartPoints。|
|[列出 points](../api/chartseries-list-points.md) |[ChartPoints](chartpoint.md) 集合| 获取 ChartPoints 对象集合。|
|[Update](../api/chartseries-update.md) | [ChartSeries](chartseries.md) |更新 ChartSeries 对象。 |
|[List](../api/chartseries-list.md) | [ChartSeries](chartseries.md) 集合 |获取 chartSeries 对象集合。 |
|[Itemat](../api/chartseriescollection-itemat.md)|[ChartSeries](chartseries.md)|根据其在集合中的位置检索系列|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|name|string|表示图表中某个系列的名称。|

## <a name="relationships"></a>Relationships
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|format|[ChartSeriesFormat](chartseriesformat.md)|表示图表系列的格式，包括填充和线条格式。只读。|
|points|[ChartPoints](chartpoint.md) 集合|表示系列中所有数据点的集合。只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartSeries"
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
