---
title: filterClause 资源类型
description: 表示候选对象必须满足的单个断言。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 91cc7f85dc4c42f806be5e365f21adb0d5e972fc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968367"
---
# <a name="filterclause-resource-type"></a>filterClause 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示候选对象必须满足的单个断言，并计算为 `true` (对象满足断言) 或 `false` (对象不满足断言) 。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|operatorName|String|要应用于源和目标操作数的运算符的名称。 必须是受支持的运算符之一。 可以发现受支持的运算符。|
|sourceOperandName|String| (所测试的操作数) 的源操作数的名称。 源操作数名称必须与源对象上的某个属性名称相匹配。|
|targetOperand|[filterOperand](synchronization-filteroperand.md)|将对源操作数进行测试的值。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterClause"
}-->

```json
{
  "operatorName": "String",
  "sourceOperandName": "String",
  "targetOperand": {"@odata.type": "microsoft.graph.filterOperand"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filterClause resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


