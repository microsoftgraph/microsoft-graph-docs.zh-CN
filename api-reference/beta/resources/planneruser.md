---
title: plannerUser 资源类型
description: '**plannerUser**资源为用户提供对 Planner 资源的访问权限。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: fd279e541df4b45e47d1c389d2e8a1e212b01a41
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344338"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="4f4bf-103">plannerUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="4f4bf-103">plannerUser resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f4bf-104">**plannerUser**资源为[用户](user.md)提供对 Planner 资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="4f4bf-104">The **plannerUser** resource provides access to Planner resources for a [user](user.md).</span></span> 


## <a name="methods"></a><span data-ttu-id="4f4bf-105">方法</span><span class="sxs-lookup"><span data-stu-id="4f4bf-105">Methods</span></span>

| <span data-ttu-id="4f4bf-106">方法</span><span class="sxs-lookup"><span data-stu-id="4f4bf-106">Method</span></span>           | <span data-ttu-id="4f4bf-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="4f4bf-107">Return Type</span></span>    |<span data-ttu-id="4f4bf-108">说明</span><span class="sxs-lookup"><span data-stu-id="4f4bf-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4f4bf-109">List tasks</span><span class="sxs-lookup"><span data-stu-id="4f4bf-109">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="4f4bf-110">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="4f4bf-110">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="4f4bf-111">获取分配给用户的[plannerTasks](plannertask.md) 。</span><span class="sxs-lookup"><span data-stu-id="4f4bf-111">Get the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|[<span data-ttu-id="4f4bf-112">列出 favoritePlans</span><span class="sxs-lookup"><span data-stu-id="4f4bf-112">List favoritePlans</span></span>](../api/planneruser-list-favoriteplans.md) |<span data-ttu-id="4f4bf-113">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4f4bf-113">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="4f4bf-114">获取用户标记为收藏的[plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="4f4bf-114">Get the [plannerPlans](plannerplan.md) marked as favorite by the user.</span></span>|
|[<span data-ttu-id="4f4bf-115">列出 recentPlans</span><span class="sxs-lookup"><span data-stu-id="4f4bf-115">List recentPlans</span></span>](../api/planneruser-list-recentplans.md) |<span data-ttu-id="4f4bf-116">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4f4bf-116">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="4f4bf-117">获取用户最近查看过的[plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="4f4bf-117">Get the [plannerPlans](plannerplan.md) recently viewed by the user.</span></span>|
|[<span data-ttu-id="4f4bf-118">更新</span><span class="sxs-lookup"><span data-stu-id="4f4bf-118">Update</span></span>](../api/planneruser-update.md) | [<span data-ttu-id="4f4bf-119">plannerUser</span><span class="sxs-lookup"><span data-stu-id="4f4bf-119">plannerUser</span></span>](planneruser.md)| <span data-ttu-id="4f4bf-120">更新**plannerUser**对象。</span><span class="sxs-lookup"><span data-stu-id="4f4bf-120">Update a **plannerUser** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="4f4bf-121">属性</span><span class="sxs-lookup"><span data-stu-id="4f4bf-121">Properties</span></span>
| <span data-ttu-id="4f4bf-122">属性</span><span class="sxs-lookup"><span data-stu-id="4f4bf-122">Property</span></span>     | <span data-ttu-id="4f4bf-123">类型</span><span class="sxs-lookup"><span data-stu-id="4f4bf-123">Type</span></span>   |<span data-ttu-id="4f4bf-124">说明</span><span class="sxs-lookup"><span data-stu-id="4f4bf-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4f4bf-125">id</span><span class="sxs-lookup"><span data-stu-id="4f4bf-125">id</span></span>|<span data-ttu-id="4f4bf-126">String</span><span class="sxs-lookup"><span data-stu-id="4f4bf-126">String</span></span>| <span data-ttu-id="4f4bf-127">只读。</span><span class="sxs-lookup"><span data-stu-id="4f4bf-127">Read-only.</span></span> <span data-ttu-id="4f4bf-128">plannerUser 的标识符</span><span class="sxs-lookup"><span data-stu-id="4f4bf-128">Identifier of the plannerUser</span></span>|
|<span data-ttu-id="4f4bf-129">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="4f4bf-129">favoritePlanReferences</span></span>|[<span data-ttu-id="4f4bf-130">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="4f4bf-130">plannerFavoritePlanReferenceCollection</span></span>](plannerfavoriteplanreferencecollection.md)| <span data-ttu-id="4f4bf-131">包含对用户已标记为收藏夹的计划引用的集合。</span><span class="sxs-lookup"><span data-stu-id="4f4bf-131">A collection containing the references to the plans that the user has marked as favorites.</span></span>|
|<span data-ttu-id="4f4bf-132">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="4f4bf-132">recentPlanReferences</span></span>|[<span data-ttu-id="4f4bf-133">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="4f4bf-133">plannerRecentPlanReferenceCollection</span></span>](plannerrecentplanreferencecollection.md)| <span data-ttu-id="4f4bf-134">包含对计划的引用的集合, 该用户最近在支持最近计划的应用程序中查看了这些计划。</span><span class="sxs-lookup"><span data-stu-id="4f4bf-134">A collection containing references to the plans that were viewed recently by the user in apps that support recent plans.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f4bf-135">关系</span><span class="sxs-lookup"><span data-stu-id="4f4bf-135">Relationships</span></span>
| <span data-ttu-id="4f4bf-136">关系</span><span class="sxs-lookup"><span data-stu-id="4f4bf-136">Relationship</span></span> | <span data-ttu-id="4f4bf-137">类型</span><span class="sxs-lookup"><span data-stu-id="4f4bf-137">Type</span></span>   |<span data-ttu-id="4f4bf-138">说明</span><span class="sxs-lookup"><span data-stu-id="4f4bf-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4f4bf-139">tasks</span><span class="sxs-lookup"><span data-stu-id="4f4bf-139">tasks</span></span>|<span data-ttu-id="4f4bf-140">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="4f4bf-140">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="4f4bf-141">只读。</span><span class="sxs-lookup"><span data-stu-id="4f4bf-141">Read-only.</span></span> <span data-ttu-id="4f4bf-142">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="4f4bf-142">Nullable.</span></span> <span data-ttu-id="4f4bf-143">返回分配给用户的[plannerTasks](plannertask.md) 。</span><span class="sxs-lookup"><span data-stu-id="4f4bf-143">Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="4f4bf-144">favoritePlans</span><span class="sxs-lookup"><span data-stu-id="4f4bf-144">favoritePlans</span></span>|<span data-ttu-id="4f4bf-145">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4f4bf-145">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="4f4bf-146">只读。</span><span class="sxs-lookup"><span data-stu-id="4f4bf-146">Read-only.</span></span> <span data-ttu-id="4f4bf-147">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="4f4bf-147">Nullable.</span></span> <span data-ttu-id="4f4bf-148">返回用户标记为收藏夹的[plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="4f4bf-148">Returns the [plannerPlans](plannerplan.md) that the user marked as favorites.</span></span>|
|<span data-ttu-id="4f4bf-149">recentPlans</span><span class="sxs-lookup"><span data-stu-id="4f4bf-149">recentPlans</span></span>|<span data-ttu-id="4f4bf-150">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4f4bf-150">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="4f4bf-151">只读。</span><span class="sxs-lookup"><span data-stu-id="4f4bf-151">Read-only.</span></span> <span data-ttu-id="4f4bf-152">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="4f4bf-152">Nullable.</span></span> <span data-ttu-id="4f4bf-153">返回用户最近在支持最近计划的应用程序中查看的[plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="4f4bf-153">Returns the [plannerPlans](plannerplan.md) that have been recently viewed by the user in apps that support recent plans.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4f4bf-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4f4bf-154">JSON representation</span></span>
<span data-ttu-id="4f4bf-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f4bf-155">The following is a JSON representation of the resource.</span></span>

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
