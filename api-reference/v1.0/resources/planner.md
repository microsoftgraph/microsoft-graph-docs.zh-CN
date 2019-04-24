---
title: planner 资源类型
description: '**planner**资源是 planner 对象模型的入口点。 它返回单一实例**planner**资源。  它不包含任何可用属性。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: f6d25238436b79dec0397df1d005e67e6b17239a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462275"
---
# <a name="planner-resource-type"></a><span data-ttu-id="f4ed6-105">planner 资源类型</span><span class="sxs-lookup"><span data-stu-id="f4ed6-105">planner resource type</span></span>

<span data-ttu-id="f4ed6-106">**planner**资源是 planner 对象模型的入口点。</span><span class="sxs-lookup"><span data-stu-id="f4ed6-106">The **planner** resource is the entry point for the Planner object model.</span></span> <span data-ttu-id="f4ed6-107">它返回单一实例**planner**资源。</span><span class="sxs-lookup"><span data-stu-id="f4ed6-107">It returns a singleton **planner** resource.</span></span>  <span data-ttu-id="f4ed6-108">它不包含任何可用属性。</span><span class="sxs-lookup"><span data-stu-id="f4ed6-108">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="f4ed6-109">方法</span><span class="sxs-lookup"><span data-stu-id="f4ed6-109">Methods</span></span>

| <span data-ttu-id="f4ed6-110">方法</span><span class="sxs-lookup"><span data-stu-id="f4ed6-110">Method</span></span>           | <span data-ttu-id="f4ed6-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="f4ed6-111">Return Type</span></span>    |<span data-ttu-id="f4ed6-112">说明</span><span class="sxs-lookup"><span data-stu-id="f4ed6-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f4ed6-113">创建 plannerBucket</span><span class="sxs-lookup"><span data-stu-id="f4ed6-113">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="f4ed6-114">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="f4ed6-114">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="f4ed6-115">通过发布到存储桶集合创建新的**plannerBucket** 。</span><span class="sxs-lookup"><span data-stu-id="f4ed6-115">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="f4ed6-116">创建 plannerPlan</span><span class="sxs-lookup"><span data-stu-id="f4ed6-116">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="f4ed6-117">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="f4ed6-117">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="f4ed6-118">通过发布到计划集合创建新的**plannerPlan** 。</span><span class="sxs-lookup"><span data-stu-id="f4ed6-118">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="f4ed6-119">创建 plannerTask</span><span class="sxs-lookup"><span data-stu-id="f4ed6-119">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="f4ed6-120">plannerTask</span><span class="sxs-lookup"><span data-stu-id="f4ed6-120">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="f4ed6-121">通过发布到 tasks 集合创建新的**plannerTask** 。</span><span class="sxs-lookup"><span data-stu-id="f4ed6-121">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4ed6-122">关系</span><span class="sxs-lookup"><span data-stu-id="f4ed6-122">Relationships</span></span>
| <span data-ttu-id="f4ed6-123">关系</span><span class="sxs-lookup"><span data-stu-id="f4ed6-123">Relationship</span></span> | <span data-ttu-id="f4ed6-124">类型</span><span class="sxs-lookup"><span data-stu-id="f4ed6-124">Type</span></span>   |<span data-ttu-id="f4ed6-125">说明</span><span class="sxs-lookup"><span data-stu-id="f4ed6-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4ed6-126">存储桶</span><span class="sxs-lookup"><span data-stu-id="f4ed6-126">buckets</span></span>|<span data-ttu-id="f4ed6-127">[plannerBucket](plannerbucket.md)集合</span><span class="sxs-lookup"><span data-stu-id="f4ed6-127">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="f4ed6-128">只读。</span><span class="sxs-lookup"><span data-stu-id="f4ed6-128">Read-only.</span></span> <span data-ttu-id="f4ed6-129">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="f4ed6-129">Nullable.</span></span> <span data-ttu-id="f4ed6-130">返回指定的存储桶的集合</span><span class="sxs-lookup"><span data-stu-id="f4ed6-130">Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="f4ed6-131">计划</span><span class="sxs-lookup"><span data-stu-id="f4ed6-131">plans</span></span>|<span data-ttu-id="f4ed6-132">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f4ed6-132">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="f4ed6-133">只读。</span><span class="sxs-lookup"><span data-stu-id="f4ed6-133">Read-only.</span></span> <span data-ttu-id="f4ed6-134">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="f4ed6-134">Nullable.</span></span> <span data-ttu-id="f4ed6-135">返回指定计划的集合</span><span class="sxs-lookup"><span data-stu-id="f4ed6-135">Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="f4ed6-136">任务</span><span class="sxs-lookup"><span data-stu-id="f4ed6-136">tasks</span></span>|<span data-ttu-id="f4ed6-137">[plannerTask](plannertask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f4ed6-137">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="f4ed6-138">只读。</span><span class="sxs-lookup"><span data-stu-id="f4ed6-138">Read-only.</span></span> <span data-ttu-id="f4ed6-139">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="f4ed6-139">Nullable.</span></span> <span data-ttu-id="f4ed6-140">返回指定任务的集合</span><span class="sxs-lookup"><span data-stu-id="f4ed6-140">Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f4ed6-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f4ed6-141">JSON representation</span></span>
<span data-ttu-id="f4ed6-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4ed6-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="f4ed6-143">示例</span><span class="sxs-lookup"><span data-stu-id="f4ed6-143">Example</span></span>

<span data-ttu-id="f4ed6-144">**planner**资源在图形的根目录中可用。</span><span class="sxs-lookup"><span data-stu-id="f4ed6-144">The **planner** resource is available at the root of the graph.</span></span>

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
