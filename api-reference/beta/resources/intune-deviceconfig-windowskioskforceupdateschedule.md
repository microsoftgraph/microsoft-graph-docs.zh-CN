---
title: windowsKioskForceUpdateSchedule 资源类型
description: 展台设备的 Windows 10 强制更新计划。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d08a5e54aca83a71b094dbcd17095e421850b5ab
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525493"
---
# <a name="windowskioskforceupdateschedule-resource-type"></a><span data-ttu-id="d1732-103">windowsKioskForceUpdateSchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="d1732-103">windowsKioskForceUpdateSchedule resource type</span></span>

<span data-ttu-id="d1732-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d1732-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1732-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d1732-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1732-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d1732-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1732-107">展台设备的 Windows 10 强制更新计划。</span><span class="sxs-lookup"><span data-stu-id="d1732-107">Windows 10 force update schedule for Kiosk devices.</span></span>

## <a name="properties"></a><span data-ttu-id="d1732-108">属性</span><span class="sxs-lookup"><span data-stu-id="d1732-108">Properties</span></span>
|<span data-ttu-id="d1732-109">属性</span><span class="sxs-lookup"><span data-stu-id="d1732-109">Property</span></span>|<span data-ttu-id="d1732-110">类型</span><span class="sxs-lookup"><span data-stu-id="d1732-110">Type</span></span>|<span data-ttu-id="d1732-111">说明</span><span class="sxs-lookup"><span data-stu-id="d1732-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1732-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d1732-112">startDateTime</span></span>|<span data-ttu-id="d1732-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1732-113">DateTimeOffset</span></span>|<span data-ttu-id="d1732-114">强制重启的开始时间。</span><span class="sxs-lookup"><span data-stu-id="d1732-114">The start time for the force restart.</span></span>|
|<span data-ttu-id="d1732-115">recurrence</span><span class="sxs-lookup"><span data-stu-id="d1732-115">recurrence</span></span>|[<span data-ttu-id="d1732-116">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="d1732-116">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="d1732-117">定期计划。</span><span class="sxs-lookup"><span data-stu-id="d1732-117">Recurrence schedule.</span></span> <span data-ttu-id="d1732-118">可取值为：`none`、`daily`、`weekly`、`monthly`。</span><span class="sxs-lookup"><span data-stu-id="d1732-118">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="d1732-119">dayofWeek</span><span class="sxs-lookup"><span data-stu-id="d1732-119">dayofWeek</span></span>|[<span data-ttu-id="d1732-120">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="d1732-120">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="d1732-121">一周中的某一天。</span><span class="sxs-lookup"><span data-stu-id="d1732-121">Day of week.</span></span> <span data-ttu-id="d1732-122">可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday` 或 `saturday`。</span><span class="sxs-lookup"><span data-stu-id="d1732-122">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="d1732-123">dayofMonth</span><span class="sxs-lookup"><span data-stu-id="d1732-123">dayofMonth</span></span>|<span data-ttu-id="d1732-124">Int32</span><span class="sxs-lookup"><span data-stu-id="d1732-124">Int32</span></span>|<span data-ttu-id="d1732-125">月中的某一天。</span><span class="sxs-lookup"><span data-stu-id="d1732-125">Day of month.</span></span> <span data-ttu-id="d1732-126">有效值为1至31</span><span class="sxs-lookup"><span data-stu-id="d1732-126">Valid values 1 to 31</span></span>|
|<span data-ttu-id="d1732-127">runImmediatelyIfAfterStartDateTime</span><span class="sxs-lookup"><span data-stu-id="d1732-127">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="d1732-128">布尔</span><span class="sxs-lookup"><span data-stu-id="d1732-128">Boolean</span></span>|<span data-ttu-id="d1732-129">如果为 true，则在 StartDateTime 为过去时立即运行任务，否则在下一个定期运行。</span><span class="sxs-lookup"><span data-stu-id="d1732-129">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1732-130">关系</span><span class="sxs-lookup"><span data-stu-id="d1732-130">Relationships</span></span>
<span data-ttu-id="d1732-131">无</span><span class="sxs-lookup"><span data-stu-id="d1732-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1732-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d1732-132">JSON Representation</span></span>
<span data-ttu-id="d1732-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d1732-133">Here is a JSON representation of the resource.</span></span>
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



