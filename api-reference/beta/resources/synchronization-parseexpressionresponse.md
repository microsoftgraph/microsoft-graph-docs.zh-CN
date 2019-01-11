---
title: parseExpressionResponse 资源类型
description: '代表来自响应[synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)操作。'
localization_priority: Normal
ms.openlocfilehash: 550a46b0c27c2ca8d2d4c01baa975d8a204546f2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832947"
---
# <a name="parseexpressionresponse-resource-type"></a>parseExpressionResponse 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

代表来自响应[synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)操作。

## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|error|odata.error|错误详细信息，如果表达式评估导致出错。|
|evaluationResult|String 集合|无条件表达式的计算值的集合。|
|evaluationSucceeded|布尔|`true`评估是否成功。|
|parsedExpression|[attributeMappingSource](synchronization-attributemappingsource.md)|一个表示已分析的表达式[attributeMappingSource](synchronization-attributemappingsource.md)对象。|
|parsingSucceeded|布尔|`true`如果成功解析的表达式。|

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
<!-- {
  "type": "#page.annotation",
  "description": "parseExpressionResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
