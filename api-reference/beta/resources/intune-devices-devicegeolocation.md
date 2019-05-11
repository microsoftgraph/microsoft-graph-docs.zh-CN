---
title: deviceGeoLocation 资源类型
description: 设备位置
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 46a92f1faad55d82e2ed8184c5f4a4d360b7d588
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33942134"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="96bd2-103">deviceGeoLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="96bd2-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="96bd2-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="96bd2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96bd2-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="96bd2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96bd2-106">设备位置</span><span class="sxs-lookup"><span data-stu-id="96bd2-106">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="96bd2-107">属性</span><span class="sxs-lookup"><span data-stu-id="96bd2-107">Properties</span></span>
|<span data-ttu-id="96bd2-108">属性</span><span class="sxs-lookup"><span data-stu-id="96bd2-108">Property</span></span>|<span data-ttu-id="96bd2-109">类型</span><span class="sxs-lookup"><span data-stu-id="96bd2-109">Type</span></span>|<span data-ttu-id="96bd2-110">说明</span><span class="sxs-lookup"><span data-stu-id="96bd2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96bd2-111">lastCollectedDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="96bd2-111">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="96bd2-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96bd2-112">DateTimeOffset</span></span>|<span data-ttu-id="96bd2-113">记录位置时的时间，相对于 UTC</span><span class="sxs-lookup"><span data-stu-id="96bd2-113">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="96bd2-114">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="96bd2-114">lastCollectedDateTime</span></span>|<span data-ttu-id="96bd2-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96bd2-115">DateTimeOffset</span></span>|<span data-ttu-id="96bd2-116">记录位置时的时间，相对于 UTC</span><span class="sxs-lookup"><span data-stu-id="96bd2-116">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="96bd2-117">longitude</span><span class="sxs-lookup"><span data-stu-id="96bd2-117">longitude</span></span>|<span data-ttu-id="96bd2-118">双精度数</span><span class="sxs-lookup"><span data-stu-id="96bd2-118">Double</span></span>|<span data-ttu-id="96bd2-119">设备位置的经度坐标</span><span class="sxs-lookup"><span data-stu-id="96bd2-119">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="96bd2-120">latitude</span><span class="sxs-lookup"><span data-stu-id="96bd2-120">latitude</span></span>|<span data-ttu-id="96bd2-121">双精度</span><span class="sxs-lookup"><span data-stu-id="96bd2-121">Double</span></span>|<span data-ttu-id="96bd2-122">设备位置的纬度坐标</span><span class="sxs-lookup"><span data-stu-id="96bd2-122">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="96bd2-123">altitude</span><span class="sxs-lookup"><span data-stu-id="96bd2-123">altitude</span></span>|<span data-ttu-id="96bd2-124">双精度</span><span class="sxs-lookup"><span data-stu-id="96bd2-124">Double</span></span>|<span data-ttu-id="96bd2-125">高度，以高出海平面的米数表示</span><span class="sxs-lookup"><span data-stu-id="96bd2-125">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="96bd2-126">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="96bd2-126">horizontalAccuracy</span></span>|<span data-ttu-id="96bd2-127">双精度</span><span class="sxs-lookup"><span data-stu-id="96bd2-127">Double</span></span>|<span data-ttu-id="96bd2-128">经度和纬度的准确度，以米为单位</span><span class="sxs-lookup"><span data-stu-id="96bd2-128">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="96bd2-129">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="96bd2-129">verticalAccuracy</span></span>|<span data-ttu-id="96bd2-130">双精度</span><span class="sxs-lookup"><span data-stu-id="96bd2-130">Double</span></span>|<span data-ttu-id="96bd2-131">高度的准确度，以米为单位</span><span class="sxs-lookup"><span data-stu-id="96bd2-131">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="96bd2-132">heading</span><span class="sxs-lookup"><span data-stu-id="96bd2-132">heading</span></span>|<span data-ttu-id="96bd2-133">双精度</span><span class="sxs-lookup"><span data-stu-id="96bd2-133">Double</span></span>|<span data-ttu-id="96bd2-134">相对于真北的方位，以度为单位</span><span class="sxs-lookup"><span data-stu-id="96bd2-134">Heading in degrees from true north</span></span>|
|<span data-ttu-id="96bd2-135">speed</span><span class="sxs-lookup"><span data-stu-id="96bd2-135">speed</span></span>|<span data-ttu-id="96bd2-136">Double</span><span class="sxs-lookup"><span data-stu-id="96bd2-136">Double</span></span>|<span data-ttu-id="96bd2-137">设备的移动速度，以米/秒为单位</span><span class="sxs-lookup"><span data-stu-id="96bd2-137">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="96bd2-138">关系</span><span class="sxs-lookup"><span data-stu-id="96bd2-138">Relationships</span></span>
<span data-ttu-id="96bd2-139">无</span><span class="sxs-lookup"><span data-stu-id="96bd2-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="96bd2-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="96bd2-140">JSON Representation</span></span>
<span data-ttu-id="96bd2-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96bd2-141">Here is a JSON representation of the resource.</span></span>
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




