---
title: serviceHostedMediaConfig 资源类型
description: ServiceHostedMediaConfig 类型。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: ec2ff24ef0bb45a9b49ecf2d0dc5e7419318b5af
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828698"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="e125f-103">serviceHostedMediaConfig 资源类型</span><span class="sxs-lookup"><span data-stu-id="e125f-103">serviceHostedMediaConfig resource type</span></span>

> <span data-ttu-id="e125f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e125f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e125f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e125f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e125f-106">ServiceHostedMediaConfig 类型。</span><span class="sxs-lookup"><span data-stu-id="e125f-106">The serviceHostedMediaConfig type.</span></span>

## <a name="properties"></a><span data-ttu-id="e125f-107">属性</span><span class="sxs-lookup"><span data-stu-id="e125f-107">Properties</span></span>

| <span data-ttu-id="e125f-108">属性</span><span class="sxs-lookup"><span data-stu-id="e125f-108">Property</span></span>                    | <span data-ttu-id="e125f-109">类型</span><span class="sxs-lookup"><span data-stu-id="e125f-109">Type</span></span>                                                        | <span data-ttu-id="e125f-110">Description</span><span class="sxs-lookup"><span data-stu-id="e125f-110">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="e125f-111">preFetchMedia</span><span class="sxs-lookup"><span data-stu-id="e125f-111">preFetchMedia</span></span>               | <span data-ttu-id="e125f-112">[mediaInfo](mediainfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="e125f-112">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="e125f-113">媒体预取列表。</span><span class="sxs-lookup"><span data-stu-id="e125f-113">The list of media to pre-fetch.</span></span>                   |
| <span data-ttu-id="e125f-114">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="e125f-114">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="e125f-115">布尔</span><span class="sxs-lookup"><span data-stu-id="e125f-115">Boolean</span></span>                                                     | <span data-ttu-id="e125f-116">从默认音频组中删除自我参与者。</span><span class="sxs-lookup"><span data-stu-id="e125f-116">Remove self participant from default audio group.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e125f-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e125f-117">JSON representation</span></span>

<span data-ttu-id="e125f-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e125f-118">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="e125f-119">示例</span><span class="sxs-lookup"><span data-stu-id="e125f-119">Example</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "serviceHostedMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
