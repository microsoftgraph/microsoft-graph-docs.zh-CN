---
title: TableSort 资源类型
description: 管理对 Table 对象的排序操作。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 612e0cb7d59011f04ae992f80119fc1da572b582
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511742"
---
# <a name="tablesort-resource-type"></a>TableSort 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

管理对 Table 对象的排序操作。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|获取 TableSort | [TableSort](tablesort.md) |读取 tableSort 对象的属性和关系。|
|[应用](../api/tablesort-apply.md)|无|执行排序操作。|
|[清除](../api/tablesort-clear.md)|None|清除表上的当前排序。尽管这不能修改表的排序，但它会清除标题按钮的状态。|
|[重新应用](../api/tablesort-reapply.md)|无|对表重新应用当前的排序参数。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|matchCase|布尔|表示最后一次对表进行排序时大小写是否有影响。只读。|
|方法|string|表示最后一次对表排序所使用的中文字符排序方法。可能的值是：`PinYin`、`StrokeCount`。只读。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|fields|[SortField](sortfield.md)|表示最后一次对表排序所使用的当前条件。只读。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tableSort"
}-->

```json
{
  "matchCase": true,
  "method": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/tablesort.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
