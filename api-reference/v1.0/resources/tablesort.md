---
title: TableSort 资源类型
description: 管理对 Table 对象的排序操作。
author: lumine2008
ms.localizationpriority: medium
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 03c951f26c2b037153b07daa461e768d62d5638b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59032123"
---
# <a name="tablesort-resource-type"></a>TableSort 资源类型

命名空间：microsoft.graph

管理对 Table 对象的排序操作。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 TableSort](../api/tablesort-get.md) | [WorkbookTableSort](tablesort.md) |读取 tableSort 对象的属性和关系。|
|[应用](../api/tablesort-apply.md)|无|执行排序操作。|
|[清除](../api/tablesort-clear.md)|None|清除表上的当前排序。尽管这不能修改表的排序，但它会清除标题按钮的状态。|
|[重新应用](../api/tablesort-reapply.md)|无|对表重新应用当前的排序参数。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|域|[WorkbookSortField](sortfield.md) 集合|表示最后一次对表排序所使用的当前条件。只读。|
|matchCase|boolean|表示最后一次对表进行排序时大小写是否有影响。只读。|
|方法|string|表示最后一次对表排序所使用的中文字符排序方法。 可能的值是 `PinYin` `StrokeCount` ：、。 只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableSort"
}-->

```json
{
  "matchCase": true,
  "method": "string",
  "fields": [{ "@odata.type": "microsoft.graph.workbookSortField" }]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

