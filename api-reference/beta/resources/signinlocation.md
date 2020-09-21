---
title: signInLocation 资源类型
description: 提供发生登录的城市、省/市/自治区和国家/地区。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: SarahBar
ms.openlocfilehash: 1bbfb01e07b5ccde134933490b06ae3ab1da53af
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067137"
---
# <a name="signinlocation-resource-type"></a><span data-ttu-id="7065f-103">signInLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="7065f-103">signInLocation resource type</span></span>

<span data-ttu-id="7065f-104">命名空间： microsoft. graph 提供了发生登录的城市、省/市/自治区和国家/地区。</span><span class="sxs-lookup"><span data-stu-id="7065f-104">Namespace: microsoft.graph Provides the city, state and country/region from where the sign-in happened.</span></span>



## <a name="properties"></a><span data-ttu-id="7065f-105">属性</span><span class="sxs-lookup"><span data-stu-id="7065f-105">Properties</span></span>
| <span data-ttu-id="7065f-106">属性</span><span class="sxs-lookup"><span data-stu-id="7065f-106">Property</span></span>     | <span data-ttu-id="7065f-107">类型</span><span class="sxs-lookup"><span data-stu-id="7065f-107">Type</span></span>   |<span data-ttu-id="7065f-108">说明</span><span class="sxs-lookup"><span data-stu-id="7065f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7065f-109">城市</span><span class="sxs-lookup"><span data-stu-id="7065f-109">city</span></span>|<span data-ttu-id="7065f-110">String</span><span class="sxs-lookup"><span data-stu-id="7065f-110">String</span></span>|<span data-ttu-id="7065f-111">提供发起登录的城市。</span><span class="sxs-lookup"><span data-stu-id="7065f-111">Provides the city where the sign-in originated.</span></span> <span data-ttu-id="7065f-112">这是通过登录活动中的纬度/经度信息计算得出的。</span><span class="sxs-lookup"><span data-stu-id="7065f-112">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="7065f-113">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="7065f-113">countryOrRegion</span></span>|<span data-ttu-id="7065f-114">String</span><span class="sxs-lookup"><span data-stu-id="7065f-114">String</span></span>|<span data-ttu-id="7065f-115">提供国家/地区代码信息 (2 号代码) 在该登录起源中。</span><span class="sxs-lookup"><span data-stu-id="7065f-115">Provides the country code info (2 letter code) where the sign-in originated.</span></span>  <span data-ttu-id="7065f-116">这是通过登录活动中的纬度/经度信息计算得出的。</span><span class="sxs-lookup"><span data-stu-id="7065f-116">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="7065f-117">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="7065f-117">geoCoordinates</span></span>|[<span data-ttu-id="7065f-118">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="7065f-118">geoCoordinates</span></span>](geocoordinates.md)|<span data-ttu-id="7065f-119">提供登录所源于的纬度、经度和海拔高度。</span><span class="sxs-lookup"><span data-stu-id="7065f-119">Provides the latitude, longitude and altitude where the sign-in originated.</span></span>|
|<span data-ttu-id="7065f-120">state</span><span class="sxs-lookup"><span data-stu-id="7065f-120">state</span></span>|<span data-ttu-id="7065f-121">String</span><span class="sxs-lookup"><span data-stu-id="7065f-121">String</span></span>|<span data-ttu-id="7065f-122">提供登录的起始状态。</span><span class="sxs-lookup"><span data-stu-id="7065f-122">Provides the State where the sign-in originated.</span></span> <span data-ttu-id="7065f-123">这是通过登录活动中的纬度/经度信息计算得出的。</span><span class="sxs-lookup"><span data-stu-id="7065f-123">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7065f-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7065f-124">JSON representation</span></span>

<span data-ttu-id="7065f-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7065f-125">Here is a JSON representation of the resource.</span></span>

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


