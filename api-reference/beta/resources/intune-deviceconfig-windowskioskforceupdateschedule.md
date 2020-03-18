---
title: windowsKioskForceUpdateSchedule 资源类型
description: 展台设备的 Windows 10 强制更新计划。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2c1b9f1b82bc5edcbe1bdc7d1521ec669de5f6af
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786393"
---
# <a name="windowskioskforceupdateschedule-resource-type"></a><span data-ttu-id="1d55e-103">windowsKioskForceUpdateSchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="1d55e-103">windowsKioskForceUpdateSchedule resource type</span></span>

> <span data-ttu-id="1d55e-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1d55e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d55e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1d55e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d55e-106">展台设备的 Windows 10 强制更新计划。</span><span class="sxs-lookup"><span data-stu-id="1d55e-106">Windows 10 force update schedule for Kiosk devices.</span></span>

## <a name="properties"></a><span data-ttu-id="1d55e-107">属性</span><span class="sxs-lookup"><span data-stu-id="1d55e-107">Properties</span></span>
|<span data-ttu-id="1d55e-108">属性</span><span class="sxs-lookup"><span data-stu-id="1d55e-108">Property</span></span>|<span data-ttu-id="1d55e-109">类型</span><span class="sxs-lookup"><span data-stu-id="1d55e-109">Type</span></span>|<span data-ttu-id="1d55e-110">说明</span><span class="sxs-lookup"><span data-stu-id="1d55e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d55e-111">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1d55e-111">startDateTime</span></span>|<span data-ttu-id="1d55e-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d55e-112">DateTimeOffset</span></span>|<span data-ttu-id="1d55e-113">强制重启的开始时间。</span><span class="sxs-lookup"><span data-stu-id="1d55e-113">The start time for the force restart.</span></span>|
|<span data-ttu-id="1d55e-114">recurrence</span><span class="sxs-lookup"><span data-stu-id="1d55e-114">recurrence</span></span>|[<span data-ttu-id="1d55e-115">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="1d55e-115">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="1d55e-116">定期计划。</span><span class="sxs-lookup"><span data-stu-id="1d55e-116">Recurrence schedule.</span></span> <span data-ttu-id="1d55e-117">可取值为：`none`、`daily`、`weekly`、`monthly`。</span><span class="sxs-lookup"><span data-stu-id="1d55e-117">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="1d55e-118">dayofWeek</span><span class="sxs-lookup"><span data-stu-id="1d55e-118">dayofWeek</span></span>|[<span data-ttu-id="1d55e-119">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="1d55e-119">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="1d55e-120">一周中的某一天。</span><span class="sxs-lookup"><span data-stu-id="1d55e-120">Day of week.</span></span> <span data-ttu-id="1d55e-121">可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday` 或 `saturday`。</span><span class="sxs-lookup"><span data-stu-id="1d55e-121">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="1d55e-122">dayofMonth</span><span class="sxs-lookup"><span data-stu-id="1d55e-122">dayofMonth</span></span>|<span data-ttu-id="1d55e-123">Int32</span><span class="sxs-lookup"><span data-stu-id="1d55e-123">Int32</span></span>|<span data-ttu-id="1d55e-124">月中的某一天。</span><span class="sxs-lookup"><span data-stu-id="1d55e-124">Day of month.</span></span> <span data-ttu-id="1d55e-125">有效值为1至31</span><span class="sxs-lookup"><span data-stu-id="1d55e-125">Valid values 1 to 31</span></span>|
|<span data-ttu-id="1d55e-126">runImmediatelyIfAfterStartDateTime</span><span class="sxs-lookup"><span data-stu-id="1d55e-126">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="1d55e-127">布尔值</span><span class="sxs-lookup"><span data-stu-id="1d55e-127">Boolean</span></span>|<span data-ttu-id="1d55e-128">如果为 true，则在 StartDateTime 为过去时立即运行任务，否则在下一个定期运行。</span><span class="sxs-lookup"><span data-stu-id="1d55e-128">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d55e-129">关系</span><span class="sxs-lookup"><span data-stu-id="1d55e-129">Relationships</span></span>
<span data-ttu-id="1d55e-130">无</span><span class="sxs-lookup"><span data-stu-id="1d55e-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d55e-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1d55e-131">JSON Representation</span></span>
<span data-ttu-id="1d55e-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d55e-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskForceUpdateSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskForceUpdateSchedule",
  "startDateTime": "String (timestamp)",
  "recurrence": "String",
  "dayofWeek": "String",
  "dayofMonth": 1024,
  "runImmediatelyIfAfterStartDateTime": true
}
```



