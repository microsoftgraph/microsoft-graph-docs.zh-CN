---
title: parseExpressionResponse 资源类型
description: '代表来自响应[synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)操作。'
localization_priority: Normal
ms.openlocfilehash: f8ea708468e1e580693b2bd0e6f0e7f3494996f0
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641055"
---
# <a name="parseexpressionresponse-resource-type"></a>parseExpressionResponse 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表来自响应[synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)操作。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|error|odata.error|错误详细信息，如果表达式评估导致出错。|
|evaluationResult|String collection|无条件表达式的计算值的集合。|
|evaluationSucceeded|布尔值|`true`评估是否成功。|
|parsedExpression|[attributeMappingSource](synchronization-attributemappingsource.md)|一个表示已分析的表达式[attributeMappingSource](synchronization-attributemappingsource.md)对象。|
|parsingSucceeded|布尔值|`true`如果成功解析的表达式。|

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-parseexpressionresponse.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
