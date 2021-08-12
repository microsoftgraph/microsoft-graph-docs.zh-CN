---
title: TableRow 资源类型
description: 表示表中的行。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 0b9d9d07a6c2382194458913217b414a30000150bf61a2e4771cb9e8a27d53b8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189273"
---
# <a name="tablerow-resource-type"></a>TableRow 资源类型

命名空间：microsoft.graph

表示表中的行。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 TableRow](../api/tablerow-get.md) | [WorkbookTableRow](tablerow.md) |读取 tableRow 对象的属性和关系。|
|[更新](../api/tablerow-update.md) | [WorkbookTableRow](tablerow.md)  |更新 TableRow 对象。 |
|[区域](../api/tablerow-range.md)|[区域](range.md)|返回与整个行相关的 range 对象。|
|[删除](../api/tablerow-delete.md)|无|从表中删除行。|
|[列出](../api/tablerow-list.md) | [WorkbookTableRow](tablerow.md) 集合 |获取 tableRow 对象的集合。 |
|[Itemat](../api/tablerowcollection-itemat.md)|[WorkbookTableRow](tablerow.md)|根据其在集合中的位置获取行。|
|[添加](../api/tablerowcollection-add.md)|[WorkbookTableRow](tablerow.md)|向表中添加新行。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|index|int|返回表的行集合内行的索引编号。从零开始编制索引。只读。|
|values|Json|表示指定区域的原始值。返回的数据类型可能是字符串、数字或布尔值。包含一个将返回错误字符串的错误的单元格。|

## <a name="relationships"></a>关系
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

