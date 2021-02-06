---
title: parseExpressionResponse 资源类型
description: 表示 synchronizationSchema： parseExpression 操作的响应。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: e564cb2ad7a80c91fec7d6298254fa19bde4537c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133145"
---
# <a name="parseexpressionresponse-resource-type"></a>parseExpressionResponse 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [parseExpression 操作的响应](../api/synchronization-synchronizationschema-parseexpression.md) 。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|error|publicError|如果表达式计算导致错误，错误详细信息。|
|evaluationResult|字符串集合|由表达式的计算生成的值集合。|
|evaluationSucceeded|Boolean|`true` 评估是否成功。|
|parsedExpression|[attributeMappingSource](synchronization-attributemappingsource.md)|一个代表已分析表达式的 [attributeMappingSource](synchronization-attributemappingsource.md) 对象。|
|parsingSucceeded|Boolean|`true` 是否成功分析表达式。|

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


