---
title: signInLocation 资源类型
description: 提供发生登录的城市、省/市/自治区和国家/地区。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: bf0cdec3a2c5feae1b178fc92d02e433d87737a1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965024"
---
# <a name="signinlocation-resource-type"></a><span data-ttu-id="12df9-103">signInLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="12df9-103">signInLocation resource type</span></span>
<span data-ttu-id="12df9-104">提供发生登录的城市、省/市/自治区和国家/地区。</span><span class="sxs-lookup"><span data-stu-id="12df9-104">Provides the city, state and country/region from where the sign-in happened.</span></span>



## <a name="properties"></a><span data-ttu-id="12df9-105">属性</span><span class="sxs-lookup"><span data-stu-id="12df9-105">Properties</span></span>
| <span data-ttu-id="12df9-106">属性</span><span class="sxs-lookup"><span data-stu-id="12df9-106">Property</span></span>     | <span data-ttu-id="12df9-107">类型</span><span class="sxs-lookup"><span data-stu-id="12df9-107">Type</span></span>   |<span data-ttu-id="12df9-108">说明</span><span class="sxs-lookup"><span data-stu-id="12df9-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12df9-109">city</span><span class="sxs-lookup"><span data-stu-id="12df9-109">city</span></span>|<span data-ttu-id="12df9-110">String</span><span class="sxs-lookup"><span data-stu-id="12df9-110">String</span></span>|<span data-ttu-id="12df9-111">提供发起登录的城市。</span><span class="sxs-lookup"><span data-stu-id="12df9-111">Provides the city where the sign-in originated.</span></span> <span data-ttu-id="12df9-112">这是通过登录活动中的纬度/经度信息计算得出的。</span><span class="sxs-lookup"><span data-stu-id="12df9-112">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="12df9-113">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="12df9-113">countryOrRegion</span></span>|<span data-ttu-id="12df9-114">String</span><span class="sxs-lookup"><span data-stu-id="12df9-114">String</span></span>|<span data-ttu-id="12df9-115">提供登录所源于的国家/地区代码信息 (2 个字母代码)。</span><span class="sxs-lookup"><span data-stu-id="12df9-115">Provides the country code info (2 letter code) where the sign-in originated.</span></span>  <span data-ttu-id="12df9-116">这是通过登录活动中的纬度/经度信息计算得出的。</span><span class="sxs-lookup"><span data-stu-id="12df9-116">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="12df9-117">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="12df9-117">geoCoordinates</span></span>|[<span data-ttu-id="12df9-118">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="12df9-118">geoCoordinates</span></span>](geocoordinates.md)|<span data-ttu-id="12df9-119">提供登录所源于的纬度、经度和海拔高度。</span><span class="sxs-lookup"><span data-stu-id="12df9-119">Provides the latitude, longitude and altitude where the sign-in originated.</span></span>|
|<span data-ttu-id="12df9-120">state</span><span class="sxs-lookup"><span data-stu-id="12df9-120">state</span></span>|<span data-ttu-id="12df9-121">String</span><span class="sxs-lookup"><span data-stu-id="12df9-121">String</span></span>|<span data-ttu-id="12df9-122">提供登录的起始状态。</span><span class="sxs-lookup"><span data-stu-id="12df9-122">Provides the State where the sign-in originated.</span></span> <span data-ttu-id="12df9-123">这是通过登录活动中的纬度/经度信息计算得出的。</span><span class="sxs-lookup"><span data-stu-id="12df9-123">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="12df9-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="12df9-124">JSON representation</span></span>

<span data-ttu-id="12df9-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12df9-125">Here is a JSON representation of the resource.</span></span>

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
