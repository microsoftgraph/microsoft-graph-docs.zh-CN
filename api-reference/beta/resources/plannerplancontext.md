---
title: plannerPlanContext 资源类型
description: '**plannerPlanContext** 资源表示 plannerPlan 与 Planner 之外的用户体验的关系。 Planner 中的计划可以显示在其他体验（如 Microsoft Teams）中，以跟踪该体验上下文中的工作。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: f8a3b82c35339bb8bc6b3d3d7923b41ed97ecc02
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720982"
---
# <a name="plannerplancontext-resource-type"></a><span data-ttu-id="0864e-104">plannerPlanContext 资源类型</span><span class="sxs-lookup"><span data-stu-id="0864e-104">plannerPlanContext resource type</span></span>

<span data-ttu-id="0864e-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0864e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0864e-106">**plannerPlanContext** 资源表示 [plannerPlan](plannerplan.md)与 Planner 之外的用户体验的关系。</span><span class="sxs-lookup"><span data-stu-id="0864e-106">The **plannerPlanContext** resource represents the relationship of a [plannerPlan](plannerplan.md) to a user experience outside of Planner.</span></span> <span data-ttu-id="0864e-107">Planner 中的计划可以显示在其他体验（如 Microsoft Teams）中，以跟踪该体验上下文中的工作。</span><span class="sxs-lookup"><span data-stu-id="0864e-107">Plans in Planner can be surfaced in other experiences, such as Microsoft Teams, to track work in the context of that experience.</span></span> <span data-ttu-id="0864e-108">[plannerPlanContextDetails](plannerplancontextdetails.md)中具有外部链接的体验可以显示在用户界面中，从而允许用户访问这些体验。</span><span class="sxs-lookup"><span data-stu-id="0864e-108">Experiences that have external links in the [plannerPlanContextDetails](plannerplancontextdetails.md) can be displayed in a user interface, allowing users to visit these experiences.</span></span>


## <a name="properties"></a><span data-ttu-id="0864e-109">属性</span><span class="sxs-lookup"><span data-stu-id="0864e-109">Properties</span></span>
| <span data-ttu-id="0864e-110">属性</span><span class="sxs-lookup"><span data-stu-id="0864e-110">Property</span></span>     | <span data-ttu-id="0864e-111">类型</span><span class="sxs-lookup"><span data-stu-id="0864e-111">Type</span></span>   |<span data-ttu-id="0864e-112">说明</span><span class="sxs-lookup"><span data-stu-id="0864e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0864e-113">associationType</span><span class="sxs-lookup"><span data-stu-id="0864e-113">associationType</span></span>|<span data-ttu-id="0864e-114">String</span><span class="sxs-lookup"><span data-stu-id="0864e-114">String</span></span>|<span data-ttu-id="0864e-115">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="0864e-115">Nullable.</span></span> <span data-ttu-id="0864e-116">plannerPlan 与应用之间的应用定义的关联[](plannerplan.md)类型。</span><span class="sxs-lookup"><span data-stu-id="0864e-116">An app-defined type of association between the [plannerPlan](plannerplan.md) and the app.</span></span> <span data-ttu-id="0864e-117">应用可以使用此信息跟踪与同一 [plannerPlan 的不同类型的关系](plannerplan.md)。</span><span class="sxs-lookup"><span data-stu-id="0864e-117">The app can use this information to track different kinds of relationships to the same [plannerPlan](plannerplan.md).</span></span>|
|<span data-ttu-id="0864e-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0864e-118">createdDateTime</span></span>|<span data-ttu-id="0864e-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0864e-119">DateTimeOffset</span></span>|<span data-ttu-id="0864e-120">只读。</span><span class="sxs-lookup"><span data-stu-id="0864e-120">Read-only.</span></span> <span data-ttu-id="0864e-121">创建 **plannerPlanContext 的** 日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0864e-121">The date and time when the **plannerPlanContext** was created.</span></span> <span data-ttu-id="0864e-122">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="0864e-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0864e-123">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="0864e-123">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="0864e-124">displayNameSegments</span><span class="sxs-lookup"><span data-stu-id="0864e-124">displayNameSegments</span></span>|<span data-ttu-id="0864e-125">字符串集合</span><span class="sxs-lookup"><span data-stu-id="0864e-125">String collection</span></span>|<span data-ttu-id="0864e-126">外部体验名称的段。</span><span class="sxs-lookup"><span data-stu-id="0864e-126">The segments of the name of the external experience.</span></span> <span data-ttu-id="0864e-127">分段表示允许其他应用显示关系的分层结构。</span><span class="sxs-lookup"><span data-stu-id="0864e-127">Segments represent a hierarchical structure that allows other apps to display the relationship.</span></span>|
|<span data-ttu-id="0864e-128">isCreationContext</span><span class="sxs-lookup"><span data-stu-id="0864e-128">isCreationContext</span></span>|<span data-ttu-id="0864e-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="0864e-129">Boolean</span></span>|<span data-ttu-id="0864e-130">只读。</span><span class="sxs-lookup"><span data-stu-id="0864e-130">Read-only.</span></span> <span data-ttu-id="0864e-131">指示是否从指定上下文创建计划。</span><span class="sxs-lookup"><span data-stu-id="0864e-131">Indicates whether the plan is created from the specified context.</span></span> <span data-ttu-id="0864e-132">根据上下文是否指定为计划创建一部分而自动生成。</span><span class="sxs-lookup"><span data-stu-id="0864e-132">Auto-generated based on whether the context is specified as part of plan creation.</span></span>|
|<span data-ttu-id="0864e-133">ownerAppId</span><span class="sxs-lookup"><span data-stu-id="0864e-133">ownerAppId</span></span>|<span data-ttu-id="0864e-134">String</span><span class="sxs-lookup"><span data-stu-id="0864e-134">String</span></span>|<span data-ttu-id="0864e-135">只读。</span><span class="sxs-lookup"><span data-stu-id="0864e-135">Read-only.</span></span> <span data-ttu-id="0864e-136">创建 **plannerPlanContext** 的应用的 ID。</span><span class="sxs-lookup"><span data-stu-id="0864e-136">ID of the app that created the **plannerPlanContext**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0864e-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0864e-137">JSON representation</span></span>

<span data-ttu-id="0864e-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0864e-138">The following is a JSON representation of the resource.</span></span>

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
  "isCreationContext": false,
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


