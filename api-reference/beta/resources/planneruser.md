---
title: plannerUser 资源类型
description: '**PlannerUser**资源的用户提供对计划工具资源的访问。 '
ms.openlocfilehash: 592a26daacd1bd6d0a780ca0180d3ec5a57b6eb1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045566"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="c52f8-103">plannerUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="c52f8-103">plannerUser resource type</span></span>

> <span data-ttu-id="c52f8-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c52f8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c52f8-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c52f8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c52f8-106">**PlannerUser**资源提供了对计划工具资源的[用户](user.md)的访问。</span><span class="sxs-lookup"><span data-stu-id="c52f8-106">The **plannerUser** resource provides access to Planner resources for a [user](user.md).</span></span> 


## <a name="methods"></a><span data-ttu-id="c52f8-107">方法</span><span class="sxs-lookup"><span data-stu-id="c52f8-107">Methods</span></span>

| <span data-ttu-id="c52f8-108">方法</span><span class="sxs-lookup"><span data-stu-id="c52f8-108">Method</span></span>           | <span data-ttu-id="c52f8-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="c52f8-109">Return Type</span></span>    |<span data-ttu-id="c52f8-110">说明</span><span class="sxs-lookup"><span data-stu-id="c52f8-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c52f8-111">List tasks</span><span class="sxs-lookup"><span data-stu-id="c52f8-111">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="c52f8-112">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="c52f8-112">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="c52f8-113">获取[plannerTasks](plannertask.md)分配给用户。</span><span class="sxs-lookup"><span data-stu-id="c52f8-113">Get the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|[<span data-ttu-id="c52f8-114">列表 favoritePlans</span><span class="sxs-lookup"><span data-stu-id="c52f8-114">List favoritePlans</span></span>](../api/planneruser-list-favoriteplans.md) |<span data-ttu-id="c52f8-115">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c52f8-115">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="c52f8-116">获取用户标记为 favorite [plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="c52f8-116">Get the [plannerPlans](plannerplan.md) marked as favorite by the user.</span></span>|
|[<span data-ttu-id="c52f8-117">列表 recentPlans</span><span class="sxs-lookup"><span data-stu-id="c52f8-117">List recentPlans</span></span>](../api/planneruser-list-recentplans.md) |<span data-ttu-id="c52f8-118">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c52f8-118">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="c52f8-119">获取由用户最近查看[plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="c52f8-119">Get the [plannerPlans](plannerplan.md) recently viewed by the user.</span></span>|
|[<span data-ttu-id="c52f8-120">Update</span><span class="sxs-lookup"><span data-stu-id="c52f8-120">Update</span></span>](../api/planneruser-update.md) | [<span data-ttu-id="c52f8-121">plannerUser</span><span class="sxs-lookup"><span data-stu-id="c52f8-121">plannerUser</span></span>](planneruser.md)| <span data-ttu-id="c52f8-122">更新**plannerUser**对象。</span><span class="sxs-lookup"><span data-stu-id="c52f8-122">Update a **plannerUser** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="c52f8-123">属性</span><span class="sxs-lookup"><span data-stu-id="c52f8-123">Properties</span></span>
| <span data-ttu-id="c52f8-124">属性</span><span class="sxs-lookup"><span data-stu-id="c52f8-124">Property</span></span>     | <span data-ttu-id="c52f8-125">类型</span><span class="sxs-lookup"><span data-stu-id="c52f8-125">Type</span></span>   |<span data-ttu-id="c52f8-126">说明</span><span class="sxs-lookup"><span data-stu-id="c52f8-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c52f8-127">id</span><span class="sxs-lookup"><span data-stu-id="c52f8-127">id</span></span>|<span data-ttu-id="c52f8-128">String</span><span class="sxs-lookup"><span data-stu-id="c52f8-128">String</span></span>| <span data-ttu-id="c52f8-129">只读。</span><span class="sxs-lookup"><span data-stu-id="c52f8-129">Read-only.</span></span> <span data-ttu-id="c52f8-130">PlannerUser 的标识符</span><span class="sxs-lookup"><span data-stu-id="c52f8-130">Identifier of the plannerUser</span></span>|
|<span data-ttu-id="c52f8-131">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="c52f8-131">favoritePlanReferences</span></span>|[<span data-ttu-id="c52f8-132">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="c52f8-132">plannerFavoritePlanReferenceCollection</span></span>](plannerfavoriteplanreferencecollection.md)| <span data-ttu-id="c52f8-133">包含对用户已标记为收藏夹的计划的引用的集合。</span><span class="sxs-lookup"><span data-stu-id="c52f8-133">A collection containing the references to the plans that the user has marked as favorites.</span></span>|
|<span data-ttu-id="c52f8-134">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="c52f8-134">recentPlanReferences</span></span>|[<span data-ttu-id="c52f8-135">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="c52f8-135">plannerRecentPlanReferenceCollection</span></span>](plannerrecentplanreferencecollection.md)| <span data-ttu-id="c52f8-136">包含支持最新的计划的应用程序中的用户最近查看的计划对引用的集合。</span><span class="sxs-lookup"><span data-stu-id="c52f8-136">A collection containing references to the plans that were viewed recently by the user in apps that support recent plans.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c52f8-137">Relationships</span><span class="sxs-lookup"><span data-stu-id="c52f8-137">Relationships</span></span>
| <span data-ttu-id="c52f8-138">关系</span><span class="sxs-lookup"><span data-stu-id="c52f8-138">Relationship</span></span> | <span data-ttu-id="c52f8-139">类型</span><span class="sxs-lookup"><span data-stu-id="c52f8-139">Type</span></span>   |<span data-ttu-id="c52f8-140">说明</span><span class="sxs-lookup"><span data-stu-id="c52f8-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c52f8-141">tasks</span><span class="sxs-lookup"><span data-stu-id="c52f8-141">tasks</span></span>|<span data-ttu-id="c52f8-142">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="c52f8-142">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="c52f8-p103">只读。可为 NULL。返回分配给用户的 [plannerTasks](plannertask.md)。</span><span class="sxs-lookup"><span data-stu-id="c52f8-p103">Read-only. Nullable. Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="c52f8-146">favoritePlans</span><span class="sxs-lookup"><span data-stu-id="c52f8-146">favoritePlans</span></span>|<span data-ttu-id="c52f8-147">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c52f8-147">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="c52f8-148">只读。</span><span class="sxs-lookup"><span data-stu-id="c52f8-148">Read-only.</span></span> <span data-ttu-id="c52f8-149">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="c52f8-149">Nullable.</span></span> <span data-ttu-id="c52f8-150">返回用户标记为收藏夹[plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="c52f8-150">Returns the [plannerPlans](plannerplan.md) that the user marked as favorites.</span></span>|
|<span data-ttu-id="c52f8-151">recentPlans</span><span class="sxs-lookup"><span data-stu-id="c52f8-151">recentPlans</span></span>|<span data-ttu-id="c52f8-152">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c52f8-152">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="c52f8-153">只读。</span><span class="sxs-lookup"><span data-stu-id="c52f8-153">Read-only.</span></span> <span data-ttu-id="c52f8-154">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="c52f8-154">Nullable.</span></span> <span data-ttu-id="c52f8-155">返回支持最新的计划的应用程序中的用户最近查看[plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="c52f8-155">Returns the [plannerPlans](plannerplan.md) that have been recently viewed by the user in apps that support recent plans.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c52f8-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c52f8-156">JSON representation</span></span>
<span data-ttu-id="c52f8-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c52f8-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUser"
}-->

```json
{
  "favoritePlanReferences": {"@odata.type": "microsoft.graph.plannerFavoritePlanReferenceCollection"},
  "id": "String (identifier)",
  "recentPlanReferences": {"@odata.type": "microsoft.graph.plannerRecentPlanReferenceCollection"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
