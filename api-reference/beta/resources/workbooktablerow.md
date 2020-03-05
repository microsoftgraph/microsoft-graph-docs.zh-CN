---
title: workbookTableRow 资源类型
description: 表示表中的行。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ba7b481f4b20033e1a4ffcd42ac92421bc3536a4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519118"
---
# <a name="workbooktablerow-resource-type"></a>workbookTableRow 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示表中的行。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 TableRow](../api/tablerow-get.md) | [workbookTableRow](workbooktablerow.md) |读取 tableRow 对象的属性和关系。|
|[更新](../api/tablerow-update.md) | [workbookTableRow](workbooktablerow.md)  |更新 TableRow 对象。 |
|[Range](../api/tablerow-range.md)|[workbookRange](workbookrange.md)|返回与整个行相关的 range 对象。|
|[删除](../api/tablerow-delete.md)|无|从表中删除行。|
|[列出](../api/tablerow-list.md) | [workbookTableRow](workbooktablerow.md)集合 |获取 tableRow 对象的集合。 |
|[Itemat](../api/tablerowcollection-itemat.md)|[workbookTableRow](workbooktablerow.md)|根据其在集合中的位置获取行。|
|[添加](../api/tablerowcollection-add.md)|[workbookTableRow](workbooktablerow.md)|向表中添加新行。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|index|int|返回表的行集合内行的索引编号。从零开始编制索引。只读。|
|values|Json|表示指定区域的原始值。返回的数据类型可能是字符串、数字或布尔值。包含一个将返回错误字符串的错误的单元格。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "TableRow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
