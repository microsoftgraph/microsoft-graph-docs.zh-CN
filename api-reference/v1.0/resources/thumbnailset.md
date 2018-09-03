---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ThumbnailSet
ms.openlocfilehash: 2ba45363b684142b91aac62d4b2a5b0d371d6b3d
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2018
ms.locfileid: "23270809"
---
# <a name="thumbnailset-resource-type"></a><span data-ttu-id="6022e-102">ThumbnailSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="6022e-102">ThumbnailSet resource type</span></span>

<span data-ttu-id="6022e-p101">**ThumbnailSet** 资源是键控的 [缩略图](thumbnail.md) 资源集合。它用来表示与 DriveItem 相关联的一组缩略图。</span><span class="sxs-lookup"><span data-stu-id="6022e-p101">The **ThumbnailSet** resource is a keyed collection of [thumbnail](thumbnail.md) resources. It is used to represent a set of thumbnails associated with a DriveItem.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6022e-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6022e-105">JSON representation</span></span>

<span data-ttu-id="6022e-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6022e-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="6022e-107">属性</span><span class="sxs-lookup"><span data-stu-id="6022e-107">Properties</span></span>

| <span data-ttu-id="6022e-108">属性</span><span class="sxs-lookup"><span data-stu-id="6022e-108">Property</span></span> | <span data-ttu-id="6022e-109">类型</span><span class="sxs-lookup"><span data-stu-id="6022e-109">Type</span></span>                      | <span data-ttu-id="6022e-110">说明</span><span class="sxs-lookup"><span data-stu-id="6022e-110">Description</span></span>                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| <span data-ttu-id="6022e-111">id</span><span class="sxs-lookup"><span data-stu-id="6022e-111">id</span></span>       | <span data-ttu-id="6022e-112">字符串</span><span class="sxs-lookup"><span data-stu-id="6022e-112">String</span></span>                    | <span data-ttu-id="6022e-p102">项目中的 id。只读。</span><span class="sxs-lookup"><span data-stu-id="6022e-p102">The id within the item. Read-only.</span></span>                                                |
| <span data-ttu-id="6022e-115">large</span><span class="sxs-lookup"><span data-stu-id="6022e-115">large</span></span>    | [<span data-ttu-id="6022e-116">缩略图</span><span class="sxs-lookup"><span data-stu-id="6022e-116">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="6022e-117">1920 x 1920 缩放后的缩略图。</span><span class="sxs-lookup"><span data-stu-id="6022e-117">A 1920x1920 scaled thumbnail.</span></span>                                                     |
| <span data-ttu-id="6022e-118">medium</span><span class="sxs-lookup"><span data-stu-id="6022e-118">medium</span></span>   | [<span data-ttu-id="6022e-119">缩略图</span><span class="sxs-lookup"><span data-stu-id="6022e-119">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="6022e-120">176x176 缩放后的缩略图。</span><span class="sxs-lookup"><span data-stu-id="6022e-120">A 176x176 scaled thumbnail.</span></span>                                                       |
| <span data-ttu-id="6022e-121">small</span><span class="sxs-lookup"><span data-stu-id="6022e-121">small</span></span>    | [<span data-ttu-id="6022e-122">缩略图</span><span class="sxs-lookup"><span data-stu-id="6022e-122">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="6022e-123">48x48 裁剪缩略图。</span><span class="sxs-lookup"><span data-stu-id="6022e-123">A 48x48 cropped thumbnail.</span></span>                                                        |
| <span data-ttu-id="6022e-124">source</span><span class="sxs-lookup"><span data-stu-id="6022e-124">source</span></span>   | [<span data-ttu-id="6022e-125">缩略图</span><span class="sxs-lookup"><span data-stu-id="6022e-125">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="6022e-126">用来生成其他缩略图的自定义缩略图图像或原始图像。</span><span class="sxs-lookup"><span data-stu-id="6022e-126">A custom thumbnail image or the original image used to generate other thumbnails.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ThumbnailSet enables access to thumbnails of different sizes",
  "section": "documentation",
  "tocPath": "Resources/ThumbnailSet"
} -->
