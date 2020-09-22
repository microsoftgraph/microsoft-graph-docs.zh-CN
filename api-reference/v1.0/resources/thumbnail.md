---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 缩略图
localization_priority: Normal
description: 缩略图资源类型表示具有位图表示的图像、视频、文档 或任何项目的缩略图。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a7415a8d1c288ce65e87cb1a8653d2f7676222c7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090870"
---
# <a name="thumbnail-resource-type"></a><span data-ttu-id="11635-103">Thumbnail 资源类型</span><span class="sxs-lookup"><span data-stu-id="11635-103">Thumbnail resource type</span></span>

<span data-ttu-id="11635-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11635-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="11635-105">**缩略图**资源类型表示具有位图表示的图像、视频、文档 或任何项目的缩略图。</span><span class="sxs-lookup"><span data-stu-id="11635-105">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="11635-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="11635-106">JSON representation</span></span>

<span data-ttu-id="11635-107">下面是**缩略图**资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="11635-107">Here is a JSON representation of the **thumbnail** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="11635-108">属性</span><span class="sxs-lookup"><span data-stu-id="11635-108">Properties</span></span>

| <span data-ttu-id="11635-109">属性</span><span class="sxs-lookup"><span data-stu-id="11635-109">Property</span></span>     | <span data-ttu-id="11635-110">类型</span><span class="sxs-lookup"><span data-stu-id="11635-110">Type</span></span>   | <span data-ttu-id="11635-111">说明</span><span class="sxs-lookup"><span data-stu-id="11635-111">Description</span></span>
| :----------- | :----- | :----------------------------------------------------
| <span data-ttu-id="11635-112">height</span><span class="sxs-lookup"><span data-stu-id="11635-112">height</span></span>       | <span data-ttu-id="11635-113">Int32</span><span class="sxs-lookup"><span data-stu-id="11635-113">Int32</span></span>  | <span data-ttu-id="11635-114">缩略图高度，以像素为单位。</span><span class="sxs-lookup"><span data-stu-id="11635-114">The height of the thumbnail, in pixels.</span></span>
| <span data-ttu-id="11635-115">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="11635-115">sourceItemId</span></span> | <span data-ttu-id="11635-116">字符串</span><span class="sxs-lookup"><span data-stu-id="11635-116">String</span></span> | <span data-ttu-id="11635-p101">提供缩略图的项的唯一标识符。仅当请求某个文件夹缩略图时可用。</span><span class="sxs-lookup"><span data-stu-id="11635-p101">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span>
| <span data-ttu-id="11635-119">url</span><span class="sxs-lookup"><span data-stu-id="11635-119">url</span></span>          | <span data-ttu-id="11635-120">String</span><span class="sxs-lookup"><span data-stu-id="11635-120">String</span></span> | <span data-ttu-id="11635-121">用于提取缩略图内容的 URL。</span><span class="sxs-lookup"><span data-stu-id="11635-121">The URL used to fetch the thumbnail content.</span></span>
| <span data-ttu-id="11635-122">width</span><span class="sxs-lookup"><span data-stu-id="11635-122">width</span></span>        | <span data-ttu-id="11635-123">Int32</span><span class="sxs-lookup"><span data-stu-id="11635-123">Int32</span></span>  | <span data-ttu-id="11635-124">缩略图宽度，以像素为单位。</span><span class="sxs-lookup"><span data-stu-id="11635-124">The width of the thumbnail, in pixels.</span></span>
| <span data-ttu-id="11635-125">content</span><span class="sxs-lookup"><span data-stu-id="11635-125">content</span></span>      | <span data-ttu-id="11635-126">流</span><span class="sxs-lookup"><span data-stu-id="11635-126">Stream</span></span> | <span data-ttu-id="11635-127">缩略图的内容流。</span><span class="sxs-lookup"><span data-stu-id="11635-127">The content stream for the thumbnail.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail"
} -->

