---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Image
ms.openlocfilehash: c9e647ef630e8822d835aec1bd72b9f3c18f2e3e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046529"
---
# <a name="image-resource-type"></a><span data-ttu-id="e47b2-102">图像资源类型</span><span class="sxs-lookup"><span data-stu-id="e47b2-102">Image resource type</span></span>

> <span data-ttu-id="e47b2-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e47b2-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e47b2-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e47b2-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e47b2-p102">**图像**资源将与图像相关的属性分组到一个单一结构。如果 [**DriveItem**](driveitem.md)具有一个非 null **图像**方面，则该项表示一个位图图像。</span><span class="sxs-lookup"><span data-stu-id="e47b2-p102">The **Image** resource groups image-related properties into a single structure. If a [**DriveItem**](driveitem.md) has a non-null **image** facet, the item represents a bitmap image.</span></span>

<span data-ttu-id="e47b2-107">**注意：** 如果该服务无法确定图像的宽度和高度，**图像**资源可能为空。</span><span class="sxs-lookup"><span data-stu-id="e47b2-107">**Note:** If the service is unable to determine the width and height of the image, the **Image** resource may be empty.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e47b2-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e47b2-108">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.image" } -->
```json
{
  "width": 100,
  "height": 200
}
```

## <a name="properties"></a><span data-ttu-id="e47b2-109">属性</span><span class="sxs-lookup"><span data-stu-id="e47b2-109">Properties</span></span>

| <span data-ttu-id="e47b2-110">属性</span><span class="sxs-lookup"><span data-stu-id="e47b2-110">Property</span></span>   | <span data-ttu-id="e47b2-111">类型</span><span class="sxs-lookup"><span data-stu-id="e47b2-111">Type</span></span>  | <span data-ttu-id="e47b2-112">说明</span><span class="sxs-lookup"><span data-stu-id="e47b2-112">Description</span></span>                                |
|:-----------|:------|:-------------------------------------------|
| <span data-ttu-id="e47b2-113">**高度**</span><span class="sxs-lookup"><span data-stu-id="e47b2-113">**height**</span></span> | <span data-ttu-id="e47b2-114">Int32</span><span class="sxs-lookup"><span data-stu-id="e47b2-114">Int32</span></span> | <span data-ttu-id="e47b2-p103">可选。图像的高度，以像素为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="e47b2-p103">Optional. Height of the image, in pixels. Read-only.</span></span> |
| <span data-ttu-id="e47b2-118">**width**</span><span class="sxs-lookup"><span data-stu-id="e47b2-118">**width**</span></span>  | <span data-ttu-id="e47b2-119">Int32</span><span class="sxs-lookup"><span data-stu-id="e47b2-119">Int32</span></span> | <span data-ttu-id="e47b2-p104">可选。图像的宽度，以像素为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="e47b2-p104">Optional. Width of the image, in pixels. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="e47b2-123">注解</span><span class="sxs-lookup"><span data-stu-id="e47b2-123">Remarks</span></span>

<span data-ttu-id="e47b2-124">在 OneDrive for Business 中，基于文件扩展名在应为图像的项中返回此类资源。</span><span class="sxs-lookup"><span data-stu-id="e47b2-124">In OneDrive for Business, this resource is returned on items that are expected to be images based on file extension.</span></span>

<span data-ttu-id="e47b2-125">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="e47b2-125">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The image facet describes properties of an image like width and height",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Image"
} -->
