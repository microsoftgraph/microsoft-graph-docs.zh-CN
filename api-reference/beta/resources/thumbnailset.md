---
author: JeremyKelley
description: ThumbnailSet 资源是键控的 缩略图 资源集合。
ms.date: 09/10/2017
title: ThumbnailSet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: bb8c286cd8c3827317edc9a24e4d14dbe963a05d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964343"
---
# <a name="thumbnailset-resource-type"></a><span data-ttu-id="f4016-103">ThumbnailSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="f4016-103">ThumbnailSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4016-p101">**ThumbnailSet** 资源是键控的 [缩略图](thumbnail.md) 资源集合。它用来表示与 DriveItem 相关联的一组缩略图。</span><span class="sxs-lookup"><span data-stu-id="f4016-p101">The **ThumbnailSet** resource is a keyed collection of [thumbnail](thumbnail.md) resources. It is used to represent a set of thumbnails associated with a DriveItem.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4016-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f4016-106">JSON representation</span></span>

<span data-ttu-id="f4016-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4016-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="f4016-108">属性</span><span class="sxs-lookup"><span data-stu-id="f4016-108">Properties</span></span>

| <span data-ttu-id="f4016-109">属性</span><span class="sxs-lookup"><span data-stu-id="f4016-109">Property</span></span> | <span data-ttu-id="f4016-110">类型</span><span class="sxs-lookup"><span data-stu-id="f4016-110">Type</span></span>                      | <span data-ttu-id="f4016-111">说明</span><span class="sxs-lookup"><span data-stu-id="f4016-111">Description</span></span>                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| <span data-ttu-id="f4016-112">id</span><span class="sxs-lookup"><span data-stu-id="f4016-112">id</span></span>       | <span data-ttu-id="f4016-113">String</span><span class="sxs-lookup"><span data-stu-id="f4016-113">String</span></span>                    | <span data-ttu-id="f4016-p102">项目中的 id。只读。</span><span class="sxs-lookup"><span data-stu-id="f4016-p102">The id within the item. Read-only.</span></span>                                                |
| <span data-ttu-id="f4016-116">大</span><span class="sxs-lookup"><span data-stu-id="f4016-116">large</span></span>    | [<span data-ttu-id="f4016-117">缩略图</span><span class="sxs-lookup"><span data-stu-id="f4016-117">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="f4016-118">1920 x 1920 缩放后的缩略图。</span><span class="sxs-lookup"><span data-stu-id="f4016-118">A 1920x1920 scaled thumbnail.</span></span>                                                     |
| <span data-ttu-id="f4016-119">中等</span><span class="sxs-lookup"><span data-stu-id="f4016-119">medium</span></span>   | [<span data-ttu-id="f4016-120">缩略图</span><span class="sxs-lookup"><span data-stu-id="f4016-120">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="f4016-121">176x176 缩放后的缩略图。</span><span class="sxs-lookup"><span data-stu-id="f4016-121">A 176x176 scaled thumbnail.</span></span>                                                       |
| <span data-ttu-id="f4016-122">小</span><span class="sxs-lookup"><span data-stu-id="f4016-122">small</span></span>    | [<span data-ttu-id="f4016-123">缩略图</span><span class="sxs-lookup"><span data-stu-id="f4016-123">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="f4016-124">48x48 裁剪缩略图。</span><span class="sxs-lookup"><span data-stu-id="f4016-124">A 48x48 cropped thumbnail.</span></span>                                                        |
| <span data-ttu-id="f4016-125">源</span><span class="sxs-lookup"><span data-stu-id="f4016-125">source</span></span>   | [<span data-ttu-id="f4016-126">缩略图</span><span class="sxs-lookup"><span data-stu-id="f4016-126">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="f4016-127">用来生成其他缩略图的自定义缩略图图像或原始图像。</span><span class="sxs-lookup"><span data-stu-id="f4016-127">A custom thumbnail image or the original image used to generate other thumbnails.</span></span> |

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
