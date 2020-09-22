---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ThumbnailSet
localization_priority: Normal
description: ThumbnailSet 资源是键控的 缩略图 资源集合。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5aa7ca5646ea0555c0f6547e7171312537343345
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090856"
---
# <a name="thumbnailset-resource-type"></a><span data-ttu-id="1f685-103">ThumbnailSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="1f685-103">ThumbnailSet resource type</span></span>

<span data-ttu-id="1f685-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f685-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1f685-p101">**ThumbnailSet** 资源是键控的 [缩略图](thumbnail.md) 资源集合。它用来表示与 DriveItem 相关联的一组缩略图。</span><span class="sxs-lookup"><span data-stu-id="1f685-p101">The **ThumbnailSet** resource is a keyed collection of [thumbnail](thumbnail.md) resources. It is used to represent a set of thumbnails associated with a DriveItem.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f685-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1f685-107">JSON representation</span></span>

<span data-ttu-id="1f685-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1f685-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="1f685-109">属性</span><span class="sxs-lookup"><span data-stu-id="1f685-109">Properties</span></span>

| <span data-ttu-id="1f685-110">属性</span><span class="sxs-lookup"><span data-stu-id="1f685-110">Property</span></span> | <span data-ttu-id="1f685-111">类型</span><span class="sxs-lookup"><span data-stu-id="1f685-111">Type</span></span>                      | <span data-ttu-id="1f685-112">说明</span><span class="sxs-lookup"><span data-stu-id="1f685-112">Description</span></span>                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| <span data-ttu-id="1f685-113">id</span><span class="sxs-lookup"><span data-stu-id="1f685-113">id</span></span>       | <span data-ttu-id="1f685-114">String</span><span class="sxs-lookup"><span data-stu-id="1f685-114">String</span></span>                    | <span data-ttu-id="1f685-p102">项目中的 id。只读。</span><span class="sxs-lookup"><span data-stu-id="1f685-p102">The id within the item. Read-only.</span></span>                                                |
| <span data-ttu-id="1f685-117">大</span><span class="sxs-lookup"><span data-stu-id="1f685-117">large</span></span>    | [<span data-ttu-id="1f685-118">缩略图</span><span class="sxs-lookup"><span data-stu-id="1f685-118">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="1f685-119">1920 x 1920 缩放后的缩略图。</span><span class="sxs-lookup"><span data-stu-id="1f685-119">A 1920x1920 scaled thumbnail.</span></span>                                                     |
| <span data-ttu-id="1f685-120">中等</span><span class="sxs-lookup"><span data-stu-id="1f685-120">medium</span></span>   | [<span data-ttu-id="1f685-121">缩略图</span><span class="sxs-lookup"><span data-stu-id="1f685-121">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="1f685-122">176x176 缩放后的缩略图。</span><span class="sxs-lookup"><span data-stu-id="1f685-122">A 176x176 scaled thumbnail.</span></span>                                                       |
| <span data-ttu-id="1f685-123">小</span><span class="sxs-lookup"><span data-stu-id="1f685-123">small</span></span>    | [<span data-ttu-id="1f685-124">缩略图</span><span class="sxs-lookup"><span data-stu-id="1f685-124">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="1f685-125">48x48 裁剪缩略图。</span><span class="sxs-lookup"><span data-stu-id="1f685-125">A 48x48 cropped thumbnail.</span></span>                                                        |
| <span data-ttu-id="1f685-126">源</span><span class="sxs-lookup"><span data-stu-id="1f685-126">source</span></span>   | [<span data-ttu-id="1f685-127">缩略图</span><span class="sxs-lookup"><span data-stu-id="1f685-127">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="1f685-128">用来生成其他缩略图的自定义缩略图图像或原始图像。</span><span class="sxs-lookup"><span data-stu-id="1f685-128">A custom thumbnail image or the original image used to generate other thumbnails.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ThumbnailSet enables access to thumbnails of different sizes",
  "section": "documentation",
  "tocPath": "Resources/ThumbnailSet"
} -->

