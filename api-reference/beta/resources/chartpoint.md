---
title: ChartPoint 资源类型
description: 表示图表中某个系列的点。
ms.openlocfilehash: 3d1bcc26fdc78bd7b844c870d40346a5f1f0496f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046182"
---
# <a name="chartpoint-resource-type"></a>ChartPoint 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

表示图表中某个系列的点。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 ChartPoint](../api/chartpoint-get.md) | [ChartPoint](chartpoint.md) |读取 chartPoint 对象的属性和关系。|
|[List](../api/chartpoint-list.md) | [ChartPoint](chartpoint.md) 集合 |获取 chartPoint 对象集合。 |
|[Itemat](../api/chartpointscollection-itemat.md)|[ChartPoint](chartpoint.md)|根据其在系列中的位置检索点。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|value|对象|返回图表点的值。只读。|

## <a name="relationships"></a>Relationships
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|format|[ChartPointFormat](chartpointformat.md)|封装图表点的格式属性。只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartPoint"
}-->

```json
{
  "value": "string"
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