---
title: TableRow 资源类型
description: 表示表中的行。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: fe95b62236322451893e3859f9d6599cc637848c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807173"
---
# <a name="tablerow-resource-type"></a>TableRow 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

表示表中的行。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 TableRow](../api/tablerow-get.md) | [TableRow](tablerow.md) |读取 tableRow 对象的属性和关系。|
|[Update](../api/tablerow-update.md) | [TableRow](tablerow.md)  |更新 TableRow 对象。 |
|[区域](../api/tablerow-range.md)|[Range](range.md)|返回与整个行相关联的范围对象。|
|[删除](../api/tablerow-delete.md)|无|从表中删除行。|
|[List](../api/tablerow-list.md) | [TableRow](tablerow.md) 集合 |获取 tableRow 对象的集合。 |
|[Itemat](../api/tablerowcollection-itemat.md)|[TableRow](tablerow.md)|按行在集合中的位置获取此对象。|
|[Add](../api/tablerowcollection-add.md)|[TableRow](tablerow.md)|向表中添加新行。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|index|int|返回表的行集合内行的索引编号。从零开始编制索引。只读。|
|values|json|表示指定区域的原始值。返回的数据类型可能是字符串、数字或布尔值。包含一个将返回错误字符串的错误的单元格。|

## <a name="relationships"></a>Relationships
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tableRow"
}-->

```json
{
  "index": 1024,
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
