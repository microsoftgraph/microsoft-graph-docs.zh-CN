---
title: outlookGeoCoordinates 资源类型
description: 地理坐标、海拔，以及它们物理位置的精确度。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7ca63aa3df6a597aaacb81fbeacf275ac87064f1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511833"
---
# <a name="outlookgeocoordinates-resource-type"></a><span data-ttu-id="175c8-103">outlookGeoCoordinates 资源类型</span><span class="sxs-lookup"><span data-stu-id="175c8-103">outlookGeoCoordinates resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="175c8-104">地理坐标、海拔，以及它们物理位置的精确度。</span><span class="sxs-lookup"><span data-stu-id="175c8-104">The geographic coordinates, elevation, and their degree of accuracy for a physical location.</span></span>

## <a name="json-representation"></a><span data-ttu-id="175c8-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="175c8-105">JSON representation</span></span>

<span data-ttu-id="175c8-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="175c8-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="175c8-107">属性</span><span class="sxs-lookup"><span data-stu-id="175c8-107">Properties</span></span>
| <span data-ttu-id="175c8-108">属性</span><span class="sxs-lookup"><span data-stu-id="175c8-108">Property</span></span>     | <span data-ttu-id="175c8-109">类型</span><span class="sxs-lookup"><span data-stu-id="175c8-109">Type</span></span>   |<span data-ttu-id="175c8-110">说明</span><span class="sxs-lookup"><span data-stu-id="175c8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="175c8-111">accuracy</span><span class="sxs-lookup"><span data-stu-id="175c8-111">accuracy</span></span>|<span data-ttu-id="175c8-112">double</span><span class="sxs-lookup"><span data-stu-id="175c8-112">double</span></span>|<span data-ttu-id="175c8-113">纬度和经度的精确度。</span><span class="sxs-lookup"><span data-stu-id="175c8-113">The accuracy of the latitude and longitude.</span></span> <span data-ttu-id="175c8-114">举个例子，精确度可以以米为单位度量，如纬度和经度可以精确到 50 米内。</span><span class="sxs-lookup"><span data-stu-id="175c8-114">As an example, the accuracy can be measured in meters, such as the latitude and longitude are accurate to within 50 meters.</span></span>|
|<span data-ttu-id="175c8-115">altitude</span><span class="sxs-lookup"><span data-stu-id="175c8-115">altitude</span></span>|<span data-ttu-id="175c8-116">double</span><span class="sxs-lookup"><span data-stu-id="175c8-116">double</span></span>|<span data-ttu-id="175c8-117">位置的海拔高度。</span><span class="sxs-lookup"><span data-stu-id="175c8-117">The altitude of the location.</span></span>|
|<span data-ttu-id="175c8-118">altitudeAccuracy</span><span class="sxs-lookup"><span data-stu-id="175c8-118">altitudeAccuracy</span></span>|<span data-ttu-id="175c8-119">double</span><span class="sxs-lookup"><span data-stu-id="175c8-119">double</span></span>|<span data-ttu-id="175c8-120">海拔高度的精确度。</span><span class="sxs-lookup"><span data-stu-id="175c8-120">The accuracy of the altitude.</span></span>|
|<span data-ttu-id="175c8-121">latitude</span><span class="sxs-lookup"><span data-stu-id="175c8-121">latitude</span></span>|<span data-ttu-id="175c8-122">double</span><span class="sxs-lookup"><span data-stu-id="175c8-122">double</span></span>|<span data-ttu-id="175c8-123">位置的纬度。</span><span class="sxs-lookup"><span data-stu-id="175c8-123">The latitude of the location.</span></span>|
|<span data-ttu-id="175c8-124">longitude</span><span class="sxs-lookup"><span data-stu-id="175c8-124">longitude</span></span>|<span data-ttu-id="175c8-125">double</span><span class="sxs-lookup"><span data-stu-id="175c8-125">double</span></span>|<span data-ttu-id="175c8-126">位置的经度。</span><span class="sxs-lookup"><span data-stu-id="175c8-126">The longitude of the location.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/outlookgeocoordinates.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
