---
title: RangeBorder 资源类型
description: 代表对象的边框。
author: lumine2008
ms.localizationpriority: medium
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 3fe1c55ca1cac12ac5514c8b703be4d85254044f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59143781"
---
# <a name="rangeborder-resource-type"></a>RangeBorder 资源类型

命名空间：microsoft.graph

代表对象的边框。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 RangeBorder](../api/rangeborder-get.md) | [WorkbookRangeBorder](rangeborder.md) |读取 rangeborder 对象的属性和关系。|
|[更新](../api/rangeborder-update.md) | [WorkbookRangeBorder](rangeborder.md) |更新 RangeBorder 对象。 |
|[列出](../api/rangeborder-list.md) | [WorkbookRangeBorder](rangeborder.md) 集合 |获取 rangeBorder 对象集合。 |
|[Itemat](../api/rangebordercollection-itemat.md)|[WorkbookRangeBorder](rangeborder.md)|使用其索引获取 border 对象|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|color|string|表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。|
|id|string|表示边框标识符。 可能的值是 `EdgeTop` `EdgeBottom` ：、、、、、、、。 `EdgeLeft` `EdgeRight` `InsideVertical` `InsideHorizontal` `DiagonalDown` `DiagonalUp` 只读。|
|sideIndex|string|指示边框的特定边的常量值。 可能的值是 `EdgeTop` `EdgeBottom` ：、、、、、、、。 `EdgeLeft` `EdgeRight` `InsideVertical` `InsideHorizontal` `DiagonalDown` `DiagonalUp` 只读。|
|style|string|线条样式的常量之一，指定边框的线条样式。 可能的值是 `None` `Continuous` ：、、、、、、、。 `Dash` `DashDot` `DashDotDot` `Dot` `Double` `SlantDashDot`|
|weight|string|指定区域周围的边框的粗细。 可能的值包括 `Hairline`、`Thin`、`Medium`、`Thick`。|

## <a name="relationships"></a>关系
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

