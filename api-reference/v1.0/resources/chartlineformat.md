---
title: ChartLineFormat 资源类型
description: 封装线条元素的格式选项。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 4ad04617e59a45cb9c0fa265759fd249243e987d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988398"
---
# <a name="chartlineformat-resource-type"></a>ChartLineFormat 资源类型

命名空间：microsoft.graph

封装线条元素的格式选项。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 ChartLineFormat](../api/chartlineformat-get.md) | [WorkbookChartLineFormat](chartlineformat.md) |读取 chartLineFormat 对象的属性和关系。|
|[更新](../api/chartlineformat-update.md) | [WorkbookChartLineFormat](chartlineformat.md) |更新 ChartLineFormat 对象。 |
|[清除](../api/chartlineformat-clear.md)|None|清除图表元素的线条格式。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|color|string|表示图表中的线条颜色的 HTML 颜色代码。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartLineFormat"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

