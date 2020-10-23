---
title: windows10AppsForceUpdateSchedule 资源类型
description: 应用程序的 Windows 10 强制更新计划
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9f902ef48caafa5f782c12d862e540bf7c482899
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732521"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a><span data-ttu-id="c5c21-103">windows10AppsForceUpdateSchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="c5c21-103">windows10AppsForceUpdateSchedule resource type</span></span>

<span data-ttu-id="c5c21-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5c21-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c5c21-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c5c21-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5c21-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c5c21-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5c21-107">应用程序的 Windows 10 强制更新计划</span><span class="sxs-lookup"><span data-stu-id="c5c21-107">Windows 10 force update schedule for Apps</span></span>

## <a name="properties"></a><span data-ttu-id="c5c21-108">属性</span><span class="sxs-lookup"><span data-stu-id="c5c21-108">Properties</span></span>
|<span data-ttu-id="c5c21-109">属性</span><span class="sxs-lookup"><span data-stu-id="c5c21-109">Property</span></span>|<span data-ttu-id="c5c21-110">类型</span><span class="sxs-lookup"><span data-stu-id="c5c21-110">Type</span></span>|<span data-ttu-id="c5c21-111">说明</span><span class="sxs-lookup"><span data-stu-id="c5c21-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5c21-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c5c21-112">startDateTime</span></span>|<span data-ttu-id="c5c21-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5c21-113">DateTimeOffset</span></span>|<span data-ttu-id="c5c21-114">强制重启的开始时间。</span><span class="sxs-lookup"><span data-stu-id="c5c21-114">The start time for the force restart.</span></span>|
|<span data-ttu-id="c5c21-115">recurrence</span><span class="sxs-lookup"><span data-stu-id="c5c21-115">recurrence</span></span>|[<span data-ttu-id="c5c21-116">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="c5c21-116">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="c5c21-117">定期计划。</span><span class="sxs-lookup"><span data-stu-id="c5c21-117">Recurrence schedule.</span></span> <span data-ttu-id="c5c21-118">可取值为：`none`、`daily`、`weekly`、`monthly`。</span><span class="sxs-lookup"><span data-stu-id="c5c21-118">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="c5c21-119">runImmediatelyIfAfterStartDateTime</span><span class="sxs-lookup"><span data-stu-id="c5c21-119">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="c5c21-120">布尔</span><span class="sxs-lookup"><span data-stu-id="c5c21-120">Boolean</span></span>|<span data-ttu-id="c5c21-121">如果为 true，则在 StartDateTime 为过去时立即运行任务，否则在下一个定期运行。</span><span class="sxs-lookup"><span data-stu-id="c5c21-121">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5c21-122">关系</span><span class="sxs-lookup"><span data-stu-id="c5c21-122">Relationships</span></span>
<span data-ttu-id="c5c21-123">无</span><span class="sxs-lookup"><span data-stu-id="c5c21-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5c21-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c5c21-124">JSON Representation</span></span>
<span data-ttu-id="c5c21-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5c21-125">Here is a JSON representation of the resource.</span></span>
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





