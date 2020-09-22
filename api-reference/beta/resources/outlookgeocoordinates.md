---
title: outlookGeoCoordinates 资源类型
description: 地理坐标、海拔，以及它们物理位置的精确度。
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: edc2d02919b876cbd77ddc8cd7995c1670628fc1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998369"
---
# <a name="outlookgeocoordinates-resource-type"></a><span data-ttu-id="99a8a-103">outlookGeoCoordinates 资源类型</span><span class="sxs-lookup"><span data-stu-id="99a8a-103">outlookGeoCoordinates resource type</span></span>

<span data-ttu-id="99a8a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99a8a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99a8a-105">地理坐标、海拔，以及它们物理位置的精确度。</span><span class="sxs-lookup"><span data-stu-id="99a8a-105">The geographic coordinates, elevation, and their degree of accuracy for a physical location.</span></span>

## <a name="json-representation"></a><span data-ttu-id="99a8a-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="99a8a-106">JSON representation</span></span>

<span data-ttu-id="99a8a-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99a8a-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookGeoCoordinates"
}-->

```json
{
  "accuracy": 1024.13,
  "altitude": 1024.13,
  "altitudeAccuracy": 1024.13,
  "latitude": 1024.13,
  "longitude": 1024.13
}

```
## <a name="properties"></a><span data-ttu-id="99a8a-108">属性</span><span class="sxs-lookup"><span data-stu-id="99a8a-108">Properties</span></span>
| <span data-ttu-id="99a8a-109">属性</span><span class="sxs-lookup"><span data-stu-id="99a8a-109">Property</span></span>     | <span data-ttu-id="99a8a-110">类型</span><span class="sxs-lookup"><span data-stu-id="99a8a-110">Type</span></span>   |<span data-ttu-id="99a8a-111">说明</span><span class="sxs-lookup"><span data-stu-id="99a8a-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99a8a-112">accuracy</span><span class="sxs-lookup"><span data-stu-id="99a8a-112">accuracy</span></span>|<span data-ttu-id="99a8a-113">double</span><span class="sxs-lookup"><span data-stu-id="99a8a-113">double</span></span>|<span data-ttu-id="99a8a-114">纬度和经度的精确度。</span><span class="sxs-lookup"><span data-stu-id="99a8a-114">The accuracy of the latitude and longitude.</span></span> <span data-ttu-id="99a8a-115">举个例子，精确度可以以米为单位度量，如纬度和经度可以精确到 50 米内。</span><span class="sxs-lookup"><span data-stu-id="99a8a-115">As an example, the accuracy can be measured in meters, such as the latitude and longitude are accurate to within 50 meters.</span></span>|
|<span data-ttu-id="99a8a-116">altitude</span><span class="sxs-lookup"><span data-stu-id="99a8a-116">altitude</span></span>|<span data-ttu-id="99a8a-117">double</span><span class="sxs-lookup"><span data-stu-id="99a8a-117">double</span></span>|<span data-ttu-id="99a8a-118">位置的海拔高度。</span><span class="sxs-lookup"><span data-stu-id="99a8a-118">The altitude of the location.</span></span>|
|<span data-ttu-id="99a8a-119">altitudeAccuracy</span><span class="sxs-lookup"><span data-stu-id="99a8a-119">altitudeAccuracy</span></span>|<span data-ttu-id="99a8a-120">double</span><span class="sxs-lookup"><span data-stu-id="99a8a-120">double</span></span>|<span data-ttu-id="99a8a-121">海拔高度的精确度。</span><span class="sxs-lookup"><span data-stu-id="99a8a-121">The accuracy of the altitude.</span></span>|
|<span data-ttu-id="99a8a-122">latitude</span><span class="sxs-lookup"><span data-stu-id="99a8a-122">latitude</span></span>|<span data-ttu-id="99a8a-123">double</span><span class="sxs-lookup"><span data-stu-id="99a8a-123">double</span></span>|<span data-ttu-id="99a8a-124">位置的纬度。</span><span class="sxs-lookup"><span data-stu-id="99a8a-124">The latitude of the location.</span></span>|
|<span data-ttu-id="99a8a-125">longitude</span><span class="sxs-lookup"><span data-stu-id="99a8a-125">longitude</span></span>|<span data-ttu-id="99a8a-126">double</span><span class="sxs-lookup"><span data-stu-id="99a8a-126">double</span></span>|<span data-ttu-id="99a8a-127">位置的经度。</span><span class="sxs-lookup"><span data-stu-id="99a8a-127">The longitude of the location.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


