---
title: feedbackTokenSet 资源类型
description: feedbackTokenSet 类型
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 054b77c64f61bd100db45ce6ed83772fd6e1fd2c0d502a4e6f578058ec8f097f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54205932"
---
# <a name="feedbacktokenset-resource-type"></a>feedbackTokenSet 资源类型

命名空间：microsoft.graph.callRecords

这是一 _个开放_ 类型，表示此终结点的用户为会话提供的反馈令牌集。 这是一组布尔属性。 不应依赖属性名称，因为它们可能会根据提供给用户的令牌而更改。

## <a name="properties"></a>属性

由于反馈令牌名称可以更改，因此不会记录显式属性名称，因此这是一个 [开放类型](/aspnet/web-api/overview/odata-support-in-aspnet-web-api/odata-v4/use-open-types-in-odata-v4)。

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