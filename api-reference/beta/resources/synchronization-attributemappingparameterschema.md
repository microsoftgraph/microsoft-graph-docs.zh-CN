---
title: attributeMappingParameterSchema 资源类型
description: 描述在 attributeMappingFunctionSchema 中使用的单个参数。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d8624851d37f475df66ec51f1951ebbbe1ea97a8
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620267"
---
# <a name="attributemappingparameterschema-resource-type"></a>attributeMappingParameterSchema 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述在[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)中使用的单个参数。

## <a name="properties"></a>属性

| 属性                   | 类型                      | 说明    |
|:---------------------------|:-------------------------|:---------------|
|allowMultipleOccurrences    |Boolean                   |给定参数可多次提供 (例如, `Concatenate(string,string,...)`函数中的多个输入字符串)。 |
|name                        |String                    |参数名称。 |
|必需                    |Boolean                   |`true`如果参数是必需的;否则`false`为。 |
|type                        |String                    |可取值为：`Boolean`、`Binary`、`Reference`、`Integer` 或 `String`。 默认值为 `String`。|

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
