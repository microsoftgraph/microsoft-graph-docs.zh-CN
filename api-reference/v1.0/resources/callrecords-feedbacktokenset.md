---
title: feedbackTokenSet 资源类型
description: FeedbackTokenSet 类型
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 307a50c7a29be3857ec1b6b2addf2fafe2189323
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491947"
---
# <a name="feedbacktokenset-resource-type"></a>feedbackTokenSet 资源类型

命名空间：microsoft.graph.callRecords

这是一_种开放类型_，表示此终结点的用户为会话提供的一组反馈令牌。 这是一组布尔属性。 属性名称不应依赖，因为它们可能会根据向用户提供的令牌而发生变化。

## <a name="properties"></a>属性

将不会记录显式属性名称，因为反馈令牌名称可能会更改，因此这是[开放类型](https://docs.microsoft.com/aspnet/web-api/overview/odata-support-in-aspnet-web-api/odata-v4/use-open-types-in-odata-v4)。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.feedbackTokenSet",
  "baseType": null
}-->

```json
{
  "DistortedSpeech": true,
  "ElectronicFeedback": false,
  "BackgroundNoise": true,
  "MuffledSpeech": true,
  "Echo": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "feedbackTokenSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->