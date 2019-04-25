---
title: planner 资源类型
description: '**planner**资源是 planner 对象模型的入口点。 它返回单一实例**planner**资源。  它不包含任何可用属性。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 50ceb8b76b398bd5898e48f31df9a6443569781e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579245"
---
# <a name="planner-resource-type"></a><span data-ttu-id="d609c-105">planner 资源类型</span><span class="sxs-lookup"><span data-stu-id="d609c-105">planner resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d609c-106">**planner**资源是 planner 对象模型的入口点。</span><span class="sxs-lookup"><span data-stu-id="d609c-106">The **planner** resource is the entry point for the Planner object model.</span></span> <span data-ttu-id="d609c-107">它返回单一实例**planner**资源。</span><span class="sxs-lookup"><span data-stu-id="d609c-107">It returns a singleton **planner** resource.</span></span>  <span data-ttu-id="d609c-108">它不包含任何可用属性。</span><span class="sxs-lookup"><span data-stu-id="d609c-108">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="d609c-109">方法</span><span class="sxs-lookup"><span data-stu-id="d609c-109">Methods</span></span>

| <span data-ttu-id="d609c-110">方法</span><span class="sxs-lookup"><span data-stu-id="d609c-110">Method</span></span>           | <span data-ttu-id="d609c-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="d609c-111">Return Type</span></span>    |<span data-ttu-id="d609c-112">说明</span><span class="sxs-lookup"><span data-stu-id="d609c-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d609c-113">创建 plannerBucket</span><span class="sxs-lookup"><span data-stu-id="d609c-113">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="d609c-114">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="d609c-114">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="d609c-115">通过发布到存储桶集合创建新的**plannerBucket** 。</span><span class="sxs-lookup"><span data-stu-id="d609c-115">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="d609c-116">创建 plannerPlan</span><span class="sxs-lookup"><span data-stu-id="d609c-116">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="d609c-117">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="d609c-117">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="d609c-118">通过发布到计划集合创建新的**plannerPlan** 。</span><span class="sxs-lookup"><span data-stu-id="d609c-118">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="d609c-119">创建 plannerTask</span><span class="sxs-lookup"><span data-stu-id="d609c-119">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="d609c-120">plannerTask</span><span class="sxs-lookup"><span data-stu-id="d609c-120">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="d609c-121">通过发布到 tasks 集合创建新的**plannerTask** 。</span><span class="sxs-lookup"><span data-stu-id="d609c-121">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="d609c-122">属性</span><span class="sxs-lookup"><span data-stu-id="d609c-122">Properties</span></span>
| <span data-ttu-id="d609c-123">属性</span><span class="sxs-lookup"><span data-stu-id="d609c-123">Property</span></span>     | <span data-ttu-id="d609c-124">类型</span><span class="sxs-lookup"><span data-stu-id="d609c-124">Type</span></span>   |<span data-ttu-id="d609c-125">说明</span><span class="sxs-lookup"><span data-stu-id="d609c-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d609c-126">id</span><span class="sxs-lookup"><span data-stu-id="d609c-126">id</span></span>|<span data-ttu-id="d609c-127">String</span><span class="sxs-lookup"><span data-stu-id="d609c-127">String</span></span>| <span data-ttu-id="d609c-128">只读。</span><span class="sxs-lookup"><span data-stu-id="d609c-128">Read-only.</span></span> <span data-ttu-id="d609c-129">**planner**资源的标识符。</span><span class="sxs-lookup"><span data-stu-id="d609c-129">Identifier of the **planner** resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d609c-130">关系</span><span class="sxs-lookup"><span data-stu-id="d609c-130">Relationships</span></span>
| <span data-ttu-id="d609c-131">关系</span><span class="sxs-lookup"><span data-stu-id="d609c-131">Relationship</span></span> | <span data-ttu-id="d609c-132">类型</span><span class="sxs-lookup"><span data-stu-id="d609c-132">Type</span></span>   |<span data-ttu-id="d609c-133">说明</span><span class="sxs-lookup"><span data-stu-id="d609c-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d609c-134">存储桶</span><span class="sxs-lookup"><span data-stu-id="d609c-134">buckets</span></span>|<span data-ttu-id="d609c-135">[plannerBucket](plannerbucket.md)集合</span><span class="sxs-lookup"><span data-stu-id="d609c-135">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="d609c-136">只读。</span><span class="sxs-lookup"><span data-stu-id="d609c-136">Read-only.</span></span> <span data-ttu-id="d609c-137">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="d609c-137">Nullable.</span></span> <span data-ttu-id="d609c-138">返回指定的存储桶的集合</span><span class="sxs-lookup"><span data-stu-id="d609c-138">Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="d609c-139">计划</span><span class="sxs-lookup"><span data-stu-id="d609c-139">plans</span></span>|<span data-ttu-id="d609c-140">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d609c-140">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="d609c-141">只读。</span><span class="sxs-lookup"><span data-stu-id="d609c-141">Read-only.</span></span> <span data-ttu-id="d609c-142">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="d609c-142">Nullable.</span></span> <span data-ttu-id="d609c-143">返回指定计划的集合</span><span class="sxs-lookup"><span data-stu-id="d609c-143">Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="d609c-144">任务</span><span class="sxs-lookup"><span data-stu-id="d609c-144">tasks</span></span>|<span data-ttu-id="d609c-145">[plannerTask](plannertask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d609c-145">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="d609c-146">只读。</span><span class="sxs-lookup"><span data-stu-id="d609c-146">Read-only.</span></span> <span data-ttu-id="d609c-147">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="d609c-147">Nullable.</span></span> <span data-ttu-id="d609c-148">返回指定任务的集合</span><span class="sxs-lookup"><span data-stu-id="d609c-148">Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d609c-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d609c-149">JSON representation</span></span>
<span data-ttu-id="d609c-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d609c-150">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/planner.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
