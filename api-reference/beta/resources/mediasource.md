---
author: MarcMroz
description: mediaSource 资源包含有关媒体源的元数据 (驱动器项) 元数据。
title: mediaSource 资源类型
localization_priority: Normal
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: c0b2f93095d7e7a4b9176073cc8688b5eb473cd3
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236309"
---
# <a name="mediasource-resouce-type"></a><span data-ttu-id="3dfc9-103">mediaSource 资源类型</span><span class="sxs-lookup"><span data-stu-id="3dfc9-103">mediaSource resouce type</span></span>

<span data-ttu-id="3dfc9-104">**mediaSource** 资源包含有关媒体源的元数据 (驱动器项) 元数据。</span><span class="sxs-lookup"><span data-stu-id="3dfc9-104">The **mediaSource** resource contains metadata about the source of media (audio or video) drive item.</span></span>

<span data-ttu-id="3dfc9-105">可用于 [driveItem][item-resource] 资源的媒体属性。</span><span class="sxs-lookup"><span data-stu-id="3dfc9-105">It is available on the media property of [driveItem][item-resource] resources.</span></span>

## <a name="properties"></a><span data-ttu-id="3dfc9-106">属性</span><span class="sxs-lookup"><span data-stu-id="3dfc9-106">Properties</span></span>

| <span data-ttu-id="3dfc9-107">属性</span><span class="sxs-lookup"><span data-stu-id="3dfc9-107">Property</span></span>                 | <span data-ttu-id="3dfc9-108">类型</span><span class="sxs-lookup"><span data-stu-id="3dfc9-108">Type</span></span>                       | <span data-ttu-id="3dfc9-109">说明</span><span class="sxs-lookup"><span data-stu-id="3dfc9-109">Description</span></span>                                                                                      |
| :----------------------- | :------------------------  | :----------------------------------------------------------------------------------------------- |
| <span data-ttu-id="3dfc9-110">**contentCategory**</span><span class="sxs-lookup"><span data-stu-id="3dfc9-110">**contentCategory**</span></span>      | <span data-ttu-id="3dfc9-111">mediaSourceContentCategory</span><span class="sxs-lookup"><span data-stu-id="3dfc9-111">mediaSourceContentCategory</span></span> | <span data-ttu-id="3dfc9-112">指示媒体内容类别的枚举值。</span><span class="sxs-lookup"><span data-stu-id="3dfc9-112">Enumeration value that indicates the media content category.</span></span>                                     |

### <a name="mediasourcecontentcategory-values"></a><span data-ttu-id="3dfc9-113">mediaSourceContentCategory 值</span><span class="sxs-lookup"><span data-stu-id="3dfc9-113">mediaSourceContentCategory values</span></span>

| <span data-ttu-id="3dfc9-114">值</span><span class="sxs-lookup"><span data-stu-id="3dfc9-114">Value</span></span>               | <span data-ttu-id="3dfc9-115">说明</span><span class="sxs-lookup"><span data-stu-id="3dfc9-115">Description</span></span>                                         |
|:------------------- |:----------------------------------------------------|
| <span data-ttu-id="3dfc9-116">meeting</span><span class="sxs-lookup"><span data-stu-id="3dfc9-116">meeting</span></span>             | <span data-ttu-id="3dfc9-117">媒体是会议。</span><span class="sxs-lookup"><span data-stu-id="3dfc9-117">The media is a meeting.</span></span>                             |
| <span data-ttu-id="3dfc9-118">liveStream</span><span class="sxs-lookup"><span data-stu-id="3dfc9-118">liveStream</span></span>          | <span data-ttu-id="3dfc9-119">媒体是实时流。</span><span class="sxs-lookup"><span data-stu-id="3dfc9-119">The media is a live stream.</span></span>                         |
| <span data-ttu-id="3dfc9-120">presentation</span><span class="sxs-lookup"><span data-stu-id="3dfc9-120">presentation</span></span>        | <span data-ttu-id="3dfc9-121">媒体是演示文稿。</span><span class="sxs-lookup"><span data-stu-id="3dfc9-121">The media is a presentation.</span></span>                        |
| <span data-ttu-id="3dfc9-122">screenRecording</span><span class="sxs-lookup"><span data-stu-id="3dfc9-122">screenRecording</span></span>     | <span data-ttu-id="3dfc9-123">媒体是屏幕录制。</span><span class="sxs-lookup"><span data-stu-id="3dfc9-123">The media is a screen recording.</span></span>                    |
| <span data-ttu-id="3dfc9-124">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="3dfc9-124">unknownFutureValue</span></span>  | <span data-ttu-id="3dfc9-125">用于将来兼容性的标记值。</span><span class="sxs-lookup"><span data-stu-id="3dfc9-125">Marker value for future compatibility.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="3dfc9-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3dfc9-126">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "contentCategory"
  ],
  "@odata.type": "microsoft.graph.mediaSource"
}-->

```json
{
  "contentCategory" : "string"
}
```

## <a name="see-also"></a><span data-ttu-id="3dfc9-127">另请参阅</span><span class="sxs-lookup"><span data-stu-id="3dfc9-127">See also</span></span>

<span data-ttu-id="3dfc9-128">有关 driveItem 上 Facet 的信息，请参阅 [driveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="3dfc9-128">For more information about the facets on a driveItem, see [driveItem](driveitem.md).</span></span>

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The mediaSource facet provides information about drive item source.",
  "keywords": "mediaSource,client,media info,onedrive",
  "section": "documentation",
  "tocPath&quot;: &quot;Facets/MediaSource"
} -->
