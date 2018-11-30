---
title: planner 资源类型
description: '**planner** 资源是 Planner 对象模型的入口点。其返回单一的 **planner** 资源。它不包含任何可用属性。'
ms.openlocfilehash: e5980f6f4037b57e977b12ef223e8a5a2cf7c77c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010941"
---
# <a name="planner-resource-type"></a><span data-ttu-id="d1b1b-105">planner 资源类型</span><span class="sxs-lookup"><span data-stu-id="d1b1b-105">planner resource type</span></span>

<span data-ttu-id="d1b1b-p102">**planner** 资源是 Planner 对象模型的入口点。其返回单一的 **planner** 资源。它不包含任何可用属性。</span><span class="sxs-lookup"><span data-stu-id="d1b1b-p102">The **planner** resource is the entry point for the Planner object model. It returns a singleton **planner** resource.  It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="d1b1b-109">方法</span><span class="sxs-lookup"><span data-stu-id="d1b1b-109">Methods</span></span>

| <span data-ttu-id="d1b1b-110">方法</span><span class="sxs-lookup"><span data-stu-id="d1b1b-110">Method</span></span>           | <span data-ttu-id="d1b1b-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="d1b1b-111">Return Type</span></span>    |<span data-ttu-id="d1b1b-112">说明</span><span class="sxs-lookup"><span data-stu-id="d1b1b-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d1b1b-113">Create plannerBucket</span><span class="sxs-lookup"><span data-stu-id="d1b1b-113">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="d1b1b-114">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="d1b1b-114">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="d1b1b-115">通过发布到存储桶集合新建 **plannerBucket**。</span><span class="sxs-lookup"><span data-stu-id="d1b1b-115">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="d1b1b-116">Create plannerPlan</span><span class="sxs-lookup"><span data-stu-id="d1b1b-116">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="d1b1b-117">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="d1b1b-117">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="d1b1b-118">通过发布到计划集合新建 **plannerPlan**。</span><span class="sxs-lookup"><span data-stu-id="d1b1b-118">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="d1b1b-119">Create plannerTask</span><span class="sxs-lookup"><span data-stu-id="d1b1b-119">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="d1b1b-120">plannerTask</span><span class="sxs-lookup"><span data-stu-id="d1b1b-120">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="d1b1b-121">通过发布到任务集合新建 **plannerTask**。</span><span class="sxs-lookup"><span data-stu-id="d1b1b-121">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1b1b-122">Relationships</span><span class="sxs-lookup"><span data-stu-id="d1b1b-122">Relationships</span></span>
| <span data-ttu-id="d1b1b-123">关系</span><span class="sxs-lookup"><span data-stu-id="d1b1b-123">Relationship</span></span> | <span data-ttu-id="d1b1b-124">类型</span><span class="sxs-lookup"><span data-stu-id="d1b1b-124">Type</span></span>   |<span data-ttu-id="d1b1b-125">说明</span><span class="sxs-lookup"><span data-stu-id="d1b1b-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1b1b-126">buckets</span><span class="sxs-lookup"><span data-stu-id="d1b1b-126">buckets</span></span>|<span data-ttu-id="d1b1b-127">[plannerBucket](plannerbucket.md) collection</span><span class="sxs-lookup"><span data-stu-id="d1b1b-127">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="d1b1b-p103">只读。可为 NULL。返回指定存储桶的集合</span><span class="sxs-lookup"><span data-stu-id="d1b1b-p103">Read-only. Nullable. Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="d1b1b-131">plans</span><span class="sxs-lookup"><span data-stu-id="d1b1b-131">plans</span></span>|<span data-ttu-id="d1b1b-132">[plannerPlan](plannerplan.md) collection</span><span class="sxs-lookup"><span data-stu-id="d1b1b-132">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="d1b1b-p104">只读。可为 NULL。返回指定计划的集合</span><span class="sxs-lookup"><span data-stu-id="d1b1b-p104">Read-only. Nullable. Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="d1b1b-136">tasks</span><span class="sxs-lookup"><span data-stu-id="d1b1b-136">tasks</span></span>|<span data-ttu-id="d1b1b-137">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="d1b1b-137">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="d1b1b-p105">只读。可为 NULL。返回指定任务的集合</span><span class="sxs-lookup"><span data-stu-id="d1b1b-p105">Read-only. Nullable. Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d1b1b-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d1b1b-141">JSON representation</span></span>
<span data-ttu-id="d1b1b-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d1b1b-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="d1b1b-143">示例</span><span class="sxs-lookup"><span data-stu-id="d1b1b-143">Example</span></span>

<span data-ttu-id="d1b1b-144">**计划工具**资源是可在图的根。</span><span class="sxs-lookup"><span data-stu-id="d1b1b-144">The **planner** resource is available at the root of the graph.</span></span>

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