---
title: filterClause 资源类型
description: 表示候选对象必须满足的单个断言, 并计算为`true` (object 满足断言) 或`false` (对象不满足断言)。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 83b9c68bd86f716b47a3ba3774022ff3ba520770
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007933"
---
# <a name="filterclause-resource-type"></a>filterClause 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示候选对象必须满足的单个断言, 并计算为`true` (object 满足断言) 或`false` (对象不满足断言)。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|operatorName|String|要应用于源和目标操作数的运算符的名称。 必须是受支持的运算符之一。 可以发现受支持的运算符。|
|sourceOperandName|String|源操作数的名称 (所测试的操作数)。 源操作数名称必须与源对象上的某个属性名称相匹配。|
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
