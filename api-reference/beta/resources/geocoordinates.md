---
author: JeremyKelley
description: GeoCoordinates 资源根据文件中包含的元数据提供位置的地理坐标和仰角。
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 86de97358591df8dc446b91d0be7a8192c7346f8
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333253"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="5ab9b-103">geoCoordinates 资源类型</span><span class="sxs-lookup"><span data-stu-id="5ab9b-103">geoCoordinates resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ab9b-104">根据文件中包含的元数据提供位置的地理坐标和仰角。</span><span class="sxs-lookup"><span data-stu-id="5ab9b-104">Provides geographic coordinates and elevation of a location based on metadata contained within the file.</span></span>
<span data-ttu-id="5ab9b-105">如果[**driveItem**](driveitem.md)具有非 null**位置**facet，则该项目表示一个文件，其中包含一个已知的位置关联。</span><span class="sxs-lookup"><span data-stu-id="5ab9b-105">If a [**driveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

> [!NOTE]
> <span data-ttu-id="5ab9b-106">更新照片的纬度和经度时，必须提供[照片](photo.md)资源（空或其他）。</span><span class="sxs-lookup"><span data-stu-id="5ab9b-106">When updating the latitude and longitude of a photo, a [photo](photo.md) resource (empty or otherwise) must be provided.</span></span>

## <a name="properties"></a><span data-ttu-id="5ab9b-107">属性</span><span class="sxs-lookup"><span data-stu-id="5ab9b-107">Properties</span></span>

| <span data-ttu-id="5ab9b-108">属性</span><span class="sxs-lookup"><span data-stu-id="5ab9b-108">Property</span></span>  | <span data-ttu-id="5ab9b-109">类型</span><span class="sxs-lookup"><span data-stu-id="5ab9b-109">Type</span></span>   | <span data-ttu-id="5ab9b-110">说明</span><span class="sxs-lookup"><span data-stu-id="5ab9b-110">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="5ab9b-111">海拔</span><span class="sxs-lookup"><span data-stu-id="5ab9b-111">altitude</span></span>  | <span data-ttu-id="5ab9b-112">双精度</span><span class="sxs-lookup"><span data-stu-id="5ab9b-112">Double</span></span> | <span data-ttu-id="5ab9b-p102">可选。此项高于海平面的高度（以英尺为单位）。只读。</span><span class="sxs-lookup"><span data-stu-id="5ab9b-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="5ab9b-116">纬度</span><span class="sxs-lookup"><span data-stu-id="5ab9b-116">latitude</span></span>  | <span data-ttu-id="5ab9b-117">Double</span><span class="sxs-lookup"><span data-stu-id="5ab9b-117">Double</span></span> | <span data-ttu-id="5ab9b-118">可选。</span><span class="sxs-lookup"><span data-stu-id="5ab9b-118">Optional.</span></span> <span data-ttu-id="5ab9b-119">此项的纬度（以十进制表示）。</span><span class="sxs-lookup"><span data-stu-id="5ab9b-119">The latitude, in decimal, for the item.</span></span> <span data-ttu-id="5ab9b-120">在 OneDrive 个人版上是可写的。</span><span class="sxs-lookup"><span data-stu-id="5ab9b-120">Writable on OneDrive Personal.</span></span>
| <span data-ttu-id="5ab9b-121">longitude</span><span class="sxs-lookup"><span data-stu-id="5ab9b-121">longitude</span></span> | <span data-ttu-id="5ab9b-122">Double</span><span class="sxs-lookup"><span data-stu-id="5ab9b-122">Double</span></span> | <span data-ttu-id="5ab9b-123">可选。</span><span class="sxs-lookup"><span data-stu-id="5ab9b-123">Optional.</span></span> <span data-ttu-id="5ab9b-124">此项的经度（以十进制表示）。</span><span class="sxs-lookup"><span data-stu-id="5ab9b-124">The longitude, in decimal, for the item.</span></span> <span data-ttu-id="5ab9b-125">在 OneDrive 个人版上是可写的。</span><span class="sxs-lookup"><span data-stu-id="5ab9b-125">Writable on OneDrive Personal.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5ab9b-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5ab9b-126">JSON representation</span></span>

<span data-ttu-id="5ab9b-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5ab9b-127">Here is a JSON representation of the resource</span></span>

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
