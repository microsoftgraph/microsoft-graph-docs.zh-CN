---
title: workbookChartLegend 资源类型
description: 表示图表中的图例。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 60d37ab606668fbe6828293112997980c7e4580c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519307"
---
# <a name="workbookchartlegend-resource-type"></a>workbookChartLegend 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示图表中的图例。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 workbookChartLegend](../api/chartlegend-get.md) | [workbookChartLegend](workbookchartlegend.md) |读取 chartlegend 对象的属性和关系。|
|[更新](../api/chartlegend-update.md) | [workbookChartLegend](workbookchartlegend.md) |更新 chartlegend 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|overlay|布尔|表示图表图例是否应该与图表主体重叠的布尔值。|
|position|string|表示图例在图表上的位置。 可能的值包括 `Top`、`Bottom`、`Left`、`Right`、`Corner`、`Custom`。|
|visible|布尔|表示 ChartLegend 对象的可见性的布尔值。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|format|[workbookChartLegendFormat](workbookchartlegendformat.md)|表示图表图例的格式，包括填充和字体格式。 只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [
    "format"        
  ],
  "@odata.type": "microsoft.graph.workbookChartLegend"
}-->

```json
{
  "overlay": true,
  "position": "string",
  "visible": true,
  "format": {"@odata.type":"microsoft.graph.workbookChartLegendFormat"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartLegend resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
