---
title: planner 资源类型
description: '**Planner**资源是 planner 对象模型的入口点。 它返回单一实例**planner**资源。  它不包含任何可用属性。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 45dc3ee05f5cee36ac1eecc99aff03f71b93c515
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521826"
---
# <a name="planner-resource-type"></a><span data-ttu-id="a66e0-105">planner 资源类型</span><span class="sxs-lookup"><span data-stu-id="a66e0-105">planner resource type</span></span>

<span data-ttu-id="a66e0-106">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a66e0-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a66e0-107">**Planner**资源是 planner 对象模型的入口点。</span><span class="sxs-lookup"><span data-stu-id="a66e0-107">The **planner** resource is the entry point for the Planner object model.</span></span> <span data-ttu-id="a66e0-108">它返回单一实例**planner**资源。</span><span class="sxs-lookup"><span data-stu-id="a66e0-108">It returns a singleton **planner** resource.</span></span>  <span data-ttu-id="a66e0-109">它不包含任何可用属性。</span><span class="sxs-lookup"><span data-stu-id="a66e0-109">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="a66e0-110">方法</span><span class="sxs-lookup"><span data-stu-id="a66e0-110">Methods</span></span>

| <span data-ttu-id="a66e0-111">方法</span><span class="sxs-lookup"><span data-stu-id="a66e0-111">Method</span></span>           | <span data-ttu-id="a66e0-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="a66e0-112">Return Type</span></span>    |<span data-ttu-id="a66e0-113">说明</span><span class="sxs-lookup"><span data-stu-id="a66e0-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a66e0-114">创建 plannerBucket</span><span class="sxs-lookup"><span data-stu-id="a66e0-114">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="a66e0-115">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="a66e0-115">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="a66e0-116">通过发布到存储桶集合创建新的**plannerBucket** 。</span><span class="sxs-lookup"><span data-stu-id="a66e0-116">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="a66e0-117">创建 plannerPlan</span><span class="sxs-lookup"><span data-stu-id="a66e0-117">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="a66e0-118">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="a66e0-118">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="a66e0-119">通过发布到计划集合创建新的**plannerPlan** 。</span><span class="sxs-lookup"><span data-stu-id="a66e0-119">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="a66e0-120">创建 plannerTask</span><span class="sxs-lookup"><span data-stu-id="a66e0-120">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="a66e0-121">plannerTask</span><span class="sxs-lookup"><span data-stu-id="a66e0-121">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="a66e0-122">通过发布到 tasks 集合创建新的**plannerTask** 。</span><span class="sxs-lookup"><span data-stu-id="a66e0-122">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="a66e0-123">属性</span><span class="sxs-lookup"><span data-stu-id="a66e0-123">Properties</span></span>
| <span data-ttu-id="a66e0-124">属性</span><span class="sxs-lookup"><span data-stu-id="a66e0-124">Property</span></span>     | <span data-ttu-id="a66e0-125">类型</span><span class="sxs-lookup"><span data-stu-id="a66e0-125">Type</span></span>   |<span data-ttu-id="a66e0-126">说明</span><span class="sxs-lookup"><span data-stu-id="a66e0-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a66e0-127">id</span><span class="sxs-lookup"><span data-stu-id="a66e0-127">id</span></span>|<span data-ttu-id="a66e0-128">String</span><span class="sxs-lookup"><span data-stu-id="a66e0-128">String</span></span>| <span data-ttu-id="a66e0-129">只读。</span><span class="sxs-lookup"><span data-stu-id="a66e0-129">Read-only.</span></span> <span data-ttu-id="a66e0-130">**Planner**资源的标识符。</span><span class="sxs-lookup"><span data-stu-id="a66e0-130">Identifier of the **planner** resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a66e0-131">关系</span><span class="sxs-lookup"><span data-stu-id="a66e0-131">Relationships</span></span>
| <span data-ttu-id="a66e0-132">关系</span><span class="sxs-lookup"><span data-stu-id="a66e0-132">Relationship</span></span> | <span data-ttu-id="a66e0-133">类型</span><span class="sxs-lookup"><span data-stu-id="a66e0-133">Type</span></span>   |<span data-ttu-id="a66e0-134">说明</span><span class="sxs-lookup"><span data-stu-id="a66e0-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a66e0-135">buckets</span><span class="sxs-lookup"><span data-stu-id="a66e0-135">buckets</span></span>|<span data-ttu-id="a66e0-136">[plannerBucket](plannerbucket.md) collection</span><span class="sxs-lookup"><span data-stu-id="a66e0-136">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="a66e0-137">只读。</span><span class="sxs-lookup"><span data-stu-id="a66e0-137">Read-only.</span></span> <span data-ttu-id="a66e0-138">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="a66e0-138">Nullable.</span></span> <span data-ttu-id="a66e0-139">返回指定的存储桶的集合</span><span class="sxs-lookup"><span data-stu-id="a66e0-139">Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="a66e0-140">计划</span><span class="sxs-lookup"><span data-stu-id="a66e0-140">plans</span></span>|<span data-ttu-id="a66e0-141">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a66e0-141">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="a66e0-142">只读。</span><span class="sxs-lookup"><span data-stu-id="a66e0-142">Read-only.</span></span> <span data-ttu-id="a66e0-143">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="a66e0-143">Nullable.</span></span> <span data-ttu-id="a66e0-144">返回指定计划的集合</span><span class="sxs-lookup"><span data-stu-id="a66e0-144">Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="a66e0-145">tasks</span><span class="sxs-lookup"><span data-stu-id="a66e0-145">tasks</span></span>|<span data-ttu-id="a66e0-146">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="a66e0-146">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="a66e0-147">只读。</span><span class="sxs-lookup"><span data-stu-id="a66e0-147">Read-only.</span></span> <span data-ttu-id="a66e0-148">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="a66e0-148">Nullable.</span></span> <span data-ttu-id="a66e0-149">返回指定任务的集合</span><span class="sxs-lookup"><span data-stu-id="a66e0-149">Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a66e0-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a66e0-150">JSON representation</span></span>
<span data-ttu-id="a66e0-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a66e0-151">Here is a JSON representation of the resource.</span></span>

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
