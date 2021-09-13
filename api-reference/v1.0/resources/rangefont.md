---
title: RangeFont 资源类型
description: 此对象表示对象的字体属性（字体名称、字体大小、颜色等）。
ms.localizationpriority: medium
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 760883a43ef534dc52ab69a098f9d9f688d46172
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59143704"
---
# <a name="rangefont-resource-type"></a>RangeFont 资源类型

命名空间：microsoft.graph

此对象表示对象的字体属性（字体名称、字体大小、颜色等）。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 RangeFont](../api/rangefont-get.md) | [WorkbookRangeFont](rangefont.md) |读取 rangeFont 对象的属性和关系。|
|[更新](../api/rangefont-update.md) | [WorkbookRangeFont](rangefont.md)   |更新 RangeFont 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|bold|布尔|表示字体的加粗状态。|
|color|string|文本颜色的 HTML 颜色代码表示。例如，#FF0000 表示红色。|
|italic|布尔|表示字体的斜体状态。|
|name|string|字体名称（例如"Calibri"）|
|大小|double|字号|
|underline|string|应用于字体的下划线类型。 可能的值包括 `None`、`Single`、`Double`、`SingleAccountant`、`DoubleAccountant`。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeFont"
}-->

```json
{
  "bold": true,
  "color": "string",
  "italic": true,
  "name": "string",
  "size": 1024,
  "underline": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

