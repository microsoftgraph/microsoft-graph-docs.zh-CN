---
title: serviceHostedMediaConfig 资源类型
description: 远程承载的媒体。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 405f6b40260908d7492a3b02c8535588c8475ca8
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870087"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="1b2ba-103">serviceHostedMediaConfig 资源类型</span><span class="sxs-lookup"><span data-stu-id="1b2ba-103">serviceHostedMediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b2ba-104">远程承载的媒体。</span><span class="sxs-lookup"><span data-stu-id="1b2ba-104">The media that's hosted remotely.</span></span> <span data-ttu-id="1b2ba-105">这是从[mediaConfig](mediaconfig.md)继承的。</span><span class="sxs-lookup"><span data-stu-id="1b2ba-105">This is inherited from [mediaConfig](mediaconfig.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1b2ba-106">属性</span><span class="sxs-lookup"><span data-stu-id="1b2ba-106">Properties</span></span>

| <span data-ttu-id="1b2ba-107">属性</span><span class="sxs-lookup"><span data-stu-id="1b2ba-107">Property</span></span>                    | <span data-ttu-id="1b2ba-108">类型</span><span class="sxs-lookup"><span data-stu-id="1b2ba-108">Type</span></span>                                                        | <span data-ttu-id="1b2ba-109">说明</span><span class="sxs-lookup"><span data-stu-id="1b2ba-109">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="1b2ba-110">preFetchMedia</span><span class="sxs-lookup"><span data-stu-id="1b2ba-110">preFetchMedia</span></span>               | <span data-ttu-id="1b2ba-111">[mediaInfo](mediainfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="1b2ba-111">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="1b2ba-112">预回迁的介质列表。</span><span class="sxs-lookup"><span data-stu-id="1b2ba-112">The list of media to pre-fetch.</span></span>                   |
| <span data-ttu-id="1b2ba-113">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="1b2ba-113">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="1b2ba-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b2ba-114">Boolean</span></span>                                                     | <span data-ttu-id="1b2ba-115">从默认的音频组中删除自参与者。</span><span class="sxs-lookup"><span data-stu-id="1b2ba-115">Remove self participant from default audio group.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1b2ba-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1b2ba-116">JSON representation</span></span>

<span data-ttu-id="1b2ba-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b2ba-117">The following is a JSON representation of the resource.</span></span>

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
