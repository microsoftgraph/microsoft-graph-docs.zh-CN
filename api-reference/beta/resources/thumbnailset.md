---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ThumbnailSet
ms.openlocfilehash: d88e19242ea6c271e206a4c1a582fdbbfac8877b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042700"
---
# <a name="thumbnailset-resource-type"></a><span data-ttu-id="d69a2-102">ThumbnailSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="d69a2-102">ThumbnailSet resource type</span></span>

> <span data-ttu-id="d69a2-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d69a2-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d69a2-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d69a2-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d69a2-p102">**ThumbnailSet** 资源是键控的 [缩略图](thumbnail.md) 资源集合。它用来表示与 DriveItem 相关联的一组缩略图。</span><span class="sxs-lookup"><span data-stu-id="d69a2-p102">The **ThumbnailSet** resource is a keyed collection of [thumbnail](thumbnail.md) resources. It is used to represent a set of thumbnails associated with a DriveItem.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d69a2-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d69a2-107">JSON representation</span></span>

<span data-ttu-id="d69a2-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d69a2-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="d69a2-109">属性</span><span class="sxs-lookup"><span data-stu-id="d69a2-109">Properties</span></span>

| <span data-ttu-id="d69a2-110">属性</span><span class="sxs-lookup"><span data-stu-id="d69a2-110">Property</span></span> | <span data-ttu-id="d69a2-111">类型</span><span class="sxs-lookup"><span data-stu-id="d69a2-111">Type</span></span>                      | <span data-ttu-id="d69a2-112">说明</span><span class="sxs-lookup"><span data-stu-id="d69a2-112">Description</span></span>                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| <span data-ttu-id="d69a2-113">id</span><span class="sxs-lookup"><span data-stu-id="d69a2-113">id</span></span>       | <span data-ttu-id="d69a2-114">字符串</span><span class="sxs-lookup"><span data-stu-id="d69a2-114">String</span></span>                    | <span data-ttu-id="d69a2-p103">项目中的 id。只读。</span><span class="sxs-lookup"><span data-stu-id="d69a2-p103">The id within the item. Read-only.</span></span>                                                |
| <span data-ttu-id="d69a2-117">大</span><span class="sxs-lookup"><span data-stu-id="d69a2-117">large</span></span>    | [<span data-ttu-id="d69a2-118">缩略图</span><span class="sxs-lookup"><span data-stu-id="d69a2-118">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="d69a2-119">1920 x 1920 缩放后的缩略图。</span><span class="sxs-lookup"><span data-stu-id="d69a2-119">A 1920x1920 scaled thumbnail.</span></span>                                                     |
| <span data-ttu-id="d69a2-120">中等</span><span class="sxs-lookup"><span data-stu-id="d69a2-120">medium</span></span>   | [<span data-ttu-id="d69a2-121">缩略图</span><span class="sxs-lookup"><span data-stu-id="d69a2-121">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="d69a2-122">176x176 缩放后的缩略图。</span><span class="sxs-lookup"><span data-stu-id="d69a2-122">A 176x176 scaled thumbnail.</span></span>                                                       |
| <span data-ttu-id="d69a2-123">小</span><span class="sxs-lookup"><span data-stu-id="d69a2-123">small</span></span>    | [<span data-ttu-id="d69a2-124">缩略图</span><span class="sxs-lookup"><span data-stu-id="d69a2-124">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="d69a2-125">48x48 裁剪缩略图。</span><span class="sxs-lookup"><span data-stu-id="d69a2-125">A 48x48 cropped thumbnail.</span></span>                                                        |
| <span data-ttu-id="d69a2-126">源</span><span class="sxs-lookup"><span data-stu-id="d69a2-126">source</span></span>   | [<span data-ttu-id="d69a2-127">缩略图</span><span class="sxs-lookup"><span data-stu-id="d69a2-127">Thumbnail</span></span>](thumbnail.md) | <span data-ttu-id="d69a2-128">用来生成其他缩略图的自定义缩略图图像或原始图像。</span><span class="sxs-lookup"><span data-stu-id="d69a2-128">A custom thumbnail image or the original image used to generate other thumbnails.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ThumbnailSet enables access to thumbnails of different sizes",
  "section": "documentation",
  "tocPath": "Resources/ThumbnailSet"
} -->
