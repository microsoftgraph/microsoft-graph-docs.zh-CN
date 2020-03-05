---
title: signInLocation 资源类型
description: 提供发生登录的城市、省/市/自治区和国家/地区。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 58c3dc2b25b85963e6a0f6f88552dbf2a121d5f7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446854"
---
# <a name="signinlocation-resource-type"></a><span data-ttu-id="3ba5f-103">signInLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="3ba5f-103">signInLocation resource type</span></span>

<span data-ttu-id="3ba5f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="3ba5f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3ba5f-105">提供发生登录的城市、省/市/自治区和国家/地区。</span><span class="sxs-lookup"><span data-stu-id="3ba5f-105">Provides the city, state and country/region from where the sign-in happened.</span></span>

## <a name="properties"></a><span data-ttu-id="3ba5f-106">属性</span><span class="sxs-lookup"><span data-stu-id="3ba5f-106">Properties</span></span>

| <span data-ttu-id="3ba5f-107">属性</span><span class="sxs-lookup"><span data-stu-id="3ba5f-107">Property</span></span>     | <span data-ttu-id="3ba5f-108">类型</span><span class="sxs-lookup"><span data-stu-id="3ba5f-108">Type</span></span>   |<span data-ttu-id="3ba5f-109">说明</span><span class="sxs-lookup"><span data-stu-id="3ba5f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3ba5f-110">城市</span><span class="sxs-lookup"><span data-stu-id="3ba5f-110">city</span></span>|<span data-ttu-id="3ba5f-111">String</span><span class="sxs-lookup"><span data-stu-id="3ba5f-111">String</span></span>|<span data-ttu-id="3ba5f-112">提供发起登录的城市。</span><span class="sxs-lookup"><span data-stu-id="3ba5f-112">Provides the city where the sign-in originated.</span></span> <span data-ttu-id="3ba5f-113">这是通过登录活动中的纬度/经度信息计算得出的。</span><span class="sxs-lookup"><span data-stu-id="3ba5f-113">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="3ba5f-114">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="3ba5f-114">countryOrRegion</span></span>|<span data-ttu-id="3ba5f-115">String</span><span class="sxs-lookup"><span data-stu-id="3ba5f-115">String</span></span>|<span data-ttu-id="3ba5f-116">提供登录所源于的国家/地区代码信息（2个字母代码）。</span><span class="sxs-lookup"><span data-stu-id="3ba5f-116">Provides the country code info (2 letter code) where the sign-in originated.</span></span>  <span data-ttu-id="3ba5f-117">这是通过登录活动中的纬度/经度信息计算得出的。</span><span class="sxs-lookup"><span data-stu-id="3ba5f-117">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="3ba5f-118">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="3ba5f-118">geoCoordinates</span></span>|[<span data-ttu-id="3ba5f-119">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="3ba5f-119">geoCoordinates</span></span>](geocoordinates.md)|<span data-ttu-id="3ba5f-120">提供登录所源于的纬度、经度和海拔高度。</span><span class="sxs-lookup"><span data-stu-id="3ba5f-120">Provides the latitude, longitude and altitude where the sign-in originated.</span></span>|
|<span data-ttu-id="3ba5f-121">state</span><span class="sxs-lookup"><span data-stu-id="3ba5f-121">state</span></span>|<span data-ttu-id="3ba5f-122">String</span><span class="sxs-lookup"><span data-stu-id="3ba5f-122">String</span></span>|<span data-ttu-id="3ba5f-123">提供登录的起始状态。</span><span class="sxs-lookup"><span data-stu-id="3ba5f-123">Provides the State where the sign-in originated.</span></span> <span data-ttu-id="3ba5f-124">这是通过登录活动中的纬度/经度信息计算得出的。</span><span class="sxs-lookup"><span data-stu-id="3ba5f-124">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3ba5f-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3ba5f-125">JSON representation</span></span>

<span data-ttu-id="3ba5f-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3ba5f-126">Here is a JSON representation of the resource.</span></span>

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
