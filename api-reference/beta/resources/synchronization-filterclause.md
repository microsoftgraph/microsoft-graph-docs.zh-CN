---
title: filterClause 资源类型
description: 代表单个断言候选对象必须满足的要求，并计算到`true`（对象满足断言） 或`false`（对象不满足声明）。
localization_priority: Normal
ms.openlocfilehash: 89807a6086f661388c8d5b1d5f82bfe973c3af39
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833857"
---
# <a name="filterclause-resource-type"></a>filterClause 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

代表单个断言候选对象必须满足的要求，并计算到`true`（对象满足断言） 或`false`（对象不满足声明）。

## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|operatorName|字符串|要应用于的源和目标操作数的运算符的名称。 必须是受支持运算符之一。 可以发现受支持的运算符。|
|sourceOperandName|字符串|源操作数 （正在测试的操作数） 的名称。 源操作数名称必须匹配源对象上的属性名称之一。|
|targetOperand|[filterOperand](synchronization-filteroperand.md)|将对照测试源操作数的值。|

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
<!-- {
  "type": "#page.annotation",
  "description": "filterClause resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
