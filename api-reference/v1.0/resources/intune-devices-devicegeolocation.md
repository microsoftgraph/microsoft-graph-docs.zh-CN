---
title: deviceGeoLocation 资源类型
description: 设备位置
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 48c0b4224225c70a9f5c4a636e1e15e4ddea3364
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533296"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="aea25-103">deviceGeoLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="aea25-103">deviceGeoLocation resource type</span></span>

<span data-ttu-id="aea25-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aea25-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aea25-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aea25-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aea25-106">设备位置</span><span class="sxs-lookup"><span data-stu-id="aea25-106">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="aea25-107">属性</span><span class="sxs-lookup"><span data-stu-id="aea25-107">Properties</span></span>
|<span data-ttu-id="aea25-108">属性</span><span class="sxs-lookup"><span data-stu-id="aea25-108">Property</span></span>|<span data-ttu-id="aea25-109">类型</span><span class="sxs-lookup"><span data-stu-id="aea25-109">Type</span></span>|<span data-ttu-id="aea25-110">说明</span><span class="sxs-lookup"><span data-stu-id="aea25-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aea25-111">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="aea25-111">lastCollectedDateTime</span></span>|<span data-ttu-id="aea25-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aea25-112">DateTimeOffset</span></span>|<span data-ttu-id="aea25-113">记录位置时的时间，相对于 UTC</span><span class="sxs-lookup"><span data-stu-id="aea25-113">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="aea25-114">longitude</span><span class="sxs-lookup"><span data-stu-id="aea25-114">longitude</span></span>|<span data-ttu-id="aea25-115">双精度数</span><span class="sxs-lookup"><span data-stu-id="aea25-115">Double</span></span>|<span data-ttu-id="aea25-116">设备位置的经度坐标</span><span class="sxs-lookup"><span data-stu-id="aea25-116">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="aea25-117">latitude</span><span class="sxs-lookup"><span data-stu-id="aea25-117">latitude</span></span>|<span data-ttu-id="aea25-118">双精度</span><span class="sxs-lookup"><span data-stu-id="aea25-118">Double</span></span>|<span data-ttu-id="aea25-119">设备位置的纬度坐标</span><span class="sxs-lookup"><span data-stu-id="aea25-119">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="aea25-120">altitude</span><span class="sxs-lookup"><span data-stu-id="aea25-120">altitude</span></span>|<span data-ttu-id="aea25-121">双精度</span><span class="sxs-lookup"><span data-stu-id="aea25-121">Double</span></span>|<span data-ttu-id="aea25-122">高度，以高出海平面的米数表示</span><span class="sxs-lookup"><span data-stu-id="aea25-122">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="aea25-123">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="aea25-123">horizontalAccuracy</span></span>|<span data-ttu-id="aea25-124">双精度</span><span class="sxs-lookup"><span data-stu-id="aea25-124">Double</span></span>|<span data-ttu-id="aea25-125">经度和纬度的准确度，以米为单位</span><span class="sxs-lookup"><span data-stu-id="aea25-125">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="aea25-126">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="aea25-126">verticalAccuracy</span></span>|<span data-ttu-id="aea25-127">双精度</span><span class="sxs-lookup"><span data-stu-id="aea25-127">Double</span></span>|<span data-ttu-id="aea25-128">高度的准确度，以米为单位</span><span class="sxs-lookup"><span data-stu-id="aea25-128">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="aea25-129">heading</span><span class="sxs-lookup"><span data-stu-id="aea25-129">heading</span></span>|<span data-ttu-id="aea25-130">双精度</span><span class="sxs-lookup"><span data-stu-id="aea25-130">Double</span></span>|<span data-ttu-id="aea25-131">相对于真北的方位，以度为单位</span><span class="sxs-lookup"><span data-stu-id="aea25-131">Heading in degrees from true north</span></span>|
|<span data-ttu-id="aea25-132">speed</span><span class="sxs-lookup"><span data-stu-id="aea25-132">speed</span></span>|<span data-ttu-id="aea25-133">Double</span><span class="sxs-lookup"><span data-stu-id="aea25-133">Double</span></span>|<span data-ttu-id="aea25-134">设备的移动速度，以米/秒为单位</span><span class="sxs-lookup"><span data-stu-id="aea25-134">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="aea25-135">关系</span><span class="sxs-lookup"><span data-stu-id="aea25-135">Relationships</span></span>
<span data-ttu-id="aea25-136">无</span><span class="sxs-lookup"><span data-stu-id="aea25-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aea25-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aea25-137">JSON Representation</span></span>
<span data-ttu-id="aea25-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aea25-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceGeoLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceGeoLocation",
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




