---
title: ChartLegend 资源类型
description: 表示图表中的图例。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: dbb95979e30143bf1c078edebf85c1e70c06e95e7c9818ec051602d394a48331
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54121296"
---
# <a name="chartlegend-resource-type"></a>ChartLegend 资源类型

命名空间：microsoft.graph

表示图表中的图例。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 ChartLegend](../api/chartlegend-get.md) | [WorkbookChartLegend](chartlegend.md) |读取 chartlegend 对象的属性和关系。|
|[更新](../api/chartlegend-update.md) | [WorkbookChartLegend](chartlegend.md) |更新 chartlegend 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|overlay|布尔|表示图表图例是否应该与图表主体重叠的布尔值。|
|position|string|表示图例在图表上的位置。 可能的值包括 `Top`、`Bottom`、`Left`、`Right`、`Corner`、`Custom`。|
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
<!-- {
  "type": "#page.annotation",
  "description": "ChartLegend resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

