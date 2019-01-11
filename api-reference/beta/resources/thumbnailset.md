---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ThumbnailSet
localization_priority: Normal
ms.openlocfilehash: 145134d6a3ad85134ea2d6c4d72e050bc17b31d1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830188"
---
# <a name="thumbnailset-resource-type"></a><span data-ttu-id="738d9-102">ThumbnailSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="738d9-102">ThumbnailSet resource type</span></span>

> <span data-ttu-id="738d9-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="738d9-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="738d9-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="738d9-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="738d9-p102">**ThumbnailSet** 资源是键控的 [缩略图](thumbnail.md) 资源集合。它用来表示与 DriveItem 相关联的一组缩略图。</span><span class="sxs-lookup"><span data-stu-id="738d9-p102">The **ThumbnailSet** resource is a keyed collection of [thumbnail](thumbnail.md) resources. It is used to represent a set of thumbnails associated with a DriveItem.</span></span>

## <a name="json-representation"></a><span data-ttu-id="738d9-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="738d9-107">JSON representation</span></span>

<span data-ttu-id="738d9-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="738d9-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="738d9-109">属性</span><span class="sxs-lookup"><span data-stu-id="738d9-109">Properties</span></span>

| <span data-ttu-id="738d9-110">属性</span><span class="sxs-lookup"><span data-stu-id="738d9-110">Property</span></span> | <span data-ttu-id="738d9-111">类型</span><span class="sxs-lookup"><span data-stu-id="738d9-111">Type</span></span>                      | <span data-ttu-id="738d9-112">说明</span><span class="sxs-lookup"><span data-stu-id="738d9-112">Description</span></span>                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| <span data-ttu-id="738d9-113">id</span><span class="sxs-lookup"><span data-stu-id="738d9-113">id</span></span>       | <span data-ttu-id="738d9-114">字符串</span><span class="sxs-lookup"><span data-stu-id="738d9-114">String</span></span>                    | <span data-ttu-id="738d9-p103">项目中的 id。只读。</span><span class="sxs-lookup"><span data-stu-id="738d9-p103">The id within the item. Read-only.</span></span>                                                |
| <span data-ttu-id="738d9-117">大</span><span class="sxs-lookup"><span data-stu-id="738d9-117">large</span></span>    | [<span data-ttu-id="738d9-118">缩略图</span><span class="sxs-lookup"><span data-stu-id="738d9-118">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="738d9-119">1920 x 1920 缩放后的缩略图。</span><span class="sxs-lookup"><span data-stu-id="738d9-119">A 1920x1920 scaled thumbnail.</span></span>                                                     |
| <span data-ttu-id="738d9-120">中等</span><span class="sxs-lookup"><span data-stu-id="738d9-120">medium</span></span>   | [<span data-ttu-id="738d9-121">缩略图</span><span class="sxs-lookup"><span data-stu-id="738d9-121">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="738d9-122">176x176 缩放后的缩略图。</span><span class="sxs-lookup"><span data-stu-id="738d9-122">A 176x176 scaled thumbnail.</span></span>                                                       |
| <span data-ttu-id="738d9-123">小</span><span class="sxs-lookup"><span data-stu-id="738d9-123">small</span></span>    | [<span data-ttu-id="738d9-124">缩略图</span><span class="sxs-lookup"><span data-stu-id="738d9-124">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="738d9-125">48x48 裁剪缩略图。</span><span class="sxs-lookup"><span data-stu-id="738d9-125">A 48x48 cropped thumbnail.</span></span>                                                        |
| <span data-ttu-id="738d9-126">源</span><span class="sxs-lookup"><span data-stu-id="738d9-126">source</span></span>   | [<span data-ttu-id="738d9-127">缩略图</span><span class="sxs-lookup"><span data-stu-id="738d9-127">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="738d9-128">用来生成其他缩略图的自定义缩略图图像或原始图像。</span><span class="sxs-lookup"><span data-stu-id="738d9-128">A custom thumbnail image or the original image used to generate other thumbnails.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ThumbnailSet enables access to thumbnails of different sizes",
  "section": "documentation",
  "tocPath": "Resources/ThumbnailSet"
} -->
