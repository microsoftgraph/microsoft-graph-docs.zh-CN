---
title: windows10AppsForceUpdateSchedule 资源类型
description: 应用程序的 Windows 10 强制更新计划
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 20ea28b176f05bb1e6d2e2579715ebe5bdd500a2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49273030"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a><span data-ttu-id="77f16-103">windows10AppsForceUpdateSchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="77f16-103">windows10AppsForceUpdateSchedule resource type</span></span>

<span data-ttu-id="77f16-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77f16-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77f16-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="77f16-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77f16-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="77f16-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77f16-107">应用程序的 Windows 10 强制更新计划</span><span class="sxs-lookup"><span data-stu-id="77f16-107">Windows 10 force update schedule for Apps</span></span>

## <a name="properties"></a><span data-ttu-id="77f16-108">属性</span><span class="sxs-lookup"><span data-stu-id="77f16-108">Properties</span></span>
|<span data-ttu-id="77f16-109">属性</span><span class="sxs-lookup"><span data-stu-id="77f16-109">Property</span></span>|<span data-ttu-id="77f16-110">类型</span><span class="sxs-lookup"><span data-stu-id="77f16-110">Type</span></span>|<span data-ttu-id="77f16-111">说明</span><span class="sxs-lookup"><span data-stu-id="77f16-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77f16-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="77f16-112">startDateTime</span></span>|<span data-ttu-id="77f16-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77f16-113">DateTimeOffset</span></span>|<span data-ttu-id="77f16-114">强制重启的开始时间。</span><span class="sxs-lookup"><span data-stu-id="77f16-114">The start time for the force restart.</span></span>|
|<span data-ttu-id="77f16-115">recurrence</span><span class="sxs-lookup"><span data-stu-id="77f16-115">recurrence</span></span>|[<span data-ttu-id="77f16-116">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="77f16-116">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="77f16-117">定期计划。</span><span class="sxs-lookup"><span data-stu-id="77f16-117">Recurrence schedule.</span></span> <span data-ttu-id="77f16-118">可取值为：`none`、`daily`、`weekly`、`monthly`。</span><span class="sxs-lookup"><span data-stu-id="77f16-118">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="77f16-119">runImmediatelyIfAfterStartDateTime</span><span class="sxs-lookup"><span data-stu-id="77f16-119">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="77f16-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="77f16-120">Boolean</span></span>|<span data-ttu-id="77f16-121">如果为 true，则在 StartDateTime 为过去时立即运行任务，否则在下一个定期运行。</span><span class="sxs-lookup"><span data-stu-id="77f16-121">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="77f16-122">关系</span><span class="sxs-lookup"><span data-stu-id="77f16-122">Relationships</span></span>
<span data-ttu-id="77f16-123">无</span><span class="sxs-lookup"><span data-stu-id="77f16-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="77f16-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="77f16-124">JSON Representation</span></span>
<span data-ttu-id="77f16-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="77f16-125">Here is a JSON representation of the resource.</span></span>
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




