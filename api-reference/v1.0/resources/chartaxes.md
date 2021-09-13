---
title: ChartAxes 资源类型
description: 表示图表坐标轴。
author: lumine2008
ms.localizationpriority: medium
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 7d743695c6d7cd94636a795f75a8059976f743e8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59032396"
---
# <a name="chartaxes-resource-type"></a>ChartAxes 资源类型

命名空间：microsoft.graph

表示图表坐标轴。


## <a name="methods"></a>方法
None

## <a name="properties"></a>属性
无

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|categoryAxis|[WorkbookChartAxis](chartaxis.md)|表示图表中的类别轴。只读。|
|seriesAxis|[WorkbookChartAxis](chartaxis.md)|表示三维图表的系列轴。只读。|
|valueAxis|[WorkbookChartAxis](chartaxis.md)|表示坐标轴中的数值轴。只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxes"
}-->

```json
{
  "categoryAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"},
  "seriesAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"},
  "valueAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

