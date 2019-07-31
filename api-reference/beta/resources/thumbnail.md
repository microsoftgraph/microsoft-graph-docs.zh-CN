---
author: JeremyKelley
description: 缩略图资源类型表示具有位图表示的图像、视频、文档 或任何项目的缩略图。
ms.date: 09/10/2017
title: 缩略图
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 752d46f1c8a769f9f571fd13d940586fda653a58
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007660"
---
# <a name="thumbnail-resource-type"></a><span data-ttu-id="e7cbe-103">Thumbnail 资源类型</span><span class="sxs-lookup"><span data-stu-id="e7cbe-103">Thumbnail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7cbe-104">**缩略图**资源类型表示具有位图表示的图像、视频、文档 或任何项目的缩略图。</span><span class="sxs-lookup"><span data-stu-id="e7cbe-104">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e7cbe-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e7cbe-105">JSON representation</span></span>

<span data-ttu-id="e7cbe-106">下面是**缩略图**资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7cbe-106">Here is a JSON representation of the **thumbnail** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="e7cbe-107">属性</span><span class="sxs-lookup"><span data-stu-id="e7cbe-107">Properties</span></span>

| <span data-ttu-id="e7cbe-108">属性</span><span class="sxs-lookup"><span data-stu-id="e7cbe-108">Property</span></span>     | <span data-ttu-id="e7cbe-109">类型</span><span class="sxs-lookup"><span data-stu-id="e7cbe-109">Type</span></span>   | <span data-ttu-id="e7cbe-110">说明</span><span class="sxs-lookup"><span data-stu-id="e7cbe-110">Description</span></span>                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="e7cbe-111">height</span><span class="sxs-lookup"><span data-stu-id="e7cbe-111">height</span></span>       | <span data-ttu-id="e7cbe-112">Int32</span><span class="sxs-lookup"><span data-stu-id="e7cbe-112">Int32</span></span>  | <span data-ttu-id="e7cbe-113">缩略图高度，以像素为单位。</span><span class="sxs-lookup"><span data-stu-id="e7cbe-113">The height of the thumbnail, in pixels.</span></span>                                                                                     |
| <span data-ttu-id="e7cbe-114">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="e7cbe-114">sourceItemId</span></span> | <span data-ttu-id="e7cbe-115">字符串</span><span class="sxs-lookup"><span data-stu-id="e7cbe-115">String</span></span> | <span data-ttu-id="e7cbe-p101">提供缩略图的项的唯一标识符。仅当请求某个文件夹缩略图时可用。</span><span class="sxs-lookup"><span data-stu-id="e7cbe-p101">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span> |
| <span data-ttu-id="e7cbe-118">url</span><span class="sxs-lookup"><span data-stu-id="e7cbe-118">url</span></span>          | <span data-ttu-id="e7cbe-119">String</span><span class="sxs-lookup"><span data-stu-id="e7cbe-119">String</span></span> | <span data-ttu-id="e7cbe-120">用于提取缩略图内容的 URL。</span><span class="sxs-lookup"><span data-stu-id="e7cbe-120">The URL used to fetch the thumbnail content.</span></span>                                                                                |
| <span data-ttu-id="e7cbe-121">width</span><span class="sxs-lookup"><span data-stu-id="e7cbe-121">width</span></span>        | <span data-ttu-id="e7cbe-122">Int32</span><span class="sxs-lookup"><span data-stu-id="e7cbe-122">Int32</span></span>  | <span data-ttu-id="e7cbe-123">缩略图宽度，以像素为单位。</span><span class="sxs-lookup"><span data-stu-id="e7cbe-123">The width of the thumbnail, in pixels.</span></span>                                                                                      |
| <span data-ttu-id="e7cbe-124">content</span><span class="sxs-lookup"><span data-stu-id="e7cbe-124">content</span></span> | <span data-ttu-id="e7cbe-125">流</span><span class="sxs-lookup"><span data-stu-id="e7cbe-125">Stream</span></span> | <span data-ttu-id="e7cbe-126">缩略图的内容流。</span><span class="sxs-lookup"><span data-stu-id="e7cbe-126">The content stream for the thumbnail.</span></span> |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail",
  "suppressions": []
}
-->
