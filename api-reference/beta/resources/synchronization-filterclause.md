---
title: filterClause 资源类型
description: 表示候选对象必须满足的单个断言。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: fc633f6e25373713679da30a5b319ab8ae99fb04
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131920"
---
# <a name="filterclause-resource-type"></a>filterClause 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示候选对象必须满足的单个断言，并计算为 (对象满足断言) 或 (对象不满足断言 `true` `false`) 。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|operatorName|字符串|要应用于源操作数和目标操作数的运算符的名称。 必须是受支持的运算符之一。 可以发现支持的运算符。|
|sourceOperandName|字符串|要测试 (操作数的源操作数) 。 源操作数名称必须与源对象上的某个属性名称匹配。|
|targetOperand|[filterOperand](synchronization-filteroperand.md)|将针对其测试源操作数值。|

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


