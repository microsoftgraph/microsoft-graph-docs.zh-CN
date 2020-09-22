---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 图像
localization_priority: Normal
description: 图像资源将与图像相关的属性分组到一个单一结构。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e43bf96a34693b19a191d09417623828e1b399be
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086660"
---
# <a name="image-resource-type"></a><span data-ttu-id="7ea4f-103">图像资源类型</span><span class="sxs-lookup"><span data-stu-id="7ea4f-103">Image resource type</span></span>

<span data-ttu-id="7ea4f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ea4f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7ea4f-p101">**图像**资源将与图像相关的属性分组到一个单一结构。如果 [**DriveItem**](driveitem.md)具有一个非 null **图像**方面，则该项表示一个位图图像。</span><span class="sxs-lookup"><span data-stu-id="7ea4f-p101">The **Image** resource groups image-related properties into a single structure. If a [**DriveItem**](driveitem.md) has a non-null **image** facet, the item represents a bitmap image.</span></span>

<span data-ttu-id="7ea4f-107">**注意：** 如果该服务无法确定图像的宽度和高度，**图像**资源可能为空。</span><span class="sxs-lookup"><span data-stu-id="7ea4f-107">**Note:** If the service is unable to determine the width and height of the image, the **Image** resource may be empty.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ea4f-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ea4f-108">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.image" } -->
```json
{
  "width": 100,
  "height": 200
}
```

## <a name="properties"></a><span data-ttu-id="7ea4f-109">属性</span><span class="sxs-lookup"><span data-stu-id="7ea4f-109">Properties</span></span>

| <span data-ttu-id="7ea4f-110">属性</span><span class="sxs-lookup"><span data-stu-id="7ea4f-110">Property</span></span>   | <span data-ttu-id="7ea4f-111">类型</span><span class="sxs-lookup"><span data-stu-id="7ea4f-111">Type</span></span>  | <span data-ttu-id="7ea4f-112">说明</span><span class="sxs-lookup"><span data-stu-id="7ea4f-112">Description</span></span>                                |
|:-----------|:------|:-------------------------------------------|
| <span data-ttu-id="7ea4f-113">**高度**</span><span class="sxs-lookup"><span data-stu-id="7ea4f-113">**height**</span></span> | <span data-ttu-id="7ea4f-114">Int32</span><span class="sxs-lookup"><span data-stu-id="7ea4f-114">Int32</span></span> | <span data-ttu-id="7ea4f-p102">可选。图像的高度，以像素为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="7ea4f-p102">Optional. Height of the image, in pixels. Read-only.</span></span> |
| <span data-ttu-id="7ea4f-118">**width**</span><span class="sxs-lookup"><span data-stu-id="7ea4f-118">**width**</span></span>  | <span data-ttu-id="7ea4f-119">Int32</span><span class="sxs-lookup"><span data-stu-id="7ea4f-119">Int32</span></span> | <span data-ttu-id="7ea4f-p103">可选。图像的宽度，以像素为单位。只读。</span><span class="sxs-lookup"><span data-stu-id="7ea4f-p103">Optional. Width of the image, in pixels. Read-only.</span></span>  |

## <a name="remarks"></a><span data-ttu-id="7ea4f-123">注解</span><span class="sxs-lookup"><span data-stu-id="7ea4f-123">Remarks</span></span>

<span data-ttu-id="7ea4f-124">在 OneDrive for Business 中，基于文件扩展名在应为图像的项中返回此类资源。</span><span class="sxs-lookup"><span data-stu-id="7ea4f-124">In OneDrive for Business, this resource is returned on items that are expected to be images based on file extension.</span></span>

<span data-ttu-id="7ea4f-125">有关 DriveItem 上 Facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="7ea4f-125">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The image facet describes properties of an image like width and height",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Image"
} -->

