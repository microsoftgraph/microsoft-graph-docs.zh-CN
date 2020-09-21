---
title: serviceHostedMediaConfig 资源类型
description: 远程承载的媒体。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d006a4417401859c0c385f9537656993f985198d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023952"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="b8eb5-103">serviceHostedMediaConfig 资源类型</span><span class="sxs-lookup"><span data-stu-id="b8eb5-103">serviceHostedMediaConfig resource type</span></span>

<span data-ttu-id="b8eb5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8eb5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8eb5-105">远程承载的媒体。</span><span class="sxs-lookup"><span data-stu-id="b8eb5-105">The media that's hosted remotely.</span></span> <span data-ttu-id="b8eb5-106">这是从 [mediaConfig](mediaconfig.md)继承的。</span><span class="sxs-lookup"><span data-stu-id="b8eb5-106">This is inherited from [mediaConfig](mediaconfig.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b8eb5-107">属性</span><span class="sxs-lookup"><span data-stu-id="b8eb5-107">Properties</span></span>

| <span data-ttu-id="b8eb5-108">属性</span><span class="sxs-lookup"><span data-stu-id="b8eb5-108">Property</span></span>                    | <span data-ttu-id="b8eb5-109">类型</span><span class="sxs-lookup"><span data-stu-id="b8eb5-109">Type</span></span>                                                        | <span data-ttu-id="b8eb5-110">说明</span><span class="sxs-lookup"><span data-stu-id="b8eb5-110">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="b8eb5-111">preFetchMedia</span><span class="sxs-lookup"><span data-stu-id="b8eb5-111">preFetchMedia</span></span>               | <span data-ttu-id="b8eb5-112">[mediaInfo](mediainfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b8eb5-112">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="b8eb5-113">预回迁的介质列表。</span><span class="sxs-lookup"><span data-stu-id="b8eb5-113">The list of media to pre-fetch.</span></span>                   |
| <span data-ttu-id="b8eb5-114">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="b8eb5-114">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="b8eb5-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8eb5-115">Boolean</span></span>                                                     | <span data-ttu-id="b8eb5-116">从默认的音频组中删除自参与者。</span><span class="sxs-lookup"><span data-stu-id="b8eb5-116">Remove self participant from default audio group.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b8eb5-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b8eb5-117">JSON representation</span></span>

<span data-ttu-id="b8eb5-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8eb5-118">The following is a JSON representation of the resource.</span></span>

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


