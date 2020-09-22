---
title: deviceHealthScriptRunOnceSchedule 资源类型
description: 设备运行状况脚本运行一次计划。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4df6220bc95cd98e07a49073c3a7e5da6ab4096d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060270"
---
# <a name="devicehealthscriptrunonceschedule-resource-type"></a><span data-ttu-id="9b5c4-103">deviceHealthScriptRunOnceSchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="9b5c4-103">deviceHealthScriptRunOnceSchedule resource type</span></span>

<span data-ttu-id="9b5c4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b5c4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b5c4-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9b5c4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b5c4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9b5c4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b5c4-107">设备运行状况脚本运行一次计划。</span><span class="sxs-lookup"><span data-stu-id="9b5c4-107">Device health script run once schedule.</span></span>


<span data-ttu-id="9b5c4-108">继承自 [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)</span><span class="sxs-lookup"><span data-stu-id="9b5c4-108">Inherits from [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9b5c4-109">属性</span><span class="sxs-lookup"><span data-stu-id="9b5c4-109">Properties</span></span>
|<span data-ttu-id="9b5c4-110">属性</span><span class="sxs-lookup"><span data-stu-id="9b5c4-110">Property</span></span>|<span data-ttu-id="9b5c4-111">类型</span><span class="sxs-lookup"><span data-stu-id="9b5c4-111">Type</span></span>|<span data-ttu-id="9b5c4-112">说明</span><span class="sxs-lookup"><span data-stu-id="9b5c4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b5c4-113">interval</span><span class="sxs-lookup"><span data-stu-id="9b5c4-113">interval</span></span>|<span data-ttu-id="9b5c4-114">Int32</span><span class="sxs-lookup"><span data-stu-id="9b5c4-114">Int32</span></span>|<span data-ttu-id="9b5c4-115">每小时计划的 x 值，每隔 x 小时在每日计划的每 x 小时，每周计划的 x 周，每个 x 个月的日程安排。</span><span class="sxs-lookup"><span data-stu-id="9b5c4-115">The x value of every x hours for hourly schedule, every x days for Daily Schedule, every x weeks for weekly schedule, every x months for Monthly Schedule.</span></span> <span data-ttu-id="9b5c4-116">从[DeviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)继承的有效值1到23</span><span class="sxs-lookup"><span data-stu-id="9b5c4-116">Valid values 1 to 23 Inherited from [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span></span>|
|<span data-ttu-id="9b5c4-117">useUtc</span><span class="sxs-lookup"><span data-stu-id="9b5c4-117">useUtc</span></span>|<span data-ttu-id="9b5c4-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b5c4-118">Boolean</span></span>|<span data-ttu-id="9b5c4-119">指示时间是 Utc 还是客户端本地时间。</span><span class="sxs-lookup"><span data-stu-id="9b5c4-119">Indicate if the time is Utc or client local time.</span></span> <span data-ttu-id="9b5c4-120">继承自 [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)</span><span class="sxs-lookup"><span data-stu-id="9b5c4-120">Inherited from [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)</span></span>|
|<span data-ttu-id="9b5c4-121">time</span><span class="sxs-lookup"><span data-stu-id="9b5c4-121">time</span></span>|<span data-ttu-id="9b5c4-122">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="9b5c4-122">TimeOfDay</span></span>|<span data-ttu-id="9b5c4-123">在什么时候计划运行脚本。</span><span class="sxs-lookup"><span data-stu-id="9b5c4-123">At what time the script is scheduled to run.</span></span> <span data-ttu-id="9b5c4-124">此集合最多可包含20个元素。</span><span class="sxs-lookup"><span data-stu-id="9b5c4-124">This collection can contain a maximum of 20 elements.</span></span> <span data-ttu-id="9b5c4-125">继承自 [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)</span><span class="sxs-lookup"><span data-stu-id="9b5c4-125">Inherited from [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)</span></span>|
|<span data-ttu-id="9b5c4-126">date</span><span class="sxs-lookup"><span data-stu-id="9b5c4-126">date</span></span>|<span data-ttu-id="9b5c4-127">Date</span><span class="sxs-lookup"><span data-stu-id="9b5c4-127">Date</span></span>|<span data-ttu-id="9b5c4-128">计划运行脚本的日期。</span><span class="sxs-lookup"><span data-stu-id="9b5c4-128">The date the script is scheduled to run.</span></span> <span data-ttu-id="9b5c4-129">此集合最多可包含20个元素。</span><span class="sxs-lookup"><span data-stu-id="9b5c4-129">This collection can contain a maximum of 20 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b5c4-130">关系</span><span class="sxs-lookup"><span data-stu-id="9b5c4-130">Relationships</span></span>
<span data-ttu-id="9b5c4-131">无</span><span class="sxs-lookup"><span data-stu-id="9b5c4-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b5c4-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9b5c4-132">JSON Representation</span></span>
<span data-ttu-id="9b5c4-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9b5c4-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRunOnceSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunOnceSchedule",
  "interval": 1024,
  "useUtc": true,
  "time": "String (time of day)",
  "date": "String (Date)"
}
```






