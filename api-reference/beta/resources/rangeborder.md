---
title: RangeBorder 资源类型
description: 表示对象的边框。
ms.openlocfilehash: ace494607d7e5803bf0ab0be5d5b3c86be875dcb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049027"
---
# <a name="rangeborder-resource-type"></a>RangeBorder 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

表示对象的边框。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 RangeBorder](../api/rangeborder-get.md) | [RangeBorder](rangeborder.md) |读取 rangeborder 对象的属性和关系。|
|[Update](../api/rangeborder-update.md) | [RangeBorder](rangeborder.md) |更新 RangeBorder 对象。 |
|[List](../api/rangeborder-list.md) | [RangeBorder](rangeborder.md) 集合 |获取 rangeBorder 对象集合。 |
|[Itemat](../api/rangebordercollection-itemat.md)|[RangeBorder](rangeborder.md)|使用其索引获取 border 对象|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|color|string|表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。|
|id|string|表示边框标识符。可能的值是：`EdgeTop`、`EdgeBottom`、`EdgeLeft`、`EdgeRight`、`InsideVertical`、`InsideHorizontal`、`DiagonalDown`、`DiagonalUp`。只读。|
|sideIndex|string|指示边框的特定边的常量值。可能的值是：`EdgeTop`、`EdgeBottom`、`EdgeLeft`、`EdgeRight`、`InsideVertical`、`InsideHorizontal`、`DiagonalDown`、`DiagonalUp`。只读。|
|style|string|线条样式的常量之一，指定边框的线条样式。可能的值是：`None`、`Continuous`、`Dash`、`DashDot`、`DashDotDot`、`Dot`、`Double`、`SlantDashDot`。|
|weight|string|指定区域周围边框的权重。可能的值是：`Hairline`、`Thin`、`Medium`、`Thick`。|

## <a name="relationships"></a>Relationships
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeBorder"
}-->

```json
{
  "color": "string",
  "id": "string",
  "sideIndex": "string",
  "style": "string",
  "weight": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->