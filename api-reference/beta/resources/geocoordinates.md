---
author: JeremyKelley
description: GeoCoordinates 资源根据文件中包含的元数据提供位置的地理坐标和仰角。
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: d091858c4856ad133b72e757e837fb49b3c0594f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033837"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="16c30-103">geoCoordinates 资源类型</span><span class="sxs-lookup"><span data-stu-id="16c30-103">geoCoordinates resource type</span></span>

<span data-ttu-id="16c30-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16c30-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16c30-105">根据文件中包含的元数据提供位置的地理坐标和仰角。</span><span class="sxs-lookup"><span data-stu-id="16c30-105">Provides geographic coordinates and elevation of a location based on metadata contained within the file.</span></span>
<span data-ttu-id="16c30-106">如果 [**driveItem**](driveitem.md) 具有非 null **位置** facet，则该项目表示一个文件，其中包含一个已知的位置关联。</span><span class="sxs-lookup"><span data-stu-id="16c30-106">If a [**driveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

> [!NOTE]
> <span data-ttu-id="16c30-107">更新照片的纬度和经度时，必须提供 [照片](photo.md) 资源 (空或其他) 。</span><span class="sxs-lookup"><span data-stu-id="16c30-107">When updating the latitude and longitude of a photo, a [photo](photo.md) resource (empty or otherwise) must be provided.</span></span>

## <a name="properties"></a><span data-ttu-id="16c30-108">属性</span><span class="sxs-lookup"><span data-stu-id="16c30-108">Properties</span></span>

| <span data-ttu-id="16c30-109">属性</span><span class="sxs-lookup"><span data-stu-id="16c30-109">Property</span></span>  | <span data-ttu-id="16c30-110">类型</span><span class="sxs-lookup"><span data-stu-id="16c30-110">Type</span></span>   | <span data-ttu-id="16c30-111">说明</span><span class="sxs-lookup"><span data-stu-id="16c30-111">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="16c30-112">海拔</span><span class="sxs-lookup"><span data-stu-id="16c30-112">altitude</span></span>  | <span data-ttu-id="16c30-113">Double</span><span class="sxs-lookup"><span data-stu-id="16c30-113">Double</span></span> | <span data-ttu-id="16c30-p102">可选。此项高于海平面的高度（以英尺为单位）。只读。</span><span class="sxs-lookup"><span data-stu-id="16c30-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="16c30-117">纬度</span><span class="sxs-lookup"><span data-stu-id="16c30-117">latitude</span></span>  | <span data-ttu-id="16c30-118">Double</span><span class="sxs-lookup"><span data-stu-id="16c30-118">Double</span></span> | <span data-ttu-id="16c30-119">可选。</span><span class="sxs-lookup"><span data-stu-id="16c30-119">Optional.</span></span> <span data-ttu-id="16c30-120">此项的纬度（以十进制表示）。</span><span class="sxs-lookup"><span data-stu-id="16c30-120">The latitude, in decimal, for the item.</span></span> <span data-ttu-id="16c30-121">在 OneDrive 个人版上是可写的。</span><span class="sxs-lookup"><span data-stu-id="16c30-121">Writable on OneDrive Personal.</span></span>
| <span data-ttu-id="16c30-122">longitude</span><span class="sxs-lookup"><span data-stu-id="16c30-122">longitude</span></span> | <span data-ttu-id="16c30-123">Double</span><span class="sxs-lookup"><span data-stu-id="16c30-123">Double</span></span> | <span data-ttu-id="16c30-124">可选。</span><span class="sxs-lookup"><span data-stu-id="16c30-124">Optional.</span></span> <span data-ttu-id="16c30-125">此项的经度（以十进制表示）。</span><span class="sxs-lookup"><span data-stu-id="16c30-125">The longitude, in decimal, for the item.</span></span> <span data-ttu-id="16c30-126">在 OneDrive 个人版上是可写的。</span><span class="sxs-lookup"><span data-stu-id="16c30-126">Writable on OneDrive Personal.</span></span>

## <a name="json-representation"></a><span data-ttu-id="16c30-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="16c30-127">JSON representation</span></span>

<span data-ttu-id="16c30-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="16c30-128">Here is a JSON representation of the resource</span></span>

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


