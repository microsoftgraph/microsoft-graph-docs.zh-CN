---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ThumbnailSet
localization_priority: Normal
ms.openlocfilehash: a9d92d84c8495b8c138c34f752700ccd0aad64fd
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480129"
---
# <a name="thumbnailset-resource-type"></a><span data-ttu-id="d6fb0-102">ThumbnailSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="d6fb0-102">ThumbnailSet resource type</span></span>

<span data-ttu-id="d6fb0-p101">**ThumbnailSet** 资源是键控的 [缩略图](thumbnail.md) 资源集合。它用来表示与 DriveItem 相关联的一组缩略图。</span><span class="sxs-lookup"><span data-stu-id="d6fb0-p101">The **ThumbnailSet** resource is a keyed collection of [thumbnail](thumbnail.md) resources. It is used to represent a set of thumbnails associated with a DriveItem.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6fb0-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d6fb0-105">JSON representation</span></span>

<span data-ttu-id="d6fb0-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d6fb0-106">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "source",
    "small",
    "medium",
    "large"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.thumbnailSet",
  "openType": true
}-->

```json
{
  "id": "string (identifier)",
  "large": { "@odata.type": "microsoft.graph.thumbnail" },
  "medium": { "@odata.type": "microsoft.graph.thumbnail" },
  "small": { "@odata.type": "microsoft.graph.thumbnail" },
  "source": { "@odata.type": "microsoft.graph.thumbnail" }
}
```

## <a name="properties"></a><span data-ttu-id="d6fb0-107">属性</span><span class="sxs-lookup"><span data-stu-id="d6fb0-107">Properties</span></span>

| <span data-ttu-id="d6fb0-108">属性</span><span class="sxs-lookup"><span data-stu-id="d6fb0-108">Property</span></span> | <span data-ttu-id="d6fb0-109">类型</span><span class="sxs-lookup"><span data-stu-id="d6fb0-109">Type</span></span>                      | <span data-ttu-id="d6fb0-110">说明</span><span class="sxs-lookup"><span data-stu-id="d6fb0-110">Description</span></span>                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| <span data-ttu-id="d6fb0-111">id</span><span class="sxs-lookup"><span data-stu-id="d6fb0-111">id</span></span>       | <span data-ttu-id="d6fb0-112">String</span><span class="sxs-lookup"><span data-stu-id="d6fb0-112">String</span></span>                    | <span data-ttu-id="d6fb0-p102">项目中的 id。只读。</span><span class="sxs-lookup"><span data-stu-id="d6fb0-p102">The id within the item. Read-only.</span></span>                                                |
| <span data-ttu-id="d6fb0-115">大</span><span class="sxs-lookup"><span data-stu-id="d6fb0-115">large</span></span>    | [<span data-ttu-id="d6fb0-116">缩略图</span><span class="sxs-lookup"><span data-stu-id="d6fb0-116">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="d6fb0-117">1920 x 1920 缩放后的缩略图。</span><span class="sxs-lookup"><span data-stu-id="d6fb0-117">A 1920x1920 scaled thumbnail.</span></span>                                                     |
| <span data-ttu-id="d6fb0-118">中等</span><span class="sxs-lookup"><span data-stu-id="d6fb0-118">medium</span></span>   | [<span data-ttu-id="d6fb0-119">缩略图</span><span class="sxs-lookup"><span data-stu-id="d6fb0-119">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="d6fb0-120">176x176 缩放后的缩略图。</span><span class="sxs-lookup"><span data-stu-id="d6fb0-120">A 176x176 scaled thumbnail.</span></span>                                                       |
| <span data-ttu-id="d6fb0-121">小</span><span class="sxs-lookup"><span data-stu-id="d6fb0-121">small</span></span>    | [<span data-ttu-id="d6fb0-122">缩略图</span><span class="sxs-lookup"><span data-stu-id="d6fb0-122">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="d6fb0-123">48x48 裁剪缩略图。</span><span class="sxs-lookup"><span data-stu-id="d6fb0-123">A 48x48 cropped thumbnail.</span></span>                                                        |
| <span data-ttu-id="d6fb0-124">源</span><span class="sxs-lookup"><span data-stu-id="d6fb0-124">source</span></span>   | [<span data-ttu-id="d6fb0-125">缩略图</span><span class="sxs-lookup"><span data-stu-id="d6fb0-125">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="d6fb0-126">用来生成其他缩略图的自定义缩略图图像或原始图像。</span><span class="sxs-lookup"><span data-stu-id="d6fb0-126">A custom thumbnail image or the original image used to generate other thumbnails.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ThumbnailSet enables access to thumbnails of different sizes",
  "section": "documentation",
  "tocPath": "Resources/ThumbnailSet"
} -->
