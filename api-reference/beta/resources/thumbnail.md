---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 缩略图
ms.openlocfilehash: 8e56612185028891cf380d3240c999af78ff4740
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044978"
---
# <a name="thumbnail-resource-type"></a><span data-ttu-id="19410-102">Thumbnail 资源类型</span><span class="sxs-lookup"><span data-stu-id="19410-102">Thumbnail resource type</span></span>

> <span data-ttu-id="19410-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="19410-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19410-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="19410-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="19410-105">**缩略图**资源类型表示具有位图表示的图像、视频、文档 或任何项目的缩略图。</span><span class="sxs-lookup"><span data-stu-id="19410-105">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="19410-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="19410-106">JSON representation</span></span>

<span data-ttu-id="19410-107">下面是**缩略图**资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="19410-107">Here is a JSON representation of the **thumbnail** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="19410-108">属性</span><span class="sxs-lookup"><span data-stu-id="19410-108">Properties</span></span>

| <span data-ttu-id="19410-109">属性</span><span class="sxs-lookup"><span data-stu-id="19410-109">Property</span></span>     | <span data-ttu-id="19410-110">类型</span><span class="sxs-lookup"><span data-stu-id="19410-110">Type</span></span>   | <span data-ttu-id="19410-111">说明</span><span class="sxs-lookup"><span data-stu-id="19410-111">Description</span></span>                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="19410-112">height</span><span class="sxs-lookup"><span data-stu-id="19410-112">height</span></span>       | <span data-ttu-id="19410-113">Int32</span><span class="sxs-lookup"><span data-stu-id="19410-113">Int32</span></span>  | <span data-ttu-id="19410-114">缩略图高度，以像素为单位。</span><span class="sxs-lookup"><span data-stu-id="19410-114">The height of the thumbnail, in pixels.</span></span>                                                                                     |
| <span data-ttu-id="19410-115">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="19410-115">sourceItemId</span></span> | <span data-ttu-id="19410-116">字符串</span><span class="sxs-lookup"><span data-stu-id="19410-116">String</span></span> | <span data-ttu-id="19410-p102">提供缩略图的项的唯一标识符。仅当请求某个文件夹缩略图时可用。</span><span class="sxs-lookup"><span data-stu-id="19410-p102">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span> |
| <span data-ttu-id="19410-119">url</span><span class="sxs-lookup"><span data-stu-id="19410-119">url</span></span>          | <span data-ttu-id="19410-120">String</span><span class="sxs-lookup"><span data-stu-id="19410-120">String</span></span> | <span data-ttu-id="19410-121">用于提取缩略图内容的 URL。</span><span class="sxs-lookup"><span data-stu-id="19410-121">The URL used to fetch the thumbnail content.</span></span>                                                                                |
| <span data-ttu-id="19410-122">width</span><span class="sxs-lookup"><span data-stu-id="19410-122">width</span></span>        | <span data-ttu-id="19410-123">Int32</span><span class="sxs-lookup"><span data-stu-id="19410-123">Int32</span></span>  | <span data-ttu-id="19410-124">缩略图宽度，以像素为单位。</span><span class="sxs-lookup"><span data-stu-id="19410-124">The width of the thumbnail, in pixels.</span></span>                                                                                      |

## <a name="relationships"></a><span data-ttu-id="19410-125">Relationships</span><span class="sxs-lookup"><span data-stu-id="19410-125">Relationships</span></span>

| <span data-ttu-id="19410-126">名称</span><span class="sxs-lookup"><span data-stu-id="19410-126">Name</span></span>    | <span data-ttu-id="19410-127">类型</span><span class="sxs-lookup"><span data-stu-id="19410-127">Type</span></span>   | <span data-ttu-id="19410-128">说明</span><span class="sxs-lookup"><span data-stu-id="19410-128">Description</span></span>                           |
| :------ | :----- | :------------------------------------ |
| <span data-ttu-id="19410-129">内容</span><span class="sxs-lookup"><span data-stu-id="19410-129">content</span></span> | <span data-ttu-id="19410-130">流</span><span class="sxs-lookup"><span data-stu-id="19410-130">Stream</span></span> | <span data-ttu-id="19410-131">缩略图的内容流。</span><span class="sxs-lookup"><span data-stu-id="19410-131">The content stream for the thumbnail.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail"
} -->
