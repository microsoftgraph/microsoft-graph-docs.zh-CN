---
title: ChartPoint 资源类型
description: 表示图表中某个系列的点。
author: lumine2008
ms.localizationpriority: medium
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: e49df91420d27ea36aa3bda4c410299d61273550
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59062801"
---
# <a name="chartpoint-resource-type"></a>ChartPoint 资源类型

命名空间：microsoft.graph

表示图表中某个系列的点。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 ChartPoint](../api/chartpoint-get.md) | [WorkbookChartPoint](chartpoint.md) |读取 chartPoint 对象的属性和关系。|
|[列出](../api/chartpoint-list.md) | [WorkbookChartPoint](chartpoint.md) 集合 |获取 chartPoint 对象集合。 |
|[ItemAt](../api/chartpointscollection-itemat.md)|[WorkbookChartPoint](chartpoint.md)|根据其在系列中的位置检索点。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|值|Json|返回图表点的值。只读。|
|id|string|唯一标识符|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|format|[WorkbookChartPointFormat](chartpointformat.md)|封装图表点的格式属性。只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPoint"
}-->

```json
{
  "value": "string",
  "id": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

