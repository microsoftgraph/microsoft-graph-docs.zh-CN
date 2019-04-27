---
title: workbookChartLineFormat 资源类型
description: 封装线条元素的格式选项。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b40c72240771edd3517f2b29df269d83adeec8f8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348598"
---
# <a name="workbookchartlineformat-resource-type"></a>workbookChartLineFormat 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

封装线条元素的格式选项。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 workbookChartLineFormat](../api/chartlineformat-get.md) | [workbookChartLineFormat](workbookchartlineformat.md) |读取 chartLineFormat 对象的属性和关系。|
|[更新](../api/chartlineformat-update.md) | [workbookChartLineFormat](workbookchartlineformat.md) |更新 ChartLineFormat 对象。 |
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
<!--
{
  "type": "#page.annotation",
  "description": "workbookChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
