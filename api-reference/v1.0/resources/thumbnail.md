---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 缩略图
localization_priority: Normal
ms.openlocfilehash: d11f9eead6faf885bee579c634267e038f8a8ee4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522221"
---
# <a name="thumbnail-resource-type"></a><span data-ttu-id="c82df-102">Thumbnail 资源类型</span><span class="sxs-lookup"><span data-stu-id="c82df-102">Thumbnail resource type</span></span>

<span data-ttu-id="c82df-103">**缩略图**资源类型表示具有位图表示的图像、视频、文档 或任何项目的缩略图。</span><span class="sxs-lookup"><span data-stu-id="c82df-103">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c82df-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c82df-104">JSON representation</span></span>

<span data-ttu-id="c82df-105">下面是**缩略图**资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c82df-105">Here is a JSON representation of the **thumbnail** resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "content",
    "height",
    "width",
    "sourceItemId"
  ],
  "@odata.type": "microsoft.graph.thumbnail"
}-->

```json
{
  "height": 1024,
  "sourceItemId": "string",
  "url": "string",
  "width": 1024,
  "content": "stream"
}
```

## <a name="properties"></a><span data-ttu-id="c82df-106">属性</span><span class="sxs-lookup"><span data-stu-id="c82df-106">Properties</span></span>

| <span data-ttu-id="c82df-107">属性</span><span class="sxs-lookup"><span data-stu-id="c82df-107">Property</span></span>     | <span data-ttu-id="c82df-108">类型</span><span class="sxs-lookup"><span data-stu-id="c82df-108">Type</span></span>   | <span data-ttu-id="c82df-109">说明</span><span class="sxs-lookup"><span data-stu-id="c82df-109">Description</span></span>
| :----------- | :----- | :----------------------------------------------------
| <span data-ttu-id="c82df-110">height</span><span class="sxs-lookup"><span data-stu-id="c82df-110">height</span></span>       | <span data-ttu-id="c82df-111">Int32</span><span class="sxs-lookup"><span data-stu-id="c82df-111">Int32</span></span>  | <span data-ttu-id="c82df-112">缩略图高度，以像素为单位。</span><span class="sxs-lookup"><span data-stu-id="c82df-112">The height of the thumbnail, in pixels.</span></span>
| <span data-ttu-id="c82df-113">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="c82df-113">sourceItemId</span></span> | <span data-ttu-id="c82df-114">字符串</span><span class="sxs-lookup"><span data-stu-id="c82df-114">String</span></span> | <span data-ttu-id="c82df-p101">提供缩略图的项的唯一标识符。仅当请求某个文件夹缩略图时可用。</span><span class="sxs-lookup"><span data-stu-id="c82df-p101">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span>
| <span data-ttu-id="c82df-117">url</span><span class="sxs-lookup"><span data-stu-id="c82df-117">url</span></span>          | <span data-ttu-id="c82df-118">String</span><span class="sxs-lookup"><span data-stu-id="c82df-118">String</span></span> | <span data-ttu-id="c82df-119">用于提取缩略图内容的 URL。</span><span class="sxs-lookup"><span data-stu-id="c82df-119">The URL used to fetch the thumbnail content.</span></span>
| <span data-ttu-id="c82df-120">width</span><span class="sxs-lookup"><span data-stu-id="c82df-120">width</span></span>        | <span data-ttu-id="c82df-121">Int32</span><span class="sxs-lookup"><span data-stu-id="c82df-121">Int32</span></span>  | <span data-ttu-id="c82df-122">缩略图宽度，以像素为单位。</span><span class="sxs-lookup"><span data-stu-id="c82df-122">The width of the thumbnail, in pixels.</span></span>
| <span data-ttu-id="c82df-123">content</span><span class="sxs-lookup"><span data-stu-id="c82df-123">content</span></span>      | <span data-ttu-id="c82df-124">流</span><span class="sxs-lookup"><span data-stu-id="c82df-124">Stream</span></span> | <span data-ttu-id="c82df-125">缩略图的内容流。</span><span class="sxs-lookup"><span data-stu-id="c82df-125">The content stream for the thumbnail.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail"
} -->
