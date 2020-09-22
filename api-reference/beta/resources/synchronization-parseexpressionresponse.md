---
title: parseExpressionResponse 资源类型
description: 表示来自 synchronizationSchema： parseExpression 操作的响应。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9bd675b079f42856e85f54b7da84a091a0f57f4f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988812"
---
# <a name="parseexpressionresponse-resource-type"></a>parseExpressionResponse 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示来自 [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) 操作的响应。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|error|publicError|如果表达式求值导致错误，则为错误详细信息。|
|evaluationResult|String collection|由表达式的计算产生的值的集合。|
|evaluationSucceeded|Boolean|`true` 如果评估成功。|
|parsedExpression|[attributeMappingSource](synchronization-attributemappingsource.md)|一个代表已分析的表达式的 [attributeMappingSource](synchronization-attributemappingsource.md) 对象。|
|parsingSucceeded|Boolean|`true` 如果表达式已成功分析。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.parseExpressionResponse"
}-->

```json
{
  "error": {"@odata.type": "microsoft.graph.publicError"},
  "evaluationResult": ["String"],
  "evaluationSucceeded": true,
  "parsedExpression": {"@odata.type": "microsoft.graph.attributeMappingSource"},
  "parsingSucceeded": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "parseExpressionResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


