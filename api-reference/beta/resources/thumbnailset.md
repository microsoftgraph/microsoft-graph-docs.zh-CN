---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ThumbnailSet
localization_priority: Normal
ms.openlocfilehash: e3e3305e398651478c88d4c3aa75e753ce26acd5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342042"
---
# <a name="thumbnailset-resource-type"></a><span data-ttu-id="ab4e8-102">ThumbnailSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="ab4e8-102">ThumbnailSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab4e8-p101">**ThumbnailSet** 资源是键控的 [缩略图](thumbnail.md) 资源集合。它用来表示与 DriveItem 相关联的一组缩略图。</span><span class="sxs-lookup"><span data-stu-id="ab4e8-p101">The **ThumbnailSet** resource is a keyed collection of [thumbnail](thumbnail.md) resources. It is used to represent a set of thumbnails associated with a DriveItem.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ab4e8-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ab4e8-105">JSON representation</span></span>

<span data-ttu-id="ab4e8-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab4e8-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": ["source", "small", "medium", "large"],
  "openType": true,
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.thumbnailSet"
} -->

```json
{
  "id": "string (identifier)",
  "large": { "@odata.type": "microsoft.graph.thumbnail" },
  "medium": { "@odata.type": "microsoft.graph.thumbnail" },
  "small": { "@odata.type": "microsoft.graph.thumbnail" },
  "source": { "@odata.type": "microsoft.graph.thumbnail" }
}
```

## <a name="properties"></a><span data-ttu-id="ab4e8-107">属性</span><span class="sxs-lookup"><span data-stu-id="ab4e8-107">Properties</span></span>

| <span data-ttu-id="ab4e8-108">属性</span><span class="sxs-lookup"><span data-stu-id="ab4e8-108">Property</span></span> | <span data-ttu-id="ab4e8-109">类型</span><span class="sxs-lookup"><span data-stu-id="ab4e8-109">Type</span></span>                      | <span data-ttu-id="ab4e8-110">说明</span><span class="sxs-lookup"><span data-stu-id="ab4e8-110">Description</span></span>                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| <span data-ttu-id="ab4e8-111">id</span><span class="sxs-lookup"><span data-stu-id="ab4e8-111">id</span></span>       | <span data-ttu-id="ab4e8-112">String</span><span class="sxs-lookup"><span data-stu-id="ab4e8-112">String</span></span>                    | <span data-ttu-id="ab4e8-p102">项目中的 id。只读。</span><span class="sxs-lookup"><span data-stu-id="ab4e8-p102">The id within the item. Read-only.</span></span>                                                |
| <span data-ttu-id="ab4e8-115">大</span><span class="sxs-lookup"><span data-stu-id="ab4e8-115">large</span></span>    | [<span data-ttu-id="ab4e8-116">缩略图</span><span class="sxs-lookup"><span data-stu-id="ab4e8-116">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="ab4e8-117">1920 x 1920 缩放后的缩略图。</span><span class="sxs-lookup"><span data-stu-id="ab4e8-117">A 1920x1920 scaled thumbnail.</span></span>                                                     |
| <span data-ttu-id="ab4e8-118">中等</span><span class="sxs-lookup"><span data-stu-id="ab4e8-118">medium</span></span>   | [<span data-ttu-id="ab4e8-119">缩略图</span><span class="sxs-lookup"><span data-stu-id="ab4e8-119">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="ab4e8-120">176x176 缩放后的缩略图。</span><span class="sxs-lookup"><span data-stu-id="ab4e8-120">A 176x176 scaled thumbnail.</span></span>                                                       |
| <span data-ttu-id="ab4e8-121">小</span><span class="sxs-lookup"><span data-stu-id="ab4e8-121">small</span></span>    | [<span data-ttu-id="ab4e8-122">缩略图</span><span class="sxs-lookup"><span data-stu-id="ab4e8-122">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="ab4e8-123">48x48 裁剪缩略图。</span><span class="sxs-lookup"><span data-stu-id="ab4e8-123">A 48x48 cropped thumbnail.</span></span>                                                        |
| <span data-ttu-id="ab4e8-124">源</span><span class="sxs-lookup"><span data-stu-id="ab4e8-124">source</span></span>   | [<span data-ttu-id="ab4e8-125">缩略图</span><span class="sxs-lookup"><span data-stu-id="ab4e8-125">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="ab4e8-126">用来生成其他缩略图的自定义缩略图图像或原始图像。</span><span class="sxs-lookup"><span data-stu-id="ab4e8-126">A custom thumbnail image or the original image used to generate other thumbnails.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ThumbnailSet enables access to thumbnails of different sizes",
  "section": "documentation",
  "tocPath": "Resources/ThumbnailSet",
  "suppressions": []
}
-->
