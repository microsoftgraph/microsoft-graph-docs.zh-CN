---
title: filterOperatorSchema 资源类型
description: 介绍可在筛选器中使用的运算符。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2e80b80a7f37af8b86dfd3925fe268dba89cea17
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217810"
---
# <a name="filteroperatorschema-resource-type"></a>filterOperatorSchema 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

介绍可在[筛选器](synchronization-filter.md)中使用的运算符。

## <a name="properties"></a>属性

| 属性                   | 类型                      | 说明    |
|:---------------------------|:--------------------------|:---------------|
|源语言                       |字符串          |运算符的 Arity。 可取值为：`Binary`、`Unary`。 默认值为`Binary`。|
|multivaluedComparisonType   |scopeOperatorMultiValuedComparisonType          |可取值为：`All`、`Any`。 仅适用于多值属性。 `All`表示所有值都必须满足条件。 `Any`表示必须至少有一个值满足条件。 默认值为`All`。|
|name                        |字符串                     |运算符名称。 |
|supportedAttributeTypes     |String collection         |运算符支持的属性类型。 可取值为：`Boolean`、`Binary`、`Reference`、`Integer`、`String`。|

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
<!--
{
  "type": "#page.annotation",
  "description": "filterOperatorSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
