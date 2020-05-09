---
title: deviceHealthScriptTimeSchedule 资源类型
description: 设备运行状况脚本时间计划的基本类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 75767d71b56b848cc045c08544b0633633eb73ac
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44176126"
---
# <a name="devicehealthscripttimeschedule-resource-type"></a><span data-ttu-id="761d6-103">deviceHealthScriptTimeSchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="761d6-103">deviceHealthScriptTimeSchedule resource type</span></span>

<span data-ttu-id="761d6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="761d6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="761d6-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="761d6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="761d6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="761d6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="761d6-107">设备运行状况脚本时间计划的基本类型。</span><span class="sxs-lookup"><span data-stu-id="761d6-107">Base type of Device health script time schedule.</span></span>


<span data-ttu-id="761d6-108">继承自[deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span><span class="sxs-lookup"><span data-stu-id="761d6-108">Inherits from [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="761d6-109">属性</span><span class="sxs-lookup"><span data-stu-id="761d6-109">Properties</span></span>
|<span data-ttu-id="761d6-110">属性</span><span class="sxs-lookup"><span data-stu-id="761d6-110">Property</span></span>|<span data-ttu-id="761d6-111">类型</span><span class="sxs-lookup"><span data-stu-id="761d6-111">Type</span></span>|<span data-ttu-id="761d6-112">说明</span><span class="sxs-lookup"><span data-stu-id="761d6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="761d6-113">interval</span><span class="sxs-lookup"><span data-stu-id="761d6-113">interval</span></span>|<span data-ttu-id="761d6-114">Int32</span><span class="sxs-lookup"><span data-stu-id="761d6-114">Int32</span></span>|<span data-ttu-id="761d6-115">每小时计划的 x 值，每隔 x 小时在每日计划的每 x 小时，每周计划的 x 周，每个 x 个月的日程安排。</span><span class="sxs-lookup"><span data-stu-id="761d6-115">The x value of every x hours for hourly schedule, every x days for Daily Schedule, every x weeks for weekly schedule, every x months for Monthly Schedule.</span></span> <span data-ttu-id="761d6-116">从[DeviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)继承的有效值1到23</span><span class="sxs-lookup"><span data-stu-id="761d6-116">Valid values 1 to 23 Inherited from [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span></span>|
|<span data-ttu-id="761d6-117">useUtc</span><span class="sxs-lookup"><span data-stu-id="761d6-117">useUtc</span></span>|<span data-ttu-id="761d6-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="761d6-118">Boolean</span></span>|<span data-ttu-id="761d6-119">指示时间是 Utc 还是客户端本地时间。</span><span class="sxs-lookup"><span data-stu-id="761d6-119">Indicate if the time is Utc or client local time.</span></span>|
|<span data-ttu-id="761d6-120">time</span><span class="sxs-lookup"><span data-stu-id="761d6-120">time</span></span>|<span data-ttu-id="761d6-121">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="761d6-121">TimeOfDay</span></span>|<span data-ttu-id="761d6-122">在什么时候计划运行脚本。</span><span class="sxs-lookup"><span data-stu-id="761d6-122">At what time the script is scheduled to run.</span></span> <span data-ttu-id="761d6-123">此集合最多可包含20个元素。</span><span class="sxs-lookup"><span data-stu-id="761d6-123">This collection can contain a maximum of 20 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="761d6-124">关系</span><span class="sxs-lookup"><span data-stu-id="761d6-124">Relationships</span></span>
<span data-ttu-id="761d6-125">无</span><span class="sxs-lookup"><span data-stu-id="761d6-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="761d6-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="761d6-126">JSON Representation</span></span>
<span data-ttu-id="761d6-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="761d6-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptTimeSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptTimeSchedule",
  "interval": 1024,
  "useUtc": true,
  "time": "String (time of day)"
}
```



