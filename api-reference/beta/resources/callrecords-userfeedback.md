---
title: userFeedback 资源类型
description: UserFeedback 类型。
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5bc315bcb1cd780cb725b2586b8e02e109aa2868
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601501"
---
# <a name="userfeedback-resource-type"></a>userFeedback 资源类型

命名空间：microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表用户提供的有关会话质量的终结点的反馈。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|评估|callRecords。 userFeedbackRating|此终结点的用户提供的有关此会话的质量的分级。 可取值为：`notRated`、`bad`、`poor`、`fair`、`good`、`excellent` 或 `unknownFutureValue`。|
|text|String|此终结点的用户提供的反馈文本，用于会话。|
|等级|[callRecords。 feedbackTokenSet](callrecords-feedbacktokenset.md)|此终结点的用户为会话提供的一组反馈令牌。 这是一组布尔属性。 属性名称不应依赖，因为它们可能会根据向用户提供的令牌而发生变化。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.userFeedback",
  "baseType": null
}-->

```json
{
  "rating": "String",
  "text": "String",
  "tokens": {"@odata.type": "microsoft.graph.callRecords.feedbackTokenSet"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userFeedback resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

