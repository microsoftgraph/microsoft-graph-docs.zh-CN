---
title: feedbackTokenSet 资源类型
description: FeedbackTokenSet 类型
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 77455a28333b6b1f94196397b329442e1d0ecb60
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071525"
---
# <a name="feedbacktokenset-resource-type"></a><span data-ttu-id="44fa5-103">feedbackTokenSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="44fa5-103">feedbackTokenSet resource type</span></span>

<span data-ttu-id="44fa5-104">命名空间：microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="44fa5-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44fa5-105">这是一 _种开放类型_ ，表示此终结点的用户为会话提供的一组反馈令牌。</span><span class="sxs-lookup"><span data-stu-id="44fa5-105">This is an _open type_ that represents the set of feedback tokens provided by the user of this endpoint for the Session.</span></span> <span data-ttu-id="44fa5-106">这是一组布尔属性。</span><span class="sxs-lookup"><span data-stu-id="44fa5-106">This is a set of Boolean properties.</span></span> <span data-ttu-id="44fa5-107">属性名称不应依赖，因为它们可能会根据向用户提供的令牌而发生变化。</span><span class="sxs-lookup"><span data-stu-id="44fa5-107">The property names should not be relied upon since they may change depending on what tokens are offered to the user.</span></span>

## <a name="properties"></a><span data-ttu-id="44fa5-108">属性</span><span class="sxs-lookup"><span data-stu-id="44fa5-108">Properties</span></span>

<span data-ttu-id="44fa5-109">将不会记录显式属性名称，因为反馈令牌名称可能会更改，因此这是 [开放类型](https://docs.microsoft.com/aspnet/web-api/overview/odata-support-in-aspnet-web-api/odata-v4/use-open-types-in-odata-v4)。</span><span class="sxs-lookup"><span data-stu-id="44fa5-109">Explicit property names will not be documented since the feedback token names can change, hence this is an [open type](https://docs.microsoft.com/aspnet/web-api/overview/odata-support-in-aspnet-web-api/odata-v4/use-open-types-in-odata-v4).</span></span>

## <a name="json-representation"></a><span data-ttu-id="44fa5-110">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="44fa5-110">JSON representation</span></span>

<span data-ttu-id="44fa5-111">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44fa5-111">The following is a JSON representation of the resource.</span></span>

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

