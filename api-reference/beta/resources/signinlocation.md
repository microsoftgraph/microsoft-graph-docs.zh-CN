---
title: signInLocation 资源类型
description: 提供市/县、 状态和国家/地区从其中登录发生。
ms.openlocfilehash: a3d4f6ca5ec18e70960f45a3da1bb06d51ee1e65
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045572"
---
# <a name="signinlocation-resource-type"></a><span data-ttu-id="f6490-103">signInLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="f6490-103">signInLocation resource type</span></span>
<span data-ttu-id="f6490-104">提供市/县、 状态和国家/地区从其中登录发生。</span><span class="sxs-lookup"><span data-stu-id="f6490-104">Provides the city, state and country/region from where the sign-in happened.</span></span>



## <a name="properties"></a><span data-ttu-id="f6490-105">属性</span><span class="sxs-lookup"><span data-stu-id="f6490-105">Properties</span></span>
| <span data-ttu-id="f6490-106">属性</span><span class="sxs-lookup"><span data-stu-id="f6490-106">Property</span></span>     | <span data-ttu-id="f6490-107">类型</span><span class="sxs-lookup"><span data-stu-id="f6490-107">Type</span></span>   |<span data-ttu-id="f6490-108">说明</span><span class="sxs-lookup"><span data-stu-id="f6490-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6490-109">city</span><span class="sxs-lookup"><span data-stu-id="f6490-109">city</span></span>|<span data-ttu-id="f6490-110">字符串</span><span class="sxs-lookup"><span data-stu-id="f6490-110">String</span></span>|<span data-ttu-id="f6490-111">提供登录发起的城市。</span><span class="sxs-lookup"><span data-stu-id="f6490-111">Provides the city where the sign-in originated.</span></span> <span data-ttu-id="f6490-112">这被计算使用登录活动纬度/经度信息。</span><span class="sxs-lookup"><span data-stu-id="f6490-112">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="f6490-113">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="f6490-113">countryOrRegion</span></span>|<span data-ttu-id="f6490-114">字符串</span><span class="sxs-lookup"><span data-stu-id="f6490-114">String</span></span>|<span data-ttu-id="f6490-115">提供的国家/地区代码信息 （2 字母代码） 的登录来源。</span><span class="sxs-lookup"><span data-stu-id="f6490-115">Provides the country code info (2 letter code) where the sign-in originated.</span></span>  <span data-ttu-id="f6490-116">这被计算使用登录活动纬度/经度信息。</span><span class="sxs-lookup"><span data-stu-id="f6490-116">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|
|<span data-ttu-id="f6490-117">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="f6490-117">geoCoordinates</span></span>|[<span data-ttu-id="f6490-118">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="f6490-118">geoCoordinates</span></span>](geocoordinates.md)|<span data-ttu-id="f6490-119">提供、 纬度和海拔高度的登录来源。</span><span class="sxs-lookup"><span data-stu-id="f6490-119">Provides the latitude, longitude and altitude where the sign-in originated.</span></span>|
|<span data-ttu-id="f6490-120">状态</span><span class="sxs-lookup"><span data-stu-id="f6490-120">state</span></span>|<span data-ttu-id="f6490-121">字符串</span><span class="sxs-lookup"><span data-stu-id="f6490-121">String</span></span>|<span data-ttu-id="f6490-122">提供登录发起的状态。</span><span class="sxs-lookup"><span data-stu-id="f6490-122">Provides the State where the sign-in originated.</span></span> <span data-ttu-id="f6490-123">这被计算使用登录活动纬度/经度信息。</span><span class="sxs-lookup"><span data-stu-id="f6490-123">This is calculated using latitude/longitude information from the sign-in activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f6490-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f6490-124">JSON representation</span></span>

<span data-ttu-id="f6490-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6490-125">Here is a JSON representation of the resource.</span></span>

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