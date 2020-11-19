---
title: deviceHealthScriptHourlySchedule 资源类型
description: 设备运行状况脚本每小时计划的类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 883ae445447d358342b9c817d3cacd732b3a9b79
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49226515"
---
# <a name="devicehealthscripthourlyschedule-resource-type"></a><span data-ttu-id="e210d-103">deviceHealthScriptHourlySchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="e210d-103">deviceHealthScriptHourlySchedule resource type</span></span>

<span data-ttu-id="e210d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e210d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e210d-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e210d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e210d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e210d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e210d-107">设备运行状况脚本每小时计划的类型。</span><span class="sxs-lookup"><span data-stu-id="e210d-107">Type of Device health script hourly schedule.</span></span>


<span data-ttu-id="e210d-108">继承自 [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span><span class="sxs-lookup"><span data-stu-id="e210d-108">Inherits from [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e210d-109">属性</span><span class="sxs-lookup"><span data-stu-id="e210d-109">Properties</span></span>
|<span data-ttu-id="e210d-110">属性</span><span class="sxs-lookup"><span data-stu-id="e210d-110">Property</span></span>|<span data-ttu-id="e210d-111">类型</span><span class="sxs-lookup"><span data-stu-id="e210d-111">Type</span></span>|<span data-ttu-id="e210d-112">说明</span><span class="sxs-lookup"><span data-stu-id="e210d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e210d-113">interval</span><span class="sxs-lookup"><span data-stu-id="e210d-113">interval</span></span>|<span data-ttu-id="e210d-114">Int32</span><span class="sxs-lookup"><span data-stu-id="e210d-114">Int32</span></span>|<span data-ttu-id="e210d-115">每小时计划的 x 值，每隔 x 小时在每日计划的每 x 小时，每周计划的 x 周，每个 x 个月的日程安排。</span><span class="sxs-lookup"><span data-stu-id="e210d-115">The x value of every x hours for hourly schedule, every x days for Daily Schedule, every x weeks for weekly schedule, every x months for Monthly Schedule.</span></span> <span data-ttu-id="e210d-116">从[DeviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)继承的有效值1到23</span><span class="sxs-lookup"><span data-stu-id="e210d-116">Valid values 1 to 23 Inherited from [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="e210d-117">关系</span><span class="sxs-lookup"><span data-stu-id="e210d-117">Relationships</span></span>
<span data-ttu-id="e210d-118">无</span><span class="sxs-lookup"><span data-stu-id="e210d-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e210d-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e210d-119">JSON Representation</span></span>
<span data-ttu-id="e210d-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e210d-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptHourlySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptHourlySchedule",
  "interval": 1024
}
```




