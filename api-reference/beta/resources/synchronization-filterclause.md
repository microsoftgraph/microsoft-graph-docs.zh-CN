---
title: filterClause 资源类型
description: 代表单个断言候选对象必须满足的要求，并计算到`true`（对象满足断言） 或`false`（对象不满足声明）。
ms.openlocfilehash: 0861324849f224c4e750f0c7b926464280b9a377
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042697"
---
# <a name="filterclause-resource-type"></a>filterClause 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

代表单个断言候选对象必须满足的要求，并计算到`true`（对象满足断言） 或`false`（对象不满足声明）。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
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