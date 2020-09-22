---
title: windows10AppsForceUpdateSchedule 资源类型
description: 应用程序的 Windows 10 强制更新计划
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7041f61bfe56a12c238426864e82563c88d23f98
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985928"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a><span data-ttu-id="65339-103">windows10AppsForceUpdateSchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="65339-103">windows10AppsForceUpdateSchedule resource type</span></span>

<span data-ttu-id="65339-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65339-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="65339-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="65339-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65339-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="65339-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65339-107">应用程序的 Windows 10 强制更新计划</span><span class="sxs-lookup"><span data-stu-id="65339-107">Windows 10 force update schedule for Apps</span></span>

## <a name="properties"></a><span data-ttu-id="65339-108">属性</span><span class="sxs-lookup"><span data-stu-id="65339-108">Properties</span></span>
|<span data-ttu-id="65339-109">属性</span><span class="sxs-lookup"><span data-stu-id="65339-109">Property</span></span>|<span data-ttu-id="65339-110">类型</span><span class="sxs-lookup"><span data-stu-id="65339-110">Type</span></span>|<span data-ttu-id="65339-111">说明</span><span class="sxs-lookup"><span data-stu-id="65339-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65339-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="65339-112">startDateTime</span></span>|<span data-ttu-id="65339-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65339-113">DateTimeOffset</span></span>|<span data-ttu-id="65339-114">强制重启的开始时间。</span><span class="sxs-lookup"><span data-stu-id="65339-114">The start time for the force restart.</span></span>|
|<span data-ttu-id="65339-115">定期</span><span class="sxs-lookup"><span data-stu-id="65339-115">recurrence</span></span>|[<span data-ttu-id="65339-116">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="65339-116">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="65339-117">定期计划。</span><span class="sxs-lookup"><span data-stu-id="65339-117">Recurrence schedule.</span></span> <span data-ttu-id="65339-118">可取值为：`none`、`daily`、`weekly`、`monthly`。</span><span class="sxs-lookup"><span data-stu-id="65339-118">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="65339-119">runImmediatelyIfAfterStartDateTime</span><span class="sxs-lookup"><span data-stu-id="65339-119">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="65339-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="65339-120">Boolean</span></span>|<span data-ttu-id="65339-121">如果为 true，则在 StartDateTime 为过去时立即运行任务，否则在下一个定期运行。</span><span class="sxs-lookup"><span data-stu-id="65339-121">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65339-122">关系</span><span class="sxs-lookup"><span data-stu-id="65339-122">Relationships</span></span>
<span data-ttu-id="65339-123">无</span><span class="sxs-lookup"><span data-stu-id="65339-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="65339-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="65339-124">JSON Representation</span></span>
<span data-ttu-id="65339-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65339-125">Here is a JSON representation of the resource.</span></span>
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






