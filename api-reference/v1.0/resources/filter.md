---
title: 筛选器资源类型
description: 管理表格列的筛选。
ms.openlocfilehash: 272b4ea0ee91c25ea845217512a12e33b08ed7b8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009270"
---
# <a name="filter-resource-type"></a>筛选器资源类型

管理表格列的筛选。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[应用](../api/filter-apply.md)|无|在给定列中应用给定的筛选条件。|
|[Clear](../api/filter-clear.md)|无|清除给定列上的筛选器。|

## <a name="properties"></a>属性

| 名称 | 类型   |说明|
|:---------------|:--------|:----------|
|条件|[WorkbookFilterCriteria](filtercriteria.md)|给定列上当前应用的筛选器。只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilter"
}-->

```json
{
  "criteria": {"@odata.type": "microsoft.graph.workbookFilterCriteria" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->