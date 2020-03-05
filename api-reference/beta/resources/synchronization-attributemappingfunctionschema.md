---
title: attributeMappingFunctionSchema 资源类型
description: 介绍可在属性映射中用于在同步期间转换值的函数。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 195f8e11737d2f9ae48675cdb7a7046869090e19
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520245"
---
# <a name="attributemappingfunctionschema-resource-type"></a>attributeMappingFunctionSchema 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

介绍可在[属性映射](synchronization-attributemapping.md)中用于在同步期间转换值的函数。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[List](../api/synchronization-synchronizationschema-functions.md) | [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)集合|列出受支持的属性映射函数。|

## <a name="properties"></a>属性

| 属性                   | 类型                      | 说明    |
|:---------------------------|:-------------------------|:---------------|
|name                        |String                    |运算符名称。 |
|parameters                  |[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md)集合  |函数参数的集合。|

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
