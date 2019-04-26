---
title: plannerUser 资源类型
description: '**plannerUser**资源为用户提供对 Planner 资源的访问权限。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 1f10810f6debf2346ed12484bac8e1f4bfd2f372
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563651"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="f59ed-103">plannerUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="f59ed-103">plannerUser resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f59ed-104">**plannerUser**资源为[用户](user.md)提供对 Planner 资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="f59ed-104">The **plannerUser** resource provides access to Planner resources for a [user](user.md).</span></span> 


## <a name="methods"></a><span data-ttu-id="f59ed-105">方法</span><span class="sxs-lookup"><span data-stu-id="f59ed-105">Methods</span></span>

| <span data-ttu-id="f59ed-106">方法</span><span class="sxs-lookup"><span data-stu-id="f59ed-106">Method</span></span>           | <span data-ttu-id="f59ed-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="f59ed-107">Return Type</span></span>    |<span data-ttu-id="f59ed-108">说明</span><span class="sxs-lookup"><span data-stu-id="f59ed-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f59ed-109">列出任务</span><span class="sxs-lookup"><span data-stu-id="f59ed-109">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="f59ed-110">[plannerTask](plannertask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f59ed-110">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="f59ed-111">获取分配给用户的[plannerTasks](plannertask.md) 。</span><span class="sxs-lookup"><span data-stu-id="f59ed-111">Get the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|[<span data-ttu-id="f59ed-112">列出 favoritePlans</span><span class="sxs-lookup"><span data-stu-id="f59ed-112">List favoritePlans</span></span>](../api/planneruser-list-favoriteplans.md) |<span data-ttu-id="f59ed-113">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f59ed-113">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="f59ed-114">获取用户标记为收藏的[plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="f59ed-114">Get the [plannerPlans](plannerplan.md) marked as favorite by the user.</span></span>|
|[<span data-ttu-id="f59ed-115">列出 recentPlans</span><span class="sxs-lookup"><span data-stu-id="f59ed-115">List recentPlans</span></span>](../api/planneruser-list-recentplans.md) |<span data-ttu-id="f59ed-116">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f59ed-116">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="f59ed-117">获取用户最近查看过的[plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="f59ed-117">Get the [plannerPlans](plannerplan.md) recently viewed by the user.</span></span>|
|[<span data-ttu-id="f59ed-118">更新</span><span class="sxs-lookup"><span data-stu-id="f59ed-118">Update</span></span>](../api/planneruser-update.md) | [<span data-ttu-id="f59ed-119">plannerUser</span><span class="sxs-lookup"><span data-stu-id="f59ed-119">plannerUser</span></span>](planneruser.md)| <span data-ttu-id="f59ed-120">更新**plannerUser**对象。</span><span class="sxs-lookup"><span data-stu-id="f59ed-120">Update a **plannerUser** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="f59ed-121">属性</span><span class="sxs-lookup"><span data-stu-id="f59ed-121">Properties</span></span>
| <span data-ttu-id="f59ed-122">属性</span><span class="sxs-lookup"><span data-stu-id="f59ed-122">Property</span></span>     | <span data-ttu-id="f59ed-123">类型</span><span class="sxs-lookup"><span data-stu-id="f59ed-123">Type</span></span>   |<span data-ttu-id="f59ed-124">说明</span><span class="sxs-lookup"><span data-stu-id="f59ed-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f59ed-125">id</span><span class="sxs-lookup"><span data-stu-id="f59ed-125">id</span></span>|<span data-ttu-id="f59ed-126">String</span><span class="sxs-lookup"><span data-stu-id="f59ed-126">String</span></span>| <span data-ttu-id="f59ed-127">只读。</span><span class="sxs-lookup"><span data-stu-id="f59ed-127">Read-only.</span></span> <span data-ttu-id="f59ed-128">plannerUser 的标识符</span><span class="sxs-lookup"><span data-stu-id="f59ed-128">Identifier of the plannerUser</span></span>|
|<span data-ttu-id="f59ed-129">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="f59ed-129">favoritePlanReferences</span></span>|[<span data-ttu-id="f59ed-130">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="f59ed-130">plannerFavoritePlanReferenceCollection</span></span>](plannerfavoriteplanreferencecollection.md)| <span data-ttu-id="f59ed-131">包含对用户已标记为收藏夹的计划引用的集合。</span><span class="sxs-lookup"><span data-stu-id="f59ed-131">A collection containing the references to the plans that the user has marked as favorites.</span></span>|
|<span data-ttu-id="f59ed-132">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="f59ed-132">recentPlanReferences</span></span>|[<span data-ttu-id="f59ed-133">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="f59ed-133">plannerRecentPlanReferenceCollection</span></span>](plannerrecentplanreferencecollection.md)| <span data-ttu-id="f59ed-134">包含对计划的引用的集合, 该用户最近在支持最近计划的应用程序中查看了这些计划。</span><span class="sxs-lookup"><span data-stu-id="f59ed-134">A collection containing references to the plans that were viewed recently by the user in apps that support recent plans.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f59ed-135">关系</span><span class="sxs-lookup"><span data-stu-id="f59ed-135">Relationships</span></span>
| <span data-ttu-id="f59ed-136">关系</span><span class="sxs-lookup"><span data-stu-id="f59ed-136">Relationship</span></span> | <span data-ttu-id="f59ed-137">类型</span><span class="sxs-lookup"><span data-stu-id="f59ed-137">Type</span></span>   |<span data-ttu-id="f59ed-138">说明</span><span class="sxs-lookup"><span data-stu-id="f59ed-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f59ed-139">任务</span><span class="sxs-lookup"><span data-stu-id="f59ed-139">tasks</span></span>|<span data-ttu-id="f59ed-140">[plannerTask](plannertask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f59ed-140">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="f59ed-141">只读。</span><span class="sxs-lookup"><span data-stu-id="f59ed-141">Read-only.</span></span> <span data-ttu-id="f59ed-142">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="f59ed-142">Nullable.</span></span> <span data-ttu-id="f59ed-143">返回分配给用户的[plannerTasks](plannertask.md) 。</span><span class="sxs-lookup"><span data-stu-id="f59ed-143">Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="f59ed-144">favoritePlans</span><span class="sxs-lookup"><span data-stu-id="f59ed-144">favoritePlans</span></span>|<span data-ttu-id="f59ed-145">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f59ed-145">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="f59ed-146">只读。</span><span class="sxs-lookup"><span data-stu-id="f59ed-146">Read-only.</span></span> <span data-ttu-id="f59ed-147">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="f59ed-147">Nullable.</span></span> <span data-ttu-id="f59ed-148">返回用户标记为收藏夹的[plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="f59ed-148">Returns the [plannerPlans](plannerplan.md) that the user marked as favorites.</span></span>|
|<span data-ttu-id="f59ed-149">recentPlans</span><span class="sxs-lookup"><span data-stu-id="f59ed-149">recentPlans</span></span>|<span data-ttu-id="f59ed-150">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f59ed-150">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="f59ed-151">只读。</span><span class="sxs-lookup"><span data-stu-id="f59ed-151">Read-only.</span></span> <span data-ttu-id="f59ed-152">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="f59ed-152">Nullable.</span></span> <span data-ttu-id="f59ed-153">返回用户最近在支持最近计划的应用程序中查看的[plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="f59ed-153">Returns the [plannerPlans](plannerplan.md) that have been recently viewed by the user in apps that support recent plans.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f59ed-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f59ed-154">JSON representation</span></span>
<span data-ttu-id="f59ed-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f59ed-155">The following is a JSON representation of the resource.</span></span>

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
