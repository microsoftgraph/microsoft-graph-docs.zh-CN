---
title: windows10AppsForceUpdateSchedule 资源类型
description: Windows 10 强制更新计划程序
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 50793ee4ba26adc4b89cc8d36b3e8186debc402a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981985"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a><span data-ttu-id="f44f1-103">windows10AppsForceUpdateSchedule 资源类型</span><span class="sxs-lookup"><span data-stu-id="f44f1-103">windows10AppsForceUpdateSchedule resource type</span></span>

> <span data-ttu-id="f44f1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f44f1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f44f1-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f44f1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f44f1-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f44f1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f44f1-107">Windows 10 强制更新计划程序</span><span class="sxs-lookup"><span data-stu-id="f44f1-107">Windows 10 force update schedule for Apps</span></span>
## <a name="properties"></a><span data-ttu-id="f44f1-108">属性</span><span class="sxs-lookup"><span data-stu-id="f44f1-108">Properties</span></span>
|<span data-ttu-id="f44f1-109">属性</span><span class="sxs-lookup"><span data-stu-id="f44f1-109">Property</span></span>|<span data-ttu-id="f44f1-110">类型</span><span class="sxs-lookup"><span data-stu-id="f44f1-110">Type</span></span>|<span data-ttu-id="f44f1-111">说明</span><span class="sxs-lookup"><span data-stu-id="f44f1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f44f1-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f44f1-112">startDateTime</span></span>|<span data-ttu-id="f44f1-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f44f1-113">DateTimeOffset</span></span>|<span data-ttu-id="f44f1-114">强制的开始时间重新启动。</span><span class="sxs-lookup"><span data-stu-id="f44f1-114">The start time for the force restart.</span></span>|
|<span data-ttu-id="f44f1-115">recurrence</span><span class="sxs-lookup"><span data-stu-id="f44f1-115">recurrence</span></span>|[<span data-ttu-id="f44f1-116">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="f44f1-116">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="f44f1-117">定期计划。</span><span class="sxs-lookup"><span data-stu-id="f44f1-117">Recurrence schedule.</span></span> <span data-ttu-id="f44f1-118">可取值为：`none`、`daily`、`weekly`、`monthly`。</span><span class="sxs-lookup"><span data-stu-id="f44f1-118">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="f44f1-119">runImmediatelyIfAfterStartDateTime</span><span class="sxs-lookup"><span data-stu-id="f44f1-119">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="f44f1-120">布尔</span><span class="sxs-lookup"><span data-stu-id="f44f1-120">Boolean</span></span>|<span data-ttu-id="f44f1-121">如果为 true，请在过去，其他人，会在下一个定期运行开始日期时间是否立即运行任务。</span><span class="sxs-lookup"><span data-stu-id="f44f1-121">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f44f1-122">Relationships</span><span class="sxs-lookup"><span data-stu-id="f44f1-122">Relationships</span></span>
<span data-ttu-id="f44f1-123">无</span><span class="sxs-lookup"><span data-stu-id="f44f1-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f44f1-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f44f1-124">JSON Representation</span></span>
<span data-ttu-id="f44f1-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f44f1-125">Here is a JSON representation of the resource.</span></span>
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





