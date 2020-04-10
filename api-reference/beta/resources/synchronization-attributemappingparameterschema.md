---
title: attributeMappingParameterSchema 资源类型
description: 描述在 attributeMappingFunctionSchema 中使用的单个参数。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 12f1a38340b4c341d65930000c22a6cd2daeb567
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219170"
---
# <a name="attributemappingparameterschema-resource-type"></a>attributeMappingParameterSchema 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述在[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)中使用的单个参数。

## <a name="properties"></a>属性

| 属性                   | 类型                      | 说明    |
|:---------------------------|:-------------------------|:---------------|
|allowMultipleOccurrences    |Boolean                   |给定参数可多次提供（例如， `Concatenate(string,string,...)`函数中的多个输入字符串）。 |
|name                        |String                    |参数名称。 |
|必需                    |Boolean                   |`true`如果参数是必需的;否则`false`为。 |
|type                        |字符串                    |可取值为：`Boolean`、`Binary`、`Reference`、`Integer` 或 `String`。 默认值为 `String`。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingParameterSchema"
}-->

```json
{
  "allowMultipleOccurrences": "Boolean",
  "name": "String",
  "required": "Boolean",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeMappingParameterSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
