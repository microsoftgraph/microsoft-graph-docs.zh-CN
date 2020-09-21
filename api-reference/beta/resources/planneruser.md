---
title: plannerUser 资源类型
description: '**PlannerUser**资源为用户提供对 Planner 资源的访问权限。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 309f464afe33f09366f7905af7698660dd161094
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063968"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="50780-103">plannerUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="50780-103">plannerUser resource type</span></span>

<span data-ttu-id="50780-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50780-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50780-105">**PlannerUser**资源为[用户](user.md)提供对 Planner 资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="50780-105">The **plannerUser** resource provides access to Planner resources for a [user](user.md).</span></span> 


## <a name="methods"></a><span data-ttu-id="50780-106">方法</span><span class="sxs-lookup"><span data-stu-id="50780-106">Methods</span></span>

| <span data-ttu-id="50780-107">方法</span><span class="sxs-lookup"><span data-stu-id="50780-107">Method</span></span>           | <span data-ttu-id="50780-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="50780-108">Return Type</span></span>    |<span data-ttu-id="50780-109">说明</span><span class="sxs-lookup"><span data-stu-id="50780-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="50780-110">List tasks</span><span class="sxs-lookup"><span data-stu-id="50780-110">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="50780-111">[plannerTask](plannertask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="50780-111">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="50780-112">获取分配给用户的 [plannerTasks](plannertask.md) 。</span><span class="sxs-lookup"><span data-stu-id="50780-112">Get the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|[<span data-ttu-id="50780-113">列出 favoritePlans</span><span class="sxs-lookup"><span data-stu-id="50780-113">List favoritePlans</span></span>](../api/planneruser-list-favoriteplans.md) |<span data-ttu-id="50780-114">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="50780-114">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="50780-115">获取用户标记为收藏的 [plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="50780-115">Get the [plannerPlans](plannerplan.md) marked as favorite by the user.</span></span>|
|[<span data-ttu-id="50780-116">列出 recentPlans</span><span class="sxs-lookup"><span data-stu-id="50780-116">List recentPlans</span></span>](../api/planneruser-list-recentplans.md) |<span data-ttu-id="50780-117">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="50780-117">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="50780-118">获取用户最近查看过的 [plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="50780-118">Get the [plannerPlans](plannerplan.md) recently viewed by the user.</span></span>|
|[<span data-ttu-id="50780-119">更新</span><span class="sxs-lookup"><span data-stu-id="50780-119">Update</span></span>](../api/planneruser-update.md) | [<span data-ttu-id="50780-120">plannerUser</span><span class="sxs-lookup"><span data-stu-id="50780-120">plannerUser</span></span>](planneruser.md)| <span data-ttu-id="50780-121">更新 **plannerUser** 对象。</span><span class="sxs-lookup"><span data-stu-id="50780-121">Update a **plannerUser** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="50780-122">属性</span><span class="sxs-lookup"><span data-stu-id="50780-122">Properties</span></span>
| <span data-ttu-id="50780-123">属性</span><span class="sxs-lookup"><span data-stu-id="50780-123">Property</span></span>     | <span data-ttu-id="50780-124">类型</span><span class="sxs-lookup"><span data-stu-id="50780-124">Type</span></span>   |<span data-ttu-id="50780-125">说明</span><span class="sxs-lookup"><span data-stu-id="50780-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50780-126">id</span><span class="sxs-lookup"><span data-stu-id="50780-126">id</span></span>|<span data-ttu-id="50780-127">String</span><span class="sxs-lookup"><span data-stu-id="50780-127">String</span></span>| <span data-ttu-id="50780-128">只读。</span><span class="sxs-lookup"><span data-stu-id="50780-128">Read-only.</span></span> <span data-ttu-id="50780-129">PlannerUser 的标识符</span><span class="sxs-lookup"><span data-stu-id="50780-129">Identifier of the plannerUser</span></span>|
|<span data-ttu-id="50780-130">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="50780-130">favoritePlanReferences</span></span>|[<span data-ttu-id="50780-131">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="50780-131">plannerFavoritePlanReferenceCollection</span></span>](plannerfavoriteplanreferencecollection.md)| <span data-ttu-id="50780-132">包含对用户已标记为收藏夹的计划引用的集合。</span><span class="sxs-lookup"><span data-stu-id="50780-132">A collection containing the references to the plans that the user has marked as favorites.</span></span>|
|<span data-ttu-id="50780-133">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="50780-133">recentPlanReferences</span></span>|[<span data-ttu-id="50780-134">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="50780-134">plannerRecentPlanReferenceCollection</span></span>](plannerrecentplanreferencecollection.md)| <span data-ttu-id="50780-135">包含对计划的引用的集合，该用户最近在支持最近计划的应用程序中查看了这些计划。</span><span class="sxs-lookup"><span data-stu-id="50780-135">A collection containing references to the plans that were viewed recently by the user in apps that support recent plans.</span></span>|

## <a name="relationships"></a><span data-ttu-id="50780-136">关系</span><span class="sxs-lookup"><span data-stu-id="50780-136">Relationships</span></span>
| <span data-ttu-id="50780-137">关系</span><span class="sxs-lookup"><span data-stu-id="50780-137">Relationship</span></span> | <span data-ttu-id="50780-138">类型</span><span class="sxs-lookup"><span data-stu-id="50780-138">Type</span></span>   |<span data-ttu-id="50780-139">说明</span><span class="sxs-lookup"><span data-stu-id="50780-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50780-140">tasks</span><span class="sxs-lookup"><span data-stu-id="50780-140">tasks</span></span>|<span data-ttu-id="50780-141">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="50780-141">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="50780-142">只读。</span><span class="sxs-lookup"><span data-stu-id="50780-142">Read-only.</span></span> <span data-ttu-id="50780-143">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="50780-143">Nullable.</span></span> <span data-ttu-id="50780-144">返回分配给用户的 [plannerTasks](plannertask.md) 。</span><span class="sxs-lookup"><span data-stu-id="50780-144">Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="50780-145">favoritePlans</span><span class="sxs-lookup"><span data-stu-id="50780-145">favoritePlans</span></span>|<span data-ttu-id="50780-146">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="50780-146">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="50780-147">只读。</span><span class="sxs-lookup"><span data-stu-id="50780-147">Read-only.</span></span> <span data-ttu-id="50780-148">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="50780-148">Nullable.</span></span> <span data-ttu-id="50780-149">返回用户标记为收藏夹的 [plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="50780-149">Returns the [plannerPlans](plannerplan.md) that the user marked as favorites.</span></span>|
|<span data-ttu-id="50780-150">recentPlans</span><span class="sxs-lookup"><span data-stu-id="50780-150">recentPlans</span></span>|<span data-ttu-id="50780-151">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="50780-151">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="50780-152">只读。</span><span class="sxs-lookup"><span data-stu-id="50780-152">Read-only.</span></span> <span data-ttu-id="50780-153">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="50780-153">Nullable.</span></span> <span data-ttu-id="50780-154">返回用户最近在支持最近计划的应用程序中查看的 [plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="50780-154">Returns the [plannerPlans](plannerplan.md) that have been recently viewed by the user in apps that support recent plans.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="50780-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="50780-155">JSON representation</span></span>
<span data-ttu-id="50780-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50780-156">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
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
<!--
{
  "type": "#page.annotation",
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


