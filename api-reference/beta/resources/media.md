---
author: MarcMroz
description: 媒体资源包含有关驱动器项 (或视频) 元数据。
title: 媒体资源类型
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 488201407363469ff09220c1dcce3c15f02e3b93
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236310"
---
# <a name="media-resouce-type"></a><span data-ttu-id="687c8-103">media resouce 类型</span><span class="sxs-lookup"><span data-stu-id="687c8-103">media resouce type</span></span>

<span data-ttu-id="687c8-104">包含有关驱动器项 (或视频) 元数据。</span><span class="sxs-lookup"><span data-stu-id="687c8-104">Contains metadata about the media (audio or video) drive item.</span></span>

<span data-ttu-id="687c8-105">可用于 [driveItem][item-resource] 资源的媒体属性。</span><span class="sxs-lookup"><span data-stu-id="687c8-105">It is available on the media property of [driveItem][item-resource] resources.</span></span>


## <a name="properties"></a><span data-ttu-id="687c8-106">属性</span><span class="sxs-lookup"><span data-stu-id="687c8-106">Properties</span></span>

| <span data-ttu-id="687c8-107">属性</span><span class="sxs-lookup"><span data-stu-id="687c8-107">Property</span></span>                 | <span data-ttu-id="687c8-108">类型</span><span class="sxs-lookup"><span data-stu-id="687c8-108">Type</span></span>                  | <span data-ttu-id="687c8-109">说明</span><span class="sxs-lookup"><span data-stu-id="687c8-109">Description</span></span>                                                                                                   |
| :----------------------- | :-------------------- | :------------------------------------------------------------------------------------------------------------ 
| <span data-ttu-id="687c8-110">**isTranscriptionShown**</span><span class="sxs-lookup"><span data-stu-id="687c8-110">**isTranscriptionShown**</span></span> | <span data-ttu-id="687c8-111">布尔值</span><span class="sxs-lookup"><span data-stu-id="687c8-111">Boolean</span></span>               | <span data-ttu-id="687c8-112">如果文件具有脚本，则此设置控制在查看过程中是否向用户显示媒体文件的隐藏式字幕/转录。</span><span class="sxs-lookup"><span data-stu-id="687c8-112">If a file has a transcript, this setting controls if the closed captions / transcription for the media file should be shown to people during viewing.</span></span> <span data-ttu-id="687c8-113">读写。</span><span class="sxs-lookup"><span data-stu-id="687c8-113">Read-Write.</span></span>                                                    |
| <span data-ttu-id="687c8-114">**mediaSource**</span><span class="sxs-lookup"><span data-stu-id="687c8-114">**mediaSource**</span></span>          | [<span data-ttu-id="687c8-115">mediaSource</span><span class="sxs-lookup"><span data-stu-id="687c8-115">mediaSource</span></span>](mediaSource.md)         | <span data-ttu-id="687c8-116">有关媒体源的信息。</span><span class="sxs-lookup"><span data-stu-id="687c8-116">Information about the source of media.</span></span> <span data-ttu-id="687c8-117">只读。</span><span class="sxs-lookup"><span data-stu-id="687c8-117">Read-only.</span></span>                                                             | 


## <a name="json-representation"></a><span data-ttu-id="687c8-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="687c8-118">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.media"
}-->

```json
{
  "isTranscriptionShown" : true,
  "mediaSource": { "@odata.type": "microsoft.graph.mediaSource" }
}
```

## <a name="see-also"></a><span data-ttu-id="687c8-119">另请参阅</span><span class="sxs-lookup"><span data-stu-id="687c8-119">See also</span></span> 

<span data-ttu-id="687c8-120">有关 driveItem 上 Facet 的信息，请参阅 [driveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="687c8-120">For more information about the facets on a driveItem, see [driveItem](driveitem.md).</span></span>

[item-resource]: ../resources/driveitem.md
[mediaSource]: mediaSource.md

<!-- {
  "type": "#page.annotation",
  "description": "The media resource type provides information about the media item.",
  "keywords": "mediaItem,client,media info,onedrive",
  "section": "documentation",
  "tocPath&quot;: &quot;Facets/Media"
} -->
