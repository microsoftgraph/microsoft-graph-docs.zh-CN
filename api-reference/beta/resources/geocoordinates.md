---
author: JeremyKelley
description: geoCoordinates 资源基于文件中包含的元数据提供位置的地理坐标和提升。
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
ms.openlocfilehash: e3b0ac4f616afe648b5c30dc9d15978036a7ab80
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129420"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="e5def-103">geoCoordinates 资源类型</span><span class="sxs-lookup"><span data-stu-id="e5def-103">geoCoordinates resource type</span></span>

<span data-ttu-id="e5def-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5def-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5def-105">基于文件中包含的元数据提供位置的地理坐标和提升。</span><span class="sxs-lookup"><span data-stu-id="e5def-105">Provides geographic coordinates and elevation of a location based on metadata contained within the file.</span></span>
<span data-ttu-id="e5def-106">如果 [**driveItem**](driveitem.md) 具有非 null **位置** Facet，则该项表示包含已知位置的文件。</span><span class="sxs-lookup"><span data-stu-id="e5def-106">If a [**driveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

> [!NOTE]
> <span data-ttu-id="e5def-107">更新照片的纬度和经度时，必须 (空白或其他) [](photo.md)照片资源。</span><span class="sxs-lookup"><span data-stu-id="e5def-107">When updating the latitude and longitude of a photo, a [photo](photo.md) resource (empty or otherwise) must be provided.</span></span>

## <a name="properties"></a><span data-ttu-id="e5def-108">属性</span><span class="sxs-lookup"><span data-stu-id="e5def-108">Properties</span></span>

| <span data-ttu-id="e5def-109">属性</span><span class="sxs-lookup"><span data-stu-id="e5def-109">Property</span></span>  | <span data-ttu-id="e5def-110">类型</span><span class="sxs-lookup"><span data-stu-id="e5def-110">Type</span></span>   | <span data-ttu-id="e5def-111">说明</span><span class="sxs-lookup"><span data-stu-id="e5def-111">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="e5def-112">海拔</span><span class="sxs-lookup"><span data-stu-id="e5def-112">altitude</span></span>  | <span data-ttu-id="e5def-113">Double</span><span class="sxs-lookup"><span data-stu-id="e5def-113">Double</span></span> | <span data-ttu-id="e5def-p102">可选。此项高于海平面的高度（以英尺为单位）。只读。</span><span class="sxs-lookup"><span data-stu-id="e5def-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="e5def-117">纬度</span><span class="sxs-lookup"><span data-stu-id="e5def-117">latitude</span></span>  | <span data-ttu-id="e5def-118">Double</span><span class="sxs-lookup"><span data-stu-id="e5def-118">Double</span></span> | <span data-ttu-id="e5def-119">可选。</span><span class="sxs-lookup"><span data-stu-id="e5def-119">Optional.</span></span> <span data-ttu-id="e5def-120">此项的纬度（以十进制表示）。</span><span class="sxs-lookup"><span data-stu-id="e5def-120">The latitude, in decimal, for the item.</span></span> <span data-ttu-id="e5def-121">在 OneDrive 个人上可写。</span><span class="sxs-lookup"><span data-stu-id="e5def-121">Writable on OneDrive Personal.</span></span>
| <span data-ttu-id="e5def-122">longitude</span><span class="sxs-lookup"><span data-stu-id="e5def-122">longitude</span></span> | <span data-ttu-id="e5def-123">Double</span><span class="sxs-lookup"><span data-stu-id="e5def-123">Double</span></span> | <span data-ttu-id="e5def-124">可选。</span><span class="sxs-lookup"><span data-stu-id="e5def-124">Optional.</span></span> <span data-ttu-id="e5def-125">此项的经度（以十进制表示）。</span><span class="sxs-lookup"><span data-stu-id="e5def-125">The longitude, in decimal, for the item.</span></span> <span data-ttu-id="e5def-126">在 OneDrive 个人上可写。</span><span class="sxs-lookup"><span data-stu-id="e5def-126">Writable on OneDrive Personal.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5def-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e5def-127">JSON representation</span></span>

<span data-ttu-id="e5def-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5def-128">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.geoCoordinates"
}-->

```json
{
  "altitude": 1024.13,
  "latitude": 26.13246,
  "longitude": 24.34616
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location",
  "suppressions": []
}
-->


