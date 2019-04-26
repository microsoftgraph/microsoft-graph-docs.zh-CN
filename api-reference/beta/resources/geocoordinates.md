---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
ms.openlocfilehash: 39764148ce1a2d42226aafc24ef17ad1e5f19027
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340218"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="48b4b-102">GeoCoordinates 资源类型</span><span class="sxs-lookup"><span data-stu-id="48b4b-102">GeoCoordinates resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48b4b-p101">**GeoCoordinates** 资源基于文件中包含的元数据提供位置的地理坐标和海拔。如果 [**DriveItem**](driveitem.md) 具有一个非 null **位置**方面，则该项表示一个已知位置和与其相关的文件。</span><span class="sxs-lookup"><span data-stu-id="48b4b-p101">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="48b4b-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="48b4b-105">JSON representation</span></span>

<span data-ttu-id="48b4b-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="48b4b-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="48b4b-107">属性</span><span class="sxs-lookup"><span data-stu-id="48b4b-107">Properties</span></span>

| <span data-ttu-id="48b4b-108">属性</span><span class="sxs-lookup"><span data-stu-id="48b4b-108">Property</span></span>  | <span data-ttu-id="48b4b-109">类型</span><span class="sxs-lookup"><span data-stu-id="48b4b-109">Type</span></span>   | <span data-ttu-id="48b4b-110">说明</span><span class="sxs-lookup"><span data-stu-id="48b4b-110">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="48b4b-111">海拔</span><span class="sxs-lookup"><span data-stu-id="48b4b-111">altitude</span></span>  | <span data-ttu-id="48b4b-112">双精度</span><span class="sxs-lookup"><span data-stu-id="48b4b-112">Double</span></span> | <span data-ttu-id="48b4b-p102">可选。此项高于海平面的高度（以英尺为单位）。只读。</span><span class="sxs-lookup"><span data-stu-id="48b4b-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="48b4b-116">纬度</span><span class="sxs-lookup"><span data-stu-id="48b4b-116">latitude</span></span>  | <span data-ttu-id="48b4b-117">双精度</span><span class="sxs-lookup"><span data-stu-id="48b4b-117">Double</span></span> | <span data-ttu-id="48b4b-p103">可选。此项的纬度（以十进制表示）。只读。</span><span class="sxs-lookup"><span data-stu-id="48b4b-p103">Optional. The latitude, in decimal, for the item. Read-only.</span></span>
| <span data-ttu-id="48b4b-121">经度</span><span class="sxs-lookup"><span data-stu-id="48b4b-121">longitude</span></span> | <span data-ttu-id="48b4b-122">Double</span><span class="sxs-lookup"><span data-stu-id="48b4b-122">Double</span></span> | <span data-ttu-id="48b4b-p104">可选。此项的经度（以十进制表示）。只读。</span><span class="sxs-lookup"><span data-stu-id="48b4b-p104">Optional. The longitude, in decimal, for the item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="48b4b-126">注解</span><span class="sxs-lookup"><span data-stu-id="48b4b-126">Remarks</span></span>

<span data-ttu-id="48b4b-127">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="48b4b-127">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

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
