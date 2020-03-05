---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 缩略图
localization_priority: Normal
description: 缩略图资源类型表示具有位图表示的图像、视频、文档 或任何项目的缩略图。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9db187516cd133ebeab0a352d56470e6b2e172c7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446826"
---
# <a name="thumbnail-resource-type"></a><span data-ttu-id="75f40-103">Thumbnail 资源类型</span><span class="sxs-lookup"><span data-stu-id="75f40-103">Thumbnail resource type</span></span>

<span data-ttu-id="75f40-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="75f40-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="75f40-105">**缩略图**资源类型表示具有位图表示的图像、视频、文档 或任何项目的缩略图。</span><span class="sxs-lookup"><span data-stu-id="75f40-105">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="75f40-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="75f40-106">JSON representation</span></span>

<span data-ttu-id="75f40-107">下面是**缩略图**资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="75f40-107">Here is a JSON representation of the **thumbnail** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="75f40-108">属性</span><span class="sxs-lookup"><span data-stu-id="75f40-108">Properties</span></span>

| <span data-ttu-id="75f40-109">属性</span><span class="sxs-lookup"><span data-stu-id="75f40-109">Property</span></span>     | <span data-ttu-id="75f40-110">类型</span><span class="sxs-lookup"><span data-stu-id="75f40-110">Type</span></span>   | <span data-ttu-id="75f40-111">说明</span><span class="sxs-lookup"><span data-stu-id="75f40-111">Description</span></span>
| :----------- | :----- | :----------------------------------------------------
| <span data-ttu-id="75f40-112">height</span><span class="sxs-lookup"><span data-stu-id="75f40-112">height</span></span>       | <span data-ttu-id="75f40-113">Int32</span><span class="sxs-lookup"><span data-stu-id="75f40-113">Int32</span></span>  | <span data-ttu-id="75f40-114">缩略图高度，以像素为单位。</span><span class="sxs-lookup"><span data-stu-id="75f40-114">The height of the thumbnail, in pixels.</span></span>
| <span data-ttu-id="75f40-115">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="75f40-115">sourceItemId</span></span> | <span data-ttu-id="75f40-116">字符串</span><span class="sxs-lookup"><span data-stu-id="75f40-116">String</span></span> | <span data-ttu-id="75f40-p101">提供缩略图的项的唯一标识符。仅当请求某个文件夹缩略图时可用。</span><span class="sxs-lookup"><span data-stu-id="75f40-p101">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span>
| <span data-ttu-id="75f40-119">url</span><span class="sxs-lookup"><span data-stu-id="75f40-119">url</span></span>          | <span data-ttu-id="75f40-120">String</span><span class="sxs-lookup"><span data-stu-id="75f40-120">String</span></span> | <span data-ttu-id="75f40-121">用于提取缩略图内容的 URL。</span><span class="sxs-lookup"><span data-stu-id="75f40-121">The URL used to fetch the thumbnail content.</span></span>
| <span data-ttu-id="75f40-122">width</span><span class="sxs-lookup"><span data-stu-id="75f40-122">width</span></span>        | <span data-ttu-id="75f40-123">Int32</span><span class="sxs-lookup"><span data-stu-id="75f40-123">Int32</span></span>  | <span data-ttu-id="75f40-124">缩略图宽度，以像素为单位。</span><span class="sxs-lookup"><span data-stu-id="75f40-124">The width of the thumbnail, in pixels.</span></span>
| <span data-ttu-id="75f40-125">content</span><span class="sxs-lookup"><span data-stu-id="75f40-125">content</span></span>      | <span data-ttu-id="75f40-126">流</span><span class="sxs-lookup"><span data-stu-id="75f40-126">Stream</span></span> | <span data-ttu-id="75f40-127">缩略图的内容流。</span><span class="sxs-lookup"><span data-stu-id="75f40-127">The content stream for the thumbnail.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail"
} -->
