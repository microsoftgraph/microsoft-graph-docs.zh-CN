---
title: signInLocation 资源类型
description: 提供登录发生位置的城市、省/市/自治区和国家/地区。
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: c003fda44e54bbee5957e794d02b90f008f4b8f5
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137093"
---
# <a name="signinlocation-resource-type"></a><span data-ttu-id="2a889-103">signInLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="2a889-103">signInLocation resource type</span></span>

<span data-ttu-id="2a889-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a889-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2a889-105">提供登录发生位置的城市、省/市/自治区和国家/地区。</span><span class="sxs-lookup"><span data-stu-id="2a889-105">Provides the city, state and country/region from where the sign-in happened.</span></span>

## <a name="properties"></a><span data-ttu-id="2a889-106">属性</span><span class="sxs-lookup"><span data-stu-id="2a889-106">Properties</span></span>

| <span data-ttu-id="2a889-107">属性</span><span class="sxs-lookup"><span data-stu-id="2a889-107">Property</span></span>     | <span data-ttu-id="2a889-108">类型</span><span class="sxs-lookup"><span data-stu-id="2a889-108">Type</span></span>   |<span data-ttu-id="2a889-109">说明</span><span class="sxs-lookup"><span data-stu-id="2a889-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a889-110">城市</span><span class="sxs-lookup"><span data-stu-id="2a889-110">city</span></span>|<span data-ttu-id="2a889-111">String</span><span class="sxs-lookup"><span data-stu-id="2a889-111">String</span></span>|<span data-ttu-id="2a889-112">提供登录来源城市。</span><span class="sxs-lookup"><span data-stu-id="2a889-112">Provides the city where the sign-in originated.</span></span> <span data-ttu-id="2a889-113">这是使用登录活动中的纬度/经度信息计算得出的。</span><span class="sxs-lookup"><span data-stu-id="2a889-113">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="2a889-114">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="2a889-114">countryOrRegion</span></span>|<span data-ttu-id="2a889-115">String</span><span class="sxs-lookup"><span data-stu-id="2a889-115">String</span></span>|<span data-ttu-id="2a889-116">提供登录 (位置) 2 个字母代码的国家/地区代码信息。</span><span class="sxs-lookup"><span data-stu-id="2a889-116">Provides the country code info (2 letter code) where the sign-in originated.</span></span>  <span data-ttu-id="2a889-117">这是使用登录活动中的纬度/经度信息计算得出的。</span><span class="sxs-lookup"><span data-stu-id="2a889-117">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="2a889-118">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="2a889-118">geoCoordinates</span></span>|[<span data-ttu-id="2a889-119">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="2a889-119">geoCoordinates</span></span>](geocoordinates.md)|<span data-ttu-id="2a889-120">提供登录来源的纬度、经度和高度。</span><span class="sxs-lookup"><span data-stu-id="2a889-120">Provides the latitude, longitude and altitude where the sign-in originated.</span></span>|
|<span data-ttu-id="2a889-121">state</span><span class="sxs-lookup"><span data-stu-id="2a889-121">state</span></span>|<span data-ttu-id="2a889-122">String</span><span class="sxs-lookup"><span data-stu-id="2a889-122">String</span></span>|<span data-ttu-id="2a889-123">提供登录来源的状态。</span><span class="sxs-lookup"><span data-stu-id="2a889-123">Provides the State where the sign-in originated.</span></span> <span data-ttu-id="2a889-124">这是使用登录活动中的纬度/经度信息计算得出的。</span><span class="sxs-lookup"><span data-stu-id="2a889-124">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2a889-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2a889-125">JSON representation</span></span>

<span data-ttu-id="2a889-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a889-126">Here is a JSON representation of the resource.</span></span>

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

