---
title: plannerUser 资源类型
description: '**PlannerUser**资源的用户提供对计划工具资源的访问。 '
localization_priority: Normal
ms.openlocfilehash: 709b259c88d8fe0f02defaa57e77727a7b967cfd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820802"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="213f7-103">plannerUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="213f7-103">plannerUser resource type</span></span>

> <span data-ttu-id="213f7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="213f7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="213f7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="213f7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="213f7-106">**PlannerUser**资源提供了对计划工具资源的[用户](user.md)的访问。</span><span class="sxs-lookup"><span data-stu-id="213f7-106">The **plannerUser** resource provides access to Planner resources for a [user](user.md).</span></span> 


## <a name="methods"></a><span data-ttu-id="213f7-107">方法</span><span class="sxs-lookup"><span data-stu-id="213f7-107">Methods</span></span>

| <span data-ttu-id="213f7-108">方法</span><span class="sxs-lookup"><span data-stu-id="213f7-108">Method</span></span>           | <span data-ttu-id="213f7-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="213f7-109">Return Type</span></span>    |<span data-ttu-id="213f7-110">说明</span><span class="sxs-lookup"><span data-stu-id="213f7-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="213f7-111">List tasks</span><span class="sxs-lookup"><span data-stu-id="213f7-111">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="213f7-112">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="213f7-112">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="213f7-113">获取[plannerTasks](plannertask.md)分配给用户。</span><span class="sxs-lookup"><span data-stu-id="213f7-113">Get the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|[<span data-ttu-id="213f7-114">列表 favoritePlans</span><span class="sxs-lookup"><span data-stu-id="213f7-114">List favoritePlans</span></span>](../api/planneruser-list-favoriteplans.md) |<span data-ttu-id="213f7-115">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="213f7-115">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="213f7-116">获取用户标记为 favorite [plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="213f7-116">Get the [plannerPlans](plannerplan.md) marked as favorite by the user.</span></span>|
|[<span data-ttu-id="213f7-117">列表 recentPlans</span><span class="sxs-lookup"><span data-stu-id="213f7-117">List recentPlans</span></span>](../api/planneruser-list-recentplans.md) |<span data-ttu-id="213f7-118">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="213f7-118">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="213f7-119">获取由用户最近查看[plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="213f7-119">Get the [plannerPlans](plannerplan.md) recently viewed by the user.</span></span>|
|[<span data-ttu-id="213f7-120">Update</span><span class="sxs-lookup"><span data-stu-id="213f7-120">Update</span></span>](../api/planneruser-update.md) | [<span data-ttu-id="213f7-121">plannerUser</span><span class="sxs-lookup"><span data-stu-id="213f7-121">plannerUser</span></span>](planneruser.md)| <span data-ttu-id="213f7-122">更新**plannerUser**对象。</span><span class="sxs-lookup"><span data-stu-id="213f7-122">Update a **plannerUser** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="213f7-123">属性</span><span class="sxs-lookup"><span data-stu-id="213f7-123">Properties</span></span>
| <span data-ttu-id="213f7-124">属性</span><span class="sxs-lookup"><span data-stu-id="213f7-124">Property</span></span>     | <span data-ttu-id="213f7-125">类型</span><span class="sxs-lookup"><span data-stu-id="213f7-125">Type</span></span>   |<span data-ttu-id="213f7-126">说明</span><span class="sxs-lookup"><span data-stu-id="213f7-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="213f7-127">id</span><span class="sxs-lookup"><span data-stu-id="213f7-127">id</span></span>|<span data-ttu-id="213f7-128">String</span><span class="sxs-lookup"><span data-stu-id="213f7-128">String</span></span>| <span data-ttu-id="213f7-129">只读。</span><span class="sxs-lookup"><span data-stu-id="213f7-129">Read-only.</span></span> <span data-ttu-id="213f7-130">PlannerUser 的标识符</span><span class="sxs-lookup"><span data-stu-id="213f7-130">Identifier of the plannerUser</span></span>|
|<span data-ttu-id="213f7-131">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="213f7-131">favoritePlanReferences</span></span>|[<span data-ttu-id="213f7-132">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="213f7-132">plannerFavoritePlanReferenceCollection</span></span>](plannerfavoriteplanreferencecollection.md)| <span data-ttu-id="213f7-133">包含对用户已标记为收藏夹的计划的引用的集合。</span><span class="sxs-lookup"><span data-stu-id="213f7-133">A collection containing the references to the plans that the user has marked as favorites.</span></span>|
|<span data-ttu-id="213f7-134">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="213f7-134">recentPlanReferences</span></span>|[<span data-ttu-id="213f7-135">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="213f7-135">plannerRecentPlanReferenceCollection</span></span>](plannerrecentplanreferencecollection.md)| <span data-ttu-id="213f7-136">包含支持最新的计划的应用程序中的用户最近查看的计划对引用的集合。</span><span class="sxs-lookup"><span data-stu-id="213f7-136">A collection containing references to the plans that were viewed recently by the user in apps that support recent plans.</span></span>|

## <a name="relationships"></a><span data-ttu-id="213f7-137">Relationships</span><span class="sxs-lookup"><span data-stu-id="213f7-137">Relationships</span></span>
| <span data-ttu-id="213f7-138">关系</span><span class="sxs-lookup"><span data-stu-id="213f7-138">Relationship</span></span> | <span data-ttu-id="213f7-139">类型</span><span class="sxs-lookup"><span data-stu-id="213f7-139">Type</span></span>   |<span data-ttu-id="213f7-140">说明</span><span class="sxs-lookup"><span data-stu-id="213f7-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="213f7-141">tasks</span><span class="sxs-lookup"><span data-stu-id="213f7-141">tasks</span></span>|<span data-ttu-id="213f7-142">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="213f7-142">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="213f7-p103">只读。可为 NULL。返回分配给用户的 [plannerTasks](plannertask.md)。</span><span class="sxs-lookup"><span data-stu-id="213f7-p103">Read-only. Nullable. Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="213f7-146">favoritePlans</span><span class="sxs-lookup"><span data-stu-id="213f7-146">favoritePlans</span></span>|<span data-ttu-id="213f7-147">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="213f7-147">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="213f7-148">只读。</span><span class="sxs-lookup"><span data-stu-id="213f7-148">Read-only.</span></span> <span data-ttu-id="213f7-149">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="213f7-149">Nullable.</span></span> <span data-ttu-id="213f7-150">返回用户标记为收藏夹[plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="213f7-150">Returns the [plannerPlans](plannerplan.md) that the user marked as favorites.</span></span>|
|<span data-ttu-id="213f7-151">recentPlans</span><span class="sxs-lookup"><span data-stu-id="213f7-151">recentPlans</span></span>|<span data-ttu-id="213f7-152">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="213f7-152">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="213f7-153">只读。</span><span class="sxs-lookup"><span data-stu-id="213f7-153">Read-only.</span></span> <span data-ttu-id="213f7-154">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="213f7-154">Nullable.</span></span> <span data-ttu-id="213f7-155">返回支持最新的计划的应用程序中的用户最近查看[plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="213f7-155">Returns the [plannerPlans](plannerplan.md) that have been recently viewed by the user in apps that support recent plans.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="213f7-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="213f7-156">JSON representation</span></span>
<span data-ttu-id="213f7-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="213f7-157">The following is a JSON representation of the resource.</span></span>

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
