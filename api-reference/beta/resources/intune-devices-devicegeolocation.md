---
title: deviceGeoLocation 资源类型
description: 设备位置
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c189b21570dcc218586f4cc74cd605aa6712f0c1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060480"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="77dee-103">deviceGeoLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="77dee-103">deviceGeoLocation resource type</span></span>

<span data-ttu-id="77dee-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77dee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77dee-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="77dee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77dee-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="77dee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77dee-107">设备位置</span><span class="sxs-lookup"><span data-stu-id="77dee-107">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="77dee-108">属性</span><span class="sxs-lookup"><span data-stu-id="77dee-108">Properties</span></span>
|<span data-ttu-id="77dee-109">属性</span><span class="sxs-lookup"><span data-stu-id="77dee-109">Property</span></span>|<span data-ttu-id="77dee-110">类型</span><span class="sxs-lookup"><span data-stu-id="77dee-110">Type</span></span>|<span data-ttu-id="77dee-111">说明</span><span class="sxs-lookup"><span data-stu-id="77dee-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77dee-112">lastCollectedDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="77dee-112">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="77dee-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77dee-113">DateTimeOffset</span></span>|<span data-ttu-id="77dee-114">记录位置时的时间，相对于 UTC</span><span class="sxs-lookup"><span data-stu-id="77dee-114">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="77dee-115">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="77dee-115">lastCollectedDateTime</span></span>|<span data-ttu-id="77dee-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77dee-116">DateTimeOffset</span></span>|<span data-ttu-id="77dee-117">记录位置时的时间，相对于 UTC</span><span class="sxs-lookup"><span data-stu-id="77dee-117">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="77dee-118">longitude</span><span class="sxs-lookup"><span data-stu-id="77dee-118">longitude</span></span>|<span data-ttu-id="77dee-119">Double</span><span class="sxs-lookup"><span data-stu-id="77dee-119">Double</span></span>|<span data-ttu-id="77dee-120">设备位置的经度坐标</span><span class="sxs-lookup"><span data-stu-id="77dee-120">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="77dee-121">latitude</span><span class="sxs-lookup"><span data-stu-id="77dee-121">latitude</span></span>|<span data-ttu-id="77dee-122">Double</span><span class="sxs-lookup"><span data-stu-id="77dee-122">Double</span></span>|<span data-ttu-id="77dee-123">设备位置的纬度坐标</span><span class="sxs-lookup"><span data-stu-id="77dee-123">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="77dee-124">altitude</span><span class="sxs-lookup"><span data-stu-id="77dee-124">altitude</span></span>|<span data-ttu-id="77dee-125">Double</span><span class="sxs-lookup"><span data-stu-id="77dee-125">Double</span></span>|<span data-ttu-id="77dee-126">高度，以高出海平面的米数表示</span><span class="sxs-lookup"><span data-stu-id="77dee-126">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="77dee-127">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="77dee-127">horizontalAccuracy</span></span>|<span data-ttu-id="77dee-128">Double</span><span class="sxs-lookup"><span data-stu-id="77dee-128">Double</span></span>|<span data-ttu-id="77dee-129">经度和纬度的准确度，以米为单位</span><span class="sxs-lookup"><span data-stu-id="77dee-129">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="77dee-130">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="77dee-130">verticalAccuracy</span></span>|<span data-ttu-id="77dee-131">Double</span><span class="sxs-lookup"><span data-stu-id="77dee-131">Double</span></span>|<span data-ttu-id="77dee-132">高度的准确度，以米为单位</span><span class="sxs-lookup"><span data-stu-id="77dee-132">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="77dee-133">heading</span><span class="sxs-lookup"><span data-stu-id="77dee-133">heading</span></span>|<span data-ttu-id="77dee-134">Double</span><span class="sxs-lookup"><span data-stu-id="77dee-134">Double</span></span>|<span data-ttu-id="77dee-135">相对于真北的方位，以度为单位</span><span class="sxs-lookup"><span data-stu-id="77dee-135">Heading in degrees from true north</span></span>|
|<span data-ttu-id="77dee-136">speed</span><span class="sxs-lookup"><span data-stu-id="77dee-136">speed</span></span>|<span data-ttu-id="77dee-137">Double</span><span class="sxs-lookup"><span data-stu-id="77dee-137">Double</span></span>|<span data-ttu-id="77dee-138">设备的移动速度，以米/秒为单位</span><span class="sxs-lookup"><span data-stu-id="77dee-138">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="77dee-139">关系</span><span class="sxs-lookup"><span data-stu-id="77dee-139">Relationships</span></span>
<span data-ttu-id="77dee-140">无</span><span class="sxs-lookup"><span data-stu-id="77dee-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="77dee-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="77dee-141">JSON Representation</span></span>
<span data-ttu-id="77dee-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="77dee-142">Here is a JSON representation of the resource.</span></span>
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
  "longitude": "4.2",
  "latitude": "4.2",
  "altitude": "4.2",
  "horizontalAccuracy": "4.2",
  "verticalAccuracy": "4.2",
  "heading": "4.2",
  "speed": "4.2"
}
```






