---
title: deviceGeoLocation 资源类型
description: 设备位置
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 68e89b2e63b99324332874a3ad6a2f2e3c335832
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816126"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="6fe61-103">deviceGeoLocation 资源类型</span><span class="sxs-lookup"><span data-stu-id="6fe61-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="6fe61-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6fe61-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6fe61-105">设备位置</span><span class="sxs-lookup"><span data-stu-id="6fe61-105">Device location</span></span>
## <a name="properties"></a><span data-ttu-id="6fe61-106">属性</span><span class="sxs-lookup"><span data-stu-id="6fe61-106">Properties</span></span>
|<span data-ttu-id="6fe61-107">属性</span><span class="sxs-lookup"><span data-stu-id="6fe61-107">Property</span></span>|<span data-ttu-id="6fe61-108">类型</span><span class="sxs-lookup"><span data-stu-id="6fe61-108">Type</span></span>|<span data-ttu-id="6fe61-109">说明</span><span class="sxs-lookup"><span data-stu-id="6fe61-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fe61-110">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="6fe61-110">lastCollectedDateTime</span></span>|<span data-ttu-id="6fe61-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fe61-111">DateTimeOffset</span></span>|<span data-ttu-id="6fe61-112">记录位置时的时间，相对于 UTC</span><span class="sxs-lookup"><span data-stu-id="6fe61-112">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="6fe61-113">longitude</span><span class="sxs-lookup"><span data-stu-id="6fe61-113">longitude</span></span>|<span data-ttu-id="6fe61-114">Double</span><span class="sxs-lookup"><span data-stu-id="6fe61-114">Double</span></span>|<span data-ttu-id="6fe61-115">设备位置的经度坐标</span><span class="sxs-lookup"><span data-stu-id="6fe61-115">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="6fe61-116">latitude</span><span class="sxs-lookup"><span data-stu-id="6fe61-116">latitude</span></span>|<span data-ttu-id="6fe61-117">Double</span><span class="sxs-lookup"><span data-stu-id="6fe61-117">Double</span></span>|<span data-ttu-id="6fe61-118">设备位置的纬度坐标</span><span class="sxs-lookup"><span data-stu-id="6fe61-118">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="6fe61-119">altitude</span><span class="sxs-lookup"><span data-stu-id="6fe61-119">altitude</span></span>|<span data-ttu-id="6fe61-120">Double</span><span class="sxs-lookup"><span data-stu-id="6fe61-120">Double</span></span>|<span data-ttu-id="6fe61-121">高度，以高出海平面的米数表示</span><span class="sxs-lookup"><span data-stu-id="6fe61-121">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="6fe61-122">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="6fe61-122">horizontalAccuracy</span></span>|<span data-ttu-id="6fe61-123">Double</span><span class="sxs-lookup"><span data-stu-id="6fe61-123">Double</span></span>|<span data-ttu-id="6fe61-124">经度和纬度的准确度，以米为单位</span><span class="sxs-lookup"><span data-stu-id="6fe61-124">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="6fe61-125">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="6fe61-125">verticalAccuracy</span></span>|<span data-ttu-id="6fe61-126">Double</span><span class="sxs-lookup"><span data-stu-id="6fe61-126">Double</span></span>|<span data-ttu-id="6fe61-127">高度的准确度，以米为单位</span><span class="sxs-lookup"><span data-stu-id="6fe61-127">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="6fe61-128">heading</span><span class="sxs-lookup"><span data-stu-id="6fe61-128">heading</span></span>|<span data-ttu-id="6fe61-129">Double</span><span class="sxs-lookup"><span data-stu-id="6fe61-129">Double</span></span>|<span data-ttu-id="6fe61-130">相对于真北的方位，以度为单位</span><span class="sxs-lookup"><span data-stu-id="6fe61-130">Heading in degrees from true north</span></span>|
|<span data-ttu-id="6fe61-131">speed</span><span class="sxs-lookup"><span data-stu-id="6fe61-131">speed</span></span>|<span data-ttu-id="6fe61-132">Double</span><span class="sxs-lookup"><span data-stu-id="6fe61-132">Double</span></span>|<span data-ttu-id="6fe61-133">设备的移动速度，以米/秒为单位</span><span class="sxs-lookup"><span data-stu-id="6fe61-133">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="6fe61-134">关系</span><span class="sxs-lookup"><span data-stu-id="6fe61-134">Relationships</span></span>
<span data-ttu-id="6fe61-135">无</span><span class="sxs-lookup"><span data-stu-id="6fe61-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6fe61-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6fe61-136">JSON Representation</span></span>
<span data-ttu-id="6fe61-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6fe61-137">Here is a JSON representation of the resource.</span></span>
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



