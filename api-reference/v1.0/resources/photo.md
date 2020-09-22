---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Photo
localization_priority: Normal
description: 照片资源提供 driveItem 中的照片和相机属性，例如 EXIF 元数据。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 362d4f76f56fa5824985a3580d6008d8c5081a7c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48072849"
---
# <a name="photo-resource-type"></a><span data-ttu-id="e5d22-103">Photo 资源类型</span><span class="sxs-lookup"><span data-stu-id="e5d22-103">Photo resource type</span></span>

<span data-ttu-id="e5d22-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5d22-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e5d22-105">**照片**资源提供 [driveItem](driveitem.md) 中的照片和相机属性，例如 EXIF 元数据。</span><span class="sxs-lookup"><span data-stu-id="e5d22-105">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5d22-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e5d22-106">JSON representation</span></span>

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
  "orientation": 3,
  "takenDateTime": "String (timestamp)"
}
```

## <a name="properties"></a><span data-ttu-id="e5d22-107">属性</span><span class="sxs-lookup"><span data-stu-id="e5d22-107">Properties</span></span>

| <span data-ttu-id="e5d22-108">属性</span><span class="sxs-lookup"><span data-stu-id="e5d22-108">Property</span></span>                | <span data-ttu-id="e5d22-109">类型</span><span class="sxs-lookup"><span data-stu-id="e5d22-109">Type</span></span>           | <span data-ttu-id="e5d22-110">说明</span><span class="sxs-lookup"><span data-stu-id="e5d22-110">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="e5d22-111">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="e5d22-111">**takenDateTime**</span></span>       | <span data-ttu-id="e5d22-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5d22-112">DateTimeOffset</span></span> | <span data-ttu-id="e5d22-p101">表示照片拍摄的时间和日期。只读。</span><span class="sxs-lookup"><span data-stu-id="e5d22-p101">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="e5d22-115">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="e5d22-115">**cameraMake**</span></span>          | <span data-ttu-id="e5d22-116">String</span><span class="sxs-lookup"><span data-stu-id="e5d22-116">String</span></span>         | <span data-ttu-id="e5d22-p102">相机制造商。只读。</span><span class="sxs-lookup"><span data-stu-id="e5d22-p102">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="e5d22-119">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="e5d22-119">**cameraModel**</span></span>         | <span data-ttu-id="e5d22-120">String</span><span class="sxs-lookup"><span data-stu-id="e5d22-120">String</span></span>         | <span data-ttu-id="e5d22-p103">相机型号。只读。</span><span class="sxs-lookup"><span data-stu-id="e5d22-p103">Camera model. Read-only.</span></span>
| <span data-ttu-id="e5d22-123">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="e5d22-123">**fNumber**</span></span>             | <span data-ttu-id="e5d22-124">Double</span><span class="sxs-lookup"><span data-stu-id="e5d22-124">Double</span></span>         | <span data-ttu-id="e5d22-p104">相机的 F-stop 值。只读。</span><span class="sxs-lookup"><span data-stu-id="e5d22-p104">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="e5d22-127">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="e5d22-127">**exposureDenominator**</span></span> | <span data-ttu-id="e5d22-128">Double</span><span class="sxs-lookup"><span data-stu-id="e5d22-128">Double</span></span>         | <span data-ttu-id="e5d22-p105">相机的曝光时间分数的分母。只读。</span><span class="sxs-lookup"><span data-stu-id="e5d22-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="e5d22-131">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="e5d22-131">**exposureNumerator**</span></span>   | <span data-ttu-id="e5d22-132">Double</span><span class="sxs-lookup"><span data-stu-id="e5d22-132">Double</span></span>         | <span data-ttu-id="e5d22-p106">相机的曝光时间分数的分子。只读。</span><span class="sxs-lookup"><span data-stu-id="e5d22-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="e5d22-135">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="e5d22-135">**focalLength**</span></span>         | <span data-ttu-id="e5d22-136">Double</span><span class="sxs-lookup"><span data-stu-id="e5d22-136">Double</span></span>         | <span data-ttu-id="e5d22-p107">相机的焦距。只读。</span><span class="sxs-lookup"><span data-stu-id="e5d22-p107">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="e5d22-139">**iso**</span><span class="sxs-lookup"><span data-stu-id="e5d22-139">**iso**</span></span>                 | <span data-ttu-id="e5d22-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e5d22-140">Int32</span></span>          | <span data-ttu-id="e5d22-p108">相机的 ISO 值。只读。</span><span class="sxs-lookup"><span data-stu-id="e5d22-p108">The ISO value from the camera. Read-only.</span></span>
| <span data-ttu-id="e5d22-143">**orientation**</span><span class="sxs-lookup"><span data-stu-id="e5d22-143">**orientation**</span></span>         | <span data-ttu-id="e5d22-144">Int16</span><span class="sxs-lookup"><span data-stu-id="e5d22-144">Int16</span></span>          | <span data-ttu-id="e5d22-145">相机中的方向值。</span><span class="sxs-lookup"><span data-stu-id="e5d22-145">The orientation value from the camera.</span></span> <span data-ttu-id="e5d22-146">在 OneDrive 个人版上是可写的。</span><span class="sxs-lookup"><span data-stu-id="e5d22-146">Writable on OneDrive Personal.</span></span>      |

## <a name="remarks"></a><span data-ttu-id="e5d22-147">注解</span><span class="sxs-lookup"><span data-stu-id="e5d22-147">Remarks</span></span>

<span data-ttu-id="e5d22-148">OneDrive for Business 和 SharePoint 仅返回 **takenDateTime** 属性。</span><span class="sxs-lookup"><span data-stu-id="e5d22-148">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="e5d22-149">有关 DriveItem 方面的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="e5d22-149">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso, orientation",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->

