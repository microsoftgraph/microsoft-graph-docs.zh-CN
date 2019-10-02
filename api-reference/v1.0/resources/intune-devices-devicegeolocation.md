---
title: deviceGeoLocation 资源类型
description: 设备位置
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: eb11f4c8d4d2ce87d28d92f13e359ce213c3ca9c
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356979"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="87dba-103">deviceGeoLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="87dba-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="87dba-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="87dba-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87dba-105">设备位置</span><span class="sxs-lookup"><span data-stu-id="87dba-105">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="87dba-106">属性</span><span class="sxs-lookup"><span data-stu-id="87dba-106">Properties</span></span>
|<span data-ttu-id="87dba-107">属性</span><span class="sxs-lookup"><span data-stu-id="87dba-107">Property</span></span>|<span data-ttu-id="87dba-108">类型</span><span class="sxs-lookup"><span data-stu-id="87dba-108">Type</span></span>|<span data-ttu-id="87dba-109">说明</span><span class="sxs-lookup"><span data-stu-id="87dba-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87dba-110">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="87dba-110">lastCollectedDateTime</span></span>|<span data-ttu-id="87dba-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87dba-111">DateTimeOffset</span></span>|<span data-ttu-id="87dba-112">记录位置时的时间，相对于 UTC</span><span class="sxs-lookup"><span data-stu-id="87dba-112">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="87dba-113">longitude</span><span class="sxs-lookup"><span data-stu-id="87dba-113">longitude</span></span>|<span data-ttu-id="87dba-114">双精度数</span><span class="sxs-lookup"><span data-stu-id="87dba-114">Double</span></span>|<span data-ttu-id="87dba-115">设备位置的经度坐标</span><span class="sxs-lookup"><span data-stu-id="87dba-115">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="87dba-116">latitude</span><span class="sxs-lookup"><span data-stu-id="87dba-116">latitude</span></span>|<span data-ttu-id="87dba-117">双精度</span><span class="sxs-lookup"><span data-stu-id="87dba-117">Double</span></span>|<span data-ttu-id="87dba-118">设备位置的纬度坐标</span><span class="sxs-lookup"><span data-stu-id="87dba-118">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="87dba-119">altitude</span><span class="sxs-lookup"><span data-stu-id="87dba-119">altitude</span></span>|<span data-ttu-id="87dba-120">双精度</span><span class="sxs-lookup"><span data-stu-id="87dba-120">Double</span></span>|<span data-ttu-id="87dba-121">高度，以高出海平面的米数表示</span><span class="sxs-lookup"><span data-stu-id="87dba-121">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="87dba-122">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="87dba-122">horizontalAccuracy</span></span>|<span data-ttu-id="87dba-123">双精度</span><span class="sxs-lookup"><span data-stu-id="87dba-123">Double</span></span>|<span data-ttu-id="87dba-124">经度和纬度的准确度，以米为单位</span><span class="sxs-lookup"><span data-stu-id="87dba-124">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="87dba-125">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="87dba-125">verticalAccuracy</span></span>|<span data-ttu-id="87dba-126">双精度</span><span class="sxs-lookup"><span data-stu-id="87dba-126">Double</span></span>|<span data-ttu-id="87dba-127">高度的准确度，以米为单位</span><span class="sxs-lookup"><span data-stu-id="87dba-127">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="87dba-128">heading</span><span class="sxs-lookup"><span data-stu-id="87dba-128">heading</span></span>|<span data-ttu-id="87dba-129">双精度</span><span class="sxs-lookup"><span data-stu-id="87dba-129">Double</span></span>|<span data-ttu-id="87dba-130">相对于真北的方位，以度为单位</span><span class="sxs-lookup"><span data-stu-id="87dba-130">Heading in degrees from true north</span></span>|
|<span data-ttu-id="87dba-131">speed</span><span class="sxs-lookup"><span data-stu-id="87dba-131">speed</span></span>|<span data-ttu-id="87dba-132">Double</span><span class="sxs-lookup"><span data-stu-id="87dba-132">Double</span></span>|<span data-ttu-id="87dba-133">设备的移动速度，以米/秒为单位</span><span class="sxs-lookup"><span data-stu-id="87dba-133">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="87dba-134">关系</span><span class="sxs-lookup"><span data-stu-id="87dba-134">Relationships</span></span>
<span data-ttu-id="87dba-135">无</span><span class="sxs-lookup"><span data-stu-id="87dba-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="87dba-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="87dba-136">JSON Representation</span></span>
<span data-ttu-id="87dba-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="87dba-137">Here is a JSON representation of the resource.</span></span>
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




