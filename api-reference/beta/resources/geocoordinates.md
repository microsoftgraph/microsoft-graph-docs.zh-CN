---
author: JeremyKelley
description: GeoCoordinates 资源基于文件中包含的元数据提供位置的地理坐标和海拔。
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 98f9c09c4604311c0cc741028565be860eb996ef
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971945"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="b0c88-103">GeoCoordinates 资源类型</span><span class="sxs-lookup"><span data-stu-id="b0c88-103">GeoCoordinates resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0c88-p101">**GeoCoordinates** 资源基于文件中包含的元数据提供位置的地理坐标和海拔。如果 [**DriveItem**](driveitem.md) 具有一个非 null **位置**方面，则该项表示一个已知位置和与其相关的文件。</span><span class="sxs-lookup"><span data-stu-id="b0c88-p101">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0c88-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b0c88-106">JSON representation</span></span>

<span data-ttu-id="b0c88-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0c88-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="b0c88-108">属性</span><span class="sxs-lookup"><span data-stu-id="b0c88-108">Properties</span></span>

| <span data-ttu-id="b0c88-109">属性</span><span class="sxs-lookup"><span data-stu-id="b0c88-109">Property</span></span>  | <span data-ttu-id="b0c88-110">类型</span><span class="sxs-lookup"><span data-stu-id="b0c88-110">Type</span></span>   | <span data-ttu-id="b0c88-111">说明</span><span class="sxs-lookup"><span data-stu-id="b0c88-111">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="b0c88-112">海拔</span><span class="sxs-lookup"><span data-stu-id="b0c88-112">altitude</span></span>  | <span data-ttu-id="b0c88-113">双精度</span><span class="sxs-lookup"><span data-stu-id="b0c88-113">Double</span></span> | <span data-ttu-id="b0c88-p102">可选。此项高于海平面的高度（以英尺为单位）。只读。</span><span class="sxs-lookup"><span data-stu-id="b0c88-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="b0c88-117">纬度</span><span class="sxs-lookup"><span data-stu-id="b0c88-117">latitude</span></span>  | <span data-ttu-id="b0c88-118">双精度</span><span class="sxs-lookup"><span data-stu-id="b0c88-118">Double</span></span> | <span data-ttu-id="b0c88-p103">可选。此项的纬度（以十进制表示）。只读。</span><span class="sxs-lookup"><span data-stu-id="b0c88-p103">Optional. The latitude, in decimal, for the item. Read-only.</span></span>
| <span data-ttu-id="b0c88-122">经度</span><span class="sxs-lookup"><span data-stu-id="b0c88-122">longitude</span></span> | <span data-ttu-id="b0c88-123">Double</span><span class="sxs-lookup"><span data-stu-id="b0c88-123">Double</span></span> | <span data-ttu-id="b0c88-p104">可选。此项的经度（以十进制表示）。只读。</span><span class="sxs-lookup"><span data-stu-id="b0c88-p104">Optional. The longitude, in decimal, for the item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="b0c88-127">注解</span><span class="sxs-lookup"><span data-stu-id="b0c88-127">Remarks</span></span>

<span data-ttu-id="b0c88-128">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="b0c88-128">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

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
