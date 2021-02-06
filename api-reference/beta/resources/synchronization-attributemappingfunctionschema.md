---
title: attributeMappingFunctionSchema 资源类型
description: 描述可在属性映射中使用的函数，以在同步期间转换值。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: a62d2d635504208fc8266e98add66a8503e3e4d2
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128741"
---
# <a name="attributemappingfunctionschema-resource-type"></a>attributeMappingFunctionSchema 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

描述可在属性映射中使用的函数 [，](synchronization-attributemapping.md) 以在同步期间转换值。

## <a name="methods"></a>方法

| 方法           | 返回类型    |Description|
|:---------------|:--------|:----------|
|[List](../api/synchronization-synchronizationschema-functions.md) | [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) 集合|列出支持的属性映射函数。|

## <a name="properties"></a>属性

| 属性                   | 类型                      | 说明    |
|:---------------------------|:-------------------------|:---------------|
|name                        |字符串                    |运算符名称。 |
|parameters                  |[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) 集合  |函数参数的集合。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingFunctionSchema"
}-->

```json
{
  "name": "String (identifier)",
  "parameters": [{"@odata.type": "microsoft.graph.attributeMappingParameterSchema"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeMappingFunctionSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


