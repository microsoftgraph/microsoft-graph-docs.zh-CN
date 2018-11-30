---
title: planner 资源类型
description: '**planner** 资源是 Planner 对象模型的入口点。其返回单一的 **planner** 资源。它不包含任何可用属性。'
ms.openlocfilehash: c076eda1660cef9e31f584e5fe439f916eba81d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049328"
---
# <a name="planner-resource-type"></a><span data-ttu-id="4f3b0-105">planner 资源类型</span><span class="sxs-lookup"><span data-stu-id="4f3b0-105">planner resource type</span></span>

> <span data-ttu-id="4f3b0-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4f3b0-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4f3b0-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4f3b0-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4f3b0-p103">**planner** 资源是 Planner 对象模型的入口点。其返回单一的 **planner** 资源。它不包含任何可用属性。</span><span class="sxs-lookup"><span data-stu-id="4f3b0-p103">The **planner** resource is the entry point for the Planner object model. It returns a singleton **planner** resource.  It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="4f3b0-111">方法</span><span class="sxs-lookup"><span data-stu-id="4f3b0-111">Methods</span></span>

| <span data-ttu-id="4f3b0-112">方法</span><span class="sxs-lookup"><span data-stu-id="4f3b0-112">Method</span></span>           | <span data-ttu-id="4f3b0-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="4f3b0-113">Return Type</span></span>    |<span data-ttu-id="4f3b0-114">说明</span><span class="sxs-lookup"><span data-stu-id="4f3b0-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4f3b0-115">Create plannerBucket</span><span class="sxs-lookup"><span data-stu-id="4f3b0-115">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="4f3b0-116">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="4f3b0-116">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="4f3b0-117">通过发布到存储桶集合新建 **plannerBucket**。</span><span class="sxs-lookup"><span data-stu-id="4f3b0-117">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="4f3b0-118">Create plannerPlan</span><span class="sxs-lookup"><span data-stu-id="4f3b0-118">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="4f3b0-119">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="4f3b0-119">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="4f3b0-120">通过发布到计划集合新建 **plannerPlan**。</span><span class="sxs-lookup"><span data-stu-id="4f3b0-120">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="4f3b0-121">Create plannerTask</span><span class="sxs-lookup"><span data-stu-id="4f3b0-121">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="4f3b0-122">plannerTask</span><span class="sxs-lookup"><span data-stu-id="4f3b0-122">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="4f3b0-123">通过发布到任务集合新建 **plannerTask**。</span><span class="sxs-lookup"><span data-stu-id="4f3b0-123">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="4f3b0-124">属性</span><span class="sxs-lookup"><span data-stu-id="4f3b0-124">Properties</span></span>
| <span data-ttu-id="4f3b0-125">属性</span><span class="sxs-lookup"><span data-stu-id="4f3b0-125">Property</span></span>     | <span data-ttu-id="4f3b0-126">类型</span><span class="sxs-lookup"><span data-stu-id="4f3b0-126">Type</span></span>   |<span data-ttu-id="4f3b0-127">说明</span><span class="sxs-lookup"><span data-stu-id="4f3b0-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4f3b0-128">id</span><span class="sxs-lookup"><span data-stu-id="4f3b0-128">id</span></span>|<span data-ttu-id="4f3b0-129">String</span><span class="sxs-lookup"><span data-stu-id="4f3b0-129">String</span></span>| <span data-ttu-id="4f3b0-p104">只读。**planner** 资源的标识符</span><span class="sxs-lookup"><span data-stu-id="4f3b0-p104">Read-only. Identifier of the **planner** resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f3b0-132">关系</span><span class="sxs-lookup"><span data-stu-id="4f3b0-132">Relationships</span></span>
| <span data-ttu-id="4f3b0-133">关系</span><span class="sxs-lookup"><span data-stu-id="4f3b0-133">Relationship</span></span> | <span data-ttu-id="4f3b0-134">类型</span><span class="sxs-lookup"><span data-stu-id="4f3b0-134">Type</span></span>   |<span data-ttu-id="4f3b0-135">说明</span><span class="sxs-lookup"><span data-stu-id="4f3b0-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4f3b0-136">buckets</span><span class="sxs-lookup"><span data-stu-id="4f3b0-136">buckets</span></span>|<span data-ttu-id="4f3b0-137">[plannerBucket](plannerbucket.md) collection</span><span class="sxs-lookup"><span data-stu-id="4f3b0-137">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="4f3b0-p105">只读。可为 NULL。返回指定存储桶的集合</span><span class="sxs-lookup"><span data-stu-id="4f3b0-p105">Read-only. Nullable. Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="4f3b0-141">plans</span><span class="sxs-lookup"><span data-stu-id="4f3b0-141">plans</span></span>|<span data-ttu-id="4f3b0-142">[plannerPlan](plannerplan.md) collection</span><span class="sxs-lookup"><span data-stu-id="4f3b0-142">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="4f3b0-p106">只读。可为 NULL。返回指定计划的集合</span><span class="sxs-lookup"><span data-stu-id="4f3b0-p106">Read-only. Nullable. Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="4f3b0-146">tasks</span><span class="sxs-lookup"><span data-stu-id="4f3b0-146">tasks</span></span>|<span data-ttu-id="4f3b0-147">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="4f3b0-147">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="4f3b0-p107">只读。可为 NULL。返回指定任务的集合</span><span class="sxs-lookup"><span data-stu-id="4f3b0-p107">Read-only. Nullable. Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4f3b0-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4f3b0-151">JSON representation</span></span>
<span data-ttu-id="4f3b0-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f3b0-152">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.planner"
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
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->