---
title: attributeMappingSource 资源类型
description: 定义如何从源对象中提取 (或) 转换值。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 50443eb85ed87bce466e7842f46d0c457f28e216
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133236"
---
# <a name="attributemappingsource-resource-type"></a>attributeMappingSource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义如何从源对象中提取 (或) 转换值。 例如，它可以是一个从源对象的给定属性提取的简单值，也可以是基于多个源属性的更复杂的字符串连接/提取/替换表达式。

## <a name="properties"></a>属性

| 属性              | 类型                      | 说明               |
|:----------------------|:--------------------------|:--------------------------|
|表达式             |字符串                     |此 **attributeMappingSource 对象的等效表达式** 表示形式。|
|name                   |字符串                     |映射源的名称参数。 根据 **类型** 属性值，它可以是函数的名称、源属性的名称或要使用的常量值。 |
|parameters             |[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md) 集合 | 如果此对象代表函数，则列出函数参数。 参数由 **attributeMappingSource** 对象本身组成，允许使用复杂的表达式。 如果 **type** 不是 `Function` ，则此属性将为 null/空数组。 |
|type                   | 字符串                    |此属性映射源的类型。 可取值为：`Attribute`、`Constant`、`Function`。 默认值为“`Attribute`”。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingSource"
}-->

```json
{
  "expression": "String",
  "name": "String",
  "parameters": [{"@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair"}],
  "type": "String"
}
```

## <a name="json-examples"></a>JSON 示例

简单属性到属性映射

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingSource"
}-->

```json
{
    "expression": "[mail]",
    "name": "mail",
    "type": "Attribute"
}
```

从源属性提取前 8 个字符的表达式

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingSource"
}-->

```json
 {
    "expression": "Mid([userPrincipalName], 1, 8)",
    "name": "Mid",
    "parameters": [
        {
            "key": "source",
            "value": {
                "expression": "[userPrincipalName]",
                "name": "userPrincipalName",
                "parameters": [],
                "type": "Attribute"
            }
        },
        {
            "key": "start",
            "value": {
                "expression": "\"1\"",
                "name": "1",
                "parameters": [],
                "type": "Constant"
            }
        },
        {
            "key": "length",
            "value": {
                "expression": "\"8\"",
                "name": "8",
                "parameters": [],
                "type": "Constant"
            }
        }
    ],
    "type": "Function"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeMappingSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


