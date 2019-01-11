---
title: filterOperatorSchema 资源类型
description: 介绍可用于筛选器运算符。
localization_priority: Normal
ms.openlocfilehash: 0d26fb58b77369b70ab185fa8ad5214d6b6c1e71
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848277"
---
# <a name="filteroperatorschema-resource-type"></a>filterOperatorSchema 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

介绍可用于[筛选器](synchronization-filter.md)运算符。

## <a name="properties"></a>属性

| 属性                   | 类型                      | Description    |
|:---------------------------|:--------------------------|:---------------|
|实参数量                       |字符串          |实参运算符的数量。 可取值为：`Binary`、`Unary`。 默认值是`Binary`。|
|multivaluedComparisonType   |scopeOperatorMultiValuedComparisonType          |可取值为：`All`、`Any`。 仅适用于多值属性。 `All`所有的值必须满足条件的方法。 `Any`至少一个值必须满足条件的方法。 默认值是`All`。|
|name                        |字符串                     |运算符名称。 |
|supportedAttributeTypes     |String 集合         |属性类型支持的运算符。 可取值为：`Boolean`、`Binary`、`Reference`、`Integer`、`String`。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterOperatorSchema"
}-->

```json
{
  "arity": "String",
  "multivaluedComparisonType": "String",
  "name": "String",
  "supportedAttributeTypes": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "filterOperatorSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
