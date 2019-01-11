---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Photo
localization_priority: Normal
ms.openlocfilehash: 4d108e4849595fcb945b676426d3d9c05dfb5ba0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873001"
---
# <a name="photo-resource-type"></a><span data-ttu-id="a0d50-102">Photo 资源类型</span><span class="sxs-lookup"><span data-stu-id="a0d50-102">Photo resource type</span></span>

<span data-ttu-id="a0d50-103">**照片**资源提供 [driveItem](driveitem.md) 中的照片和相机属性，例如 EXIF 元数据。</span><span class="sxs-lookup"><span data-stu-id="a0d50-103">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0d50-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a0d50-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="a0d50-105">属性</span><span class="sxs-lookup"><span data-stu-id="a0d50-105">Properties</span></span>

| <span data-ttu-id="a0d50-106">属性</span><span class="sxs-lookup"><span data-stu-id="a0d50-106">Property</span></span>                | <span data-ttu-id="a0d50-107">类型</span><span class="sxs-lookup"><span data-stu-id="a0d50-107">Type</span></span>           | <span data-ttu-id="a0d50-108">说明</span><span class="sxs-lookup"><span data-stu-id="a0d50-108">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="a0d50-109">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="a0d50-109">**takenDateTime**</span></span>       | <span data-ttu-id="a0d50-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0d50-110">DateTimeOffset</span></span> | <span data-ttu-id="a0d50-p101">表示照片拍摄的时间和日期。只读。</span><span class="sxs-lookup"><span data-stu-id="a0d50-p101">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="a0d50-113">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="a0d50-113">**cameraMake**</span></span>          | <span data-ttu-id="a0d50-114">String</span><span class="sxs-lookup"><span data-stu-id="a0d50-114">String</span></span>         | <span data-ttu-id="a0d50-p102">相机制造商。只读。</span><span class="sxs-lookup"><span data-stu-id="a0d50-p102">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="a0d50-117">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="a0d50-117">**cameraModel**</span></span>         | <span data-ttu-id="a0d50-118">String</span><span class="sxs-lookup"><span data-stu-id="a0d50-118">String</span></span>         | <span data-ttu-id="a0d50-p103">相机型号。只读。</span><span class="sxs-lookup"><span data-stu-id="a0d50-p103">Camera model. Read-only.</span></span>
| <span data-ttu-id="a0d50-121">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="a0d50-121">**fNumber**</span></span>             | <span data-ttu-id="a0d50-122">双精度数</span><span class="sxs-lookup"><span data-stu-id="a0d50-122">Double</span></span>         | <span data-ttu-id="a0d50-p104">相机的 F-stop 值。只读。</span><span class="sxs-lookup"><span data-stu-id="a0d50-p104">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="a0d50-125">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="a0d50-125">**exposureDenominator**</span></span> | <span data-ttu-id="a0d50-126">Double</span><span class="sxs-lookup"><span data-stu-id="a0d50-126">Double</span></span>         | <span data-ttu-id="a0d50-p105">相机的曝光时间分数的分母。只读。</span><span class="sxs-lookup"><span data-stu-id="a0d50-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="a0d50-129">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="a0d50-129">**exposureNumerator**</span></span>   | <span data-ttu-id="a0d50-130">Double</span><span class="sxs-lookup"><span data-stu-id="a0d50-130">Double</span></span>         | <span data-ttu-id="a0d50-p106">相机的曝光时间分数的分子。只读。</span><span class="sxs-lookup"><span data-stu-id="a0d50-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="a0d50-133">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="a0d50-133">**focalLength**</span></span>         | <span data-ttu-id="a0d50-134">双精度数</span><span class="sxs-lookup"><span data-stu-id="a0d50-134">Double</span></span>         | <span data-ttu-id="a0d50-p107">相机的焦距。只读。</span><span class="sxs-lookup"><span data-stu-id="a0d50-p107">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="a0d50-137">**iso**</span><span class="sxs-lookup"><span data-stu-id="a0d50-137">**iso**</span></span>                 | <span data-ttu-id="a0d50-138">Int32</span><span class="sxs-lookup"><span data-stu-id="a0d50-138">Int32</span></span>          | <span data-ttu-id="a0d50-p108">相机的 ISO 值。只读。</span><span class="sxs-lookup"><span data-stu-id="a0d50-p108">The ISO value from the camera. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="a0d50-141">注解</span><span class="sxs-lookup"><span data-stu-id="a0d50-141">Remarks</span></span>

<span data-ttu-id="a0d50-142">OneDrive for Business 和 SharePoint 仅返回 **takenDateTime** 属性。</span><span class="sxs-lookup"><span data-stu-id="a0d50-142">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="a0d50-143">有关 DriveItem 方面的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="a0d50-143">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
