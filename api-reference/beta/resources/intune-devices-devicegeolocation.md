---
title: deviceGeoLocation 资源类型
description: 设备位置
ms.openlocfilehash: 2ab7f777d00b891ceb7aae127ac87868aec582cc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043056"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="91599-103">deviceGeoLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="91599-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="91599-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="91599-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91599-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="91599-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="91599-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="91599-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91599-107">设备位置</span><span class="sxs-lookup"><span data-stu-id="91599-107">Device location</span></span>
## <a name="properties"></a><span data-ttu-id="91599-108">属性</span><span class="sxs-lookup"><span data-stu-id="91599-108">Properties</span></span>
|<span data-ttu-id="91599-109">属性</span><span class="sxs-lookup"><span data-stu-id="91599-109">Property</span></span>|<span data-ttu-id="91599-110">类型</span><span class="sxs-lookup"><span data-stu-id="91599-110">Type</span></span>|<span data-ttu-id="91599-111">说明</span><span class="sxs-lookup"><span data-stu-id="91599-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91599-112">lastCollectedDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="91599-112">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="91599-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91599-113">DateTimeOffset</span></span>|<span data-ttu-id="91599-114">记录位置时的时间，相对于 UTC</span><span class="sxs-lookup"><span data-stu-id="91599-114">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="91599-115">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="91599-115">lastCollectedDateTime</span></span>|<span data-ttu-id="91599-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91599-116">DateTimeOffset</span></span>|<span data-ttu-id="91599-117">记录位置时的时间，相对于 UTC</span><span class="sxs-lookup"><span data-stu-id="91599-117">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="91599-118">longitude</span><span class="sxs-lookup"><span data-stu-id="91599-118">longitude</span></span>|<span data-ttu-id="91599-119">Double</span><span class="sxs-lookup"><span data-stu-id="91599-119">Double</span></span>|<span data-ttu-id="91599-120">设备位置的经度坐标</span><span class="sxs-lookup"><span data-stu-id="91599-120">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="91599-121">latitude</span><span class="sxs-lookup"><span data-stu-id="91599-121">latitude</span></span>|<span data-ttu-id="91599-122">Double</span><span class="sxs-lookup"><span data-stu-id="91599-122">Double</span></span>|<span data-ttu-id="91599-123">设备位置的纬度坐标</span><span class="sxs-lookup"><span data-stu-id="91599-123">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="91599-124">altitude</span><span class="sxs-lookup"><span data-stu-id="91599-124">altitude</span></span>|<span data-ttu-id="91599-125">Double</span><span class="sxs-lookup"><span data-stu-id="91599-125">Double</span></span>|<span data-ttu-id="91599-126">高度，以高出海平面的米数表示</span><span class="sxs-lookup"><span data-stu-id="91599-126">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="91599-127">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="91599-127">horizontalAccuracy</span></span>|<span data-ttu-id="91599-128">Double</span><span class="sxs-lookup"><span data-stu-id="91599-128">Double</span></span>|<span data-ttu-id="91599-129">经度和纬度的准确度，以米为单位</span><span class="sxs-lookup"><span data-stu-id="91599-129">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="91599-130">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="91599-130">verticalAccuracy</span></span>|<span data-ttu-id="91599-131">Double</span><span class="sxs-lookup"><span data-stu-id="91599-131">Double</span></span>|<span data-ttu-id="91599-132">高度的准确度，以米为单位</span><span class="sxs-lookup"><span data-stu-id="91599-132">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="91599-133">heading</span><span class="sxs-lookup"><span data-stu-id="91599-133">heading</span></span>|<span data-ttu-id="91599-134">Double</span><span class="sxs-lookup"><span data-stu-id="91599-134">Double</span></span>|<span data-ttu-id="91599-135">相对于真北的方位，以度为单位</span><span class="sxs-lookup"><span data-stu-id="91599-135">Heading in degrees from true north</span></span>|
|<span data-ttu-id="91599-136">speed</span><span class="sxs-lookup"><span data-stu-id="91599-136">speed</span></span>|<span data-ttu-id="91599-137">Double</span><span class="sxs-lookup"><span data-stu-id="91599-137">Double</span></span>|<span data-ttu-id="91599-138">设备的移动速度，以米/秒为单位</span><span class="sxs-lookup"><span data-stu-id="91599-138">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="91599-139">关系</span><span class="sxs-lookup"><span data-stu-id="91599-139">Relationships</span></span>
<span data-ttu-id="91599-140">无</span><span class="sxs-lookup"><span data-stu-id="91599-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="91599-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="91599-141">JSON Representation</span></span>
<span data-ttu-id="91599-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91599-142">Here is a JSON representation of the resource.</span></span>
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





