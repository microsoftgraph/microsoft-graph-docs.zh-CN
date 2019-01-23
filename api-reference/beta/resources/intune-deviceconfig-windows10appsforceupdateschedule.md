---
title: windows10AppsForceUpdateSchedule 资源类型
description: Windows 10 强制更新计划程序
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3e0bd9b0963f8547b03243aa7ef791a351dc2b08
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418832"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a><span data-ttu-id="28a24-103">windows10AppsForceUpdateSchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="28a24-103">windows10AppsForceUpdateSchedule resource type</span></span>

> <span data-ttu-id="28a24-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="28a24-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="28a24-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="28a24-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="28a24-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="28a24-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28a24-107">Windows 10 强制更新计划程序</span><span class="sxs-lookup"><span data-stu-id="28a24-107">Windows 10 force update schedule for Apps</span></span>

## <a name="properties"></a><span data-ttu-id="28a24-108">属性</span><span class="sxs-lookup"><span data-stu-id="28a24-108">Properties</span></span>
|<span data-ttu-id="28a24-109">属性</span><span class="sxs-lookup"><span data-stu-id="28a24-109">Property</span></span>|<span data-ttu-id="28a24-110">类型</span><span class="sxs-lookup"><span data-stu-id="28a24-110">Type</span></span>|<span data-ttu-id="28a24-111">说明</span><span class="sxs-lookup"><span data-stu-id="28a24-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28a24-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="28a24-112">startDateTime</span></span>|<span data-ttu-id="28a24-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28a24-113">DateTimeOffset</span></span>|<span data-ttu-id="28a24-114">强制的开始时间重新启动。</span><span class="sxs-lookup"><span data-stu-id="28a24-114">The start time for the force restart.</span></span>|
|<span data-ttu-id="28a24-115">recurrence</span><span class="sxs-lookup"><span data-stu-id="28a24-115">recurrence</span></span>|[<span data-ttu-id="28a24-116">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="28a24-116">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="28a24-117">定期计划。</span><span class="sxs-lookup"><span data-stu-id="28a24-117">Recurrence schedule.</span></span> <span data-ttu-id="28a24-118">可取值为：`none`、`daily`、`weekly`、`monthly`。</span><span class="sxs-lookup"><span data-stu-id="28a24-118">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="28a24-119">runImmediatelyIfAfterStartDateTime</span><span class="sxs-lookup"><span data-stu-id="28a24-119">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="28a24-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="28a24-120">Boolean</span></span>|<span data-ttu-id="28a24-121">如果为 true，请在过去，其他人，会在下一个定期运行开始日期时间是否立即运行任务。</span><span class="sxs-lookup"><span data-stu-id="28a24-121">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="28a24-122">关系</span><span class="sxs-lookup"><span data-stu-id="28a24-122">Relationships</span></span>
<span data-ttu-id="28a24-123">无</span><span class="sxs-lookup"><span data-stu-id="28a24-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="28a24-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="28a24-124">JSON Representation</span></span>
<span data-ttu-id="28a24-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28a24-125">Here is a JSON representation of the resource.</span></span>
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




