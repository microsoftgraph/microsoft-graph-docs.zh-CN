---
title: deviceGeoLocation 资源类型
description: 设备位置
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1da2a612a777491731fa0b85e2f754605ffa04bc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370163"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="a2cd4-103">deviceGeoLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="a2cd4-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="a2cd4-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a2cd4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2cd4-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a2cd4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2cd4-106">设备位置</span><span class="sxs-lookup"><span data-stu-id="a2cd4-106">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="a2cd4-107">属性</span><span class="sxs-lookup"><span data-stu-id="a2cd4-107">Properties</span></span>
|<span data-ttu-id="a2cd4-108">属性</span><span class="sxs-lookup"><span data-stu-id="a2cd4-108">Property</span></span>|<span data-ttu-id="a2cd4-109">类型</span><span class="sxs-lookup"><span data-stu-id="a2cd4-109">Type</span></span>|<span data-ttu-id="a2cd4-110">说明</span><span class="sxs-lookup"><span data-stu-id="a2cd4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2cd4-111">lastCollectedDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="a2cd4-111">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="a2cd4-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2cd4-112">DateTimeOffset</span></span>|<span data-ttu-id="a2cd4-113">记录位置时的时间，相对于 UTC</span><span class="sxs-lookup"><span data-stu-id="a2cd4-113">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="a2cd4-114">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2cd4-114">lastCollectedDateTime</span></span>|<span data-ttu-id="a2cd4-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2cd4-115">DateTimeOffset</span></span>|<span data-ttu-id="a2cd4-116">记录位置时的时间，相对于 UTC</span><span class="sxs-lookup"><span data-stu-id="a2cd4-116">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="a2cd4-117">longitude</span><span class="sxs-lookup"><span data-stu-id="a2cd4-117">longitude</span></span>|<span data-ttu-id="a2cd4-118">双精度数</span><span class="sxs-lookup"><span data-stu-id="a2cd4-118">Double</span></span>|<span data-ttu-id="a2cd4-119">设备位置的经度坐标</span><span class="sxs-lookup"><span data-stu-id="a2cd4-119">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="a2cd4-120">latitude</span><span class="sxs-lookup"><span data-stu-id="a2cd4-120">latitude</span></span>|<span data-ttu-id="a2cd4-121">双精度</span><span class="sxs-lookup"><span data-stu-id="a2cd4-121">Double</span></span>|<span data-ttu-id="a2cd4-122">设备位置的纬度坐标</span><span class="sxs-lookup"><span data-stu-id="a2cd4-122">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="a2cd4-123">altitude</span><span class="sxs-lookup"><span data-stu-id="a2cd4-123">altitude</span></span>|<span data-ttu-id="a2cd4-124">双精度</span><span class="sxs-lookup"><span data-stu-id="a2cd4-124">Double</span></span>|<span data-ttu-id="a2cd4-125">高度，以高出海平面的米数表示</span><span class="sxs-lookup"><span data-stu-id="a2cd4-125">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="a2cd4-126">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="a2cd4-126">horizontalAccuracy</span></span>|<span data-ttu-id="a2cd4-127">双精度</span><span class="sxs-lookup"><span data-stu-id="a2cd4-127">Double</span></span>|<span data-ttu-id="a2cd4-128">经度和纬度的准确度，以米为单位</span><span class="sxs-lookup"><span data-stu-id="a2cd4-128">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="a2cd4-129">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="a2cd4-129">verticalAccuracy</span></span>|<span data-ttu-id="a2cd4-130">双精度</span><span class="sxs-lookup"><span data-stu-id="a2cd4-130">Double</span></span>|<span data-ttu-id="a2cd4-131">高度的准确度，以米为单位</span><span class="sxs-lookup"><span data-stu-id="a2cd4-131">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="a2cd4-132">heading</span><span class="sxs-lookup"><span data-stu-id="a2cd4-132">heading</span></span>|<span data-ttu-id="a2cd4-133">双精度</span><span class="sxs-lookup"><span data-stu-id="a2cd4-133">Double</span></span>|<span data-ttu-id="a2cd4-134">相对于真北的方位，以度为单位</span><span class="sxs-lookup"><span data-stu-id="a2cd4-134">Heading in degrees from true north</span></span>|
|<span data-ttu-id="a2cd4-135">speed</span><span class="sxs-lookup"><span data-stu-id="a2cd4-135">speed</span></span>|<span data-ttu-id="a2cd4-136">Double</span><span class="sxs-lookup"><span data-stu-id="a2cd4-136">Double</span></span>|<span data-ttu-id="a2cd4-137">设备的移动速度，以米/秒为单位</span><span class="sxs-lookup"><span data-stu-id="a2cd4-137">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2cd4-138">关系</span><span class="sxs-lookup"><span data-stu-id="a2cd4-138">Relationships</span></span>
<span data-ttu-id="a2cd4-139">无</span><span class="sxs-lookup"><span data-stu-id="a2cd4-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2cd4-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a2cd4-140">JSON Representation</span></span>
<span data-ttu-id="a2cd4-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2cd4-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceGeoLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceGeoLocation",
  "lastCollectedDateTimeUtc": "String (timestamp)",
  "lastCollectedDateTime": "String (timestamp)",
  "longitude": "<Unknown Primitive Type Edm.Double>",
  "latitude": "<Unknown Primitive Type Edm.Double>",
  "altitude": "<Unknown Primitive Type Edm.Double>",
  "horizontalAccuracy": "<Unknown Primitive Type Edm.Double>",
  "verticalAccuracy": "<Unknown Primitive Type Edm.Double>",
  "heading": "<Unknown Primitive Type Edm.Double>",
  "speed": "<Unknown Primitive Type Edm.Double>"
}
```



