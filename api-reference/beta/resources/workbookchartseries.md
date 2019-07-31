---
title: workbookChartSeries 资源类型
description: 代表图表上的系列。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: c7f7c8108ac17e6705b8bf5f69b0e87f0dc96b31
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007247"
---
# <a name="workbookchartseries-resource-type"></a>workbookChartSeries 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表图表上的系列。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 ChartSeries](../api/chartseries-get.md) | [workbookChartSeries](workbookchartseries.md) |读取 chartSeries 对象的属性和关系。|
|[创建 ChartPoint](../api/chartseries-post-points.md) |[chartPoints](workbookchartpoint.md)| 通过发布到点集合创建新的 chartPoint。|
|[列出 points](../api/chartseries-list-points.md) |[workbookChartPoints](workbookchartpoint.md)集合| 获取 chartPoints 对象集合。|
|[更新](../api/chartseries-update.md) | [workbookChartSeries](workbookchartseries.md) |更新 chartSeries 对象。 |
|[List](../api/chartseries-list.md) | [workbookChartSeries](workbookchartseries.md)集合 |获取 chartSeries 对象集合。 |
|[ItemAt](../api/chartseriescollection-itemat.md)|[workbookChartSeries](workbookchartseries.md)|根据其在集合中的位置检索系列|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|name|string|表示图表中某个系列的名称。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|format|[workbookChartSeriesFormat](workbookchartseriesformat.md)|表示图表系列的格式，包括填充和线条格式。只读。|
|points|[workbookChartPoint](workbookchartpoint.md)集合|表示系列中所有数据点的集合。 只读。|

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartSeries resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
