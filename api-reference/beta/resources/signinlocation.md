---
title: signInLocation 资源类型
description: 提供登录发生位置的城市、省/市/自治区和国家/地区。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: SarahBar
ms.openlocfilehash: bc45d94896cbd822cdad4e3451f471bc3b540888
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134678"
---
# <a name="signinlocation-resource-type"></a><span data-ttu-id="3811f-103">signInLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="3811f-103">signInLocation resource type</span></span>

<span data-ttu-id="3811f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3811f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3811f-105">提供登录发生位置的城市、省/市/自治区和国家/地区。</span><span class="sxs-lookup"><span data-stu-id="3811f-105">Provides the city, state and country/region from where the sign-in happened.</span></span>



## <a name="properties"></a><span data-ttu-id="3811f-106">属性</span><span class="sxs-lookup"><span data-stu-id="3811f-106">Properties</span></span>
| <span data-ttu-id="3811f-107">属性</span><span class="sxs-lookup"><span data-stu-id="3811f-107">Property</span></span>     | <span data-ttu-id="3811f-108">类型</span><span class="sxs-lookup"><span data-stu-id="3811f-108">Type</span></span>   |<span data-ttu-id="3811f-109">说明</span><span class="sxs-lookup"><span data-stu-id="3811f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3811f-110">城市</span><span class="sxs-lookup"><span data-stu-id="3811f-110">city</span></span>|<span data-ttu-id="3811f-111">String</span><span class="sxs-lookup"><span data-stu-id="3811f-111">String</span></span>|<span data-ttu-id="3811f-112">提供登录来源城市。</span><span class="sxs-lookup"><span data-stu-id="3811f-112">Provides the city where the sign-in originated.</span></span> <span data-ttu-id="3811f-113">这是使用登录活动中的纬度/经度信息计算得出的。</span><span class="sxs-lookup"><span data-stu-id="3811f-113">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="3811f-114">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="3811f-114">countryOrRegion</span></span>|<span data-ttu-id="3811f-115">String</span><span class="sxs-lookup"><span data-stu-id="3811f-115">String</span></span>|<span data-ttu-id="3811f-116">提供登录 (位置) 2 个字母代码的国家/地区代码信息。</span><span class="sxs-lookup"><span data-stu-id="3811f-116">Provides the country code info (2 letter code) where the sign-in originated.</span></span>  <span data-ttu-id="3811f-117">这是使用登录活动中的纬度/经度信息计算得出的。</span><span class="sxs-lookup"><span data-stu-id="3811f-117">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="3811f-118">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="3811f-118">geoCoordinates</span></span>|[<span data-ttu-id="3811f-119">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="3811f-119">geoCoordinates</span></span>](geocoordinates.md)|<span data-ttu-id="3811f-120">提供登录来源的纬度、经度和高度。</span><span class="sxs-lookup"><span data-stu-id="3811f-120">Provides the latitude, longitude and altitude where the sign-in originated.</span></span>|
|<span data-ttu-id="3811f-121">state</span><span class="sxs-lookup"><span data-stu-id="3811f-121">state</span></span>|<span data-ttu-id="3811f-122">String</span><span class="sxs-lookup"><span data-stu-id="3811f-122">String</span></span>|<span data-ttu-id="3811f-123">提供登录来源的状态。</span><span class="sxs-lookup"><span data-stu-id="3811f-123">Provides the State where the sign-in originated.</span></span> <span data-ttu-id="3811f-124">这是使用登录活动中的纬度/经度信息计算得出的。</span><span class="sxs-lookup"><span data-stu-id="3811f-124">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3811f-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3811f-125">JSON representation</span></span>

<span data-ttu-id="3811f-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3811f-126">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInLocation"
}-->

```json
{
  "city": "String",
  "countryOrRegion": "String",
  "geoCoordinates": {"@odata.type": "microsoft.graph.geoCoordinates"},
  "state": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


