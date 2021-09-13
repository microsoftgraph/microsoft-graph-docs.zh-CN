---
title: userFeedback 资源类型
description: userFeedback 类型。
ms.localizationpriority: medium
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 830b279c4021ec08677a4a5ebaf637bc73b7beaf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084662"
---
# <a name="userfeedback-resource-type"></a>userFeedback 资源类型

命名空间：microsoft.graph.callRecords

表示终结点提供的有关会话质量的反馈。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|rating|microsoft.graph.callRecords.userFeedbackRating|此终结点的用户提供的有关此会话质量的分级。 可取值为：`notRated`、`bad`、`poor`、`fair`、`good`、`excellent` 或 `unknownFutureValue`。|
|text|String|此终结点的用户为会话提供的反馈文本。|
|tokens|[microsoft.graph.callRecords.feedbackTokenSet](callrecords-feedbacktokenset.md)|此终结点的用户为会话提供的反馈令牌集。 这是一组布尔属性。 不应依赖属性名称，因为它们可能会根据提供给用户的令牌而更改。|

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
