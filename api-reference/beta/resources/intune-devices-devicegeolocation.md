---
title: deviceGeoLocation 资源类型
description: 设备位置
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3b2105711a9a8f84b705a5a01c658c87cbe48c75
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395053"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="e65b5-103">deviceGeoLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="e65b5-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="e65b5-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="e65b5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e65b5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e65b5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e65b5-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e65b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e65b5-107">设备位置</span><span class="sxs-lookup"><span data-stu-id="e65b5-107">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="e65b5-108">属性</span><span class="sxs-lookup"><span data-stu-id="e65b5-108">Properties</span></span>
|<span data-ttu-id="e65b5-109">属性</span><span class="sxs-lookup"><span data-stu-id="e65b5-109">Property</span></span>|<span data-ttu-id="e65b5-110">类型</span><span class="sxs-lookup"><span data-stu-id="e65b5-110">Type</span></span>|<span data-ttu-id="e65b5-111">说明</span><span class="sxs-lookup"><span data-stu-id="e65b5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e65b5-112">lastCollectedDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="e65b5-112">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="e65b5-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e65b5-113">DateTimeOffset</span></span>|<span data-ttu-id="e65b5-114">记录位置时的时间，相对于 UTC</span><span class="sxs-lookup"><span data-stu-id="e65b5-114">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="e65b5-115">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="e65b5-115">lastCollectedDateTime</span></span>|<span data-ttu-id="e65b5-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e65b5-116">DateTimeOffset</span></span>|<span data-ttu-id="e65b5-117">记录位置时的时间，相对于 UTC</span><span class="sxs-lookup"><span data-stu-id="e65b5-117">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="e65b5-118">longitude</span><span class="sxs-lookup"><span data-stu-id="e65b5-118">longitude</span></span>|<span data-ttu-id="e65b5-119">Double</span><span class="sxs-lookup"><span data-stu-id="e65b5-119">Double</span></span>|<span data-ttu-id="e65b5-120">设备位置的经度坐标</span><span class="sxs-lookup"><span data-stu-id="e65b5-120">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="e65b5-121">latitude</span><span class="sxs-lookup"><span data-stu-id="e65b5-121">latitude</span></span>|<span data-ttu-id="e65b5-122">Double</span><span class="sxs-lookup"><span data-stu-id="e65b5-122">Double</span></span>|<span data-ttu-id="e65b5-123">设备位置的纬度坐标</span><span class="sxs-lookup"><span data-stu-id="e65b5-123">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="e65b5-124">altitude</span><span class="sxs-lookup"><span data-stu-id="e65b5-124">altitude</span></span>|<span data-ttu-id="e65b5-125">Double</span><span class="sxs-lookup"><span data-stu-id="e65b5-125">Double</span></span>|<span data-ttu-id="e65b5-126">高度，以高出海平面的米数表示</span><span class="sxs-lookup"><span data-stu-id="e65b5-126">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="e65b5-127">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="e65b5-127">horizontalAccuracy</span></span>|<span data-ttu-id="e65b5-128">Double</span><span class="sxs-lookup"><span data-stu-id="e65b5-128">Double</span></span>|<span data-ttu-id="e65b5-129">经度和纬度的准确度，以米为单位</span><span class="sxs-lookup"><span data-stu-id="e65b5-129">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="e65b5-130">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="e65b5-130">verticalAccuracy</span></span>|<span data-ttu-id="e65b5-131">Double</span><span class="sxs-lookup"><span data-stu-id="e65b5-131">Double</span></span>|<span data-ttu-id="e65b5-132">高度的准确度，以米为单位</span><span class="sxs-lookup"><span data-stu-id="e65b5-132">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="e65b5-133">heading</span><span class="sxs-lookup"><span data-stu-id="e65b5-133">heading</span></span>|<span data-ttu-id="e65b5-134">Double</span><span class="sxs-lookup"><span data-stu-id="e65b5-134">Double</span></span>|<span data-ttu-id="e65b5-135">相对于真北的方位，以度为单位</span><span class="sxs-lookup"><span data-stu-id="e65b5-135">Heading in degrees from true north</span></span>|
|<span data-ttu-id="e65b5-136">speed</span><span class="sxs-lookup"><span data-stu-id="e65b5-136">speed</span></span>|<span data-ttu-id="e65b5-137">Double</span><span class="sxs-lookup"><span data-stu-id="e65b5-137">Double</span></span>|<span data-ttu-id="e65b5-138">设备的移动速度，以米/秒为单位</span><span class="sxs-lookup"><span data-stu-id="e65b5-138">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="e65b5-139">关系</span><span class="sxs-lookup"><span data-stu-id="e65b5-139">Relationships</span></span>
<span data-ttu-id="e65b5-140">无</span><span class="sxs-lookup"><span data-stu-id="e65b5-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e65b5-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e65b5-141">JSON Representation</span></span>
<span data-ttu-id="e65b5-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e65b5-142">Here is a JSON representation of the resource.</span></span>
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




