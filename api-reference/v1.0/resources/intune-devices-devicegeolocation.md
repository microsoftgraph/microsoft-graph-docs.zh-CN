---
title: deviceGeoLocation 资源类型
description: 设备位置
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a406ede926ad637a338437559840cdefdadc64ce
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754579"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="9421d-103">deviceGeoLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="9421d-103">deviceGeoLocation resource type</span></span>

<span data-ttu-id="9421d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9421d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9421d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9421d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9421d-106">设备位置</span><span class="sxs-lookup"><span data-stu-id="9421d-106">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="9421d-107">属性</span><span class="sxs-lookup"><span data-stu-id="9421d-107">Properties</span></span>
|<span data-ttu-id="9421d-108">属性</span><span class="sxs-lookup"><span data-stu-id="9421d-108">Property</span></span>|<span data-ttu-id="9421d-109">类型</span><span class="sxs-lookup"><span data-stu-id="9421d-109">Type</span></span>|<span data-ttu-id="9421d-110">Description</span><span class="sxs-lookup"><span data-stu-id="9421d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9421d-111">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="9421d-111">lastCollectedDateTime</span></span>|<span data-ttu-id="9421d-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9421d-112">DateTimeOffset</span></span>|<span data-ttu-id="9421d-113">记录位置时的时间，相对于 UTC</span><span class="sxs-lookup"><span data-stu-id="9421d-113">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="9421d-114">longitude</span><span class="sxs-lookup"><span data-stu-id="9421d-114">longitude</span></span>|<span data-ttu-id="9421d-115">Double</span><span class="sxs-lookup"><span data-stu-id="9421d-115">Double</span></span>|<span data-ttu-id="9421d-116">设备位置的经度坐标</span><span class="sxs-lookup"><span data-stu-id="9421d-116">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="9421d-117">latitude</span><span class="sxs-lookup"><span data-stu-id="9421d-117">latitude</span></span>|<span data-ttu-id="9421d-118">Double</span><span class="sxs-lookup"><span data-stu-id="9421d-118">Double</span></span>|<span data-ttu-id="9421d-119">设备位置的纬度坐标</span><span class="sxs-lookup"><span data-stu-id="9421d-119">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="9421d-120">altitude</span><span class="sxs-lookup"><span data-stu-id="9421d-120">altitude</span></span>|<span data-ttu-id="9421d-121">Double</span><span class="sxs-lookup"><span data-stu-id="9421d-121">Double</span></span>|<span data-ttu-id="9421d-122">高度，以高出海平面的米数表示</span><span class="sxs-lookup"><span data-stu-id="9421d-122">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="9421d-123">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="9421d-123">horizontalAccuracy</span></span>|<span data-ttu-id="9421d-124">Double</span><span class="sxs-lookup"><span data-stu-id="9421d-124">Double</span></span>|<span data-ttu-id="9421d-125">经度和纬度的准确度，以米为单位</span><span class="sxs-lookup"><span data-stu-id="9421d-125">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="9421d-126">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="9421d-126">verticalAccuracy</span></span>|<span data-ttu-id="9421d-127">Double</span><span class="sxs-lookup"><span data-stu-id="9421d-127">Double</span></span>|<span data-ttu-id="9421d-128">高度的准确度，以米为单位</span><span class="sxs-lookup"><span data-stu-id="9421d-128">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="9421d-129">heading</span><span class="sxs-lookup"><span data-stu-id="9421d-129">heading</span></span>|<span data-ttu-id="9421d-130">Double</span><span class="sxs-lookup"><span data-stu-id="9421d-130">Double</span></span>|<span data-ttu-id="9421d-131">相对于真北的方位，以度为单位</span><span class="sxs-lookup"><span data-stu-id="9421d-131">Heading in degrees from true north</span></span>|
|<span data-ttu-id="9421d-132">speed</span><span class="sxs-lookup"><span data-stu-id="9421d-132">speed</span></span>|<span data-ttu-id="9421d-133">Double</span><span class="sxs-lookup"><span data-stu-id="9421d-133">Double</span></span>|<span data-ttu-id="9421d-134">设备的移动速度，以米/秒为单位</span><span class="sxs-lookup"><span data-stu-id="9421d-134">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="9421d-135">关系</span><span class="sxs-lookup"><span data-stu-id="9421d-135">Relationships</span></span>
<span data-ttu-id="9421d-136">无</span><span class="sxs-lookup"><span data-stu-id="9421d-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9421d-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9421d-137">JSON Representation</span></span>
<span data-ttu-id="9421d-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9421d-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceGeoLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceGeoLocation",
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




