---
title: plannerRecentPlanReference 资源类型
description: '**plannerRecentPlanReference** 资源类型表示对最近由用户查看的 plannerPlan 的引用。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 8a8fbf3ce9f39c49dde4bbeee96a3aab15a00077
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720975"
---
# <a name="plannerrecentplanreference-resource-type"></a><span data-ttu-id="17430-103">plannerRecentPlanReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="17430-103">plannerRecentPlanReference resource type</span></span>

<span data-ttu-id="17430-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17430-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17430-105">**plannerRecentPlanReference** 资源类型表示对最近由用户查看的 [plannerPlan](plannerplan.md)的引用。</span><span class="sxs-lookup"><span data-stu-id="17430-105">The **plannerRecentPlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has recently been viewed by a user.</span></span> <span data-ttu-id="17430-106">**用户的 plannerRecentPlanReferences** 由应用显式维护。</span><span class="sxs-lookup"><span data-stu-id="17430-106">The **plannerRecentPlanReferences** for a user are explicitly maintained by apps.</span></span> <span data-ttu-id="17430-107">任何实现最近计划功能的应用都应记录用户上次查看计划时，并相应地更新 **plannerRecentPlanReference** 条目。</span><span class="sxs-lookup"><span data-stu-id="17430-107">Any app that implements the recent plans feature should record when the user last viewed a plan, and update **plannerRecentPlanReference** entries accordingly.</span></span>
<span data-ttu-id="17430-108">应用应注意 **plannerRecentPlanReference** 条目可以引用已删除、用户无法再访问或已使用其他标题更新的 **plannerPlans。**</span><span class="sxs-lookup"><span data-stu-id="17430-108">Apps should note that **plannerRecentPlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>
<span data-ttu-id="17430-109">我们建议应用在存在差异时通知用户，并保持条目最新。</span><span class="sxs-lookup"><span data-stu-id="17430-109">We recommend that apps notify users when there are discrepancies and keep the entries up to date.</span></span>

## <a name="properties"></a><span data-ttu-id="17430-110">属性</span><span class="sxs-lookup"><span data-stu-id="17430-110">Properties</span></span>
| <span data-ttu-id="17430-111">属性</span><span class="sxs-lookup"><span data-stu-id="17430-111">Property</span></span>     | <span data-ttu-id="17430-112">类型</span><span class="sxs-lookup"><span data-stu-id="17430-112">Type</span></span>   |<span data-ttu-id="17430-113">说明</span><span class="sxs-lookup"><span data-stu-id="17430-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17430-114">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="17430-114">lastAccessedDateTime</span></span>|<span data-ttu-id="17430-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17430-115">DateTimeOffset</span></span>|<span data-ttu-id="17430-116">用户上次查看计划的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="17430-116">The date and time the plan was last viewed by the user.</span></span> <span data-ttu-id="17430-117">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="17430-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="17430-118">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="17430-118">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="17430-119">planTitle</span><span class="sxs-lookup"><span data-stu-id="17430-119">planTitle</span></span>|<span data-ttu-id="17430-120">String</span><span class="sxs-lookup"><span data-stu-id="17430-120">String</span></span>|<span data-ttu-id="17430-121">用户查看计划时计划的标题。</span><span class="sxs-lookup"><span data-stu-id="17430-121">The title of the plan at the time the user viewed it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="17430-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="17430-122">JSON representation</span></span>

<span data-ttu-id="17430-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="17430-123">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->


