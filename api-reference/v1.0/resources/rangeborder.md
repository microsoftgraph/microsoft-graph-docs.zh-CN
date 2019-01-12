---
title: RangeBorder 资源类型
description: 表示对象的边框。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9c32264311400951152f892e6f88d70645f47064
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947608"
---
# <a name="rangeborder-resource-type"></a>RangeBorder 资源类型

表示对象的边框。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 RangeBorder](../api/rangeborder-get.md) | [WorkbookRangeBorder](rangeborder.md) |读取 rangeborder 对象的属性和关系。|
|[Update](../api/rangeborder-update.md) | [WorkbookRangeBorder](rangeborder.md) |更新 RangeBorder 对象。 |
|[List](../api/rangeborder-list.md) | [WorkbookRangeBorder](rangeborder.md)集合 |获取 rangeBorder 对象集合。 |
|[Itemat](../api/rangebordercollection-itemat.md)|[WorkbookRangeBorder](rangeborder.md)|使用其索引获取 border 对象|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|color|string|表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。|
|id|string|代表边框标识符。 可能的值为： `EdgeTop`， `EdgeBottom`， `EdgeLeft`， `EdgeRight`， `InsideVertical`， `InsideHorizontal`， `DiagonalDown`， `DiagonalUp`。 此为只读属性。|
|sideIndex|string|常量值，该值指示的特定的一侧边框。 可能的值为： `EdgeTop`， `EdgeBottom`， `EdgeLeft`， `EdgeRight`， `InsideVertical`， `InsideHorizontal`， `DiagonalDown`， `DiagonalUp`。 此为只读属性。|
|style|string|指定边框线型的线条样式的常量之一。 可能的值为： `None`， `Continuous`， `Dash`， `DashDot`， `DashDotDot`， `Dot`， `Double`， `SlantDashDot`。|
|weight|string|指定某一区域周围的边框的粗细。 可能的值为： `Hairline`， `Thin`， `Medium`， `Thick`。|

## <a name="relationships"></a>Relationships
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeBorder"
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
