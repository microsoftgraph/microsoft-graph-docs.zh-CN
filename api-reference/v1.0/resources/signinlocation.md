---
title: signInLocation 资源类型
description: 提供发生登录的城市、省/市/自治区和国家/地区。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 35c6511b7dba69a362b44a9390974913c46b73ee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034214"
---
# <a name="signinlocation-resource-type"></a><span data-ttu-id="7734c-103">signInLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="7734c-103">signInLocation resource type</span></span>

<span data-ttu-id="7734c-104">提供发生登录的城市、省/市/自治区和国家/地区。</span><span class="sxs-lookup"><span data-stu-id="7734c-104">Provides the city, state and country/region from where the sign-in happened.</span></span>

## <a name="properties"></a><span data-ttu-id="7734c-105">属性</span><span class="sxs-lookup"><span data-stu-id="7734c-105">Properties</span></span>

| <span data-ttu-id="7734c-106">属性</span><span class="sxs-lookup"><span data-stu-id="7734c-106">Property</span></span>     | <span data-ttu-id="7734c-107">类型</span><span class="sxs-lookup"><span data-stu-id="7734c-107">Type</span></span>   |<span data-ttu-id="7734c-108">说明</span><span class="sxs-lookup"><span data-stu-id="7734c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7734c-109">city</span><span class="sxs-lookup"><span data-stu-id="7734c-109">city</span></span>|<span data-ttu-id="7734c-110">String</span><span class="sxs-lookup"><span data-stu-id="7734c-110">String</span></span>|<span data-ttu-id="7734c-111">提供发起登录的城市。</span><span class="sxs-lookup"><span data-stu-id="7734c-111">Provides the city where the sign-in originated.</span></span> <span data-ttu-id="7734c-112">这是通过登录活动中的纬度/经度信息计算得出的。</span><span class="sxs-lookup"><span data-stu-id="7734c-112">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="7734c-113">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="7734c-113">countryOrRegion</span></span>|<span data-ttu-id="7734c-114">String</span><span class="sxs-lookup"><span data-stu-id="7734c-114">String</span></span>|<span data-ttu-id="7734c-115">提供登录所源于的国家/地区代码信息 (2 个字母代码)。</span><span class="sxs-lookup"><span data-stu-id="7734c-115">Provides the country code info (2 letter code) where the sign-in originated.</span></span>  <span data-ttu-id="7734c-116">这是通过登录活动中的纬度/经度信息计算得出的。</span><span class="sxs-lookup"><span data-stu-id="7734c-116">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="7734c-117">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="7734c-117">geoCoordinates</span></span>|[<span data-ttu-id="7734c-118">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="7734c-118">geoCoordinates</span></span>](geocoordinates.md)|<span data-ttu-id="7734c-119">提供登录所源于的纬度、经度和海拔高度。</span><span class="sxs-lookup"><span data-stu-id="7734c-119">Provides the latitude, longitude and altitude where the sign-in originated.</span></span>|
|<span data-ttu-id="7734c-120">state</span><span class="sxs-lookup"><span data-stu-id="7734c-120">state</span></span>|<span data-ttu-id="7734c-121">String</span><span class="sxs-lookup"><span data-stu-id="7734c-121">String</span></span>|<span data-ttu-id="7734c-122">提供登录的起始状态。</span><span class="sxs-lookup"><span data-stu-id="7734c-122">Provides the State where the sign-in originated.</span></span> <span data-ttu-id="7734c-123">这是通过登录活动中的纬度/经度信息计算得出的。</span><span class="sxs-lookup"><span data-stu-id="7734c-123">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7734c-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7734c-124">JSON representation</span></span>

<span data-ttu-id="7734c-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7734c-125">Here is a JSON representation of the resource.</span></span>

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
