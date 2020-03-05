---
title: plannerUser 资源类型
description: '**PlannerUser**资源为用户提供对 Planner 资源的访问权限。 它不包含任何可用属性。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 49b8989bd8526cbe8074a386ae31e76fd195642d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447092"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="02bb5-104">plannerUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="02bb5-104">plannerUser resource type</span></span>

<span data-ttu-id="02bb5-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="02bb5-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="02bb5-106">**PlannerUser**资源为[用户](user.md)提供对 Planner 资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="02bb5-106">The **plannerUser** resource provide access to Planner resources for a [user](user.md).</span></span> <span data-ttu-id="02bb5-107">它不包含任何可用属性。</span><span class="sxs-lookup"><span data-stu-id="02bb5-107">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="02bb5-108">方法</span><span class="sxs-lookup"><span data-stu-id="02bb5-108">Methods</span></span>

| <span data-ttu-id="02bb5-109">方法</span><span class="sxs-lookup"><span data-stu-id="02bb5-109">Method</span></span>           | <span data-ttu-id="02bb5-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="02bb5-110">Return Type</span></span>    |<span data-ttu-id="02bb5-111">说明</span><span class="sxs-lookup"><span data-stu-id="02bb5-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="02bb5-112">列出计划</span><span class="sxs-lookup"><span data-stu-id="02bb5-112">List plans</span></span>](../api/planneruser-list-plans.md) |<span data-ttu-id="02bb5-113">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="02bb5-113">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="02bb5-114">获取**plannerPlan**对象集合。</span><span class="sxs-lookup"><span data-stu-id="02bb5-114">Get a **plannerPlan** object collection.</span></span>|
|[<span data-ttu-id="02bb5-115">List tasks</span><span class="sxs-lookup"><span data-stu-id="02bb5-115">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="02bb5-116">[plannerTask](plannertask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="02bb5-116">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="02bb5-117">获取 **plannerTask** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="02bb5-117">Get a **plannerTask** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="02bb5-118">属性</span><span class="sxs-lookup"><span data-stu-id="02bb5-118">Properties</span></span>
| <span data-ttu-id="02bb5-119">属性</span><span class="sxs-lookup"><span data-stu-id="02bb5-119">Property</span></span>     | <span data-ttu-id="02bb5-120">类型</span><span class="sxs-lookup"><span data-stu-id="02bb5-120">Type</span></span>   |<span data-ttu-id="02bb5-121">说明</span><span class="sxs-lookup"><span data-stu-id="02bb5-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02bb5-122">id</span><span class="sxs-lookup"><span data-stu-id="02bb5-122">id</span></span>|<span data-ttu-id="02bb5-123">String</span><span class="sxs-lookup"><span data-stu-id="02bb5-123">String</span></span>| <span data-ttu-id="02bb5-124">只读。</span><span class="sxs-lookup"><span data-stu-id="02bb5-124">Read-only.</span></span> <span data-ttu-id="02bb5-125">PlanenrUser 的标识符</span><span class="sxs-lookup"><span data-stu-id="02bb5-125">Identifier of the planenrUser</span></span>|

## <a name="relationships"></a><span data-ttu-id="02bb5-126">关系</span><span class="sxs-lookup"><span data-stu-id="02bb5-126">Relationships</span></span>
| <span data-ttu-id="02bb5-127">关系</span><span class="sxs-lookup"><span data-stu-id="02bb5-127">Relationship</span></span> | <span data-ttu-id="02bb5-128">类型</span><span class="sxs-lookup"><span data-stu-id="02bb5-128">Type</span></span>   |<span data-ttu-id="02bb5-129">说明</span><span class="sxs-lookup"><span data-stu-id="02bb5-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02bb5-130">计划</span><span class="sxs-lookup"><span data-stu-id="02bb5-130">plans</span></span>|<span data-ttu-id="02bb5-131">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="02bb5-131">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="02bb5-132">只读。</span><span class="sxs-lookup"><span data-stu-id="02bb5-132">Read-only.</span></span> <span data-ttu-id="02bb5-133">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="02bb5-133">Nullable.</span></span> <span data-ttu-id="02bb5-134">返回分配给用户的[plannerTasks](plannertask.md) 。</span><span class="sxs-lookup"><span data-stu-id="02bb5-134">Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="02bb5-135">tasks</span><span class="sxs-lookup"><span data-stu-id="02bb5-135">tasks</span></span>|<span data-ttu-id="02bb5-136">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="02bb5-136">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="02bb5-137">只读。</span><span class="sxs-lookup"><span data-stu-id="02bb5-137">Read-only.</span></span> <span data-ttu-id="02bb5-138">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="02bb5-138">Nullable.</span></span> <span data-ttu-id="02bb5-139">返回与用户共享的[plannerPlans](plannerplan.md) 。</span><span class="sxs-lookup"><span data-stu-id="02bb5-139">Returns the [plannerPlans](plannerplan.md) shared with the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="02bb5-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="02bb5-140">JSON representation</span></span>
<span data-ttu-id="02bb5-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="02bb5-141">Here is a JSON representation of the resource.</span></span>

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
