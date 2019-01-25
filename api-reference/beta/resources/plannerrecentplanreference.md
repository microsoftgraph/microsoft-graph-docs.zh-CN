---
title: plannerRecentPlanReference 资源类型
description: '**PlannerRecentPlanReference**资源类型代表最近已由用户查看 plannerPlan 的引用。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 55ccf34055d7d181dbbeecd5b6c30a3843f211d5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509159"
---
# <a name="plannerrecentplanreference-resource-type"></a><span data-ttu-id="613f2-103">plannerRecentPlanReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="613f2-103">plannerRecentPlanReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="613f2-104">**PlannerRecentPlanReference**资源类型代表最近已由用户查看[plannerPlan](plannerplan.md)的引用。</span><span class="sxs-lookup"><span data-stu-id="613f2-104">The **plannerRecentPlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has recently been viewed by a user.</span></span> <span data-ttu-id="613f2-105">**PlannerRecentPlanReferences**用户明确维护应用程序中。</span><span class="sxs-lookup"><span data-stu-id="613f2-105">The **plannerRecentPlanReferences** for a user are explicitly maintained by apps.</span></span> <span data-ttu-id="613f2-106">用户上次查看的计划和更新**plannerRecentPlanReference**条目相应时，应记录实现最新的计划功能任何应用程序。</span><span class="sxs-lookup"><span data-stu-id="613f2-106">Any app that implements the recent plans feature should record when the user last viewed a plan, and update **plannerRecentPlanReference** entries accordingly.</span></span>
<span data-ttu-id="613f2-107">应用程序应注意**plannerRecentPlanReference**条目可以引用**plannerPlans**的被删除，用户不再可以访问，或已更新具有不同的标题。</span><span class="sxs-lookup"><span data-stu-id="613f2-107">Apps should note that **plannerRecentPlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>
<span data-ttu-id="613f2-108">建议的应用程序差异时通知用户，并保持最新条目。</span><span class="sxs-lookup"><span data-stu-id="613f2-108">We recommend that apps notify users when there are discrepancies and keep the entries up to date.</span></span>

## <a name="properties"></a><span data-ttu-id="613f2-109">属性</span><span class="sxs-lookup"><span data-stu-id="613f2-109">Properties</span></span>
| <span data-ttu-id="613f2-110">属性</span><span class="sxs-lookup"><span data-stu-id="613f2-110">Property</span></span>     | <span data-ttu-id="613f2-111">类型</span><span class="sxs-lookup"><span data-stu-id="613f2-111">Type</span></span>   |<span data-ttu-id="613f2-112">说明</span><span class="sxs-lookup"><span data-stu-id="613f2-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="613f2-113">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="613f2-113">lastAccessedDateTime</span></span>|<span data-ttu-id="613f2-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="613f2-114">DateTimeOffset</span></span>|<span data-ttu-id="613f2-115">日期和时间计划上次查看的用户。</span><span class="sxs-lookup"><span data-stu-id="613f2-115">The date and time the plan was last viewed by the user.</span></span> <span data-ttu-id="613f2-116">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="613f2-116">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="613f2-117">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="613f2-117">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="613f2-118">planTitle</span><span class="sxs-lookup"><span data-stu-id="613f2-118">planTitle</span></span>|<span data-ttu-id="613f2-119">String</span><span class="sxs-lookup"><span data-stu-id="613f2-119">String</span></span>|<span data-ttu-id="613f2-120">标题时计划的用户查看它。</span><span class="sxs-lookup"><span data-stu-id="613f2-120">The title of the plan at the time the user viewed it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="613f2-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="613f2-121">JSON representation</span></span>

<span data-ttu-id="613f2-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="613f2-122">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerRecentPlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerrecentplanreference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
