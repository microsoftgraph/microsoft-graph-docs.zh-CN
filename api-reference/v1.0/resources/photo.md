---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Photo
localization_priority: Normal
description: 照片资源提供 driveItem 中的照片和相机属性，例如 EXIF 元数据。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a62a138cbd48645b6b296abcde72af0cef19e259
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863731"
---
# <a name="photo-resource-type"></a><span data-ttu-id="8d872-103">Photo 资源类型</span><span class="sxs-lookup"><span data-stu-id="8d872-103">Photo resource type</span></span>

<span data-ttu-id="8d872-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d872-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8d872-105">**照片**资源提供 [driveItem](driveitem.md) 中的照片和相机属性，例如 EXIF 元数据。</span><span class="sxs-lookup"><span data-stu-id="8d872-105">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d872-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8d872-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="8d872-107">属性</span><span class="sxs-lookup"><span data-stu-id="8d872-107">Properties</span></span>

| <span data-ttu-id="8d872-108">属性</span><span class="sxs-lookup"><span data-stu-id="8d872-108">Property</span></span>                | <span data-ttu-id="8d872-109">类型</span><span class="sxs-lookup"><span data-stu-id="8d872-109">Type</span></span>           | <span data-ttu-id="8d872-110">说明</span><span class="sxs-lookup"><span data-stu-id="8d872-110">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="8d872-111">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="8d872-111">**takenDateTime**</span></span>       | <span data-ttu-id="8d872-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d872-112">DateTimeOffset</span></span> | <span data-ttu-id="8d872-113">Represents the date and time the photo was taken.</span><span class="sxs-lookup"><span data-stu-id="8d872-113">Represents the date and time the photo was taken.</span></span> <span data-ttu-id="8d872-114">Read-only.</span><span class="sxs-lookup"><span data-stu-id="8d872-114">Read-only.</span></span>
| <span data-ttu-id="8d872-115">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="8d872-115">**cameraMake**</span></span>          | <span data-ttu-id="8d872-116">String</span><span class="sxs-lookup"><span data-stu-id="8d872-116">String</span></span>         | <span data-ttu-id="8d872-117">Camera manufacturer.</span><span class="sxs-lookup"><span data-stu-id="8d872-117">Camera manufacturer.</span></span> <span data-ttu-id="8d872-118">Read-only.</span><span class="sxs-lookup"><span data-stu-id="8d872-118">Read-only.</span></span>
| <span data-ttu-id="8d872-119">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="8d872-119">**cameraModel**</span></span>         | <span data-ttu-id="8d872-120">String</span><span class="sxs-lookup"><span data-stu-id="8d872-120">String</span></span>         | <span data-ttu-id="8d872-121">Camera model.</span><span class="sxs-lookup"><span data-stu-id="8d872-121">Camera model.</span></span> <span data-ttu-id="8d872-122">Read-only.</span><span class="sxs-lookup"><span data-stu-id="8d872-122">Read-only.</span></span>
| <span data-ttu-id="8d872-123">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="8d872-123">**fNumber**</span></span>             | <span data-ttu-id="8d872-124">双精度</span><span class="sxs-lookup"><span data-stu-id="8d872-124">Double</span></span>         | <span data-ttu-id="8d872-125">The F-stop value from the camera.</span><span class="sxs-lookup"><span data-stu-id="8d872-125">The F-stop value from the camera.</span></span> <span data-ttu-id="8d872-126">Read-only.</span><span class="sxs-lookup"><span data-stu-id="8d872-126">Read-only.</span></span>
| <span data-ttu-id="8d872-127">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="8d872-127">**exposureDenominator**</span></span> | <span data-ttu-id="8d872-128">双精度</span><span class="sxs-lookup"><span data-stu-id="8d872-128">Double</span></span>         | <span data-ttu-id="8d872-129">The denominator for the exposure time fraction from the camera.</span><span class="sxs-lookup"><span data-stu-id="8d872-129">The denominator for the exposure time fraction from the camera.</span></span> <span data-ttu-id="8d872-130">Read-only.</span><span class="sxs-lookup"><span data-stu-id="8d872-130">Read-only.</span></span>
| <span data-ttu-id="8d872-131">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="8d872-131">**exposureNumerator**</span></span>   | <span data-ttu-id="8d872-132">Double</span><span class="sxs-lookup"><span data-stu-id="8d872-132">Double</span></span>         | <span data-ttu-id="8d872-133">The numerator for the exposure time fraction from the camera.</span><span class="sxs-lookup"><span data-stu-id="8d872-133">The numerator for the exposure time fraction from the camera.</span></span> <span data-ttu-id="8d872-134">Read-only.</span><span class="sxs-lookup"><span data-stu-id="8d872-134">Read-only.</span></span>
| <span data-ttu-id="8d872-135">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="8d872-135">**focalLength**</span></span>         | <span data-ttu-id="8d872-136">双精度数</span><span class="sxs-lookup"><span data-stu-id="8d872-136">Double</span></span>         | <span data-ttu-id="8d872-137">The focal length from the camera.</span><span class="sxs-lookup"><span data-stu-id="8d872-137">The focal length from the camera.</span></span> <span data-ttu-id="8d872-138">Read-only.</span><span class="sxs-lookup"><span data-stu-id="8d872-138">Read-only.</span></span>
| <span data-ttu-id="8d872-139">**iso**</span><span class="sxs-lookup"><span data-stu-id="8d872-139">**iso**</span></span>                 | <span data-ttu-id="8d872-140">Int32</span><span class="sxs-lookup"><span data-stu-id="8d872-140">Int32</span></span>          | <span data-ttu-id="8d872-141">The ISO value from the camera.</span><span class="sxs-lookup"><span data-stu-id="8d872-141">The ISO value from the camera.</span></span> <span data-ttu-id="8d872-142">Read-only.</span><span class="sxs-lookup"><span data-stu-id="8d872-142">Read-only.</span></span>
| <span data-ttu-id="8d872-143">**orientation**</span><span class="sxs-lookup"><span data-stu-id="8d872-143">**orientation**</span></span>         | <span data-ttu-id="8d872-144">Int16</span><span class="sxs-lookup"><span data-stu-id="8d872-144">Int16</span></span>          | <span data-ttu-id="8d872-145">相机中的方向值。</span><span class="sxs-lookup"><span data-stu-id="8d872-145">The orientation value from the camera.</span></span> <span data-ttu-id="8d872-146">在 OneDrive 个人版上是可写的。</span><span class="sxs-lookup"><span data-stu-id="8d872-146">Writable on OneDrive Personal.</span></span>      |

## <a name="remarks"></a><span data-ttu-id="8d872-147">注解</span><span class="sxs-lookup"><span data-stu-id="8d872-147">Remarks</span></span>

<span data-ttu-id="8d872-148">OneDrive for Business 和 SharePoint 仅返回 **takenDateTime** 属性。</span><span class="sxs-lookup"><span data-stu-id="8d872-148">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="8d872-149">有关 DriveItem 方面的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="8d872-149">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso, orientation",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
