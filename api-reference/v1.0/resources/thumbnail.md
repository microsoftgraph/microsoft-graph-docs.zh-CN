---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "缩略图"
ms.openlocfilehash: 065c6ae7bbd4f6aca3172afd4399f0a1b5ff3d25
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="thumbnail-resource-type"></a><span data-ttu-id="d3e53-102">缩略图资源类型</span><span class="sxs-lookup"><span data-stu-id="d3e53-102">Thumbnail resource type</span></span>

<span data-ttu-id="d3e53-103">**缩略图**资源类型表示具有位图表示的图像、视频、文档 或任何项目的缩略图。</span><span class="sxs-lookup"><span data-stu-id="d3e53-103">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3e53-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d3e53-104">JSON representation</span></span>

<span data-ttu-id="d3e53-105">下面是**缩略图**资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3e53-105">Here is a JSON representation of the **thumbnail** resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": ["content", "height", "width", "sourceItemId"],
  "@odata.type": "microsoft.graph.thumbnail"
}-->

```json
{
  "height": 1024,
  "sourceItemId": "string",
  "url": "string",
  "width": 1024,

  /* relationships */
  "content": "stream"
}
```

## <a name="properties"></a><span data-ttu-id="d3e53-106">属性</span><span class="sxs-lookup"><span data-stu-id="d3e53-106">Properties</span></span>

| <span data-ttu-id="d3e53-107">属性</span><span class="sxs-lookup"><span data-stu-id="d3e53-107">Property</span></span>     | <span data-ttu-id="d3e53-108">类型</span><span class="sxs-lookup"><span data-stu-id="d3e53-108">Type</span></span>   | <span data-ttu-id="d3e53-109">说明</span><span class="sxs-lookup"><span data-stu-id="d3e53-109">Description</span></span>                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="d3e53-110">height</span><span class="sxs-lookup"><span data-stu-id="d3e53-110">height</span></span>       | <span data-ttu-id="d3e53-111">Int32</span><span class="sxs-lookup"><span data-stu-id="d3e53-111">Int32</span></span>  | <span data-ttu-id="d3e53-112">缩略图高度，以像素为单位。</span><span class="sxs-lookup"><span data-stu-id="d3e53-112">The height of the thumbnail, in pixels.</span></span>                                                                                     |
| <span data-ttu-id="d3e53-113">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="d3e53-113">sourceItemId</span></span> | <span data-ttu-id="d3e53-114">字符串</span><span class="sxs-lookup"><span data-stu-id="d3e53-114">String</span></span> | <span data-ttu-id="d3e53-p101">提供缩略图的项的唯一标识符。仅当请求某个文件夹缩略图时可用。</span><span class="sxs-lookup"><span data-stu-id="d3e53-p101">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span> |
| <span data-ttu-id="d3e53-117">url</span><span class="sxs-lookup"><span data-stu-id="d3e53-117">url</span></span>          | <span data-ttu-id="d3e53-118">String</span><span class="sxs-lookup"><span data-stu-id="d3e53-118">String</span></span> | <span data-ttu-id="d3e53-119">用于提取缩略图内容的 URL。</span><span class="sxs-lookup"><span data-stu-id="d3e53-119">The URL used to fetch the thumbnail content.</span></span>                                                                                |
| <span data-ttu-id="d3e53-120">width</span><span class="sxs-lookup"><span data-stu-id="d3e53-120">width</span></span>        | <span data-ttu-id="d3e53-121">Int32</span><span class="sxs-lookup"><span data-stu-id="d3e53-121">Int32</span></span>  | <span data-ttu-id="d3e53-122">缩略图宽度，以像素为单位。</span><span class="sxs-lookup"><span data-stu-id="d3e53-122">The width of the thumbnail, in pixels.</span></span>                                                                                      |

## <a name="relationships"></a><span data-ttu-id="d3e53-123">关系</span><span class="sxs-lookup"><span data-stu-id="d3e53-123">Relationships</span></span>

| <span data-ttu-id="d3e53-124">名称</span><span class="sxs-lookup"><span data-stu-id="d3e53-124">Name</span></span>    | <span data-ttu-id="d3e53-125">类型</span><span class="sxs-lookup"><span data-stu-id="d3e53-125">Type</span></span>   | <span data-ttu-id="d3e53-126">说明</span><span class="sxs-lookup"><span data-stu-id="d3e53-126">Description</span></span>                           |
| :------ | :----- | :------------------------------------ |
| <span data-ttu-id="d3e53-127">内容</span><span class="sxs-lookup"><span data-stu-id="d3e53-127">content</span></span> | <span data-ttu-id="d3e53-128">流</span><span class="sxs-lookup"><span data-stu-id="d3e53-128">Stream</span></span> | <span data-ttu-id="d3e53-129">缩略图的内容流。</span><span class="sxs-lookup"><span data-stu-id="d3e53-129">The content stream for the thumbnail.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail"
} -->
