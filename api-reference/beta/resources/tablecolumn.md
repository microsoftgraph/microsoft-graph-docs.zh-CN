---
title: TableColumn 资源类型
description: 代表表中的一列。
author: lumine2008
ms.openlocfilehash: b68051403bf57d84b51850255c8f98c0b76ea9c0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354647"
---
# <a name="tablecolumn-resource-type"></a>TableColumn 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

代表表中的一列。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 TableColumn](../api/tablecolumn-get.md) | [TableColumn](tablecolumn.md) |读取 tablecolumn 对象的属性和关系。|
|[更新](../api/tablecolumn-update.md) | [TableColumn](tablecolumn.md) |更新 TableColumn 对象 |
|[Databodyrange](../api/tablecolumn-databodyrange.md)|[区域](range.md)|获取与列的数据体相关的 range 对象。|
|[Headerrowrange](../api/tablecolumn-headerrowrange.md)|[区域](range.md)|获取与列的标头行相关的 range 对象。|
|[区域](../api/tablecolumn-range.md)|[Range](range.md)|获取与整个列相关的 range 对象。|
|[Totalrowrange](../api/tablecolumn-totalrowrange.md)|[区域](range.md)|获取与列的总计行相关的 range 对象。|
|[删除](../api/tablecolumn-delete.md)|无|从表中删除列。|
|[列出](../api/tablecolumn-list.md) | [TableColumn](tablecolumn.md) 集合 |获取 tableColumn 对象的集合。 |
|[Itemat](../api/tablecolumncollection-itemat.md)|[TableColumn](tablecolumn.md)|根据其在集合中的位置获取列。|
|[添加](../api/tablecolumncollection-add.md)|[TableColumn](tablecolumn.md)|向表中添加新列。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|ID|整数|返回标识表内的列的唯一键。只读。|
|Index|整数|返回表的列集合内列的索引编号。从零开始编制索引。只读。|
|name|string|返回表格列的名称。只读。|
|values|json|表示指定区域的原始值。返回的数据类型可能是字符串、数字或布尔值。包含一个将返回错误字符串的错误的单元格。|

## <a name="relationships"></a>Relationships
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|筛选器|[Filter](filter.md)|检索应用于列的筛选器。只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tableColumn"
}-->

```json
{
  "id": 1024,
  "index": 1024,
  "name": "string",
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->