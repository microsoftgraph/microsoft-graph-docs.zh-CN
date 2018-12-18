---
title: ChartAxis 资源类型
description: 表示图表中的单个坐标轴。
author: lumine2008
ms.openlocfilehash: 766a1a6823cc83efb3ecaf7250f230216fc13cb0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301825"
---
# <a name="chartaxis-resource-type"></a>ChartAxis 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

代表图表中的单个坐标轴。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 ChartAxis](../api/chartaxis-get.md) | [ChartAxis](chartaxis.md) |读取 chartaxis 对象的属性和关系。|
|[Update](../api/chartaxis-update.md) | [ChartAxis](chartaxis.md)   |更新 ChartAxis 对象 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|majorUnit|对象|表示两个主要刻度标记之间的间隔。可以设置为数字值或空字符串。返回的值始终为数字。|
|maximum|对象|表示数值轴上的最大值。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。|
|minimum|对象|表示数值轴上的最小值。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。|
|minorUnit|对象|表示两个次要刻度标记之间的间隔。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。|

## <a name="relationships"></a>Relationships
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|format|[ChartAxisFormat](chartaxisformat.md)|表示 chart 对象的格式，包括线条和字体格式。只读。|
|majorGridlines|[ChartGridlines](chartgridlines.md)|返回一个表示指定坐标轴的主要网格线的 gridline 对象。只读。|
|minorGridlines|[ChartGridlines](chartgridlines.md)|返回一个表示指定坐标轴的次要网格线的网格线对象。只读。|
|title|[ChartAxisTitle](chartaxistitle.md)|表示坐标轴标题。只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartaxis"
}-->

```json
{
  "majorUnit": "string",
  "maximum": "string",
  "minimum": "string",
  "minorUnit": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxis resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->