---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 图像
localization_priority: Normal
ms.openlocfilehash: a817f5b91c71d186fde1ae1ea0600b9645fe8a66
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339979"
---
# <a name="image-resource-type"></a><span data-ttu-id="bcf1c-102">图像资源类型</span><span class="sxs-lookup"><span data-stu-id="bcf1c-102">Image resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bcf1c-p101">**图像**资源将与图像相关的属性分组到一个单一结构。如果 [**DriveItem**](driveitem.md)具有一个非 null **图像**方面，则该项表示一个位图图像。</span><span class="sxs-lookup"><span data-stu-id="bcf1c-p101">The **Image** resource groups image-related properties into a single structure. If a [**DriveItem**](driveitem.md) has a non-null **image** facet, the item represents a bitmap image.</span></span>

<span data-ttu-id="bcf1c-105">**注意：** 如果该服务无法确定图像的宽度和高度，**图像**资源可能为空。</span><span class="sxs-lookup"><span data-stu-id="bcf1c-105">**Note:** If the service is unable to determine the width and height of the image, the **Image** resource may be empty.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bcf1c-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bcf1c-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.image" } -->
```json
{
  "width": 100,
  "height": 200
}
```

## <a name="properties"></a><span data-ttu-id="bcf1c-107">属性</span><span class="sxs-lookup"><span data-stu-id="bcf1c-107">Properties</span></span>

| <span data-ttu-id="bcf1c-108">属性</span><span class="sxs-lookup"><span data-stu-id="bcf1c-108">Property</span></span>   | <span data-ttu-id="bcf1c-109">类型</span><span class="sxs-lookup"><span data-stu-id="bcf1c-109">Type</span></span>  | <span data-ttu-id="bcf1c-110">说明</span><span class="sxs-lookup"><span data-stu-id="bcf1c-110">Description</span></span>                                |
|:-----------|:------|:-------------------------------------------|
| <span data-ttu-id="bcf1c-111">**高度**</span><span class="sxs-lookup"><span data-stu-id="bcf1c-111">**height**</span></span> | <span data-ttu-id="bcf1c-112">Int32</span><span class="sxs-lookup"><span data-stu-id="bcf1c-112">Int32</span></span> | <span data-ttu-id="bcf1c-p102">可选。图像的高度，以像素为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="bcf1c-p102">Optional. Height of the image, in pixels. Read-only.</span></span> |
| <span data-ttu-id="bcf1c-116">**width**</span><span class="sxs-lookup"><span data-stu-id="bcf1c-116">**width**</span></span>  | <span data-ttu-id="bcf1c-117">Int32</span><span class="sxs-lookup"><span data-stu-id="bcf1c-117">Int32</span></span> | <span data-ttu-id="bcf1c-p103">可选。图像的宽度，以像素为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="bcf1c-p103">Optional. Width of the image, in pixels. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="bcf1c-121">注解</span><span class="sxs-lookup"><span data-stu-id="bcf1c-121">Remarks</span></span>

<span data-ttu-id="bcf1c-122">在 OneDrive for Business 中，基于文件扩展名在应为图像的项中返回此类资源。</span><span class="sxs-lookup"><span data-stu-id="bcf1c-122">In OneDrive for Business, this resource is returned on items that are expected to be images based on file extension.</span></span>

<span data-ttu-id="bcf1c-123">有关 DriveItem 上 Facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="bcf1c-123">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


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
