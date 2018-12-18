---
title: deviceGeoLocation 资源类型
description: 设备位置
author: tfitzmac
ms.openlocfilehash: b3e790809f79d8d943cc12cc0e5065972c9864ff
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328628"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="cd9bb-103">deviceGeoLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="cd9bb-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="cd9bb-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cd9bb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd9bb-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cd9bb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cd9bb-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cd9bb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cd9bb-107">设备位置</span><span class="sxs-lookup"><span data-stu-id="cd9bb-107">Device location</span></span>
## <a name="properties"></a><span data-ttu-id="cd9bb-108">属性</span><span class="sxs-lookup"><span data-stu-id="cd9bb-108">Properties</span></span>
|<span data-ttu-id="cd9bb-109">属性</span><span class="sxs-lookup"><span data-stu-id="cd9bb-109">Property</span></span>|<span data-ttu-id="cd9bb-110">类型</span><span class="sxs-lookup"><span data-stu-id="cd9bb-110">Type</span></span>|<span data-ttu-id="cd9bb-111">说明</span><span class="sxs-lookup"><span data-stu-id="cd9bb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd9bb-112">lastCollectedDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="cd9bb-112">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="cd9bb-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd9bb-113">DateTimeOffset</span></span>|<span data-ttu-id="cd9bb-114">记录位置时的时间，相对于 UTC</span><span class="sxs-lookup"><span data-stu-id="cd9bb-114">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="cd9bb-115">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="cd9bb-115">lastCollectedDateTime</span></span>|<span data-ttu-id="cd9bb-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd9bb-116">DateTimeOffset</span></span>|<span data-ttu-id="cd9bb-117">记录位置时的时间，相对于 UTC</span><span class="sxs-lookup"><span data-stu-id="cd9bb-117">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="cd9bb-118">longitude</span><span class="sxs-lookup"><span data-stu-id="cd9bb-118">longitude</span></span>|<span data-ttu-id="cd9bb-119">Double</span><span class="sxs-lookup"><span data-stu-id="cd9bb-119">Double</span></span>|<span data-ttu-id="cd9bb-120">设备位置的经度坐标</span><span class="sxs-lookup"><span data-stu-id="cd9bb-120">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="cd9bb-121">latitude</span><span class="sxs-lookup"><span data-stu-id="cd9bb-121">latitude</span></span>|<span data-ttu-id="cd9bb-122">Double</span><span class="sxs-lookup"><span data-stu-id="cd9bb-122">Double</span></span>|<span data-ttu-id="cd9bb-123">设备位置的纬度坐标</span><span class="sxs-lookup"><span data-stu-id="cd9bb-123">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="cd9bb-124">altitude</span><span class="sxs-lookup"><span data-stu-id="cd9bb-124">altitude</span></span>|<span data-ttu-id="cd9bb-125">Double</span><span class="sxs-lookup"><span data-stu-id="cd9bb-125">Double</span></span>|<span data-ttu-id="cd9bb-126">高度，以高出海平面的米数表示</span><span class="sxs-lookup"><span data-stu-id="cd9bb-126">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="cd9bb-127">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="cd9bb-127">horizontalAccuracy</span></span>|<span data-ttu-id="cd9bb-128">Double</span><span class="sxs-lookup"><span data-stu-id="cd9bb-128">Double</span></span>|<span data-ttu-id="cd9bb-129">经度和纬度的准确度，以米为单位</span><span class="sxs-lookup"><span data-stu-id="cd9bb-129">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="cd9bb-130">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="cd9bb-130">verticalAccuracy</span></span>|<span data-ttu-id="cd9bb-131">Double</span><span class="sxs-lookup"><span data-stu-id="cd9bb-131">Double</span></span>|<span data-ttu-id="cd9bb-132">高度的准确度，以米为单位</span><span class="sxs-lookup"><span data-stu-id="cd9bb-132">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="cd9bb-133">heading</span><span class="sxs-lookup"><span data-stu-id="cd9bb-133">heading</span></span>|<span data-ttu-id="cd9bb-134">Double</span><span class="sxs-lookup"><span data-stu-id="cd9bb-134">Double</span></span>|<span data-ttu-id="cd9bb-135">相对于真北的方位，以度为单位</span><span class="sxs-lookup"><span data-stu-id="cd9bb-135">Heading in degrees from true north</span></span>|
|<span data-ttu-id="cd9bb-136">speed</span><span class="sxs-lookup"><span data-stu-id="cd9bb-136">speed</span></span>|<span data-ttu-id="cd9bb-137">Double</span><span class="sxs-lookup"><span data-stu-id="cd9bb-137">Double</span></span>|<span data-ttu-id="cd9bb-138">设备的移动速度，以米/秒为单位</span><span class="sxs-lookup"><span data-stu-id="cd9bb-138">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd9bb-139">关系</span><span class="sxs-lookup"><span data-stu-id="cd9bb-139">Relationships</span></span>
<span data-ttu-id="cd9bb-140">无</span><span class="sxs-lookup"><span data-stu-id="cd9bb-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cd9bb-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cd9bb-141">JSON Representation</span></span>
<span data-ttu-id="cd9bb-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd9bb-142">Here is a JSON representation of the resource.</span></span>
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





