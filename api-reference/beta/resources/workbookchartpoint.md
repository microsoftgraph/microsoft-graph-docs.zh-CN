---
title: workbookChartPoint 资源类型
description: 表示图表中某个系列的点。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 54342227c15eeb1b11c3ddfb157e1ef3bc83390e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519286"
---
# <a name="workbookchartpoint-resource-type"></a>workbookChartPoint 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示图表中某个系列的点。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 workbookChartPoint](../api/chartpoint-get.md) | [workbookChartPoint](workbookchartpoint.md) |读取 chartPoint 对象的属性和关系。|
|[列出](../api/chartpoint-list.md) | [workbookChartPoint](workbookchartpoint.md)集合 |获取 chartPoint 对象集合。 |
|[ItemAt](../api/chartpointscollection-itemat.md)|[workbookChartPoint](workbookchartpoint.md)|根据其在系列中的位置检索点。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|值|Json|返回图表点的值。 只读。|
|id|string|唯一标识符|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|format|[workbookChartPointFormat](workbookchartpointformat.md)|封装图表点的格式属性。 只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "format"
    ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPoint"
}-->

```json
{
  "value": "string",
  "id": "string",
  "format": {"@odata.type": "microsoft.graph.workbookChartPointFormat"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
