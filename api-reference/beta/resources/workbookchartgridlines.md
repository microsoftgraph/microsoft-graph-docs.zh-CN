---
title: workbookChartGridlines 资源类型
description: 代表图表坐标轴的主要或次要网格线。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ae89fb8714cfa1c9fba90961fafa3b74f679113b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979257"
---
# <a name="workbookchartgridlines-resource-type"></a>workbookChartGridlines 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表图表坐标轴的主要或次要网格线。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 workbookChartGridlines](../api/chartgridlines-get.md) | [workbookChartGridlines](workbookchartgridlines.md) |读取 chartGridlines 对象的属性和关系。|
|[更新](../api/chartgridlines-update.md) | [workbookChartGridlines](workbookchartgridlines.md)    |更新 ChartGridlines 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|visible|布尔|表示坐标轴网格线是否可见的布尔值。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|format|[workbookChartGridlinesFormat](workbookchartgridlinesformat.md)|表示图表网格线的格式。 只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartGridlines"
}-->

```json
{
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartGridlines resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


