---
title: RangeFill 资源类型
description: 表示 range 对象的背景。
author: lumine2008
ms.localizationpriority: medium
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: c601b569db032c999ecc88300ca98b698500ca8f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59143774"
---
# <a name="rangefill-resource-type"></a>RangeFill 资源类型

命名空间：microsoft.graph

表示 range 对象的背景。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 RangeFill](../api/rangefill-get.md) | [WorkbookRangeFill](rangefill.md) |读取 rangeFill 对象的属性和关系。|
|[更新](../api/rangefill-update.md) | [WorkbookRangeFill](rangefill.md)   |更新 RangeFill 对象 |
|[清除](../api/rangefill-clear.md)|None|重置区域背景。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|color|string|表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeFill"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

