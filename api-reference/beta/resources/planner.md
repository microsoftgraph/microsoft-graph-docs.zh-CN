---
title: planner 资源类型
description: '**planner**资源是 planner 对象模型的入口点。 它返回单一实例**planner**资源。  它不包含任何可用属性。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 2f1fb3b7058a87dd7b8390408590371cf1b0e9cd
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344616"
---
# <a name="planner-resource-type"></a><span data-ttu-id="1e34d-105">planner 资源类型</span><span class="sxs-lookup"><span data-stu-id="1e34d-105">planner resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e34d-106">**planner**资源是 planner 对象模型的入口点。</span><span class="sxs-lookup"><span data-stu-id="1e34d-106">The **planner** resource is the entry point for the Planner object model.</span></span> <span data-ttu-id="1e34d-107">它返回单一实例**planner**资源。</span><span class="sxs-lookup"><span data-stu-id="1e34d-107">It returns a singleton **planner** resource.</span></span>  <span data-ttu-id="1e34d-108">它不包含任何可用属性。</span><span class="sxs-lookup"><span data-stu-id="1e34d-108">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="1e34d-109">方法</span><span class="sxs-lookup"><span data-stu-id="1e34d-109">Methods</span></span>

| <span data-ttu-id="1e34d-110">方法</span><span class="sxs-lookup"><span data-stu-id="1e34d-110">Method</span></span>           | <span data-ttu-id="1e34d-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="1e34d-111">Return Type</span></span>    |<span data-ttu-id="1e34d-112">说明</span><span class="sxs-lookup"><span data-stu-id="1e34d-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1e34d-113">创建 plannerBucket</span><span class="sxs-lookup"><span data-stu-id="1e34d-113">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="1e34d-114">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="1e34d-114">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="1e34d-115">通过发布到存储桶集合创建新的**plannerBucket** 。</span><span class="sxs-lookup"><span data-stu-id="1e34d-115">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="1e34d-116">创建 plannerPlan</span><span class="sxs-lookup"><span data-stu-id="1e34d-116">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="1e34d-117">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="1e34d-117">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="1e34d-118">通过发布到计划集合创建新的**plannerPlan** 。</span><span class="sxs-lookup"><span data-stu-id="1e34d-118">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="1e34d-119">创建 plannerTask</span><span class="sxs-lookup"><span data-stu-id="1e34d-119">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="1e34d-120">plannerTask</span><span class="sxs-lookup"><span data-stu-id="1e34d-120">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="1e34d-121">通过发布到 tasks 集合创建新的**plannerTask** 。</span><span class="sxs-lookup"><span data-stu-id="1e34d-121">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="1e34d-122">属性</span><span class="sxs-lookup"><span data-stu-id="1e34d-122">Properties</span></span>
| <span data-ttu-id="1e34d-123">属性</span><span class="sxs-lookup"><span data-stu-id="1e34d-123">Property</span></span>     | <span data-ttu-id="1e34d-124">类型</span><span class="sxs-lookup"><span data-stu-id="1e34d-124">Type</span></span>   |<span data-ttu-id="1e34d-125">说明</span><span class="sxs-lookup"><span data-stu-id="1e34d-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e34d-126">id</span><span class="sxs-lookup"><span data-stu-id="1e34d-126">id</span></span>|<span data-ttu-id="1e34d-127">String</span><span class="sxs-lookup"><span data-stu-id="1e34d-127">String</span></span>| <span data-ttu-id="1e34d-128">只读。</span><span class="sxs-lookup"><span data-stu-id="1e34d-128">Read-only.</span></span> <span data-ttu-id="1e34d-129">**planner**资源的标识符。</span><span class="sxs-lookup"><span data-stu-id="1e34d-129">Identifier of the **planner** resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e34d-130">关系</span><span class="sxs-lookup"><span data-stu-id="1e34d-130">Relationships</span></span>
| <span data-ttu-id="1e34d-131">关系</span><span class="sxs-lookup"><span data-stu-id="1e34d-131">Relationship</span></span> | <span data-ttu-id="1e34d-132">类型</span><span class="sxs-lookup"><span data-stu-id="1e34d-132">Type</span></span>   |<span data-ttu-id="1e34d-133">说明</span><span class="sxs-lookup"><span data-stu-id="1e34d-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e34d-134">buckets</span><span class="sxs-lookup"><span data-stu-id="1e34d-134">buckets</span></span>|<span data-ttu-id="1e34d-135">[plannerBucket](plannerbucket.md) collection</span><span class="sxs-lookup"><span data-stu-id="1e34d-135">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="1e34d-136">只读。</span><span class="sxs-lookup"><span data-stu-id="1e34d-136">Read-only.</span></span> <span data-ttu-id="1e34d-137">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="1e34d-137">Nullable.</span></span> <span data-ttu-id="1e34d-138">返回指定的存储桶的集合</span><span class="sxs-lookup"><span data-stu-id="1e34d-138">Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="1e34d-139">计划</span><span class="sxs-lookup"><span data-stu-id="1e34d-139">plans</span></span>|<span data-ttu-id="1e34d-140">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1e34d-140">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="1e34d-141">只读。</span><span class="sxs-lookup"><span data-stu-id="1e34d-141">Read-only.</span></span> <span data-ttu-id="1e34d-142">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="1e34d-142">Nullable.</span></span> <span data-ttu-id="1e34d-143">返回指定计划的集合</span><span class="sxs-lookup"><span data-stu-id="1e34d-143">Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="1e34d-144">tasks</span><span class="sxs-lookup"><span data-stu-id="1e34d-144">tasks</span></span>|<span data-ttu-id="1e34d-145">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="1e34d-145">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="1e34d-146">只读。</span><span class="sxs-lookup"><span data-stu-id="1e34d-146">Read-only.</span></span> <span data-ttu-id="1e34d-147">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="1e34d-147">Nullable.</span></span> <span data-ttu-id="1e34d-148">返回指定任务的集合</span><span class="sxs-lookup"><span data-stu-id="1e34d-148">Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1e34d-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1e34d-149">JSON representation</span></span>
<span data-ttu-id="1e34d-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1e34d-150">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
