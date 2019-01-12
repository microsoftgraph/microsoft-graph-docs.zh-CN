---
title: plannerRecentPlanReference 资源类型
description: '**PlannerRecentPlanReference**资源类型代表最近已由用户查看 plannerPlan 的引用。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: bafaf6d20dc8f64ffe49eb4e2f998607708a2773
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943525"
---
# <a name="plannerrecentplanreference-resource-type"></a><span data-ttu-id="a64cd-103">plannerRecentPlanReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="a64cd-103">plannerRecentPlanReference resource type</span></span>

> <span data-ttu-id="a64cd-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a64cd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a64cd-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a64cd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a64cd-106">**PlannerRecentPlanReference**资源类型代表最近已由用户查看[plannerPlan](plannerplan.md)的引用。</span><span class="sxs-lookup"><span data-stu-id="a64cd-106">The **plannerRecentPlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has recently been viewed by a user.</span></span> <span data-ttu-id="a64cd-107">**PlannerRecentPlanReferences**用户明确维护应用程序中。</span><span class="sxs-lookup"><span data-stu-id="a64cd-107">The **plannerRecentPlanReferences** for a user are explicitly maintained by apps.</span></span> <span data-ttu-id="a64cd-108">用户上次查看的计划和更新**plannerRecentPlanReference**条目相应时，应记录实现最新的计划功能任何应用程序。</span><span class="sxs-lookup"><span data-stu-id="a64cd-108">Any app that implements the recent plans feature should record when the user last viewed a plan, and update **plannerRecentPlanReference** entries accordingly.</span></span>
<span data-ttu-id="a64cd-109">应用程序应注意**plannerRecentPlanReference**条目可以引用**plannerPlans**的被删除，用户不再可以访问，或已更新具有不同的标题。</span><span class="sxs-lookup"><span data-stu-id="a64cd-109">Apps should note that **plannerRecentPlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>
<span data-ttu-id="a64cd-110">建议的应用程序差异时通知用户，并保持最新条目。</span><span class="sxs-lookup"><span data-stu-id="a64cd-110">We recommend that apps notify users when there are discrepancies and keep the entries up to date.</span></span>

## <a name="properties"></a><span data-ttu-id="a64cd-111">属性</span><span class="sxs-lookup"><span data-stu-id="a64cd-111">Properties</span></span>
| <span data-ttu-id="a64cd-112">属性</span><span class="sxs-lookup"><span data-stu-id="a64cd-112">Property</span></span>     | <span data-ttu-id="a64cd-113">类型</span><span class="sxs-lookup"><span data-stu-id="a64cd-113">Type</span></span>   |<span data-ttu-id="a64cd-114">Description</span><span class="sxs-lookup"><span data-stu-id="a64cd-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a64cd-115">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="a64cd-115">lastAccessedDateTime</span></span>|<span data-ttu-id="a64cd-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a64cd-116">DateTimeOffset</span></span>|<span data-ttu-id="a64cd-117">日期和时间计划上次查看的用户。</span><span class="sxs-lookup"><span data-stu-id="a64cd-117">The date and time the plan was last viewed by the user.</span></span> <span data-ttu-id="a64cd-118">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="a64cd-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a64cd-119">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="a64cd-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="a64cd-120">planTitle</span><span class="sxs-lookup"><span data-stu-id="a64cd-120">planTitle</span></span>|<span data-ttu-id="a64cd-121">字符串</span><span class="sxs-lookup"><span data-stu-id="a64cd-121">String</span></span>|<span data-ttu-id="a64cd-122">标题时计划的用户查看它。</span><span class="sxs-lookup"><span data-stu-id="a64cd-122">The title of the plan at the time the user viewed it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a64cd-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a64cd-123">JSON representation</span></span>

<span data-ttu-id="a64cd-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a64cd-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerRecentPlanReference"
}-->

```json
{
  "lastAccessedDateTime": "String (timestamp)",
  "planTitle": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerRecentPlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
