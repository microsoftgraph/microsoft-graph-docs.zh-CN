---
title: plannerPlanContext 资源类型
description: '**PlannerPlanContext**资源表示 PlannerPlan 在计划程序外的用户体验的关系。 Planner 中的计划可以在其他体验（如 Microsoft 团队）中进行，以在该体验的上下文中跟踪工作。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: c1163843cdb393363bbb30783aa8232aa67544ca
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979336"
---
# <a name="plannerplancontext-resource-type"></a><span data-ttu-id="67519-104">plannerPlanContext 资源类型</span><span class="sxs-lookup"><span data-stu-id="67519-104">plannerPlanContext resource type</span></span>

<span data-ttu-id="67519-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67519-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67519-106">**PlannerPlanContext**资源表示[plannerPlan](plannerplan.md)在计划程序外的用户体验的关系。</span><span class="sxs-lookup"><span data-stu-id="67519-106">The **plannerPlanContext** resource represents the relationship of a [plannerPlan](plannerplan.md) to a user experience outside of Planner.</span></span> <span data-ttu-id="67519-107">Planner 中的计划可以在其他体验（如 Microsoft 团队）中进行，以在该体验的上下文中跟踪工作。</span><span class="sxs-lookup"><span data-stu-id="67519-107">Plans in Planner can be surfaced in other experiences, such as Microsoft Teams, to track work in the context of that experience.</span></span>
<span data-ttu-id="67519-108">可以基于**ownerAppId**属性来标识**plannerPlanContext**条目 reresents 的体验：</span><span class="sxs-lookup"><span data-stu-id="67519-108">The experience the **plannerPlanContext** entry reresents can be identified based on the **ownerAppId** property:</span></span>
- <span data-ttu-id="67519-109">5e3ce6c0-2b1f-4285-8d4b-75ee78787346：上下文条目属于 Microsoft 团队。</span><span class="sxs-lookup"><span data-stu-id="67519-109">5e3ce6c0-2b1f-4285-8d4b-75ee78787346 : The context entry belongs to Microsoft Teams.</span></span>
- <span data-ttu-id="67519-110">为00000003-0000-0ff1-ce00-000000000000：上下文条目属于 SharePoint。</span><span class="sxs-lookup"><span data-stu-id="67519-110">00000003-0000-0ff1-ce00-000000000000 : The context entry belongs to SharePoint.</span></span>

## <a name="properties"></a><span data-ttu-id="67519-111">属性</span><span class="sxs-lookup"><span data-stu-id="67519-111">Properties</span></span>
| <span data-ttu-id="67519-112">属性</span><span class="sxs-lookup"><span data-stu-id="67519-112">Property</span></span>     | <span data-ttu-id="67519-113">类型</span><span class="sxs-lookup"><span data-stu-id="67519-113">Type</span></span>   |<span data-ttu-id="67519-114">说明</span><span class="sxs-lookup"><span data-stu-id="67519-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67519-115">associationType</span><span class="sxs-lookup"><span data-stu-id="67519-115">associationType</span></span>|<span data-ttu-id="67519-116">String</span><span class="sxs-lookup"><span data-stu-id="67519-116">String</span></span>|<span data-ttu-id="67519-117">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="67519-117">Nullable.</span></span> <span data-ttu-id="67519-118">[PlannerPlan](plannerplan.md)与应用之间的应用程序定义类型的关联。</span><span class="sxs-lookup"><span data-stu-id="67519-118">An app-defined type of association between the [plannerPlan](plannerplan.md) and the app.</span></span> <span data-ttu-id="67519-119">应用程序可以使用此信息跟踪与同一 [plannerPlan](plannerplan.md)的不同类型的关系。</span><span class="sxs-lookup"><span data-stu-id="67519-119">The app can use this information to track different kinds of relationships to the same [plannerPlan](plannerplan.md).</span></span>|
|<span data-ttu-id="67519-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="67519-120">createdDateTime</span></span>|<span data-ttu-id="67519-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67519-121">DateTimeOffset</span></span>|<span data-ttu-id="67519-122">只读。</span><span class="sxs-lookup"><span data-stu-id="67519-122">Read-only.</span></span> <span data-ttu-id="67519-123">**PlannerPlanContext**的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="67519-123">The date and time when the **plannerPlanContext** was created.</span></span> <span data-ttu-id="67519-124">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="67519-124">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="67519-125">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="67519-125">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="67519-126">displayNameSegments</span><span class="sxs-lookup"><span data-stu-id="67519-126">displayNameSegments</span></span>|<span data-ttu-id="67519-127">String collection</span><span class="sxs-lookup"><span data-stu-id="67519-127">String collection</span></span>|<span data-ttu-id="67519-128">外部体验名称的各个部分。</span><span class="sxs-lookup"><span data-stu-id="67519-128">The segments of the name of the external experience.</span></span> <span data-ttu-id="67519-129">段表示允许其他应用显示关系的层次结构。</span><span class="sxs-lookup"><span data-stu-id="67519-129">Segments represent a hierarchical structure that allows other apps to display the relationship.</span></span>|
|<span data-ttu-id="67519-130">ownerAppId</span><span class="sxs-lookup"><span data-stu-id="67519-130">ownerAppId</span></span>|<span data-ttu-id="67519-131">String</span><span class="sxs-lookup"><span data-stu-id="67519-131">String</span></span>|<span data-ttu-id="67519-132">只读。</span><span class="sxs-lookup"><span data-stu-id="67519-132">Read-only.</span></span> <span data-ttu-id="67519-133">创建 **plannerPlanContext**的应用程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="67519-133">ID of the app that created the **plannerPlanContext**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="67519-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="67519-134">JSON representation</span></span>

<span data-ttu-id="67519-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="67519-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContext"
}-->

```json
{
  "associationType": "Board",
  "createdDateTime": "2015-10-14T00:57:28.4698344Z",
  "displayNameSegments": [
    "Finance Team",
    "Budget Plans"
  ],
  "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContext resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


