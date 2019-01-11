---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
ms.openlocfilehash: d49142ed414ad82ec149792e11e5a8c42d9837dc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852638"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="a8825-102">GeoCoordinates 资源类型</span><span class="sxs-lookup"><span data-stu-id="a8825-102">GeoCoordinates resource type</span></span>

> <span data-ttu-id="a8825-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a8825-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8825-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a8825-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a8825-p102">**GeoCoordinates** 资源基于文件中包含的元数据提供位置的地理坐标和海拔。如果 [**DriveItem**](driveitem.md) 具有一个非 null **位置**方面，则该项表示一个已知位置和与其相关的文件。</span><span class="sxs-lookup"><span data-stu-id="a8825-p102">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8825-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a8825-107">JSON representation</span></span>

<span data-ttu-id="a8825-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a8825-108">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="a8825-109">属性</span><span class="sxs-lookup"><span data-stu-id="a8825-109">Properties</span></span>

| <span data-ttu-id="a8825-110">属性</span><span class="sxs-lookup"><span data-stu-id="a8825-110">Property</span></span>  | <span data-ttu-id="a8825-111">类型</span><span class="sxs-lookup"><span data-stu-id="a8825-111">Type</span></span>   | <span data-ttu-id="a8825-112">说明</span><span class="sxs-lookup"><span data-stu-id="a8825-112">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="a8825-113">海拔</span><span class="sxs-lookup"><span data-stu-id="a8825-113">altitude</span></span>  | <span data-ttu-id="a8825-114">Double</span><span class="sxs-lookup"><span data-stu-id="a8825-114">Double</span></span> | <span data-ttu-id="a8825-p103">可选。此项高于海平面的高度（以英尺为单位）。只读。</span><span class="sxs-lookup"><span data-stu-id="a8825-p103">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="a8825-118">纬度</span><span class="sxs-lookup"><span data-stu-id="a8825-118">latitude</span></span>  | <span data-ttu-id="a8825-119">Double</span><span class="sxs-lookup"><span data-stu-id="a8825-119">Double</span></span> | <span data-ttu-id="a8825-p104">可选。此项的纬度（以十进制表示）。只读。</span><span class="sxs-lookup"><span data-stu-id="a8825-p104">Optional. The latitude, in decimal, for the item. Read-only.</span></span>
| <span data-ttu-id="a8825-123">经度</span><span class="sxs-lookup"><span data-stu-id="a8825-123">longitude</span></span> | <span data-ttu-id="a8825-124">Double</span><span class="sxs-lookup"><span data-stu-id="a8825-124">Double</span></span> | <span data-ttu-id="a8825-p105">可选。此项的经度（以十进制表示）。只读。</span><span class="sxs-lookup"><span data-stu-id="a8825-p105">Optional. The longitude, in decimal, for the item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="a8825-128">注解</span><span class="sxs-lookup"><span data-stu-id="a8825-128">Remarks</span></span>

<span data-ttu-id="a8825-129">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="a8825-129">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location"
} -->
