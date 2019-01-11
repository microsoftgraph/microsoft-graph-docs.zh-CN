---
title: ChartTitle 资源类型
description: 表示图表的 chart title 对象。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 6cf6a2e6355fc4bc8955899dde48f9cc843e920c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879413"
---
# <a name="charttitle-resource-type"></a>ChartTitle 资源类型

表示图表的 chart title 对象。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 ChartTitle](../api/charttitle-get.md) | [WorkbookChartTitle](charttitle.md) |读取 chartTitle 对象的属性和关系。|
|[Update](../api/charttitle-update.md) | [WorkbookChartTitle](charttitle.md)    |更新 ChartTitle 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|overlay|boolean|表示图表标题是否将叠加在图表上的布尔值。|
|text|string|表示图表的标题文本。|
|visible|boolean|表示 chart title 对象的可见性的布尔值。|

## <a name="relationships"></a>Relationships
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|format|[WorkbookChartTitleFormat](charttitleformat.md)|表示图表标题的格式，包括填充和字体格式。只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartTitle"
}-->

```json
{
  "overlay": true,
  "text": "string",
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
