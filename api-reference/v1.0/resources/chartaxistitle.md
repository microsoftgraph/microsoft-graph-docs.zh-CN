---
title: ChartAxisTitle 资源类型
description: 表示图表坐标轴的标题。
author: lumine2008
ms.localizationpriority: medium
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: e4c927eb6650e8effe67b432415a726f51ddefcb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59126917"
---
# <a name="chartaxistitle-resource-type"></a>ChartAxisTitle 资源类型

命名空间：microsoft.graph

表示图表坐标轴的标题。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 ChartAxisTitle](../api/chartaxistitle-get.md) | [WorkbookChartAxisTitle](chartaxistitle.md) |读取 chartAxisTitle 对象的属性和关系。|
|[更新](../api/chartaxistitle-update.md) | [WorkbookChartAxisTitle](chartaxistitle.md)    |更新 ChartAxisTitle 对象 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|text|string|表示坐标轴标题。|
|visible|布尔|指定坐标轴标题可见性的布尔值。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|format|[WorkbookChartAxisTitleFormat](chartaxistitleformat.md)|表示图表坐标轴标题的格式。只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartAxisTitle"
}-->

```json
{
  "text": "string",
  "visible": true,
  "format": {"@odata.type":"microsoft.graph.workbookChartAxisTitleFormat"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

