---
author: JeremyKelley
description: 照片资源提供 driveItem 中的照片和相机属性，例如 EXIF 元数据。
ms.date: 09/10/2017
title: Photo
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6713e66b5ca14cfa6605b9e67d4bec152a321f33
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009221"
---
# <a name="photo-resource-type"></a><span data-ttu-id="4c5dd-103">Photo 资源类型</span><span class="sxs-lookup"><span data-stu-id="4c5dd-103">Photo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c5dd-104">**照片**资源提供 [driveItem](driveitem.md) 中的照片和相机属性，例如 EXIF 元数据。</span><span class="sxs-lookup"><span data-stu-id="4c5dd-104">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c5dd-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4c5dd-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="4c5dd-106">属性</span><span class="sxs-lookup"><span data-stu-id="4c5dd-106">Properties</span></span>

| <span data-ttu-id="4c5dd-107">属性</span><span class="sxs-lookup"><span data-stu-id="4c5dd-107">Property</span></span>                | <span data-ttu-id="4c5dd-108">类型</span><span class="sxs-lookup"><span data-stu-id="4c5dd-108">Type</span></span>           | <span data-ttu-id="4c5dd-109">说明</span><span class="sxs-lookup"><span data-stu-id="4c5dd-109">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="4c5dd-110">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="4c5dd-110">**takenDateTime**</span></span>       | <span data-ttu-id="4c5dd-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c5dd-111">DateTimeOffset</span></span> | <span data-ttu-id="4c5dd-p101">表示照片拍摄的时间和日期。只读。</span><span class="sxs-lookup"><span data-stu-id="4c5dd-p101">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="4c5dd-114">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="4c5dd-114">**cameraMake**</span></span>          | <span data-ttu-id="4c5dd-115">String</span><span class="sxs-lookup"><span data-stu-id="4c5dd-115">String</span></span>         | <span data-ttu-id="4c5dd-p102">相机制造商。只读。</span><span class="sxs-lookup"><span data-stu-id="4c5dd-p102">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="4c5dd-118">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="4c5dd-118">**cameraModel**</span></span>         | <span data-ttu-id="4c5dd-119">String</span><span class="sxs-lookup"><span data-stu-id="4c5dd-119">String</span></span>         | <span data-ttu-id="4c5dd-p103">相机型号。只读。</span><span class="sxs-lookup"><span data-stu-id="4c5dd-p103">Camera model. Read-only.</span></span>
| <span data-ttu-id="4c5dd-122">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="4c5dd-122">**fNumber**</span></span>             | <span data-ttu-id="4c5dd-123">双精度</span><span class="sxs-lookup"><span data-stu-id="4c5dd-123">Double</span></span>         | <span data-ttu-id="4c5dd-p104">相机的 F-stop 值。只读。</span><span class="sxs-lookup"><span data-stu-id="4c5dd-p104">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="4c5dd-126">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="4c5dd-126">**exposureDenominator**</span></span> | <span data-ttu-id="4c5dd-127">双精度</span><span class="sxs-lookup"><span data-stu-id="4c5dd-127">Double</span></span>         | <span data-ttu-id="4c5dd-p105">相机的曝光时间分数的分母。只读。</span><span class="sxs-lookup"><span data-stu-id="4c5dd-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="4c5dd-130">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="4c5dd-130">**exposureNumerator**</span></span>   | <span data-ttu-id="4c5dd-131">Double</span><span class="sxs-lookup"><span data-stu-id="4c5dd-131">Double</span></span>         | <span data-ttu-id="4c5dd-p106">相机的曝光时间分数的分子。只读。</span><span class="sxs-lookup"><span data-stu-id="4c5dd-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="4c5dd-134">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="4c5dd-134">**focalLength**</span></span>         | <span data-ttu-id="4c5dd-135">双精度数</span><span class="sxs-lookup"><span data-stu-id="4c5dd-135">Double</span></span>         | <span data-ttu-id="4c5dd-p107">相机的焦距。只读。</span><span class="sxs-lookup"><span data-stu-id="4c5dd-p107">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="4c5dd-138">**iso**</span><span class="sxs-lookup"><span data-stu-id="4c5dd-138">**iso**</span></span>                 | <span data-ttu-id="4c5dd-139">Int64</span><span class="sxs-lookup"><span data-stu-id="4c5dd-139">Int64</span></span>          | <span data-ttu-id="4c5dd-p108">相机的 ISO 值。只读。</span><span class="sxs-lookup"><span data-stu-id="4c5dd-p108">The ISO value from the camera. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="4c5dd-142">注解</span><span class="sxs-lookup"><span data-stu-id="4c5dd-142">Remarks</span></span>
<span data-ttu-id="4c5dd-143">OneDrive for Business 和 SharePoint 仅返回 **takenDateTime** 属性。</span><span class="sxs-lookup"><span data-stu-id="4c5dd-143">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="4c5dd-144">有关 DriveItem 方面的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="4c5dd-144">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!--
{
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo",
  "suppressions": []
}
-->
