---
title: outlookGeoCoordinates 资源类型
description: 地理坐标、海拔，以及它们物理位置的精确度。
localization_priority: Normal
ms.openlocfilehash: 2522410cd55705411084945b0519738871dedaa0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845358"
---
# <a name="outlookgeocoordinates-resource-type"></a><span data-ttu-id="a5ede-103">outlookGeoCoordinates 资源类型</span><span class="sxs-lookup"><span data-stu-id="a5ede-103">outlookGeoCoordinates resource type</span></span>

> <span data-ttu-id="a5ede-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a5ede-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5ede-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a5ede-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a5ede-106">地理坐标、海拔，以及它们物理位置的精确度。</span><span class="sxs-lookup"><span data-stu-id="a5ede-106">The geographic coordinates, elevation, and their degree of accuracy for a physical location.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5ede-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a5ede-107">JSON representation</span></span>

<span data-ttu-id="a5ede-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a5ede-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="a5ede-109">属性</span><span class="sxs-lookup"><span data-stu-id="a5ede-109">Properties</span></span>
| <span data-ttu-id="a5ede-110">属性</span><span class="sxs-lookup"><span data-stu-id="a5ede-110">Property</span></span>     | <span data-ttu-id="a5ede-111">类型</span><span class="sxs-lookup"><span data-stu-id="a5ede-111">Type</span></span>   |<span data-ttu-id="a5ede-112">说明</span><span class="sxs-lookup"><span data-stu-id="a5ede-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5ede-113">accuracy</span><span class="sxs-lookup"><span data-stu-id="a5ede-113">accuracy</span></span>|<span data-ttu-id="a5ede-114">double</span><span class="sxs-lookup"><span data-stu-id="a5ede-114">double</span></span>|<span data-ttu-id="a5ede-115">纬度和经度的精确度。</span><span class="sxs-lookup"><span data-stu-id="a5ede-115">The accuracy of the latitude and longitude.</span></span> <span data-ttu-id="a5ede-116">举个例子，精确度可以以米为单位度量，如纬度和经度可以精确到 50 米内。</span><span class="sxs-lookup"><span data-stu-id="a5ede-116">As an example, the accuracy can be measured in meters, such as the latitude and longitude are accurate to within 50 meters.</span></span>|
|<span data-ttu-id="a5ede-117">altitude</span><span class="sxs-lookup"><span data-stu-id="a5ede-117">altitude</span></span>|<span data-ttu-id="a5ede-118">double</span><span class="sxs-lookup"><span data-stu-id="a5ede-118">double</span></span>|<span data-ttu-id="a5ede-119">位置的海拔高度。</span><span class="sxs-lookup"><span data-stu-id="a5ede-119">The altitude of the location.</span></span>|
|<span data-ttu-id="a5ede-120">altitudeAccuracy</span><span class="sxs-lookup"><span data-stu-id="a5ede-120">altitudeAccuracy</span></span>|<span data-ttu-id="a5ede-121">double</span><span class="sxs-lookup"><span data-stu-id="a5ede-121">double</span></span>|<span data-ttu-id="a5ede-122">海拔高度的精确度。</span><span class="sxs-lookup"><span data-stu-id="a5ede-122">The accuracy of the altitude.</span></span>|
|<span data-ttu-id="a5ede-123">latitude</span><span class="sxs-lookup"><span data-stu-id="a5ede-123">latitude</span></span>|<span data-ttu-id="a5ede-124">double</span><span class="sxs-lookup"><span data-stu-id="a5ede-124">double</span></span>|<span data-ttu-id="a5ede-125">位置的纬度。</span><span class="sxs-lookup"><span data-stu-id="a5ede-125">The latitude of the location.</span></span>|
|<span data-ttu-id="a5ede-126">longitude</span><span class="sxs-lookup"><span data-stu-id="a5ede-126">longitude</span></span>|<span data-ttu-id="a5ede-127">double</span><span class="sxs-lookup"><span data-stu-id="a5ede-127">double</span></span>|<span data-ttu-id="a5ede-128">位置的经度。</span><span class="sxs-lookup"><span data-stu-id="a5ede-128">The longitude of the location.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
