---
title: filterGroup 资源类型
description: 定义要在范围中考虑对象必须满足的一组子句。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6e7933bf2fef6240dd0dc53d7da975074225aa30
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217888"
---
# <a name="filtergroup-resource-type"></a>filterGroup 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义要在范围中考虑对象必须满足的一组子句。 仅当组的所有子句都计算为`true` `true`时，才会在组的作用域中考虑对象（组的计算结果为）。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|and|[filterClause](synchronization-filterclause.md)集合|此组的筛选子句（条件）。 必须满足组中的所有子句，筛选器组才能进行计算`true`。|
|name|字符串|易于阅读的筛选器组名称。|

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
<!--
{
  "type": "#page.annotation",
  "description": "filterGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
