---
title: plannerUser 资源类型
description: '**PlannerUser**资源的用户提供对计划工具资源的访问。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 1f10810f6debf2346ed12484bac8e1f4bfd2f372
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526877"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="975a8-103">plannerUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="975a8-103">plannerUser resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="975a8-104">**PlannerUser**资源提供了对计划工具资源的[用户](user.md)的访问。</span><span class="sxs-lookup"><span data-stu-id="975a8-104">The **plannerUser** resource provides access to Planner resources for a [user](user.md).</span></span> 


## <a name="methods"></a><span data-ttu-id="975a8-105">方法</span><span class="sxs-lookup"><span data-stu-id="975a8-105">Methods</span></span>

| <span data-ttu-id="975a8-106">方法</span><span class="sxs-lookup"><span data-stu-id="975a8-106">Method</span></span>           | <span data-ttu-id="975a8-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="975a8-107">Return Type</span></span>    |<span data-ttu-id="975a8-108">说明</span><span class="sxs-lookup"><span data-stu-id="975a8-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="975a8-109">List tasks</span><span class="sxs-lookup"><span data-stu-id="975a8-109">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="975a8-110">[plannerTask](plannertask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="975a8-110">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="975a8-111">获取[plannerTasks](plannertask.md)分配给用户。</span><span class="sxs-lookup"><span data-stu-id="975a8-111">Get the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|[<span data-ttu-id="975a8-112">列表 favoritePlans</span><span class="sxs-lookup"><span data-stu-id="975a8-112">List favoritePlans</span></span>](../api/planneruser-list-favoriteplans.md) |<span data-ttu-id="975a8-113">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="975a8-113">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="975a8-114">获取用户标记为 favorite [plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="975a8-114">Get the [plannerPlans](plannerplan.md) marked as favorite by the user.</span></span>|
|[<span data-ttu-id="975a8-115">列表 recentPlans</span><span class="sxs-lookup"><span data-stu-id="975a8-115">List recentPlans</span></span>](../api/planneruser-list-recentplans.md) |<span data-ttu-id="975a8-116">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="975a8-116">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="975a8-117">获取由用户最近查看[plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="975a8-117">Get the [plannerPlans](plannerplan.md) recently viewed by the user.</span></span>|
|[<span data-ttu-id="975a8-118">Update</span><span class="sxs-lookup"><span data-stu-id="975a8-118">Update</span></span>](../api/planneruser-update.md) | [<span data-ttu-id="975a8-119">plannerUser</span><span class="sxs-lookup"><span data-stu-id="975a8-119">plannerUser</span></span>](planneruser.md)| <span data-ttu-id="975a8-120">更新**plannerUser**对象。</span><span class="sxs-lookup"><span data-stu-id="975a8-120">Update a **plannerUser** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="975a8-121">属性</span><span class="sxs-lookup"><span data-stu-id="975a8-121">Properties</span></span>
| <span data-ttu-id="975a8-122">属性</span><span class="sxs-lookup"><span data-stu-id="975a8-122">Property</span></span>     | <span data-ttu-id="975a8-123">类型</span><span class="sxs-lookup"><span data-stu-id="975a8-123">Type</span></span>   |<span data-ttu-id="975a8-124">说明</span><span class="sxs-lookup"><span data-stu-id="975a8-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="975a8-125">id</span><span class="sxs-lookup"><span data-stu-id="975a8-125">id</span></span>|<span data-ttu-id="975a8-126">String</span><span class="sxs-lookup"><span data-stu-id="975a8-126">String</span></span>| <span data-ttu-id="975a8-127">只读。</span><span class="sxs-lookup"><span data-stu-id="975a8-127">Read-only.</span></span> <span data-ttu-id="975a8-128">PlannerUser 的标识符</span><span class="sxs-lookup"><span data-stu-id="975a8-128">Identifier of the plannerUser</span></span>|
|<span data-ttu-id="975a8-129">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="975a8-129">favoritePlanReferences</span></span>|[<span data-ttu-id="975a8-130">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="975a8-130">plannerFavoritePlanReferenceCollection</span></span>](plannerfavoriteplanreferencecollection.md)| <span data-ttu-id="975a8-131">包含对用户已标记为收藏夹的计划的引用的集合。</span><span class="sxs-lookup"><span data-stu-id="975a8-131">A collection containing the references to the plans that the user has marked as favorites.</span></span>|
|<span data-ttu-id="975a8-132">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="975a8-132">recentPlanReferences</span></span>|[<span data-ttu-id="975a8-133">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="975a8-133">plannerRecentPlanReferenceCollection</span></span>](plannerrecentplanreferencecollection.md)| <span data-ttu-id="975a8-134">包含支持最新的计划的应用程序中的用户最近查看的计划对引用的集合。</span><span class="sxs-lookup"><span data-stu-id="975a8-134">A collection containing references to the plans that were viewed recently by the user in apps that support recent plans.</span></span>|

## <a name="relationships"></a><span data-ttu-id="975a8-135">关系</span><span class="sxs-lookup"><span data-stu-id="975a8-135">Relationships</span></span>
| <span data-ttu-id="975a8-136">关系</span><span class="sxs-lookup"><span data-stu-id="975a8-136">Relationship</span></span> | <span data-ttu-id="975a8-137">类型</span><span class="sxs-lookup"><span data-stu-id="975a8-137">Type</span></span>   |<span data-ttu-id="975a8-138">说明</span><span class="sxs-lookup"><span data-stu-id="975a8-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="975a8-139">tasks</span><span class="sxs-lookup"><span data-stu-id="975a8-139">tasks</span></span>|<span data-ttu-id="975a8-140">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="975a8-140">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="975a8-p102">只读。可为 NULL。返回分配给用户的 [plannerTasks](plannertask.md)。</span><span class="sxs-lookup"><span data-stu-id="975a8-p102">Read-only. Nullable. Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="975a8-144">favoritePlans</span><span class="sxs-lookup"><span data-stu-id="975a8-144">favoritePlans</span></span>|<span data-ttu-id="975a8-145">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="975a8-145">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="975a8-146">只读。</span><span class="sxs-lookup"><span data-stu-id="975a8-146">Read-only.</span></span> <span data-ttu-id="975a8-147">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="975a8-147">Nullable.</span></span> <span data-ttu-id="975a8-148">返回用户标记为收藏夹[plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="975a8-148">Returns the [plannerPlans](plannerplan.md) that the user marked as favorites.</span></span>|
|<span data-ttu-id="975a8-149">recentPlans</span><span class="sxs-lookup"><span data-stu-id="975a8-149">recentPlans</span></span>|<span data-ttu-id="975a8-150">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="975a8-150">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="975a8-151">只读。</span><span class="sxs-lookup"><span data-stu-id="975a8-151">Read-only.</span></span> <span data-ttu-id="975a8-152">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="975a8-152">Nullable.</span></span> <span data-ttu-id="975a8-153">返回支持最新的计划的应用程序中的用户最近查看[plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="975a8-153">Returns the [plannerPlans](plannerplan.md) that have been recently viewed by the user in apps that support recent plans.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="975a8-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="975a8-154">JSON representation</span></span>
<span data-ttu-id="975a8-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="975a8-155">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/planneruser.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
