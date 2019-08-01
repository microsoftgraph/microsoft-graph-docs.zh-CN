---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Photo
localization_priority: Normal
description: 照片资源提供 driveItem 中的照片和相机属性，例如 EXIF 元数据。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c86190768c10b04bb55f59104368089cf7c77b18
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035496"
---
# <a name="photo-resource-type"></a><span data-ttu-id="799d5-103">Photo 资源类型</span><span class="sxs-lookup"><span data-stu-id="799d5-103">Photo resource type</span></span>

<span data-ttu-id="799d5-104">**照片**资源提供 [driveItem](driveitem.md) 中的照片和相机属性，例如 EXIF 元数据。</span><span class="sxs-lookup"><span data-stu-id="799d5-104">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="799d5-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="799d5-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="799d5-106">属性</span><span class="sxs-lookup"><span data-stu-id="799d5-106">Properties</span></span>

| <span data-ttu-id="799d5-107">属性</span><span class="sxs-lookup"><span data-stu-id="799d5-107">Property</span></span>                | <span data-ttu-id="799d5-108">类型</span><span class="sxs-lookup"><span data-stu-id="799d5-108">Type</span></span>           | <span data-ttu-id="799d5-109">说明</span><span class="sxs-lookup"><span data-stu-id="799d5-109">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="799d5-110">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="799d5-110">**takenDateTime**</span></span>       | <span data-ttu-id="799d5-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="799d5-111">DateTimeOffset</span></span> | <span data-ttu-id="799d5-p101">表示照片拍摄的时间和日期。只读。</span><span class="sxs-lookup"><span data-stu-id="799d5-p101">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="799d5-114">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="799d5-114">**cameraMake**</span></span>          | <span data-ttu-id="799d5-115">String</span><span class="sxs-lookup"><span data-stu-id="799d5-115">String</span></span>         | <span data-ttu-id="799d5-p102">相机制造商。只读。</span><span class="sxs-lookup"><span data-stu-id="799d5-p102">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="799d5-118">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="799d5-118">**cameraModel**</span></span>         | <span data-ttu-id="799d5-119">String</span><span class="sxs-lookup"><span data-stu-id="799d5-119">String</span></span>         | <span data-ttu-id="799d5-p103">相机型号。只读。</span><span class="sxs-lookup"><span data-stu-id="799d5-p103">Camera model. Read-only.</span></span>
| <span data-ttu-id="799d5-122">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="799d5-122">**fNumber**</span></span>             | <span data-ttu-id="799d5-123">双精度</span><span class="sxs-lookup"><span data-stu-id="799d5-123">Double</span></span>         | <span data-ttu-id="799d5-p104">相机的 F-stop 值。只读。</span><span class="sxs-lookup"><span data-stu-id="799d5-p104">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="799d5-126">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="799d5-126">**exposureDenominator**</span></span> | <span data-ttu-id="799d5-127">双精度</span><span class="sxs-lookup"><span data-stu-id="799d5-127">Double</span></span>         | <span data-ttu-id="799d5-p105">相机的曝光时间分数的分母。只读。</span><span class="sxs-lookup"><span data-stu-id="799d5-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="799d5-130">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="799d5-130">**exposureNumerator**</span></span>   | <span data-ttu-id="799d5-131">Double</span><span class="sxs-lookup"><span data-stu-id="799d5-131">Double</span></span>         | <span data-ttu-id="799d5-p106">相机的曝光时间分数的分子。只读。</span><span class="sxs-lookup"><span data-stu-id="799d5-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="799d5-134">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="799d5-134">**focalLength**</span></span>         | <span data-ttu-id="799d5-135">双精度数</span><span class="sxs-lookup"><span data-stu-id="799d5-135">Double</span></span>         | <span data-ttu-id="799d5-p107">相机的焦距。只读。</span><span class="sxs-lookup"><span data-stu-id="799d5-p107">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="799d5-138">**iso**</span><span class="sxs-lookup"><span data-stu-id="799d5-138">**iso**</span></span>                 | <span data-ttu-id="799d5-139">Int32</span><span class="sxs-lookup"><span data-stu-id="799d5-139">Int32</span></span>          | <span data-ttu-id="799d5-p108">相机的 ISO 值。只读。</span><span class="sxs-lookup"><span data-stu-id="799d5-p108">The ISO value from the camera. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="799d5-142">注解</span><span class="sxs-lookup"><span data-stu-id="799d5-142">Remarks</span></span>

<span data-ttu-id="799d5-143">OneDrive for Business 和 SharePoint 仅返回 **takenDateTime** 属性。</span><span class="sxs-lookup"><span data-stu-id="799d5-143">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="799d5-144">有关 DriveItem 方面的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="799d5-144">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
