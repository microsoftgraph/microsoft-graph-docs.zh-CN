---
title: deviceGeoLocation 资源类型
description: 设备位置
ms.openlocfilehash: 1bc72e4fb2d01c55d5d16ff2a45a020c5eaf99e5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010595"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="e4b12-103">deviceGeoLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="e4b12-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="e4b12-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e4b12-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e4b12-105">设备位置</span><span class="sxs-lookup"><span data-stu-id="e4b12-105">Device location</span></span>
## <a name="properties"></a><span data-ttu-id="e4b12-106">属性</span><span class="sxs-lookup"><span data-stu-id="e4b12-106">Properties</span></span>
|<span data-ttu-id="e4b12-107">属性</span><span class="sxs-lookup"><span data-stu-id="e4b12-107">Property</span></span>|<span data-ttu-id="e4b12-108">类型</span><span class="sxs-lookup"><span data-stu-id="e4b12-108">Type</span></span>|<span data-ttu-id="e4b12-109">说明</span><span class="sxs-lookup"><span data-stu-id="e4b12-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4b12-110">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="e4b12-110">lastCollectedDateTime</span></span>|<span data-ttu-id="e4b12-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4b12-111">DateTimeOffset</span></span>|<span data-ttu-id="e4b12-112">记录位置时的时间，相对于 UTC</span><span class="sxs-lookup"><span data-stu-id="e4b12-112">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="e4b12-113">longitude</span><span class="sxs-lookup"><span data-stu-id="e4b12-113">longitude</span></span>|<span data-ttu-id="e4b12-114">Double</span><span class="sxs-lookup"><span data-stu-id="e4b12-114">Double</span></span>|<span data-ttu-id="e4b12-115">设备位置的经度坐标</span><span class="sxs-lookup"><span data-stu-id="e4b12-115">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="e4b12-116">latitude</span><span class="sxs-lookup"><span data-stu-id="e4b12-116">latitude</span></span>|<span data-ttu-id="e4b12-117">Double</span><span class="sxs-lookup"><span data-stu-id="e4b12-117">Double</span></span>|<span data-ttu-id="e4b12-118">设备位置的纬度坐标</span><span class="sxs-lookup"><span data-stu-id="e4b12-118">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="e4b12-119">altitude</span><span class="sxs-lookup"><span data-stu-id="e4b12-119">altitude</span></span>|<span data-ttu-id="e4b12-120">Double</span><span class="sxs-lookup"><span data-stu-id="e4b12-120">Double</span></span>|<span data-ttu-id="e4b12-121">高度，以高出海平面的米数表示</span><span class="sxs-lookup"><span data-stu-id="e4b12-121">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="e4b12-122">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="e4b12-122">horizontalAccuracy</span></span>|<span data-ttu-id="e4b12-123">Double</span><span class="sxs-lookup"><span data-stu-id="e4b12-123">Double</span></span>|<span data-ttu-id="e4b12-124">经度和纬度的准确度，以米为单位</span><span class="sxs-lookup"><span data-stu-id="e4b12-124">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="e4b12-125">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="e4b12-125">verticalAccuracy</span></span>|<span data-ttu-id="e4b12-126">Double</span><span class="sxs-lookup"><span data-stu-id="e4b12-126">Double</span></span>|<span data-ttu-id="e4b12-127">高度的准确度，以米为单位</span><span class="sxs-lookup"><span data-stu-id="e4b12-127">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="e4b12-128">heading</span><span class="sxs-lookup"><span data-stu-id="e4b12-128">heading</span></span>|<span data-ttu-id="e4b12-129">Double</span><span class="sxs-lookup"><span data-stu-id="e4b12-129">Double</span></span>|<span data-ttu-id="e4b12-130">相对于真北的方位，以度为单位</span><span class="sxs-lookup"><span data-stu-id="e4b12-130">Heading in degrees from true north</span></span>|
|<span data-ttu-id="e4b12-131">speed</span><span class="sxs-lookup"><span data-stu-id="e4b12-131">speed</span></span>|<span data-ttu-id="e4b12-132">Double</span><span class="sxs-lookup"><span data-stu-id="e4b12-132">Double</span></span>|<span data-ttu-id="e4b12-133">设备的移动速度，以米/秒为单位</span><span class="sxs-lookup"><span data-stu-id="e4b12-133">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4b12-134">关系</span><span class="sxs-lookup"><span data-stu-id="e4b12-134">Relationships</span></span>
<span data-ttu-id="e4b12-135">无</span><span class="sxs-lookup"><span data-stu-id="e4b12-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e4b12-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e4b12-136">JSON Representation</span></span>
<span data-ttu-id="e4b12-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4b12-137">Here is a JSON representation of the resource.</span></span>
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



