---
author: JeremyKelley
description: 图像资源将与图像相关的属性分组到一个单一结构。
ms.date: 09/10/2017
title: 图像
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: c41925443820b96098c03de00f4c3741da0cec95
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973511"
---
# <a name="image-resource-type"></a><span data-ttu-id="ea9d3-103">图像资源类型</span><span class="sxs-lookup"><span data-stu-id="ea9d3-103">Image resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea9d3-p101">**图像**资源将与图像相关的属性分组到一个单一结构。如果 [**DriveItem**](driveitem.md)具有一个非 null **图像**方面，则该项表示一个位图图像。</span><span class="sxs-lookup"><span data-stu-id="ea9d3-p101">The **Image** resource groups image-related properties into a single structure. If a [**DriveItem**](driveitem.md) has a non-null **image** facet, the item represents a bitmap image.</span></span>

<span data-ttu-id="ea9d3-106">**注意：** 如果该服务无法确定图像的宽度和高度，**图像**资源可能为空。</span><span class="sxs-lookup"><span data-stu-id="ea9d3-106">**Note:** If the service is unable to determine the width and height of the image, the **Image** resource may be empty.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea9d3-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ea9d3-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.image" } -->
```json
{
  "width": 100,
  "height": 200
}
```

## <a name="properties"></a><span data-ttu-id="ea9d3-108">属性</span><span class="sxs-lookup"><span data-stu-id="ea9d3-108">Properties</span></span>

| <span data-ttu-id="ea9d3-109">属性</span><span class="sxs-lookup"><span data-stu-id="ea9d3-109">Property</span></span>   | <span data-ttu-id="ea9d3-110">类型</span><span class="sxs-lookup"><span data-stu-id="ea9d3-110">Type</span></span>  | <span data-ttu-id="ea9d3-111">说明</span><span class="sxs-lookup"><span data-stu-id="ea9d3-111">Description</span></span>                                |
|:-----------|:------|:-------------------------------------------|
| <span data-ttu-id="ea9d3-112">**高度**</span><span class="sxs-lookup"><span data-stu-id="ea9d3-112">**height**</span></span> | <span data-ttu-id="ea9d3-113">Int32</span><span class="sxs-lookup"><span data-stu-id="ea9d3-113">Int32</span></span> | <span data-ttu-id="ea9d3-p102">可选。图像的高度，以像素为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="ea9d3-p102">Optional. Height of the image, in pixels. Read-only.</span></span> |
| <span data-ttu-id="ea9d3-117">**width**</span><span class="sxs-lookup"><span data-stu-id="ea9d3-117">**width**</span></span>  | <span data-ttu-id="ea9d3-118">Int32</span><span class="sxs-lookup"><span data-stu-id="ea9d3-118">Int32</span></span> | <span data-ttu-id="ea9d3-p103">可选。图像的宽度，以像素为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="ea9d3-p103">Optional. Width of the image, in pixels. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="ea9d3-122">注解</span><span class="sxs-lookup"><span data-stu-id="ea9d3-122">Remarks</span></span>

<span data-ttu-id="ea9d3-123">在 OneDrive for Business 中，基于文件扩展名在应为图像的项中返回此类资源。</span><span class="sxs-lookup"><span data-stu-id="ea9d3-123">In OneDrive for Business, this resource is returned on items that are expected to be images based on file extension.</span></span>

<span data-ttu-id="ea9d3-124">有关 DriveItem 上 Facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="ea9d3-124">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "The image facet describes properties of an image like width and height",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Image",
  "suppressions": []
}
-->
