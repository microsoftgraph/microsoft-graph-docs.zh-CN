---
title: plannerRecentPlanReference 资源类型
description: '**plannerRecentPlanReference**资源类型代表一个对用户最近查看过的 plannerPlan 的引用。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 55ccf34055d7d181dbbeecd5b6c30a3843f211d5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522151"
---
# <a name="plannerrecentplanreference-resource-type"></a><span data-ttu-id="7f4c5-103">plannerRecentPlanReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="7f4c5-103">plannerRecentPlanReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f4c5-104">**plannerRecentPlanReference**资源类型代表一个对用户最近查看过的[plannerPlan](plannerplan.md)的引用。</span><span class="sxs-lookup"><span data-stu-id="7f4c5-104">The **plannerRecentPlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has recently been viewed by a user.</span></span> <span data-ttu-id="7f4c5-105">用户的**plannerRecentPlanReferences**由应用程序显式维护。</span><span class="sxs-lookup"><span data-stu-id="7f4c5-105">The **plannerRecentPlanReferences** for a user are explicitly maintained by apps.</span></span> <span data-ttu-id="7f4c5-106">任何实现最近计划功能的应用程序都应记录用户上次查看计划的时间, 并相应地更新**plannerRecentPlanReference**项。</span><span class="sxs-lookup"><span data-stu-id="7f4c5-106">Any app that implements the recent plans feature should record when the user last viewed a plan, and update **plannerRecentPlanReference** entries accordingly.</span></span>
<span data-ttu-id="7f4c5-107">应用应注意, **plannerRecentPlanReference**条目可以引用已删除的**plannerPlans** 、用户无法再访问或已使用其他标题进行更新。</span><span class="sxs-lookup"><span data-stu-id="7f4c5-107">Apps should note that **plannerRecentPlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>
<span data-ttu-id="7f4c5-108">我们建议应用在存在差异时通知用户, 并将这些条目保持为最新。</span><span class="sxs-lookup"><span data-stu-id="7f4c5-108">We recommend that apps notify users when there are discrepancies and keep the entries up to date.</span></span>

## <a name="properties"></a><span data-ttu-id="7f4c5-109">属性</span><span class="sxs-lookup"><span data-stu-id="7f4c5-109">Properties</span></span>
| <span data-ttu-id="7f4c5-110">属性</span><span class="sxs-lookup"><span data-stu-id="7f4c5-110">Property</span></span>     | <span data-ttu-id="7f4c5-111">类型</span><span class="sxs-lookup"><span data-stu-id="7f4c5-111">Type</span></span>   |<span data-ttu-id="7f4c5-112">说明</span><span class="sxs-lookup"><span data-stu-id="7f4c5-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f4c5-113">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f4c5-113">lastAccessedDateTime</span></span>|<span data-ttu-id="7f4c5-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f4c5-114">DateTimeOffset</span></span>|<span data-ttu-id="7f4c5-115">用户上次查看计划的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="7f4c5-115">The date and time the plan was last viewed by the user.</span></span> <span data-ttu-id="7f4c5-116">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="7f4c5-116">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7f4c5-117">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="7f4c5-117">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="7f4c5-118">planTitle</span><span class="sxs-lookup"><span data-stu-id="7f4c5-118">planTitle</span></span>|<span data-ttu-id="7f4c5-119">String</span><span class="sxs-lookup"><span data-stu-id="7f4c5-119">String</span></span>|<span data-ttu-id="7f4c5-120">用户查看计划时的标题。</span><span class="sxs-lookup"><span data-stu-id="7f4c5-120">The title of the plan at the time the user viewed it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7f4c5-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7f4c5-121">JSON representation</span></span>

<span data-ttu-id="7f4c5-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7f4c5-122">The following is a JSON representation of the resource.</span></span>

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
