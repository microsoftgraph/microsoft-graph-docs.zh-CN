---
title: deviceGeoLocation 资源类型
description: 设备位置
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ef73925c31b58327f0e0b89d5682035d14d38afc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943095"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="96997-103">deviceGeoLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="96997-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="96997-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="96997-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96997-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="96997-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="96997-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="96997-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96997-107">设备位置</span><span class="sxs-lookup"><span data-stu-id="96997-107">Device location</span></span>
## <a name="properties"></a><span data-ttu-id="96997-108">属性</span><span class="sxs-lookup"><span data-stu-id="96997-108">Properties</span></span>
|<span data-ttu-id="96997-109">属性</span><span class="sxs-lookup"><span data-stu-id="96997-109">Property</span></span>|<span data-ttu-id="96997-110">类型</span><span class="sxs-lookup"><span data-stu-id="96997-110">Type</span></span>|<span data-ttu-id="96997-111">Description</span><span class="sxs-lookup"><span data-stu-id="96997-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96997-112">lastCollectedDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="96997-112">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="96997-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96997-113">DateTimeOffset</span></span>|<span data-ttu-id="96997-114">记录位置时的时间，相对于 UTC</span><span class="sxs-lookup"><span data-stu-id="96997-114">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="96997-115">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="96997-115">lastCollectedDateTime</span></span>|<span data-ttu-id="96997-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96997-116">DateTimeOffset</span></span>|<span data-ttu-id="96997-117">记录位置时的时间，相对于 UTC</span><span class="sxs-lookup"><span data-stu-id="96997-117">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="96997-118">longitude</span><span class="sxs-lookup"><span data-stu-id="96997-118">longitude</span></span>|<span data-ttu-id="96997-119">Double</span><span class="sxs-lookup"><span data-stu-id="96997-119">Double</span></span>|<span data-ttu-id="96997-120">设备位置的经度坐标</span><span class="sxs-lookup"><span data-stu-id="96997-120">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="96997-121">latitude</span><span class="sxs-lookup"><span data-stu-id="96997-121">latitude</span></span>|<span data-ttu-id="96997-122">Double</span><span class="sxs-lookup"><span data-stu-id="96997-122">Double</span></span>|<span data-ttu-id="96997-123">设备位置的纬度坐标</span><span class="sxs-lookup"><span data-stu-id="96997-123">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="96997-124">altitude</span><span class="sxs-lookup"><span data-stu-id="96997-124">altitude</span></span>|<span data-ttu-id="96997-125">Double</span><span class="sxs-lookup"><span data-stu-id="96997-125">Double</span></span>|<span data-ttu-id="96997-126">高度，以高出海平面的米数表示</span><span class="sxs-lookup"><span data-stu-id="96997-126">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="96997-127">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="96997-127">horizontalAccuracy</span></span>|<span data-ttu-id="96997-128">Double</span><span class="sxs-lookup"><span data-stu-id="96997-128">Double</span></span>|<span data-ttu-id="96997-129">经度和纬度的准确度，以米为单位</span><span class="sxs-lookup"><span data-stu-id="96997-129">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="96997-130">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="96997-130">verticalAccuracy</span></span>|<span data-ttu-id="96997-131">Double</span><span class="sxs-lookup"><span data-stu-id="96997-131">Double</span></span>|<span data-ttu-id="96997-132">高度的准确度，以米为单位</span><span class="sxs-lookup"><span data-stu-id="96997-132">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="96997-133">heading</span><span class="sxs-lookup"><span data-stu-id="96997-133">heading</span></span>|<span data-ttu-id="96997-134">Double</span><span class="sxs-lookup"><span data-stu-id="96997-134">Double</span></span>|<span data-ttu-id="96997-135">相对于真北的方位，以度为单位</span><span class="sxs-lookup"><span data-stu-id="96997-135">Heading in degrees from true north</span></span>|
|<span data-ttu-id="96997-136">speed</span><span class="sxs-lookup"><span data-stu-id="96997-136">speed</span></span>|<span data-ttu-id="96997-137">Double</span><span class="sxs-lookup"><span data-stu-id="96997-137">Double</span></span>|<span data-ttu-id="96997-138">设备的移动速度，以米/秒为单位</span><span class="sxs-lookup"><span data-stu-id="96997-138">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="96997-139">关系</span><span class="sxs-lookup"><span data-stu-id="96997-139">Relationships</span></span>
<span data-ttu-id="96997-140">无</span><span class="sxs-lookup"><span data-stu-id="96997-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="96997-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="96997-141">JSON Representation</span></span>
<span data-ttu-id="96997-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96997-142">Here is a JSON representation of the resource.</span></span>
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





