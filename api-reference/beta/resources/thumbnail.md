---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 缩略图
localization_priority: Normal
ms.openlocfilehash: 05fcb6ec4b0821a4243692aab9c15419eb2f630d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529752"
---
# <a name="thumbnail-resource-type"></a><span data-ttu-id="60132-102">Thumbnail 资源类型</span><span class="sxs-lookup"><span data-stu-id="60132-102">Thumbnail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60132-103">**缩略图**资源类型表示具有位图表示的图像、视频、文档 或任何项目的缩略图。</span><span class="sxs-lookup"><span data-stu-id="60132-103">The **thumbnail** resource type represents a thumbnail for an image, video, document, or any item that has a bitmap representation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="60132-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="60132-104">JSON representation</span></span>

<span data-ttu-id="60132-105">下面是**缩略图**资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60132-105">Here is a JSON representation of the **thumbnail** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="60132-106">属性</span><span class="sxs-lookup"><span data-stu-id="60132-106">Properties</span></span>

| <span data-ttu-id="60132-107">属性</span><span class="sxs-lookup"><span data-stu-id="60132-107">Property</span></span>     | <span data-ttu-id="60132-108">类型</span><span class="sxs-lookup"><span data-stu-id="60132-108">Type</span></span>   | <span data-ttu-id="60132-109">说明</span><span class="sxs-lookup"><span data-stu-id="60132-109">Description</span></span>                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="60132-110">height</span><span class="sxs-lookup"><span data-stu-id="60132-110">height</span></span>       | <span data-ttu-id="60132-111">Int32</span><span class="sxs-lookup"><span data-stu-id="60132-111">Int32</span></span>  | <span data-ttu-id="60132-112">缩略图高度，以像素为单位。</span><span class="sxs-lookup"><span data-stu-id="60132-112">The height of the thumbnail, in pixels.</span></span>                                                                                     |
| <span data-ttu-id="60132-113">sourceItemId</span><span class="sxs-lookup"><span data-stu-id="60132-113">sourceItemId</span></span> | <span data-ttu-id="60132-114">字符串</span><span class="sxs-lookup"><span data-stu-id="60132-114">String</span></span> | <span data-ttu-id="60132-p101">提供缩略图的项的唯一标识符。仅当请求某个文件夹缩略图时可用。</span><span class="sxs-lookup"><span data-stu-id="60132-p101">The unique identifier of the item that provided the thumbnail. This is only available when a folder thumbnail is requested.</span></span> |
| <span data-ttu-id="60132-117">url</span><span class="sxs-lookup"><span data-stu-id="60132-117">url</span></span>          | <span data-ttu-id="60132-118">String</span><span class="sxs-lookup"><span data-stu-id="60132-118">String</span></span> | <span data-ttu-id="60132-119">用于提取缩略图内容的 URL。</span><span class="sxs-lookup"><span data-stu-id="60132-119">The URL used to fetch the thumbnail content.</span></span>                                                                                |
| <span data-ttu-id="60132-120">width</span><span class="sxs-lookup"><span data-stu-id="60132-120">width</span></span>        | <span data-ttu-id="60132-121">Int32</span><span class="sxs-lookup"><span data-stu-id="60132-121">Int32</span></span>  | <span data-ttu-id="60132-122">缩略图宽度，以像素为单位。</span><span class="sxs-lookup"><span data-stu-id="60132-122">The width of the thumbnail, in pixels.</span></span>                                                                                      |

## <a name="relationships"></a><span data-ttu-id="60132-123">关系</span><span class="sxs-lookup"><span data-stu-id="60132-123">Relationships</span></span>

| <span data-ttu-id="60132-124">名称</span><span class="sxs-lookup"><span data-stu-id="60132-124">Name</span></span>    | <span data-ttu-id="60132-125">类型</span><span class="sxs-lookup"><span data-stu-id="60132-125">Type</span></span>   | <span data-ttu-id="60132-126">说明</span><span class="sxs-lookup"><span data-stu-id="60132-126">Description</span></span>                           |
| :------ | :----- | :------------------------------------ |
| <span data-ttu-id="60132-127">内容</span><span class="sxs-lookup"><span data-stu-id="60132-127">content</span></span> | <span data-ttu-id="60132-128">流</span><span class="sxs-lookup"><span data-stu-id="60132-128">Stream</span></span> | <span data-ttu-id="60132-129">缩略图的内容流。</span><span class="sxs-lookup"><span data-stu-id="60132-129">The content stream for the thumbnail.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail",
  "suppressions": [
    "Error: /api-reference/beta/resources/thumbnail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
