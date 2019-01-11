---
title: filterGroup 资源类型
description: 定义一对象视为范围内必须满足的子句。 对象属于组的范围内 (组计算为`true`) 才组的所有子句都计算为`true`。
localization_priority: Normal
ms.openlocfilehash: 174c02518069e949c49887d9e21e778e8455509a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836111"
---
# <a name="filtergroup-resource-type"></a>filterGroup 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

定义一对象视为范围内必须满足的子句。 对象属于组的范围内 (组计算为`true`) 才组的所有子句都计算为`true`。

## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|子句|[filterClause](synchronization-filterclause.md)集合|筛选此组的子句 （条件）。 组中的所有子句都必须满足顺序筛选器组计算结果为`true`。|
|name|字符串|可读的筛选器组的名称。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterGroup"
}-->

```json
{
  "clauses": [{"@odata.type": "microsoft.graph.filterClause"}],
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "filterGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
