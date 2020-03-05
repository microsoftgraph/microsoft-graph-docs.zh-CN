---
title: parseExpressionResponse 资源类型
description: 表示来自[synchronizationSchema： parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)操作的响应。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c752d5c021418dd4a3154a539a61c6ab3bae8a61
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520133"
---
# <a name="parseexpressionresponse-resource-type"></a>parseExpressionResponse 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示来自[parseExpression](../api/synchronization-synchronizationschema-parseexpression.md)操作的响应。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|error|publicError|如果表达式求值导致错误，则为错误详细信息。|
|evaluationResult|String 集合|由表达式的计算产生的值的集合。|
|evaluationSucceeded|布尔|`true`如果评估成功。|
|parsedExpression|[attributeMappingSource](synchronization-attributemappingsource.md)|一个代表已分析的表达式的[attributeMappingSource](synchronization-attributemappingsource.md)对象。|
|parsingSucceeded|布尔|`true`如果表达式已成功分析。|

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
