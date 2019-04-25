---
title: plannerUser 资源类型
description: '**plannerUser**资源为用户提供对 Planner 资源的访问权限。 它不包含任何可用属性。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: b73e422e232a96068f4545def0f0fdbd9f74ff07
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549823"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="f2cc5-104">plannerUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="f2cc5-104">plannerUser resource type</span></span>

<span data-ttu-id="f2cc5-105">**plannerUser**资源为[用户](user.md)提供对 Planner 资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="f2cc5-105">The **plannerUser** resource provide access to Planner resources for a [user](user.md).</span></span> <span data-ttu-id="f2cc5-106">它不包含任何可用属性。</span><span class="sxs-lookup"><span data-stu-id="f2cc5-106">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="f2cc5-107">方法</span><span class="sxs-lookup"><span data-stu-id="f2cc5-107">Methods</span></span>

| <span data-ttu-id="f2cc5-108">方法</span><span class="sxs-lookup"><span data-stu-id="f2cc5-108">Method</span></span>           | <span data-ttu-id="f2cc5-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="f2cc5-109">Return Type</span></span>    |<span data-ttu-id="f2cc5-110">说明</span><span class="sxs-lookup"><span data-stu-id="f2cc5-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f2cc5-111">列出计划</span><span class="sxs-lookup"><span data-stu-id="f2cc5-111">List plans</span></span>](../api/planneruser-list-plans.md) |<span data-ttu-id="f2cc5-112">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f2cc5-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="f2cc5-113">获取**plannerPlan**对象集合。</span><span class="sxs-lookup"><span data-stu-id="f2cc5-113">Get a **plannerPlan** object collection.</span></span>|
|[<span data-ttu-id="f2cc5-114">列出任务</span><span class="sxs-lookup"><span data-stu-id="f2cc5-114">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="f2cc5-115">[plannerTask](plannertask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f2cc5-115">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="f2cc5-116">获取**plannerTask**对象集合。</span><span class="sxs-lookup"><span data-stu-id="f2cc5-116">Get a **plannerTask** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="f2cc5-117">属性</span><span class="sxs-lookup"><span data-stu-id="f2cc5-117">Properties</span></span>
| <span data-ttu-id="f2cc5-118">属性</span><span class="sxs-lookup"><span data-stu-id="f2cc5-118">Property</span></span>     | <span data-ttu-id="f2cc5-119">类型</span><span class="sxs-lookup"><span data-stu-id="f2cc5-119">Type</span></span>   |<span data-ttu-id="f2cc5-120">说明</span><span class="sxs-lookup"><span data-stu-id="f2cc5-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2cc5-121">id</span><span class="sxs-lookup"><span data-stu-id="f2cc5-121">id</span></span>|<span data-ttu-id="f2cc5-122">String</span><span class="sxs-lookup"><span data-stu-id="f2cc5-122">String</span></span>| <span data-ttu-id="f2cc5-123">只读。</span><span class="sxs-lookup"><span data-stu-id="f2cc5-123">Read-only.</span></span> <span data-ttu-id="f2cc5-124">planenrUser 的标识符</span><span class="sxs-lookup"><span data-stu-id="f2cc5-124">Identifier of the planenrUser</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2cc5-125">关系</span><span class="sxs-lookup"><span data-stu-id="f2cc5-125">Relationships</span></span>
| <span data-ttu-id="f2cc5-126">关系</span><span class="sxs-lookup"><span data-stu-id="f2cc5-126">Relationship</span></span> | <span data-ttu-id="f2cc5-127">类型</span><span class="sxs-lookup"><span data-stu-id="f2cc5-127">Type</span></span>   |<span data-ttu-id="f2cc5-128">说明</span><span class="sxs-lookup"><span data-stu-id="f2cc5-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2cc5-129">计划</span><span class="sxs-lookup"><span data-stu-id="f2cc5-129">plans</span></span>|<span data-ttu-id="f2cc5-130">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f2cc5-130">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="f2cc5-131">只读。</span><span class="sxs-lookup"><span data-stu-id="f2cc5-131">Read-only.</span></span> <span data-ttu-id="f2cc5-132">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="f2cc5-132">Nullable.</span></span> <span data-ttu-id="f2cc5-133">返回分配给用户的[plannerTasks](plannertask.md) 。</span><span class="sxs-lookup"><span data-stu-id="f2cc5-133">Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="f2cc5-134">任务</span><span class="sxs-lookup"><span data-stu-id="f2cc5-134">tasks</span></span>|<span data-ttu-id="f2cc5-135">[plannerTask](plannertask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f2cc5-135">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="f2cc5-136">只读。</span><span class="sxs-lookup"><span data-stu-id="f2cc5-136">Read-only.</span></span> <span data-ttu-id="f2cc5-137">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="f2cc5-137">Nullable.</span></span> <span data-ttu-id="f2cc5-138">返回与用户共享的[plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="f2cc5-138">Returns the [plannerPlans](plannerplan.md) shared with the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f2cc5-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f2cc5-139">JSON representation</span></span>
<span data-ttu-id="f2cc5-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2cc5-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUser"
}-->

```json
{
  "id": "String (identifier)"
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
