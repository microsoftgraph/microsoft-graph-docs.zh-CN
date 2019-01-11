---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
ms.openlocfilehash: 33390fa893e99ffb0d7c44642c42751c66265ec8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885510"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="4338c-102">GeoCoordinates 资源类型</span><span class="sxs-lookup"><span data-stu-id="4338c-102">GeoCoordinates resource type</span></span>

<span data-ttu-id="4338c-p101">**GeoCoordinates** 资源基于文件中包含的元数据提供位置的地理坐标和海拔。如果 [**DriveItem**](driveitem.md) 具有一个非 null **位置**方面，则该项表示一个已知位置和与其相关的文件。</span><span class="sxs-lookup"><span data-stu-id="4338c-p101">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4338c-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4338c-105">JSON representation</span></span>

<span data-ttu-id="4338c-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4338c-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="4338c-107">属性</span><span class="sxs-lookup"><span data-stu-id="4338c-107">Properties</span></span>

| <span data-ttu-id="4338c-108">属性</span><span class="sxs-lookup"><span data-stu-id="4338c-108">Property</span></span>  | <span data-ttu-id="4338c-109">类型</span><span class="sxs-lookup"><span data-stu-id="4338c-109">Type</span></span>   | <span data-ttu-id="4338c-110">说明</span><span class="sxs-lookup"><span data-stu-id="4338c-110">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="4338c-111">海拔</span><span class="sxs-lookup"><span data-stu-id="4338c-111">altitude</span></span>  | <span data-ttu-id="4338c-112">双精度数</span><span class="sxs-lookup"><span data-stu-id="4338c-112">Double</span></span> | <span data-ttu-id="4338c-p102">可选。此项高于海平面的高度（以英尺为单位）。只读。</span><span class="sxs-lookup"><span data-stu-id="4338c-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="4338c-116">纬度</span><span class="sxs-lookup"><span data-stu-id="4338c-116">latitude</span></span>  | <span data-ttu-id="4338c-117">双精度数</span><span class="sxs-lookup"><span data-stu-id="4338c-117">Double</span></span> | <span data-ttu-id="4338c-p103">可选。此项的纬度（以十进制表示）。只读。</span><span class="sxs-lookup"><span data-stu-id="4338c-p103">Optional. The latitude, in decimal, for the item. Read-only.</span></span>
| <span data-ttu-id="4338c-121">经度</span><span class="sxs-lookup"><span data-stu-id="4338c-121">longitude</span></span> | <span data-ttu-id="4338c-122">双精度数</span><span class="sxs-lookup"><span data-stu-id="4338c-122">Double</span></span> | <span data-ttu-id="4338c-p104">可选。此项的经度（以十进制表示）。只读。</span><span class="sxs-lookup"><span data-stu-id="4338c-p104">Optional. The longitude, in decimal, for the item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="4338c-126">注解</span><span class="sxs-lookup"><span data-stu-id="4338c-126">Remarks</span></span>

<span data-ttu-id="4338c-127">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="4338c-127">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location"
} -->
