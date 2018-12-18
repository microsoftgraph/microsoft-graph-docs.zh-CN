---
title: TableRow 资源类型
description: 表示表中的行。
author: lumine2008
ms.openlocfilehash: f34190aa4ac565d09ec8b07e96b2923f785b8d7c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341333"
---
# <a name="tablerow-resource-type"></a>TableRow 资源类型

表示表中的行。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 TableRow](../api/tablerow-get.md) | [WorkbookTableRow](tablerow.md) |读取 tableRow 对象的属性和关系。|
|[Update](../api/tablerow-update.md) | [WorkbookTableRow](tablerow.md)  |更新 TableRow 对象。 |
|[区域](../api/tablerow-range.md)|[Range](range.md)|返回与整个行相关联的范围对象。|
|[删除](../api/tablerow-delete.md)|无|从表中删除行。|
|[List](../api/tablerow-list.md) | [WorkbookTableRow](tablerow.md)集合 |获取 tableRow 对象的集合。 |
|[Itemat](../api/tablerowcollection-itemat.md)|[WorkbookTableRow](tablerow.md)|根据其在集合中的位置获取行。|
|[Add](../api/tablerowcollection-add.md)|[WorkbookTableRow](tablerow.md)|向表中添加新行。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|index|整数|返回表的行集合内行的索引编号。从零开始编制索引。只读。|
|values|Json|表示指定区域的原始值。返回的数据类型可能是字符串、数字或布尔值。包含一个将返回错误字符串的错误的单元格。|

## <a name="relationships"></a>Relationships
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableRow"
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