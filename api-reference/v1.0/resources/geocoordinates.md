---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: GeoCoordinates
ms.openlocfilehash: 0a4af14f08b94f0ba64f33838322fb0210bcda15
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010651"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="63409-102">GeoCoordinates 资源类型</span><span class="sxs-lookup"><span data-stu-id="63409-102">GeoCoordinates resource type</span></span>

<span data-ttu-id="63409-p101">**GeoCoordinates** 资源基于文件中包含的元数据提供位置的地理坐标和海拔。如果 [**DriveItem**](driveitem.md) 具有一个非 null **位置**方面，则该项表示一个已知位置和与其相关的文件。</span><span class="sxs-lookup"><span data-stu-id="63409-p101">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="63409-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="63409-105">JSON representation</span></span>

<span data-ttu-id="63409-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63409-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="63409-107">属性</span><span class="sxs-lookup"><span data-stu-id="63409-107">Properties</span></span>

| <span data-ttu-id="63409-108">属性</span><span class="sxs-lookup"><span data-stu-id="63409-108">Property</span></span>  | <span data-ttu-id="63409-109">类型</span><span class="sxs-lookup"><span data-stu-id="63409-109">Type</span></span>   | <span data-ttu-id="63409-110">说明</span><span class="sxs-lookup"><span data-stu-id="63409-110">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="63409-111">海拔</span><span class="sxs-lookup"><span data-stu-id="63409-111">altitude</span></span>  | <span data-ttu-id="63409-112">双精度数</span><span class="sxs-lookup"><span data-stu-id="63409-112">Double</span></span> | <span data-ttu-id="63409-p102">可选。此项高于海平面的高度（以英尺为单位）。只读。</span><span class="sxs-lookup"><span data-stu-id="63409-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="63409-116">纬度</span><span class="sxs-lookup"><span data-stu-id="63409-116">latitude</span></span>  | <span data-ttu-id="63409-117">双精度数</span><span class="sxs-lookup"><span data-stu-id="63409-117">Double</span></span> | <span data-ttu-id="63409-p103">可选。此项的纬度（以十进制表示）。只读。</span><span class="sxs-lookup"><span data-stu-id="63409-p103">Optional. The latitude, in decimal, for the item. Read-only.</span></span>
| <span data-ttu-id="63409-121">经度</span><span class="sxs-lookup"><span data-stu-id="63409-121">longitude</span></span> | <span data-ttu-id="63409-122">双精度数</span><span class="sxs-lookup"><span data-stu-id="63409-122">Double</span></span> | <span data-ttu-id="63409-p104">可选。此项的经度（以十进制表示）。只读。</span><span class="sxs-lookup"><span data-stu-id="63409-p104">Optional. The longitude, in decimal, for the item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="63409-126">注解</span><span class="sxs-lookup"><span data-stu-id="63409-126">Remarks</span></span>

<span data-ttu-id="63409-127">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="63409-127">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location"
} -->
