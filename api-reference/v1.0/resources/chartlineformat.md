---
title: ChartLineFormat 资源类型
description: 封装线条元素的格式选项。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9da0c29acf49d0e183a2ded4652fe0972f21bf76
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925915"
---
# <a name="chartlineformat-resource-type"></a>ChartLineFormat 资源类型

封装线条元素的格式选项。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 ChartLineFormat](../api/chartlineformat-get.md) | [WorkbookChartLineFormat](chartlineformat.md) |读取 chartLineFormat 对象的属性和关系。|
|[更新](../api/chartlineformat-update.md) | [WorkbookChartLineFormat](chartlineformat.md) |更新 ChartLineFormat 对象。 |
|[Clear](../api/chartlineformat-clear.md)|无|清除图表元素的线条格式。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|color|string|表示图表中的线条颜色的 HTML 颜色代码。|

## <a name="relationships"></a>Relationships
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
