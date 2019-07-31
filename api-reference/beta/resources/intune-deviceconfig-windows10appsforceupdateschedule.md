---
title: windows10AppsForceUpdateSchedule 资源类型
description: 应用程序的 Windows 10 强制更新计划
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8bb42c8741b9adbfe67c64fd67b561d1cf59d083
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969294"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a><span data-ttu-id="bb295-103">windows10AppsForceUpdateSchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="bb295-103">windows10AppsForceUpdateSchedule resource type</span></span>

> <span data-ttu-id="bb295-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bb295-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb295-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bb295-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb295-106">应用程序的 Windows 10 强制更新计划</span><span class="sxs-lookup"><span data-stu-id="bb295-106">Windows 10 force update schedule for Apps</span></span>

## <a name="properties"></a><span data-ttu-id="bb295-107">属性</span><span class="sxs-lookup"><span data-stu-id="bb295-107">Properties</span></span>
|<span data-ttu-id="bb295-108">属性</span><span class="sxs-lookup"><span data-stu-id="bb295-108">Property</span></span>|<span data-ttu-id="bb295-109">类型</span><span class="sxs-lookup"><span data-stu-id="bb295-109">Type</span></span>|<span data-ttu-id="bb295-110">说明</span><span class="sxs-lookup"><span data-stu-id="bb295-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb295-111">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bb295-111">startDateTime</span></span>|<span data-ttu-id="bb295-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb295-112">DateTimeOffset</span></span>|<span data-ttu-id="bb295-113">强制重启的开始时间。</span><span class="sxs-lookup"><span data-stu-id="bb295-113">The start time for the force restart.</span></span>|
|<span data-ttu-id="bb295-114">recurrence</span><span class="sxs-lookup"><span data-stu-id="bb295-114">recurrence</span></span>|[<span data-ttu-id="bb295-115">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="bb295-115">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="bb295-116">定期计划。</span><span class="sxs-lookup"><span data-stu-id="bb295-116">Recurrence schedule.</span></span> <span data-ttu-id="bb295-117">可取值为：`none`、`daily`、`weekly`、`monthly`。</span><span class="sxs-lookup"><span data-stu-id="bb295-117">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="bb295-118">runImmediatelyIfAfterStartDateTime</span><span class="sxs-lookup"><span data-stu-id="bb295-118">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="bb295-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb295-119">Boolean</span></span>|<span data-ttu-id="bb295-120">如果为 true, 则在 StartDateTime 为过去时立即运行任务, 否则在下一个定期运行。</span><span class="sxs-lookup"><span data-stu-id="bb295-120">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb295-121">关系</span><span class="sxs-lookup"><span data-stu-id="bb295-121">Relationships</span></span>
<span data-ttu-id="bb295-122">无</span><span class="sxs-lookup"><span data-stu-id="bb295-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb295-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bb295-123">JSON Representation</span></span>
<span data-ttu-id="bb295-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb295-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AppsForceUpdateSchedule",
  "startDateTime": "String (timestamp)",
  "recurrence": "String",
  "runImmediatelyIfAfterStartDateTime": true
}
```





