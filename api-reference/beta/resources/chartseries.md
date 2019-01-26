---
title: ChartSeries 资源类型
description: 代表图表上的系列。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: eccd0d970ffeff7b41ceb0f9af810bb7a420d663
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570657"
---
# <a name="chartseries-resource-type"></a>ChartSeries 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表图表上的系列。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 ChartSeries](../api/chartseries-get.md) | [workbookChartSeries](chartseries.md) |读取 chartSeries 对象的属性和关系。|
|[创建 ChartPoints](../api/chartseries-post-points.md) |[chartPoints](chartpoint.md)| 通过发布到点集合创建新的 ChartPoints。|
|[列出 points](../api/chartseries-list-points.md) |[chartPoints](chartpoint.md)集合| 获取 ChartPoints 对象集合。|
|[Update](../api/chartseries-update.md) | [workbookChartSeries](chartseries.md) |更新 ChartSeries 对象。 |
|[List](../api/chartseries-list.md) | [workbookChartSeries](chartseries.md)集合 |获取 chartSeries 对象集合。 |
|[ItemAt](../api/chartseriescollection-itemat.md)|[workbookChartSeries](chartseries.md)|根据其在集合中的位置检索系列|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|name|string|表示图表中某个系列的名称。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|format|[workbookChartSeriesFormat](chartseriesformat.md)|表示图表系列的格式，包括填充和线条格式。只读。|
|points|[workbookChartPoint](chartpoint.md)集合|表示系列中所有数据点的集合。只读。|

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
  "suppressions": [
    "Error: /api-reference/beta/resources/chartseries.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
