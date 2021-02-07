---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
description: GeoCoordinates 资源基于文件中包含的元数据提供位置的地理坐标和海拔。
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 048fefc8938a789a0aae06f3dd6f50c25c305c31
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130506"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="fe5cf-103">GeoCoordinates 资源类型</span><span class="sxs-lookup"><span data-stu-id="fe5cf-103">GeoCoordinates resource type</span></span>

<span data-ttu-id="fe5cf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe5cf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fe5cf-p101">**GeoCoordinates** 资源基于文件中包含的元数据提供位置的地理坐标和海拔。如果 [**DriveItem**](driveitem.md) 具有一个非 null **位置** 方面，则该项表示一个已知位置和与其相关的文件。</span><span class="sxs-lookup"><span data-stu-id="fe5cf-p101">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe5cf-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fe5cf-107">JSON representation</span></span>

<span data-ttu-id="fe5cf-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe5cf-108">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="fe5cf-109">属性</span><span class="sxs-lookup"><span data-stu-id="fe5cf-109">Properties</span></span>

| <span data-ttu-id="fe5cf-110">属性</span><span class="sxs-lookup"><span data-stu-id="fe5cf-110">Property</span></span>  | <span data-ttu-id="fe5cf-111">类型</span><span class="sxs-lookup"><span data-stu-id="fe5cf-111">Type</span></span>   | <span data-ttu-id="fe5cf-112">说明</span><span class="sxs-lookup"><span data-stu-id="fe5cf-112">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="fe5cf-113">海拔</span><span class="sxs-lookup"><span data-stu-id="fe5cf-113">altitude</span></span>  | <span data-ttu-id="fe5cf-114">Double</span><span class="sxs-lookup"><span data-stu-id="fe5cf-114">Double</span></span> | <span data-ttu-id="fe5cf-p102">可选。此项高于海平面的高度（以英尺为单位）。只读。</span><span class="sxs-lookup"><span data-stu-id="fe5cf-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="fe5cf-118">纬度</span><span class="sxs-lookup"><span data-stu-id="fe5cf-118">latitude</span></span>  | <span data-ttu-id="fe5cf-119">Double</span><span class="sxs-lookup"><span data-stu-id="fe5cf-119">Double</span></span> | <span data-ttu-id="fe5cf-p103">可选。此项的纬度（以十进制表示）。只读。</span><span class="sxs-lookup"><span data-stu-id="fe5cf-p103">Optional. The latitude, in decimal, for the item. Read-only.</span></span>
| <span data-ttu-id="fe5cf-123">经度</span><span class="sxs-lookup"><span data-stu-id="fe5cf-123">longitude</span></span> | <span data-ttu-id="fe5cf-124">Double</span><span class="sxs-lookup"><span data-stu-id="fe5cf-124">Double</span></span> | <span data-ttu-id="fe5cf-p104">可选。此项的经度（以十进制表示）。只读。</span><span class="sxs-lookup"><span data-stu-id="fe5cf-p104">Optional. The longitude, in decimal, for the item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="fe5cf-128">注解</span><span class="sxs-lookup"><span data-stu-id="fe5cf-128">Remarks</span></span>

<span data-ttu-id="fe5cf-129">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="fe5cf-129">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location"
} -->

