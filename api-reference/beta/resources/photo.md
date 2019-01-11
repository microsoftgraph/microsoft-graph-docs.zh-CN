---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Photo
localization_priority: Normal
ms.openlocfilehash: ed891f917ba8018aac349976df0455adfd269fdb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869381"
---
# <a name="photo-resource-type"></a><span data-ttu-id="ba846-102">Photo 资源类型</span><span class="sxs-lookup"><span data-stu-id="ba846-102">Photo resource type</span></span>

> <span data-ttu-id="ba846-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ba846-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ba846-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ba846-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ba846-105">**照片**资源提供 [driveItem](driveitem.md) 中的照片和相机属性，例如 EXIF 元数据。</span><span class="sxs-lookup"><span data-stu-id="ba846-105">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba846-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ba846-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="ba846-107">属性</span><span class="sxs-lookup"><span data-stu-id="ba846-107">Properties</span></span>

| <span data-ttu-id="ba846-108">属性</span><span class="sxs-lookup"><span data-stu-id="ba846-108">Property</span></span>                | <span data-ttu-id="ba846-109">类型</span><span class="sxs-lookup"><span data-stu-id="ba846-109">Type</span></span>           | <span data-ttu-id="ba846-110">说明</span><span class="sxs-lookup"><span data-stu-id="ba846-110">Description</span></span>
|:------------------------|:---------------|:----------------------------------
| <span data-ttu-id="ba846-111">**takenDateTime**</span><span class="sxs-lookup"><span data-stu-id="ba846-111">**takenDateTime**</span></span>       | <span data-ttu-id="ba846-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba846-112">DateTimeOffset</span></span> | <span data-ttu-id="ba846-p102">表示照片拍摄的时间和日期。只读。</span><span class="sxs-lookup"><span data-stu-id="ba846-p102">Represents the date and time the photo was taken. Read-only.</span></span>
| <span data-ttu-id="ba846-115">**cameraMake**</span><span class="sxs-lookup"><span data-stu-id="ba846-115">**cameraMake**</span></span>          | <span data-ttu-id="ba846-116">String</span><span class="sxs-lookup"><span data-stu-id="ba846-116">String</span></span>         | <span data-ttu-id="ba846-p103">相机制造商。只读。</span><span class="sxs-lookup"><span data-stu-id="ba846-p103">Camera manufacturer. Read-only.</span></span>
| <span data-ttu-id="ba846-119">**cameraModel**</span><span class="sxs-lookup"><span data-stu-id="ba846-119">**cameraModel**</span></span>         | <span data-ttu-id="ba846-120">String</span><span class="sxs-lookup"><span data-stu-id="ba846-120">String</span></span>         | <span data-ttu-id="ba846-p104">相机型号。只读。</span><span class="sxs-lookup"><span data-stu-id="ba846-p104">Camera model. Read-only.</span></span>
| <span data-ttu-id="ba846-123">**fNumber**</span><span class="sxs-lookup"><span data-stu-id="ba846-123">**fNumber**</span></span>             | <span data-ttu-id="ba846-124">Double</span><span class="sxs-lookup"><span data-stu-id="ba846-124">Double</span></span>         | <span data-ttu-id="ba846-p105">相机的 F-stop 值。只读。</span><span class="sxs-lookup"><span data-stu-id="ba846-p105">The F-stop value from the camera. Read-only.</span></span>
| <span data-ttu-id="ba846-127">**exposureDenominator**</span><span class="sxs-lookup"><span data-stu-id="ba846-127">**exposureDenominator**</span></span> | <span data-ttu-id="ba846-128">Double</span><span class="sxs-lookup"><span data-stu-id="ba846-128">Double</span></span>         | <span data-ttu-id="ba846-p106">相机的曝光时间分数的分母。只读。</span><span class="sxs-lookup"><span data-stu-id="ba846-p106">The denominator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="ba846-131">**exposureNumerator**</span><span class="sxs-lookup"><span data-stu-id="ba846-131">**exposureNumerator**</span></span>   | <span data-ttu-id="ba846-132">Double</span><span class="sxs-lookup"><span data-stu-id="ba846-132">Double</span></span>         | <span data-ttu-id="ba846-p107">相机的曝光时间分数的分子。只读。</span><span class="sxs-lookup"><span data-stu-id="ba846-p107">The numerator for the exposure time fraction from the camera. Read-only.</span></span>
| <span data-ttu-id="ba846-135">**focalLength**</span><span class="sxs-lookup"><span data-stu-id="ba846-135">**focalLength**</span></span>         | <span data-ttu-id="ba846-136">Double</span><span class="sxs-lookup"><span data-stu-id="ba846-136">Double</span></span>         | <span data-ttu-id="ba846-p108">相机的焦距。只读。</span><span class="sxs-lookup"><span data-stu-id="ba846-p108">The focal length from the camera. Read-only.</span></span>
| <span data-ttu-id="ba846-139">**iso**</span><span class="sxs-lookup"><span data-stu-id="ba846-139">**iso**</span></span>                 | <span data-ttu-id="ba846-140">Int64</span><span class="sxs-lookup"><span data-stu-id="ba846-140">Int64</span></span>          | <span data-ttu-id="ba846-p109">相机的 ISO 值。只读。</span><span class="sxs-lookup"><span data-stu-id="ba846-p109">The ISO value from the camera. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="ba846-143">注解</span><span class="sxs-lookup"><span data-stu-id="ba846-143">Remarks</span></span>
<span data-ttu-id="ba846-144">OneDrive for Business 和 SharePoint 仅返回 **takenDateTime** 属性。</span><span class="sxs-lookup"><span data-stu-id="ba846-144">OneDrive for Business and SharePoint only return the **takenDateTime** property.</span></span>

<span data-ttu-id="ba846-145">有关 DriveItem 方面的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="ba846-145">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
