---
title: TableColumn 资源类型
description: 代表表中的一列。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 095317b36c5242cd5e78f58192a242bd4e1f2993
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033976"
---
# <a name="tablecolumn-resource-type"></a>TableColumn 资源类型

代表表中的一列。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 TableColumn](../api/tablecolumn-get.md) | [WorkbookTableColumn](tablecolumn.md) |读取 tablecolumn 对象的属性和关系。|
|[更新](../api/tablecolumn-update.md) | [WorkbookTableColumn](tablecolumn.md) |更新 TableColumn 对象 |
|[Databodyrange](../api/tablecolumn-databodyrange.md)|[Range](range.md)|获取与列的数据体相关的 range 对象。|
|[Headerrowrange](../api/tablecolumn-headerrowrange.md)|[Range](range.md)|获取与列的标头行相关的 range 对象。|
|[区域](../api/tablecolumn-range.md)|[Range](range.md)|获取与整个列相关的 range 对象。|
|[Totalrowrange](../api/tablecolumn-totalrowrange.md)|[区域](range.md)|获取与列的总计行相关的 range 对象。|
|[删除](../api/tablecolumn-delete.md)|无|从表中删除列。|
|[列出](../api/tablecolumn-list.md) | [WorkbookTableColumn](tablecolumn.md) 集合 |获取 tableColumn 对象的集合。 |
|[Itemat](../api/tablecolumncollection-itemat.md)|[WorkbookTableColumn](tablecolumn.md)|根据其在集合中的位置获取列。|
|[添加](../api/tablecolumncollection-add.md)|[WorkbookTableColumn](tablecolumn.md)|向表中添加新列。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|string|返回用于标识表中列的唯一键。 应将此属性解析为不透明的字符串值，不得将它解析为其他任何类型。 只读。|
|index|int|返回表的列集合内列的索引编号。从零开始编制索引。只读。|
|name|string|返回表格列的名称。只读。|
|values|Json|表示指定区域的原始值。返回的数据类型可能是字符串、数字或布尔值。包含一个将返回错误字符串的错误的单元格。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|筛选器|[WorkbookFilter](filter.md)|检索应用于列的筛选器。只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableColumn"
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
