---
title: planner 资源类型
description: '**Planner**资源是 planner 对象模型的入口点。 它返回单一实例**planner**资源。  它不包含任何可用属性。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: a7387b95e933378cb089834a1af29e0c7ca45266
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534035"
---
# <a name="planner-resource-type"></a><span data-ttu-id="3090d-105">planner 资源类型</span><span class="sxs-lookup"><span data-stu-id="3090d-105">planner resource type</span></span>

<span data-ttu-id="3090d-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3090d-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3090d-107">**Planner**资源是 planner 对象模型的入口点。</span><span class="sxs-lookup"><span data-stu-id="3090d-107">The **planner** resource is the entry point for the Planner object model.</span></span> <span data-ttu-id="3090d-108">它返回单一实例**planner**资源。</span><span class="sxs-lookup"><span data-stu-id="3090d-108">It returns a singleton **planner** resource.</span></span>  <span data-ttu-id="3090d-109">它不包含任何可用属性。</span><span class="sxs-lookup"><span data-stu-id="3090d-109">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="3090d-110">Methods</span><span class="sxs-lookup"><span data-stu-id="3090d-110">Methods</span></span>

| <span data-ttu-id="3090d-111">方法</span><span class="sxs-lookup"><span data-stu-id="3090d-111">Method</span></span>           | <span data-ttu-id="3090d-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="3090d-112">Return Type</span></span>    |<span data-ttu-id="3090d-113">说明</span><span class="sxs-lookup"><span data-stu-id="3090d-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3090d-114">创建 plannerBucket</span><span class="sxs-lookup"><span data-stu-id="3090d-114">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="3090d-115">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="3090d-115">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="3090d-116">通过发布到存储桶集合创建新的**plannerBucket** 。</span><span class="sxs-lookup"><span data-stu-id="3090d-116">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="3090d-117">创建 plannerPlan</span><span class="sxs-lookup"><span data-stu-id="3090d-117">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="3090d-118">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="3090d-118">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="3090d-119">通过发布到计划集合创建新的**plannerPlan** 。</span><span class="sxs-lookup"><span data-stu-id="3090d-119">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="3090d-120">创建 plannerTask</span><span class="sxs-lookup"><span data-stu-id="3090d-120">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="3090d-121">plannerTask</span><span class="sxs-lookup"><span data-stu-id="3090d-121">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="3090d-122">通过发布到 tasks 集合创建新的**plannerTask** 。</span><span class="sxs-lookup"><span data-stu-id="3090d-122">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3090d-123">关系</span><span class="sxs-lookup"><span data-stu-id="3090d-123">Relationships</span></span>
| <span data-ttu-id="3090d-124">关系</span><span class="sxs-lookup"><span data-stu-id="3090d-124">Relationship</span></span> | <span data-ttu-id="3090d-125">类型</span><span class="sxs-lookup"><span data-stu-id="3090d-125">Type</span></span>   |<span data-ttu-id="3090d-126">说明</span><span class="sxs-lookup"><span data-stu-id="3090d-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3090d-127">buckets</span><span class="sxs-lookup"><span data-stu-id="3090d-127">buckets</span></span>|<span data-ttu-id="3090d-128">[plannerBucket](plannerbucket.md) collection</span><span class="sxs-lookup"><span data-stu-id="3090d-128">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="3090d-129">只读。</span><span class="sxs-lookup"><span data-stu-id="3090d-129">Read-only.</span></span> <span data-ttu-id="3090d-130">可为空。</span><span class="sxs-lookup"><span data-stu-id="3090d-130">Nullable.</span></span> <span data-ttu-id="3090d-131">返回指定的存储桶的集合</span><span class="sxs-lookup"><span data-stu-id="3090d-131">Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="3090d-132">计划</span><span class="sxs-lookup"><span data-stu-id="3090d-132">plans</span></span>|<span data-ttu-id="3090d-133">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3090d-133">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="3090d-134">只读。</span><span class="sxs-lookup"><span data-stu-id="3090d-134">Read-only.</span></span> <span data-ttu-id="3090d-135">可为空。</span><span class="sxs-lookup"><span data-stu-id="3090d-135">Nullable.</span></span> <span data-ttu-id="3090d-136">返回指定计划的集合</span><span class="sxs-lookup"><span data-stu-id="3090d-136">Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="3090d-137">tasks</span><span class="sxs-lookup"><span data-stu-id="3090d-137">tasks</span></span>|<span data-ttu-id="3090d-138">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="3090d-138">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="3090d-139">只读。</span><span class="sxs-lookup"><span data-stu-id="3090d-139">Read-only.</span></span> <span data-ttu-id="3090d-140">可为空。</span><span class="sxs-lookup"><span data-stu-id="3090d-140">Nullable.</span></span> <span data-ttu-id="3090d-141">返回指定任务的集合</span><span class="sxs-lookup"><span data-stu-id="3090d-141">Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3090d-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3090d-142">JSON representation</span></span>
<span data-ttu-id="3090d-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3090d-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="3090d-144">示例</span><span class="sxs-lookup"><span data-stu-id="3090d-144">Example</span></span>

<span data-ttu-id="3090d-145">**Planner**资源在图形的根目录中可用。</span><span class="sxs-lookup"><span data-stu-id="3090d-145">The **planner** resource is available at the root of the graph.</span></span>

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.planner"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
