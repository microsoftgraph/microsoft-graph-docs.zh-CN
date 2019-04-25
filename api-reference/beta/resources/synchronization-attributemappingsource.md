---
title: attributeMappingSource 资源类型
description: '定义应如何从源对象提取 (或转换) 值。 例如, 它可以是从源对象的给定属性中获取的简单值, 也可以是基于多个源属性的字符串串联/提取/替换的更复杂表达式。 '
localization_priority: Normal
ms.openlocfilehash: 1d15cd82c0a58ac8bdd3ac5805abc166322f27fe
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582135"
---
# <a name="attributemappingsource-resource-type"></a>attributeMappingSource 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义应如何从源对象提取 (或转换) 值。 例如, 它可以是从源对象的给定属性中获取的简单值, 也可以是基于多个源属性的字符串串联/提取/替换的更复杂表达式。 

## <a name="properties"></a>属性

| 属性              | 类型                      | 说明               |
|:----------------------|:--------------------------|:--------------------------|
|表达式             |String                     |此**attributeMappingSource**对象的等效表达式表示形式。|
|name                   |String                     |映射源的 Name 参数。 根据**type**属性值, 这可以是函数的名称、源属性的名称或要使用的常数值。 |
|parameters             |[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md)集合 | 如果此对象代表函数, 则列出函数参数。 参数由**attributeMappingSource**对象本身组成, 从而允许复杂的表达式。 如果**type**不`Function`是, 则此属性将为 null/空数组。 |
|type                   | String                    |此属性映射源的类型。 可取值为：`Attribute`、`Constant`、`Function`。 默认值为 `Attribute`。| 

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

属性映射的简单属性

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

从 source 属性提取前8个字符的表达式

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributemappingsource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
