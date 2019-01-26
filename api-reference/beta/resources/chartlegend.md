---
title: ChartLegend 资源类型
description: 表示图表中的图例。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 88330f98b2d652d347aae703ec91fd4de8678c9d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576393"
---
# <a name="chartlegend-resource-type"></a>ChartLegend 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示图表中的图例。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 ChartLegend](../api/chartlegend-get.md) | [WorkbookChartLegend](chartlegend.md) |读取 chartlegend 对象的属性和关系。|
|[Update](../api/chartlegend-update.md) | [WorkbookChartLegend](chartlegend.md) |更新 chartlegend 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|overlay|布尔|表示图表图例是否应该与图表主体重叠的布尔值。|
|position|string|代表图表上图例的位置。 可能的值为： `Top`， `Bottom`， `Left`， `Right`， `Corner`， `Custom`。|
|visible|布尔|表示 ChartLegend 对象的可见性的布尔值。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|format|[WorkbookChartLegendFormat](chartlegendformat.md)|表示图表图例的格式，包括填充和字体格式。只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

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
  "suppressions": [
    "Error: /api-reference/beta/resources/chartlegend.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
