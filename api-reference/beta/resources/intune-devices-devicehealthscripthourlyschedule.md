---
title: deviceHealthScriptHourlySchedule 资源类型
description: 设备运行状况脚本每小时计划的类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d2276d95d09a1628b07d3b9bc87381b0d85d431f
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44176134"
---
# <a name="devicehealthscripthourlyschedule-resource-type"></a><span data-ttu-id="18a3f-103">deviceHealthScriptHourlySchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="18a3f-103">deviceHealthScriptHourlySchedule resource type</span></span>

<span data-ttu-id="18a3f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18a3f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18a3f-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="18a3f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18a3f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="18a3f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18a3f-107">设备运行状况脚本每小时计划的类型。</span><span class="sxs-lookup"><span data-stu-id="18a3f-107">Type of Device health script hourly schedule.</span></span>


<span data-ttu-id="18a3f-108">继承自[deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span><span class="sxs-lookup"><span data-stu-id="18a3f-108">Inherits from [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="18a3f-109">属性</span><span class="sxs-lookup"><span data-stu-id="18a3f-109">Properties</span></span>
|<span data-ttu-id="18a3f-110">属性</span><span class="sxs-lookup"><span data-stu-id="18a3f-110">Property</span></span>|<span data-ttu-id="18a3f-111">类型</span><span class="sxs-lookup"><span data-stu-id="18a3f-111">Type</span></span>|<span data-ttu-id="18a3f-112">说明</span><span class="sxs-lookup"><span data-stu-id="18a3f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18a3f-113">interval</span><span class="sxs-lookup"><span data-stu-id="18a3f-113">interval</span></span>|<span data-ttu-id="18a3f-114">Int32</span><span class="sxs-lookup"><span data-stu-id="18a3f-114">Int32</span></span>|<span data-ttu-id="18a3f-115">每小时计划的 x 值，每隔 x 小时在每日计划的每 x 小时，每周计划的 x 周，每个 x 个月的日程安排。</span><span class="sxs-lookup"><span data-stu-id="18a3f-115">The x value of every x hours for hourly schedule, every x days for Daily Schedule, every x weeks for weekly schedule, every x months for Monthly Schedule.</span></span> <span data-ttu-id="18a3f-116">从[DeviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)继承的有效值1到23</span><span class="sxs-lookup"><span data-stu-id="18a3f-116">Valid values 1 to 23 Inherited from [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="18a3f-117">关系</span><span class="sxs-lookup"><span data-stu-id="18a3f-117">Relationships</span></span>
<span data-ttu-id="18a3f-118">无</span><span class="sxs-lookup"><span data-stu-id="18a3f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="18a3f-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="18a3f-119">JSON Representation</span></span>
<span data-ttu-id="18a3f-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="18a3f-120">Here is a JSON representation of the resource.</span></span>
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



