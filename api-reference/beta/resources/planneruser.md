---
title: plannerUser 资源类型
description: '**PlannerUser**资源为用户提供对 Planner 资源的访问权限。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 70ca7596cfb809a16b76f684a85c97b0c3e43a50
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521634"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="045d7-103">plannerUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="045d7-103">plannerUser resource type</span></span>

<span data-ttu-id="045d7-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="045d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="045d7-105">**PlannerUser**资源为[用户](user.md)提供对 Planner 资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="045d7-105">The **plannerUser** resource provides access to Planner resources for a [user](user.md).</span></span> 


## <a name="methods"></a><span data-ttu-id="045d7-106">方法</span><span class="sxs-lookup"><span data-stu-id="045d7-106">Methods</span></span>

| <span data-ttu-id="045d7-107">方法</span><span class="sxs-lookup"><span data-stu-id="045d7-107">Method</span></span>           | <span data-ttu-id="045d7-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="045d7-108">Return Type</span></span>    |<span data-ttu-id="045d7-109">说明</span><span class="sxs-lookup"><span data-stu-id="045d7-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="045d7-110">List tasks</span><span class="sxs-lookup"><span data-stu-id="045d7-110">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="045d7-111">[plannerTask](plannertask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="045d7-111">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="045d7-112">获取分配给用户的[plannerTasks](plannertask.md) 。</span><span class="sxs-lookup"><span data-stu-id="045d7-112">Get the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|[<span data-ttu-id="045d7-113">列出 favoritePlans</span><span class="sxs-lookup"><span data-stu-id="045d7-113">List favoritePlans</span></span>](../api/planneruser-list-favoriteplans.md) |<span data-ttu-id="045d7-114">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="045d7-114">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="045d7-115">获取用户标记为收藏的[plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="045d7-115">Get the [plannerPlans](plannerplan.md) marked as favorite by the user.</span></span>|
|[<span data-ttu-id="045d7-116">列出 recentPlans</span><span class="sxs-lookup"><span data-stu-id="045d7-116">List recentPlans</span></span>](../api/planneruser-list-recentplans.md) |<span data-ttu-id="045d7-117">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="045d7-117">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="045d7-118">获取用户最近查看过的[plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="045d7-118">Get the [plannerPlans](plannerplan.md) recently viewed by the user.</span></span>|
|[<span data-ttu-id="045d7-119">更新</span><span class="sxs-lookup"><span data-stu-id="045d7-119">Update</span></span>](../api/planneruser-update.md) | [<span data-ttu-id="045d7-120">plannerUser</span><span class="sxs-lookup"><span data-stu-id="045d7-120">plannerUser</span></span>](planneruser.md)| <span data-ttu-id="045d7-121">更新**plannerUser**对象。</span><span class="sxs-lookup"><span data-stu-id="045d7-121">Update a **plannerUser** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="045d7-122">属性</span><span class="sxs-lookup"><span data-stu-id="045d7-122">Properties</span></span>
| <span data-ttu-id="045d7-123">属性</span><span class="sxs-lookup"><span data-stu-id="045d7-123">Property</span></span>     | <span data-ttu-id="045d7-124">类型</span><span class="sxs-lookup"><span data-stu-id="045d7-124">Type</span></span>   |<span data-ttu-id="045d7-125">说明</span><span class="sxs-lookup"><span data-stu-id="045d7-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="045d7-126">id</span><span class="sxs-lookup"><span data-stu-id="045d7-126">id</span></span>|<span data-ttu-id="045d7-127">String</span><span class="sxs-lookup"><span data-stu-id="045d7-127">String</span></span>| <span data-ttu-id="045d7-128">只读。</span><span class="sxs-lookup"><span data-stu-id="045d7-128">Read-only.</span></span> <span data-ttu-id="045d7-129">PlannerUser 的标识符</span><span class="sxs-lookup"><span data-stu-id="045d7-129">Identifier of the plannerUser</span></span>|
|<span data-ttu-id="045d7-130">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="045d7-130">favoritePlanReferences</span></span>|[<span data-ttu-id="045d7-131">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="045d7-131">plannerFavoritePlanReferenceCollection</span></span>](plannerfavoriteplanreferencecollection.md)| <span data-ttu-id="045d7-132">包含对用户已标记为收藏夹的计划引用的集合。</span><span class="sxs-lookup"><span data-stu-id="045d7-132">A collection containing the references to the plans that the user has marked as favorites.</span></span>|
|<span data-ttu-id="045d7-133">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="045d7-133">recentPlanReferences</span></span>|[<span data-ttu-id="045d7-134">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="045d7-134">plannerRecentPlanReferenceCollection</span></span>](plannerrecentplanreferencecollection.md)| <span data-ttu-id="045d7-135">包含对计划的引用的集合，该用户最近在支持最近计划的应用程序中查看了这些计划。</span><span class="sxs-lookup"><span data-stu-id="045d7-135">A collection containing references to the plans that were viewed recently by the user in apps that support recent plans.</span></span>|

## <a name="relationships"></a><span data-ttu-id="045d7-136">关系</span><span class="sxs-lookup"><span data-stu-id="045d7-136">Relationships</span></span>
| <span data-ttu-id="045d7-137">关系</span><span class="sxs-lookup"><span data-stu-id="045d7-137">Relationship</span></span> | <span data-ttu-id="045d7-138">类型</span><span class="sxs-lookup"><span data-stu-id="045d7-138">Type</span></span>   |<span data-ttu-id="045d7-139">说明</span><span class="sxs-lookup"><span data-stu-id="045d7-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="045d7-140">tasks</span><span class="sxs-lookup"><span data-stu-id="045d7-140">tasks</span></span>|<span data-ttu-id="045d7-141">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="045d7-141">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="045d7-142">只读。</span><span class="sxs-lookup"><span data-stu-id="045d7-142">Read-only.</span></span> <span data-ttu-id="045d7-143">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="045d7-143">Nullable.</span></span> <span data-ttu-id="045d7-144">返回分配给用户的[plannerTasks](plannertask.md) 。</span><span class="sxs-lookup"><span data-stu-id="045d7-144">Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="045d7-145">favoritePlans</span><span class="sxs-lookup"><span data-stu-id="045d7-145">favoritePlans</span></span>|<span data-ttu-id="045d7-146">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="045d7-146">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="045d7-147">只读。</span><span class="sxs-lookup"><span data-stu-id="045d7-147">Read-only.</span></span> <span data-ttu-id="045d7-148">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="045d7-148">Nullable.</span></span> <span data-ttu-id="045d7-149">返回用户标记为收藏夹的[plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="045d7-149">Returns the [plannerPlans](plannerplan.md) that the user marked as favorites.</span></span>|
|<span data-ttu-id="045d7-150">recentPlans</span><span class="sxs-lookup"><span data-stu-id="045d7-150">recentPlans</span></span>|<span data-ttu-id="045d7-151">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="045d7-151">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="045d7-152">只读。</span><span class="sxs-lookup"><span data-stu-id="045d7-152">Read-only.</span></span> <span data-ttu-id="045d7-153">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="045d7-153">Nullable.</span></span> <span data-ttu-id="045d7-154">返回用户最近在支持最近计划的应用程序中查看的[plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="045d7-154">Returns the [plannerPlans](plannerplan.md) that have been recently viewed by the user in apps that support recent plans.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="045d7-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="045d7-155">JSON representation</span></span>
<span data-ttu-id="045d7-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="045d7-156">The following is a JSON representation of the resource.</span></span>

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
