---
title: stringKeyAttributeMappingSourceValuePair 资源类型
description: 表示键值对, 其中键是字符串, 值为 attributeMappingSource。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e513ffd0ba32780ae1a489155999716b3a7499d2
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620435"
---
# <a name="stringkeyattributemappingsourcevaluepair-resource-type"></a>stringKeyAttributeMappingSourceValuePair 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示键值对, 其中键是字符串, 值为[attributeMappingSource](synchronization-attributemappingsource.md)。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|Key|String|参数的名称。|
|值|[attributeMappingSource](synchronization-attributemappingsource.md)|参数的值。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair"
}-->

```json
{
  "key": "String",
  "value": {"@odata.type": "microsoft.graph.attributeMappingSource"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyAttributeMappingSourceValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
