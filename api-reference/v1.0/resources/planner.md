---
title: planner 资源类型
description: '**planner** 资源是 Planner 对象模型的入口点。其返回单一的 **planner** 资源。它不包含任何可用属性。'
localization_priority: Normal
ms.openlocfilehash: 35088001ca2e444c1f375426fc40ff13bd2eaaec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821252"
---
# <a name="planner-resource-type"></a><span data-ttu-id="6e443-105">planner 资源类型</span><span class="sxs-lookup"><span data-stu-id="6e443-105">planner resource type</span></span>

<span data-ttu-id="6e443-p102">**planner** 资源是 Planner 对象模型的入口点。其返回单一的 **planner** 资源。它不包含任何可用属性。</span><span class="sxs-lookup"><span data-stu-id="6e443-p102">The **planner** resource is the entry point for the Planner object model. It returns a singleton **planner** resource.  It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="6e443-109">方法</span><span class="sxs-lookup"><span data-stu-id="6e443-109">Methods</span></span>

| <span data-ttu-id="6e443-110">方法</span><span class="sxs-lookup"><span data-stu-id="6e443-110">Method</span></span>           | <span data-ttu-id="6e443-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="6e443-111">Return Type</span></span>    |<span data-ttu-id="6e443-112">说明</span><span class="sxs-lookup"><span data-stu-id="6e443-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6e443-113">Create plannerBucket</span><span class="sxs-lookup"><span data-stu-id="6e443-113">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="6e443-114">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="6e443-114">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="6e443-115">通过发布到存储桶集合新建 **plannerBucket**。</span><span class="sxs-lookup"><span data-stu-id="6e443-115">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="6e443-116">Create plannerPlan</span><span class="sxs-lookup"><span data-stu-id="6e443-116">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="6e443-117">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="6e443-117">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="6e443-118">通过发布到计划集合新建 **plannerPlan**。</span><span class="sxs-lookup"><span data-stu-id="6e443-118">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="6e443-119">Create plannerTask</span><span class="sxs-lookup"><span data-stu-id="6e443-119">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="6e443-120">plannerTask</span><span class="sxs-lookup"><span data-stu-id="6e443-120">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="6e443-121">通过发布到任务集合新建 **plannerTask**。</span><span class="sxs-lookup"><span data-stu-id="6e443-121">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e443-122">Relationships</span><span class="sxs-lookup"><span data-stu-id="6e443-122">Relationships</span></span>
| <span data-ttu-id="6e443-123">关系</span><span class="sxs-lookup"><span data-stu-id="6e443-123">Relationship</span></span> | <span data-ttu-id="6e443-124">类型</span><span class="sxs-lookup"><span data-stu-id="6e443-124">Type</span></span>   |<span data-ttu-id="6e443-125">说明</span><span class="sxs-lookup"><span data-stu-id="6e443-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e443-126">buckets</span><span class="sxs-lookup"><span data-stu-id="6e443-126">buckets</span></span>|<span data-ttu-id="6e443-127">[plannerBucket](plannerbucket.md) collection</span><span class="sxs-lookup"><span data-stu-id="6e443-127">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="6e443-p103">只读。可为 NULL。返回指定存储桶的集合</span><span class="sxs-lookup"><span data-stu-id="6e443-p103">Read-only. Nullable. Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="6e443-131">plans</span><span class="sxs-lookup"><span data-stu-id="6e443-131">plans</span></span>|<span data-ttu-id="6e443-132">[plannerPlan](plannerplan.md) collection</span><span class="sxs-lookup"><span data-stu-id="6e443-132">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="6e443-p104">只读。可为 NULL。返回指定计划的集合</span><span class="sxs-lookup"><span data-stu-id="6e443-p104">Read-only. Nullable. Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="6e443-136">tasks</span><span class="sxs-lookup"><span data-stu-id="6e443-136">tasks</span></span>|<span data-ttu-id="6e443-137">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="6e443-137">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="6e443-p105">只读。可为 NULL。返回指定任务的集合</span><span class="sxs-lookup"><span data-stu-id="6e443-p105">Read-only. Nullable. Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6e443-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6e443-141">JSON representation</span></span>
<span data-ttu-id="6e443-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6e443-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="6e443-143">示例</span><span class="sxs-lookup"><span data-stu-id="6e443-143">Example</span></span>

<span data-ttu-id="6e443-144">**计划工具**资源是可在图的根。</span><span class="sxs-lookup"><span data-stu-id="6e443-144">The **planner** resource is available at the root of the graph.</span></span>

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
