---
title: userFeedback 资源类型
description: userFeedback 类型。
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4f38484219f33432aa5f4c215869c5f6df33aba133d38bcc79ce4f52a28eb2c1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180885"
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
