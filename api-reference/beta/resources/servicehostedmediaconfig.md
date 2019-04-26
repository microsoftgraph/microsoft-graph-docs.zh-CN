---
title: serviceHostedMediaConfig 资源类型
description: serviceHostedMediaConfig 类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fbd59694940d6d0b3abea1a8d56bd426a3dfbb3a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343294"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="8ea75-103">serviceHostedMediaConfig 资源类型</span><span class="sxs-lookup"><span data-stu-id="8ea75-103">serviceHostedMediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ea75-104">serviceHostedMediaConfig 类型。</span><span class="sxs-lookup"><span data-stu-id="8ea75-104">The serviceHostedMediaConfig type.</span></span>

## <a name="properties"></a><span data-ttu-id="8ea75-105">属性</span><span class="sxs-lookup"><span data-stu-id="8ea75-105">Properties</span></span>

| <span data-ttu-id="8ea75-106">属性</span><span class="sxs-lookup"><span data-stu-id="8ea75-106">Property</span></span>                    | <span data-ttu-id="8ea75-107">类型</span><span class="sxs-lookup"><span data-stu-id="8ea75-107">Type</span></span>                                                        | <span data-ttu-id="8ea75-108">说明</span><span class="sxs-lookup"><span data-stu-id="8ea75-108">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="8ea75-109">preFetchMedia</span><span class="sxs-lookup"><span data-stu-id="8ea75-109">preFetchMedia</span></span>               | <span data-ttu-id="8ea75-110">[mediaInfo](mediainfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="8ea75-110">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="8ea75-111">预回迁的介质列表。</span><span class="sxs-lookup"><span data-stu-id="8ea75-111">The list of media to pre-fetch.</span></span>                   |
| <span data-ttu-id="8ea75-112">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="8ea75-112">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="8ea75-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ea75-113">Boolean</span></span>                                                     | <span data-ttu-id="8ea75-114">从默认的音频组中删除自参与者。</span><span class="sxs-lookup"><span data-stu-id="8ea75-114">Remove self participant from default audio group.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8ea75-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8ea75-115">JSON representation</span></span>

<span data-ttu-id="8ea75-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8ea75-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "preFetchMedia"
  ],
  "baseType": "microsoft.graph.mediaConfig",
  "@odata.type": "microsoft.graph.serviceHostedMediaConfig"
}-->
```json
{
  "preFetchMedia": [ { "@odata.type": "microsoft.graph.mediaInfo" } ],
  "removeFromDefaultAudioGroup": true
}
```

## <a name="example"></a><span data-ttu-id="8ea75-117">示例</span><span class="sxs-lookup"><span data-stu-id="8ea75-117">Example</span></span>

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
  "suppressions": []
}
-->
