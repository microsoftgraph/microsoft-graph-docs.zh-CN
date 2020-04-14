---
title: windows10AppsForceUpdateSchedule 资源类型
description: 应用程序的 Windows 10 强制更新计划
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: eb590d65a6ae60eeede42b3ce6b5d422f306b8c8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466310"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a><span data-ttu-id="85d5e-103">windows10AppsForceUpdateSchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="85d5e-103">windows10AppsForceUpdateSchedule resource type</span></span>

<span data-ttu-id="85d5e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85d5e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85d5e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="85d5e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85d5e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="85d5e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85d5e-107">应用程序的 Windows 10 强制更新计划</span><span class="sxs-lookup"><span data-stu-id="85d5e-107">Windows 10 force update schedule for Apps</span></span>

## <a name="properties"></a><span data-ttu-id="85d5e-108">属性</span><span class="sxs-lookup"><span data-stu-id="85d5e-108">Properties</span></span>
|<span data-ttu-id="85d5e-109">属性</span><span class="sxs-lookup"><span data-stu-id="85d5e-109">Property</span></span>|<span data-ttu-id="85d5e-110">类型</span><span class="sxs-lookup"><span data-stu-id="85d5e-110">Type</span></span>|<span data-ttu-id="85d5e-111">说明</span><span class="sxs-lookup"><span data-stu-id="85d5e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85d5e-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="85d5e-112">startDateTime</span></span>|<span data-ttu-id="85d5e-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85d5e-113">DateTimeOffset</span></span>|<span data-ttu-id="85d5e-114">强制重启的开始时间。</span><span class="sxs-lookup"><span data-stu-id="85d5e-114">The start time for the force restart.</span></span>|
|<span data-ttu-id="85d5e-115">recurrence</span><span class="sxs-lookup"><span data-stu-id="85d5e-115">recurrence</span></span>|[<span data-ttu-id="85d5e-116">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="85d5e-116">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="85d5e-117">定期计划。</span><span class="sxs-lookup"><span data-stu-id="85d5e-117">Recurrence schedule.</span></span> <span data-ttu-id="85d5e-118">可取值为：`none`、`daily`、`weekly`、`monthly`。</span><span class="sxs-lookup"><span data-stu-id="85d5e-118">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="85d5e-119">runImmediatelyIfAfterStartDateTime</span><span class="sxs-lookup"><span data-stu-id="85d5e-119">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="85d5e-120">布尔值</span><span class="sxs-lookup"><span data-stu-id="85d5e-120">Boolean</span></span>|<span data-ttu-id="85d5e-121">如果为 true，则在 StartDateTime 为过去时立即运行任务，否则在下一个定期运行。</span><span class="sxs-lookup"><span data-stu-id="85d5e-121">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="85d5e-122">关系</span><span class="sxs-lookup"><span data-stu-id="85d5e-122">Relationships</span></span>
<span data-ttu-id="85d5e-123">无</span><span class="sxs-lookup"><span data-stu-id="85d5e-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="85d5e-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="85d5e-124">JSON Representation</span></span>
<span data-ttu-id="85d5e-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85d5e-125">Here is a JSON representation of the resource.</span></span>
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



