---
title: workbookTableRow 资源类型
description: 表示表中的行。
author: lumine2008
ms.localizationpriority: medium
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 4b546e3593668c167479d18bcc06e1d61f59fbb4
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59777178"
---
# <a name="workbooktablerow-resource-type"></a>workbookTableRow 资源类型

命名空间：microsoft.graph

表示表中的行。


## <a name="methods"></a>方法

### <a name="manage-workbooktablerow"></a>管理 workbookTableRow
| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 workbookTableRow](../api/tablerow-get.md) | [WorkbookTableRow]( workbooktablerow.md) |读取 tableRow 对象的属性和关系。|
|[更新](../api/tablerow-update.md) | [WorkbookTableRow]( workbooktablerow.md) |更新 workbookTableRow 对象。 |
|[删除](../api/tablerow-delete.md)|无|从表中删除行。|
|[创建 workbookTableRow](../api/table-post-rows.md)|[WorkbookTableRow]( workbooktablerow.md)|向表中添加行。|
|[区域](../api/tablerow-range.md)|[区域](range.md)|返回与整个行相关的 range 对象。|
|[List](../api/tablerow-list.md) | [workbookTableRow]( workbooktablerow.md) 集合 |获取 tableRow 对象的集合。 |
|[Itemat](../api/tablerowcollection-itemat.md)|[WorkbookTableRow]( workbooktablerow.md)|根据其在集合中的位置获取行。|
|[添加](../api/tablerowcollection-add.md)|[WorkbookTableRow]( workbooktablerow.md)|向表中添加新行。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|index|Int32|返回表的行集合内行的索引编号。从零开始编制索引。只读。|
|值|[Json](../resources/json.md)|表示指定区域的原始值。返回的数据类型可能是字符串、数字或布尔值。包含一个将返回错误字符串的错误的单元格。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.workbookTableRow",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookTableRow",
  "index": "Integer",
  "values": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookTableRow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

