---
title: filterGroup 资源类型
description: 定义对象必须满足的一组子句才能在范围中考虑。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 6338ae4b02b79d1512d5e9f695a69155197e2f4a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131913"
---
# <a name="filtergroup-resource-type"></a>filterGroup 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义对象必须满足的一组子句才能在范围中考虑。 在组范围内考虑对象 (只有在组的所有子句都计算为) 计算组时，才计算为一 `true` 个对象 `true` 。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|clauses|[filterClause](synchronization-filterclause.md) 集合|Filter 子句 (此) 条件。 必须满足组内的所有子句，筛选器组才能计算结果 `true` 。|
|name|字符串|筛选器组的可读名称。|

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


