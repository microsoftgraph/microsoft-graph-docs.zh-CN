---
title: attributeMappingSource 资源类型
description: '定义如何值应为源对象中提取 （或转换）。 例如，它可以是简单取自源对象上, 一个给定属性的值或它可以是字符串串联/提取/替换基于多个源属性更为复杂的表达式。 '
localization_priority: Normal
ms.openlocfilehash: 1d15cd82c0a58ac8bdd3ac5805abc166322f27fe
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510405"
---
# <a name="attributemappingsource-resource-type"></a>attributeMappingSource 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义如何值应为源对象中提取 （或转换）。 例如，它可以是简单取自源对象上, 一个给定属性的值或它可以是字符串串联/提取/替换基于多个源属性更为复杂的表达式。 

## <a name="properties"></a>属性

| 属性              | 类型                      | 说明               |
|:----------------------|:--------------------------|:--------------------------|
|表达式             |String                     |此**attributeMappingSource**对象的表达式等效表示形式。|
|name                   |String                     |映射源名称参数。 具体取决于**type**属性值，这可以是函数，源属性或用于以常量值的名称的名称。 |
|参数             |[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md)集合 | 如果该对象代表一个函数，列出函数参数。 参数包含**attributeMappingSource**对象本身，允许使用复杂的表达式。 如果**类型**不是`Function`，此属性将为空数组。 |
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

简单属性对属性映射

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

源属性中提取前 8 个字符的表达式

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
