---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Photo
localization_priority: Normal
description: 照片资源提供 driveItem 中的照片和相机属性，例如 EXIF 元数据。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4e3f167384112c3c3354cdff88b41632f92e2637
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534049"
---
# <a name="photo-resource-type"></a><span data-ttu-id="4e159-103">Photo 资源类型</span><span class="sxs-lookup"><span data-stu-id="4e159-103">Photo resource type</span></span>

<span data-ttu-id="4e159-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e159-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4e159-105">**照片**资源提供 [driveItem](driveitem.md) 中的照片和相机属性，例如 EXIF 元数据。</span><span class="sxs-lookup"><span data-stu-id="4e159-105">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e159-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4e159-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="4e159-107">属性</span><span class="sxs-lookup"><span data-stu-id="4e159-107">Properties</span></span>

| <span data-ttu-id="4e159-108">属性</span><span class="sxs-lookup"><span data-stu-id="4e159-108">Property</span></span>                | <span data-ttu-id="4e159-109">类型</span><span class="sxs-lookup"><span data-stu-id="4e159-109">Type</span></span>           | <span data-ttu-id="4e159-110">说明</span><span class="sxs-lookup"><span data-stu-id="4e159-110">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="4e159-111">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="4e159-111">**takenDateTime**</span></span>       | <span data-ttu-id="4e159-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e159-112">DateTimeOffset</span></span> | <span data-ttu-id="4e159-p101">表示照片拍摄的时间和日期。只读。</span><span class="sxs-lookup"><span data-stu-id="4e159-p101">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="4e159-115">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="4e159-115">**cameraMake**</span></span>          | <span data-ttu-id="4e159-116">字符串</span><span class="sxs-lookup"><span data-stu-id="4e159-116">String</span></span>         | <span data-ttu-id="4e159-p102">相机制造商。只读。</span><span class="sxs-lookup"><span data-stu-id="4e159-p102">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="4e159-119">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="4e159-119">**cameraModel**</span></span>         | <span data-ttu-id="4e159-120">String</span><span class="sxs-lookup"><span data-stu-id="4e159-120">String</span></span>         | <span data-ttu-id="4e159-p103">相机型号。只读。</span><span class="sxs-lookup"><span data-stu-id="4e159-p103">Camera model. Read-only.</span></span>
| <span data-ttu-id="4e159-123">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="4e159-123">**fNumber**</span></span>             | <span data-ttu-id="4e159-124">双精度</span><span class="sxs-lookup"><span data-stu-id="4e159-124">Double</span></span>         | <span data-ttu-id="4e159-p104">相机的 F-stop 值。只读。</span><span class="sxs-lookup"><span data-stu-id="4e159-p104">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="4e159-127">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="4e159-127">**exposureDenominator**</span></span> | <span data-ttu-id="4e159-128">双精度</span><span class="sxs-lookup"><span data-stu-id="4e159-128">Double</span></span>         | <span data-ttu-id="4e159-p105">相机的曝光时间分数的分母。只读。</span><span class="sxs-lookup"><span data-stu-id="4e159-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="4e159-131">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="4e159-131">**exposureNumerator**</span></span>   | <span data-ttu-id="4e159-132">Double</span><span class="sxs-lookup"><span data-stu-id="4e159-132">Double</span></span>         | <span data-ttu-id="4e159-p106">相机的曝光时间分数的分子。只读。</span><span class="sxs-lookup"><span data-stu-id="4e159-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="4e159-135">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="4e159-135">**focalLength**</span></span>         | <span data-ttu-id="4e159-136">双精度数</span><span class="sxs-lookup"><span data-stu-id="4e159-136">Double</span></span>         | <span data-ttu-id="4e159-p107">相机的焦距。只读。</span><span class="sxs-lookup"><span data-stu-id="4e159-p107">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="4e159-139">**iso**</span><span class="sxs-lookup"><span data-stu-id="4e159-139">**iso**</span></span>                 | <span data-ttu-id="4e159-140">Int32</span><span class="sxs-lookup"><span data-stu-id="4e159-140">Int32</span></span>          | <span data-ttu-id="4e159-p108">相机的 ISO 值。只读。</span><span class="sxs-lookup"><span data-stu-id="4e159-p108">The ISO value from the camera. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="4e159-143">注解</span><span class="sxs-lookup"><span data-stu-id="4e159-143">Remarks</span></span>

<span data-ttu-id="4e159-144">OneDrive for Business 和 SharePoint 仅返回 **takenDateTime** 属性。</span><span class="sxs-lookup"><span data-stu-id="4e159-144">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="4e159-145">有关 DriveItem 方面的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="4e159-145">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
