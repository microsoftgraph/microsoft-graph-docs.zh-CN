---
title: serviceHostedMediaConfig 资源类型
description: ServiceHostedMediaConfig 类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2ab19f992dd7fac48844cd46a0600a0242517709
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642224"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="37946-103">serviceHostedMediaConfig 资源类型</span><span class="sxs-lookup"><span data-stu-id="37946-103">serviceHostedMediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37946-104">ServiceHostedMediaConfig 类型。</span><span class="sxs-lookup"><span data-stu-id="37946-104">The serviceHostedMediaConfig type.</span></span>

## <a name="properties"></a><span data-ttu-id="37946-105">属性</span><span class="sxs-lookup"><span data-stu-id="37946-105">Properties</span></span>

| <span data-ttu-id="37946-106">属性</span><span class="sxs-lookup"><span data-stu-id="37946-106">Property</span></span>                    | <span data-ttu-id="37946-107">类型</span><span class="sxs-lookup"><span data-stu-id="37946-107">Type</span></span>                                                        | <span data-ttu-id="37946-108">说明</span><span class="sxs-lookup"><span data-stu-id="37946-108">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="37946-109">preFetchMedia</span><span class="sxs-lookup"><span data-stu-id="37946-109">preFetchMedia</span></span>               | <span data-ttu-id="37946-110">[mediaInfo](mediainfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="37946-110">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="37946-111">媒体预取列表。</span><span class="sxs-lookup"><span data-stu-id="37946-111">The list of media to pre-fetch.</span></span>                   |
| <span data-ttu-id="37946-112">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="37946-112">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="37946-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="37946-113">Boolean</span></span>                                                     | <span data-ttu-id="37946-114">从默认音频组中删除自我参与者。</span><span class="sxs-lookup"><span data-stu-id="37946-114">Remove self participant from default audio group.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="37946-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="37946-115">JSON representation</span></span>

<span data-ttu-id="37946-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="37946-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "preFetchMedia"
  ],
  "@odata.type": "microsoft.graph.serviceHostedMediaConfig"
}-->
```json
{
  "preFetchMedia": [ { "@odata.type": "#microsoft.graph.mediaInfo" } ],
  "removeFromDefaultAudioGroup": true
}
```

## <a name="example"></a><span data-ttu-id="37946-117">示例</span><span class="sxs-lookup"><span data-stu-id="37946-117">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.serviceHostedMediaConfig"
}-->
```json
{
  "preFetchMedia": [
    {
      "uri": "https://cdn.contoso.com/beep.wav",
      "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
    },
    {
      "uri": "https://cdn.contoso.com/cool.wav",
      "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088F"
    }
  ],
  "removeFromDefaultAudioGroup": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "serviceHostedMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/servicehostedmediaconfig.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
