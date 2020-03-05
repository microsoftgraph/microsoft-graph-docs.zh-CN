---
title: attributeMappingParameterSchema 资源类型
description: 描述在 attributeMappingFunctionSchema 中使用的单个参数。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d4415c6ece2fc9095070eb888ad4bd7bba583d54
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520238"
---
# <a name="attributemappingparameterschema-resource-type"></a>attributeMappingParameterSchema 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述在[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)中使用的单个参数。

## <a name="properties"></a>属性

| 属性                   | 类型                      | 说明    |
|:---------------------------|:-------------------------|:---------------|
|allowMultipleOccurrences    |布尔                   |给定参数可多次提供（例如， `Concatenate(string,string,...)`函数中的多个输入字符串）。 |
|name                        |String                    |参数名称。 |
|必需                    |布尔                   |`true`如果参数是必需的;否则`false`为。 |
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
