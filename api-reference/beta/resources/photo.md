---
title: 照片资源类型
description: 照片资源提供 driveItem 中的照片和相机属性，例如 EXIF 元数据。
ms.date: 09/10/2017
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 920d6e69367517b1324b6cb66b755b6b58192219
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997822"
---
# <a name="photo-resource-type"></a><span data-ttu-id="fa995-103">照片资源类型</span><span class="sxs-lookup"><span data-stu-id="fa995-103">photo resource type</span></span>

<span data-ttu-id="fa995-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa995-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa995-105">**照片**资源提供 [driveItem](driveitem.md) 中的照片和相机属性，例如 EXIF 元数据。</span><span class="sxs-lookup"><span data-stu-id="fa995-105">The **photo** resource provides photo and camera properties, for example, EXIF metadata, on a [driveItem](driveitem.md).</span></span>

> [!NOTE]
> <span data-ttu-id="fa995-106">目前，只有 **takenDateTime** 在 OneDrive for Business 和 SharePoint 上可用。</span><span class="sxs-lookup"><span data-stu-id="fa995-106">Currently, only **takenDateTime** is available on OneDrive for Business and SharePoint.</span></span>

## <a name="properties"></a><span data-ttu-id="fa995-107">属性</span><span class="sxs-lookup"><span data-stu-id="fa995-107">Properties</span></span>

| <span data-ttu-id="fa995-108">属性</span><span class="sxs-lookup"><span data-stu-id="fa995-108">Property</span></span>          | <span data-ttu-id="fa995-109">类型</span><span class="sxs-lookup"><span data-stu-id="fa995-109">Type</span></span>          | <span data-ttu-id="fa995-110">说明</span><span class="sxs-lookup"><span data-stu-id="fa995-110">Description</span></span>                                                                |
|:------------------|:--------------|:---------------------------------------------------------------------------|
|<span data-ttu-id="fa995-111">cameraMake</span><span class="sxs-lookup"><span data-stu-id="fa995-111">cameraMake</span></span>         |<span data-ttu-id="fa995-112">String</span><span class="sxs-lookup"><span data-stu-id="fa995-112">String</span></span>         | <span data-ttu-id="fa995-p101">相机制造商。只读。</span><span class="sxs-lookup"><span data-stu-id="fa995-p101">Camera manufacturer. Read-only.</span></span>                                            |
|<span data-ttu-id="fa995-115">cameraModel</span><span class="sxs-lookup"><span data-stu-id="fa995-115">cameraModel</span></span>        |<span data-ttu-id="fa995-116">String</span><span class="sxs-lookup"><span data-stu-id="fa995-116">String</span></span>         | <span data-ttu-id="fa995-p102">相机型号。只读。</span><span class="sxs-lookup"><span data-stu-id="fa995-p102">Camera model. Read-only.</span></span>                                                   |
|<span data-ttu-id="fa995-119">exposureDenominator</span><span class="sxs-lookup"><span data-stu-id="fa995-119">exposureDenominator</span></span>|<span data-ttu-id="fa995-120">Double</span><span class="sxs-lookup"><span data-stu-id="fa995-120">Double</span></span>         | <span data-ttu-id="fa995-p103">相机的曝光时间分数的分母。只读。</span><span class="sxs-lookup"><span data-stu-id="fa995-p103">The denominator for the exposure time fraction from the camera. Read-only.</span></span> |
|<span data-ttu-id="fa995-123">exposureNumerator</span><span class="sxs-lookup"><span data-stu-id="fa995-123">exposureNumerator</span></span>  |<span data-ttu-id="fa995-124">Double</span><span class="sxs-lookup"><span data-stu-id="fa995-124">Double</span></span>         | <span data-ttu-id="fa995-p104">相机的曝光时间分数的分子。只读。</span><span class="sxs-lookup"><span data-stu-id="fa995-p104">The numerator for the exposure time fraction from the camera. Read-only.</span></span>   |
|<span data-ttu-id="fa995-127">fNumber</span><span class="sxs-lookup"><span data-stu-id="fa995-127">fNumber</span></span>            |<span data-ttu-id="fa995-128">Double</span><span class="sxs-lookup"><span data-stu-id="fa995-128">Double</span></span>         | <span data-ttu-id="fa995-p105">相机的 F-stop 值。只读。</span><span class="sxs-lookup"><span data-stu-id="fa995-p105">The F-stop value from the camera. Read-only.</span></span>                               |
|<span data-ttu-id="fa995-131">focalLength</span><span class="sxs-lookup"><span data-stu-id="fa995-131">focalLength</span></span>        |<span data-ttu-id="fa995-132">Double</span><span class="sxs-lookup"><span data-stu-id="fa995-132">Double</span></span>         | <span data-ttu-id="fa995-p106">相机的焦距。只读。</span><span class="sxs-lookup"><span data-stu-id="fa995-p106">The focal length from the camera. Read-only.</span></span>                               |
|<span data-ttu-id="fa995-135">iso</span><span class="sxs-lookup"><span data-stu-id="fa995-135">iso</span></span>                |<span data-ttu-id="fa995-136">Int32</span><span class="sxs-lookup"><span data-stu-id="fa995-136">Int32</span></span>          | <span data-ttu-id="fa995-p107">相机的 ISO 值。只读。</span><span class="sxs-lookup"><span data-stu-id="fa995-p107">The ISO value from the camera. Read-only.</span></span>                                  |
|<span data-ttu-id="fa995-139">orientation</span><span class="sxs-lookup"><span data-stu-id="fa995-139">orientation</span></span>        |<span data-ttu-id="fa995-140">Int16</span><span class="sxs-lookup"><span data-stu-id="fa995-140">Int16</span></span>          | <span data-ttu-id="fa995-141">相机中的方向值。</span><span class="sxs-lookup"><span data-stu-id="fa995-141">The orientation value from the camera.</span></span> <span data-ttu-id="fa995-142">在 OneDrive 个人版上是可写的。</span><span class="sxs-lookup"><span data-stu-id="fa995-142">Writable on OneDrive Personal.</span></span>      |
|<span data-ttu-id="fa995-143">takenDateTime</span><span class="sxs-lookup"><span data-stu-id="fa995-143">takenDateTime</span></span>      |<span data-ttu-id="fa995-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa995-144">DateTimeOffset</span></span> | <span data-ttu-id="fa995-145">以 UTC 时间拍摄照片的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="fa995-145">The date and time the photo was taken in UTC time.</span></span> <span data-ttu-id="fa995-146">只读。</span><span class="sxs-lookup"><span data-stu-id="fa995-146">Read-only.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="fa995-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fa995-147">JSON representation</span></span>

<span data-ttu-id="fa995-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa995-148">The following is a JSON representation of the resource.</span></span>

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


