---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Photo
localization_priority: Normal
ms.openlocfilehash: 688bee72464c1e518c60720a7f9ca24da1f7d149
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480976"
---
# <a name="photo-resource-type"></a><span data-ttu-id="a7243-102">Photo 资源类型</span><span class="sxs-lookup"><span data-stu-id="a7243-102">Photo resource type</span></span>

<span data-ttu-id="a7243-103">**照片**资源提供 [driveItem](driveitem.md) 中的照片和相机属性，例如 EXIF 元数据。</span><span class="sxs-lookup"><span data-stu-id="a7243-103">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7243-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a7243-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.photo"
}-->

```json
{
  "cameraMake": "string",
  "cameraModel": "string",
  "exposureDenominator": 1000.0,
  "exposureNumerator": 1.0,
  "fNumber": 1.8,
  "focalLength": 22.5,
  "iso": 100,
  "takenDateTime": "String (timestamp)"
}
```

## <a name="properties"></a><span data-ttu-id="a7243-105">属性</span><span class="sxs-lookup"><span data-stu-id="a7243-105">Properties</span></span>

| <span data-ttu-id="a7243-106">属性</span><span class="sxs-lookup"><span data-stu-id="a7243-106">Property</span></span>                | <span data-ttu-id="a7243-107">类型</span><span class="sxs-lookup"><span data-stu-id="a7243-107">Type</span></span>           | <span data-ttu-id="a7243-108">说明</span><span class="sxs-lookup"><span data-stu-id="a7243-108">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="a7243-109">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="a7243-109">**takenDateTime**</span></span>       | <span data-ttu-id="a7243-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7243-110">DateTimeOffset</span></span> | <span data-ttu-id="a7243-p101">表示照片拍摄的时间和日期。只读。</span><span class="sxs-lookup"><span data-stu-id="a7243-p101">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="a7243-113">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="a7243-113">**cameraMake**</span></span>          | <span data-ttu-id="a7243-114">String</span><span class="sxs-lookup"><span data-stu-id="a7243-114">String</span></span>         | <span data-ttu-id="a7243-p102">相机制造商。只读。</span><span class="sxs-lookup"><span data-stu-id="a7243-p102">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="a7243-117">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="a7243-117">**cameraModel**</span></span>         | <span data-ttu-id="a7243-118">String</span><span class="sxs-lookup"><span data-stu-id="a7243-118">String</span></span>         | <span data-ttu-id="a7243-p103">相机型号。只读。</span><span class="sxs-lookup"><span data-stu-id="a7243-p103">Camera model. Read-only.</span></span>
| <span data-ttu-id="a7243-121">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="a7243-121">**fNumber**</span></span>             | <span data-ttu-id="a7243-122">双精度数</span><span class="sxs-lookup"><span data-stu-id="a7243-122">Double</span></span>         | <span data-ttu-id="a7243-p104">相机的 F-stop 值。只读。</span><span class="sxs-lookup"><span data-stu-id="a7243-p104">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="a7243-125">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="a7243-125">**exposureDenominator**</span></span> | <span data-ttu-id="a7243-126">双精度数</span><span class="sxs-lookup"><span data-stu-id="a7243-126">Double</span></span>         | <span data-ttu-id="a7243-p105">相机的曝光时间分数的分母。只读。</span><span class="sxs-lookup"><span data-stu-id="a7243-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="a7243-129">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="a7243-129">**exposureNumerator**</span></span>   | <span data-ttu-id="a7243-130">Double</span><span class="sxs-lookup"><span data-stu-id="a7243-130">Double</span></span>         | <span data-ttu-id="a7243-p106">相机的曝光时间分数的分子。只读。</span><span class="sxs-lookup"><span data-stu-id="a7243-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="a7243-133">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="a7243-133">**focalLength**</span></span>         | <span data-ttu-id="a7243-134">双精度数</span><span class="sxs-lookup"><span data-stu-id="a7243-134">Double</span></span>         | <span data-ttu-id="a7243-p107">相机的焦距。只读。</span><span class="sxs-lookup"><span data-stu-id="a7243-p107">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="a7243-137">**iso**</span><span class="sxs-lookup"><span data-stu-id="a7243-137">**iso**</span></span>                 | <span data-ttu-id="a7243-138">Int32</span><span class="sxs-lookup"><span data-stu-id="a7243-138">Int32</span></span>          | <span data-ttu-id="a7243-p108">相机的 ISO 值。只读。</span><span class="sxs-lookup"><span data-stu-id="a7243-p108">The ISO value from the camera. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="a7243-141">注解</span><span class="sxs-lookup"><span data-stu-id="a7243-141">Remarks</span></span>

<span data-ttu-id="a7243-142">OneDrive for Business 和 SharePoint 仅返回 **takenDateTime** 属性。</span><span class="sxs-lookup"><span data-stu-id="a7243-142">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="a7243-143">有关 DriveItem 方面的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="a7243-143">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
