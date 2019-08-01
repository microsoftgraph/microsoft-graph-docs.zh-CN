---
title: outlookGeoCoordinates 资源类型
description: 地理坐标、海拔，以及它们物理位置的精确度。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 6cfa08c15318fdaa58ac71e01a940b621b207f12
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035670"
---
# <a name="outlookgeocoordinates-resource-type"></a><span data-ttu-id="da2f9-103">outlookGeoCoordinates 资源类型</span><span class="sxs-lookup"><span data-stu-id="da2f9-103">outlookGeoCoordinates resource type</span></span>

<span data-ttu-id="da2f9-104">地理坐标、海拔，以及它们物理位置的精确度。</span><span class="sxs-lookup"><span data-stu-id="da2f9-104">The geographic coordinates, elevation, and their degree of accuracy for a physical location.</span></span>

## <a name="json-representation"></a><span data-ttu-id="da2f9-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="da2f9-105">JSON representation</span></span>

<span data-ttu-id="da2f9-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da2f9-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="da2f9-107">属性</span><span class="sxs-lookup"><span data-stu-id="da2f9-107">Properties</span></span>
| <span data-ttu-id="da2f9-108">属性</span><span class="sxs-lookup"><span data-stu-id="da2f9-108">Property</span></span>     | <span data-ttu-id="da2f9-109">类型</span><span class="sxs-lookup"><span data-stu-id="da2f9-109">Type</span></span>   |<span data-ttu-id="da2f9-110">说明</span><span class="sxs-lookup"><span data-stu-id="da2f9-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da2f9-111">accuracy</span><span class="sxs-lookup"><span data-stu-id="da2f9-111">accuracy</span></span>|<span data-ttu-id="da2f9-112">double</span><span class="sxs-lookup"><span data-stu-id="da2f9-112">double</span></span>|<span data-ttu-id="da2f9-113">纬度和经度的精确度。</span><span class="sxs-lookup"><span data-stu-id="da2f9-113">The accuracy of the latitude and longitude.</span></span> <span data-ttu-id="da2f9-114">举个例子，精确度可以以米为单位度量，如纬度和经度可以精确到 50 米内。</span><span class="sxs-lookup"><span data-stu-id="da2f9-114">As an example, the accuracy can be measured in meters, such as the latitude and longitude are accurate to within 50 meters.</span></span>|
|<span data-ttu-id="da2f9-115">altitude</span><span class="sxs-lookup"><span data-stu-id="da2f9-115">altitude</span></span>|<span data-ttu-id="da2f9-116">double</span><span class="sxs-lookup"><span data-stu-id="da2f9-116">double</span></span>|<span data-ttu-id="da2f9-117">位置的海拔高度。</span><span class="sxs-lookup"><span data-stu-id="da2f9-117">The altitude of the location.</span></span>|
|<span data-ttu-id="da2f9-118">altitudeAccuracy</span><span class="sxs-lookup"><span data-stu-id="da2f9-118">altitudeAccuracy</span></span>|<span data-ttu-id="da2f9-119">double</span><span class="sxs-lookup"><span data-stu-id="da2f9-119">double</span></span>|<span data-ttu-id="da2f9-120">海拔高度的精确度。</span><span class="sxs-lookup"><span data-stu-id="da2f9-120">The accuracy of the altitude.</span></span>|
|<span data-ttu-id="da2f9-121">latitude</span><span class="sxs-lookup"><span data-stu-id="da2f9-121">latitude</span></span>|<span data-ttu-id="da2f9-122">double</span><span class="sxs-lookup"><span data-stu-id="da2f9-122">double</span></span>|<span data-ttu-id="da2f9-123">位置的纬度。</span><span class="sxs-lookup"><span data-stu-id="da2f9-123">The latitude of the location.</span></span>|
|<span data-ttu-id="da2f9-124">longitude</span><span class="sxs-lookup"><span data-stu-id="da2f9-124">longitude</span></span>|<span data-ttu-id="da2f9-125">double</span><span class="sxs-lookup"><span data-stu-id="da2f9-125">double</span></span>|<span data-ttu-id="da2f9-126">位置的经度。</span><span class="sxs-lookup"><span data-stu-id="da2f9-126">The longitude of the location.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
