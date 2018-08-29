---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Photo
ms.openlocfilehash: 391eafd84ab1abd4670c953720ff7097e060bfd3
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2018
ms.locfileid: "23267064"
---
# <a name="photo-resource-type"></a><span data-ttu-id="a327c-102">Photo 资源类型</span><span class="sxs-lookup"><span data-stu-id="a327c-102">Photo resource type</span></span>

<span data-ttu-id="a327c-103">**照片**资源提供 [driveItem](driveitem.md) 中的照片和相机属性，例如 EXIF 元数据。</span><span class="sxs-lookup"><span data-stu-id="a327c-103">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="a327c-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a327c-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="a327c-105">属性</span><span class="sxs-lookup"><span data-stu-id="a327c-105">Properties</span></span>

| <span data-ttu-id="a327c-106">属性</span><span class="sxs-lookup"><span data-stu-id="a327c-106">Property</span></span>                | <span data-ttu-id="a327c-107">类型</span><span class="sxs-lookup"><span data-stu-id="a327c-107">Type</span></span>           | <span data-ttu-id="a327c-108">说明</span><span class="sxs-lookup"><span data-stu-id="a327c-108">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="a327c-109">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="a327c-109">**takenDateTime**</span></span>       | <span data-ttu-id="a327c-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a327c-110">DateTimeOffset</span></span> | <span data-ttu-id="a327c-p101">表示照片拍摄的时间和日期。只读。</span><span class="sxs-lookup"><span data-stu-id="a327c-p101">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="a327c-113">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="a327c-113">**cameraMake**</span></span>          | <span data-ttu-id="a327c-114">String</span><span class="sxs-lookup"><span data-stu-id="a327c-114">String</span></span>         | <span data-ttu-id="a327c-p102">相机制造商。只读。</span><span class="sxs-lookup"><span data-stu-id="a327c-p102">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="a327c-117">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="a327c-117">**cameraModel**</span></span>         | <span data-ttu-id="a327c-118">String</span><span class="sxs-lookup"><span data-stu-id="a327c-118">String</span></span>         | <span data-ttu-id="a327c-p103">相机型号。只读。</span><span class="sxs-lookup"><span data-stu-id="a327c-p103">Camera model. Read-only.</span></span>
| <span data-ttu-id="a327c-121">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="a327c-121">**fNumber**</span></span>             | <span data-ttu-id="a327c-122">双精度数</span><span class="sxs-lookup"><span data-stu-id="a327c-122">Double</span></span>         | <span data-ttu-id="a327c-p104">相机的 F-stop 值。只读。</span><span class="sxs-lookup"><span data-stu-id="a327c-p104">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="a327c-125">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="a327c-125">**exposureDenominator**</span></span> | <span data-ttu-id="a327c-126">Double</span><span class="sxs-lookup"><span data-stu-id="a327c-126">Double</span></span>         | <span data-ttu-id="a327c-p105">相机的曝光时间分数的分母。只读。</span><span class="sxs-lookup"><span data-stu-id="a327c-p105">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="a327c-129">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="a327c-129">**exposureNumerator**</span></span>   | <span data-ttu-id="a327c-130">Double</span><span class="sxs-lookup"><span data-stu-id="a327c-130">Double</span></span>         | <span data-ttu-id="a327c-p106">相机的曝光时间分数的分子。只读。</span><span class="sxs-lookup"><span data-stu-id="a327c-p106">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="a327c-133">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="a327c-133">**focalLength**</span></span>         | <span data-ttu-id="a327c-134">双精度数</span><span class="sxs-lookup"><span data-stu-id="a327c-134">Double</span></span>         | <span data-ttu-id="a327c-p107">相机的焦距。只读。</span><span class="sxs-lookup"><span data-stu-id="a327c-p107">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="a327c-137">**iso**</span><span class="sxs-lookup"><span data-stu-id="a327c-137">**iso**</span></span>                 | <span data-ttu-id="a327c-138">Int32</span><span class="sxs-lookup"><span data-stu-id="a327c-138">Int32</span></span>          | <span data-ttu-id="a327c-p108">相机的 ISO 值。只读。</span><span class="sxs-lookup"><span data-stu-id="a327c-p108">The ISO value from the camera. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="a327c-141">注解</span><span class="sxs-lookup"><span data-stu-id="a327c-141">Remarks</span></span>

<span data-ttu-id="a327c-142">OneDrive for Business 和 SharePoint 仅返回 **takenDateTime** 属性。</span><span class="sxs-lookup"><span data-stu-id="a327c-142">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="a327c-143">有关 DriveItem 方面的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="a327c-143">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
