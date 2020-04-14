---
title: deviceGeoLocation 资源类型
description: 设备位置
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f9dc9e4883030936982b9029d1e14242b2a37e37
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43423639"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="bc4ae-103">deviceGeoLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="bc4ae-103">deviceGeoLocation resource type</span></span>

<span data-ttu-id="bc4ae-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc4ae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bc4ae-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bc4ae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc4ae-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bc4ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc4ae-107">设备位置</span><span class="sxs-lookup"><span data-stu-id="bc4ae-107">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="bc4ae-108">属性</span><span class="sxs-lookup"><span data-stu-id="bc4ae-108">Properties</span></span>
|<span data-ttu-id="bc4ae-109">属性</span><span class="sxs-lookup"><span data-stu-id="bc4ae-109">Property</span></span>|<span data-ttu-id="bc4ae-110">类型</span><span class="sxs-lookup"><span data-stu-id="bc4ae-110">Type</span></span>|<span data-ttu-id="bc4ae-111">说明</span><span class="sxs-lookup"><span data-stu-id="bc4ae-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc4ae-112">lastCollectedDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="bc4ae-112">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="bc4ae-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc4ae-113">DateTimeOffset</span></span>|<span data-ttu-id="bc4ae-114">记录位置时的时间，相对于 UTC</span><span class="sxs-lookup"><span data-stu-id="bc4ae-114">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="bc4ae-115">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc4ae-115">lastCollectedDateTime</span></span>|<span data-ttu-id="bc4ae-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc4ae-116">DateTimeOffset</span></span>|<span data-ttu-id="bc4ae-117">记录位置时的时间，相对于 UTC</span><span class="sxs-lookup"><span data-stu-id="bc4ae-117">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="bc4ae-118">longitude</span><span class="sxs-lookup"><span data-stu-id="bc4ae-118">longitude</span></span>|<span data-ttu-id="bc4ae-119">双精度数</span><span class="sxs-lookup"><span data-stu-id="bc4ae-119">Double</span></span>|<span data-ttu-id="bc4ae-120">设备位置的经度坐标</span><span class="sxs-lookup"><span data-stu-id="bc4ae-120">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="bc4ae-121">latitude</span><span class="sxs-lookup"><span data-stu-id="bc4ae-121">latitude</span></span>|<span data-ttu-id="bc4ae-122">双精度</span><span class="sxs-lookup"><span data-stu-id="bc4ae-122">Double</span></span>|<span data-ttu-id="bc4ae-123">设备位置的纬度坐标</span><span class="sxs-lookup"><span data-stu-id="bc4ae-123">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="bc4ae-124">altitude</span><span class="sxs-lookup"><span data-stu-id="bc4ae-124">altitude</span></span>|<span data-ttu-id="bc4ae-125">双精度</span><span class="sxs-lookup"><span data-stu-id="bc4ae-125">Double</span></span>|<span data-ttu-id="bc4ae-126">高度，以高出海平面的米数表示</span><span class="sxs-lookup"><span data-stu-id="bc4ae-126">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="bc4ae-127">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="bc4ae-127">horizontalAccuracy</span></span>|<span data-ttu-id="bc4ae-128">双精度</span><span class="sxs-lookup"><span data-stu-id="bc4ae-128">Double</span></span>|<span data-ttu-id="bc4ae-129">经度和纬度的准确度，以米为单位</span><span class="sxs-lookup"><span data-stu-id="bc4ae-129">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="bc4ae-130">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="bc4ae-130">verticalAccuracy</span></span>|<span data-ttu-id="bc4ae-131">双精度</span><span class="sxs-lookup"><span data-stu-id="bc4ae-131">Double</span></span>|<span data-ttu-id="bc4ae-132">高度的准确度，以米为单位</span><span class="sxs-lookup"><span data-stu-id="bc4ae-132">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="bc4ae-133">heading</span><span class="sxs-lookup"><span data-stu-id="bc4ae-133">heading</span></span>|<span data-ttu-id="bc4ae-134">双精度</span><span class="sxs-lookup"><span data-stu-id="bc4ae-134">Double</span></span>|<span data-ttu-id="bc4ae-135">相对于真北的方位，以度为单位</span><span class="sxs-lookup"><span data-stu-id="bc4ae-135">Heading in degrees from true north</span></span>|
|<span data-ttu-id="bc4ae-136">speed</span><span class="sxs-lookup"><span data-stu-id="bc4ae-136">speed</span></span>|<span data-ttu-id="bc4ae-137">Double</span><span class="sxs-lookup"><span data-stu-id="bc4ae-137">Double</span></span>|<span data-ttu-id="bc4ae-138">设备的移动速度，以米/秒为单位</span><span class="sxs-lookup"><span data-stu-id="bc4ae-138">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc4ae-139">关系</span><span class="sxs-lookup"><span data-stu-id="bc4ae-139">Relationships</span></span>
<span data-ttu-id="bc4ae-140">无</span><span class="sxs-lookup"><span data-stu-id="bc4ae-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc4ae-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bc4ae-141">JSON Representation</span></span>
<span data-ttu-id="bc4ae-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc4ae-142">Here is a JSON representation of the resource.</span></span>
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



