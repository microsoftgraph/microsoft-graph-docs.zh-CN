---
title: 照片资源类型
description: 照片资源提供 driveItem 中的照片和相机属性，例如 EXIF 元数据。
ms.date: 09/10/2017
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ed3d60fabfd367668b5c7a8230bba0f19f7d88f5
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333239"
---
# <a name="photo-resource-type"></a><span data-ttu-id="35b79-103">照片资源类型</span><span class="sxs-lookup"><span data-stu-id="35b79-103">photo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35b79-104">**照片**资源提供 [driveItem](driveitem.md) 中的照片和相机属性，例如 EXIF 元数据。</span><span class="sxs-lookup"><span data-stu-id="35b79-104">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

> [!NOTE]
> <span data-ttu-id="35b79-105">目前，只有**takenDateTime**在 OneDrive for Business 和 SharePoint 上可用。</span><span class="sxs-lookup"><span data-stu-id="35b79-105">Currently, only **takenDateTime** is available on OneDrive for Business and SharePoint.</span></span>

## <a name="properties"></a><span data-ttu-id="35b79-106">属性</span><span class="sxs-lookup"><span data-stu-id="35b79-106">Properties</span></span>

| <span data-ttu-id="35b79-107">属性</span><span class="sxs-lookup"><span data-stu-id="35b79-107">Property</span></span>          | <span data-ttu-id="35b79-108">类型</span><span class="sxs-lookup"><span data-stu-id="35b79-108">Type</span></span>          | <span data-ttu-id="35b79-109">说明</span><span class="sxs-lookup"><span data-stu-id="35b79-109">Description</span></span>                                                                |
|:------------------|:--------------|:---------------------------------------------------------------------------|
|<span data-ttu-id="35b79-110">cameraMake</span><span class="sxs-lookup"><span data-stu-id="35b79-110">cameraMake</span></span>         |<span data-ttu-id="35b79-111">String</span><span class="sxs-lookup"><span data-stu-id="35b79-111">String</span></span>         | <span data-ttu-id="35b79-p101">相机制造商。只读。</span><span class="sxs-lookup"><span data-stu-id="35b79-p101">Camera manufacturer. Read-only.</span></span>                                            |
|<span data-ttu-id="35b79-114">cameraModel</span><span class="sxs-lookup"><span data-stu-id="35b79-114">cameraModel</span></span>        |<span data-ttu-id="35b79-115">String</span><span class="sxs-lookup"><span data-stu-id="35b79-115">String</span></span>         | <span data-ttu-id="35b79-p102">相机型号。只读。</span><span class="sxs-lookup"><span data-stu-id="35b79-p102">Camera model. Read-only.</span></span>                                                   |
|<span data-ttu-id="35b79-118">exposureDenominator</span><span class="sxs-lookup"><span data-stu-id="35b79-118">exposureDenominator</span></span>|<span data-ttu-id="35b79-119">双精度</span><span class="sxs-lookup"><span data-stu-id="35b79-119">Double</span></span>         | <span data-ttu-id="35b79-p103">相机的曝光时间分数的分母。只读。</span><span class="sxs-lookup"><span data-stu-id="35b79-p103">The denominator for the exposure time fraction from the camera. Read-only.</span></span> |
|<span data-ttu-id="35b79-122">exposureNumerator</span><span class="sxs-lookup"><span data-stu-id="35b79-122">exposureNumerator</span></span>  |<span data-ttu-id="35b79-123">Double</span><span class="sxs-lookup"><span data-stu-id="35b79-123">Double</span></span>         | <span data-ttu-id="35b79-p104">相机的曝光时间分数的分子。只读。</span><span class="sxs-lookup"><span data-stu-id="35b79-p104">The numerator for the exposure time fraction from the camera. Read-only.</span></span>   |
|<span data-ttu-id="35b79-126">fNumber</span><span class="sxs-lookup"><span data-stu-id="35b79-126">fNumber</span></span>            |<span data-ttu-id="35b79-127">双精度</span><span class="sxs-lookup"><span data-stu-id="35b79-127">Double</span></span>         | <span data-ttu-id="35b79-p105">相机的 F-stop 值。只读。</span><span class="sxs-lookup"><span data-stu-id="35b79-p105">The F-stop value from the camera. Read-only.</span></span>                               |
|<span data-ttu-id="35b79-130">focalLength</span><span class="sxs-lookup"><span data-stu-id="35b79-130">focalLength</span></span>        |<span data-ttu-id="35b79-131">双精度数</span><span class="sxs-lookup"><span data-stu-id="35b79-131">Double</span></span>         | <span data-ttu-id="35b79-p106">相机的焦距。只读。</span><span class="sxs-lookup"><span data-stu-id="35b79-p106">The focal length from the camera. Read-only.</span></span>                               |
|<span data-ttu-id="35b79-134">iso</span><span class="sxs-lookup"><span data-stu-id="35b79-134">iso</span></span>                |<span data-ttu-id="35b79-135">Int32</span><span class="sxs-lookup"><span data-stu-id="35b79-135">Int32</span></span>          | <span data-ttu-id="35b79-p107">相机的 ISO 值。只读。</span><span class="sxs-lookup"><span data-stu-id="35b79-p107">The ISO value from the camera. Read-only.</span></span>                                  |
|<span data-ttu-id="35b79-138">orientation</span><span class="sxs-lookup"><span data-stu-id="35b79-138">orientation</span></span>        |<span data-ttu-id="35b79-139">Int16</span><span class="sxs-lookup"><span data-stu-id="35b79-139">Int16</span></span>          | <span data-ttu-id="35b79-140">相机中的方向值。</span><span class="sxs-lookup"><span data-stu-id="35b79-140">The orientation value from the camera.</span></span> <span data-ttu-id="35b79-141">在 OneDrive 个人版上是可写的。</span><span class="sxs-lookup"><span data-stu-id="35b79-141">Writable on OneDrive Personal.</span></span>      |
|<span data-ttu-id="35b79-142">takenDateTime</span><span class="sxs-lookup"><span data-stu-id="35b79-142">takenDateTime</span></span>      |<span data-ttu-id="35b79-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35b79-143">DateTimeOffset</span></span> | <span data-ttu-id="35b79-144">以 UTC 时间拍摄照片的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="35b79-144">The date and time the photo was taken in UTC time.</span></span> <span data-ttu-id="35b79-145">只读。</span><span class="sxs-lookup"><span data-stu-id="35b79-145">Read-only.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="35b79-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="35b79-146">JSON representation</span></span>

<span data-ttu-id="35b79-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35b79-147">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.photo",
  "baseType": null
}-->

```json
{
  "cameraMake": "String",
  "cameraModel": "String",
  "exposureDenominator": 1000.0,
  "exposureNumerator": 1.0,
  "fNumber": 1.8,
  "focalLength": 22.5,
  "iso": 100,
  "orientation": 3,
  "takenDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The photo resource provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso, orientation",
  "section": "documentation",
  "tocPath": ""
}-->
