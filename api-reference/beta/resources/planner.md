---
title: planner 资源类型
description: '**planner** 资源是 Planner 对象模型的入口点。其返回单一的 **planner** 资源。它不包含任何可用属性。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 50ceb8b76b398bd5898e48f31df9a6443569781e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523398"
---
# <a name="planner-resource-type"></a><span data-ttu-id="18b1a-105">planner 资源类型</span><span class="sxs-lookup"><span data-stu-id="18b1a-105">planner resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18b1a-p102">**planner** 资源是 Planner 对象模型的入口点。其返回单一的 **planner** 资源。它不包含任何可用属性。</span><span class="sxs-lookup"><span data-stu-id="18b1a-p102">The **planner** resource is the entry point for the Planner object model. It returns a singleton **planner** resource.  It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="18b1a-109">方法</span><span class="sxs-lookup"><span data-stu-id="18b1a-109">Methods</span></span>

| <span data-ttu-id="18b1a-110">方法</span><span class="sxs-lookup"><span data-stu-id="18b1a-110">Method</span></span>           | <span data-ttu-id="18b1a-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="18b1a-111">Return Type</span></span>    |<span data-ttu-id="18b1a-112">说明</span><span class="sxs-lookup"><span data-stu-id="18b1a-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="18b1a-113">Create plannerBucket</span><span class="sxs-lookup"><span data-stu-id="18b1a-113">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="18b1a-114">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="18b1a-114">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="18b1a-115">通过发布到存储桶集合新建 **plannerBucket**。</span><span class="sxs-lookup"><span data-stu-id="18b1a-115">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="18b1a-116">Create plannerPlan</span><span class="sxs-lookup"><span data-stu-id="18b1a-116">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="18b1a-117">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="18b1a-117">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="18b1a-118">通过发布到计划集合新建 **plannerPlan**。</span><span class="sxs-lookup"><span data-stu-id="18b1a-118">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="18b1a-119">Create plannerTask</span><span class="sxs-lookup"><span data-stu-id="18b1a-119">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="18b1a-120">plannerTask</span><span class="sxs-lookup"><span data-stu-id="18b1a-120">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="18b1a-121">通过发布到任务集合新建 **plannerTask**。</span><span class="sxs-lookup"><span data-stu-id="18b1a-121">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="18b1a-122">属性</span><span class="sxs-lookup"><span data-stu-id="18b1a-122">Properties</span></span>
| <span data-ttu-id="18b1a-123">属性</span><span class="sxs-lookup"><span data-stu-id="18b1a-123">Property</span></span>     | <span data-ttu-id="18b1a-124">类型</span><span class="sxs-lookup"><span data-stu-id="18b1a-124">Type</span></span>   |<span data-ttu-id="18b1a-125">说明</span><span class="sxs-lookup"><span data-stu-id="18b1a-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18b1a-126">id</span><span class="sxs-lookup"><span data-stu-id="18b1a-126">id</span></span>|<span data-ttu-id="18b1a-127">String</span><span class="sxs-lookup"><span data-stu-id="18b1a-127">String</span></span>| <span data-ttu-id="18b1a-p103">只读。**planner** 资源的标识符</span><span class="sxs-lookup"><span data-stu-id="18b1a-p103">Read-only. Identifier of the **planner** resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="18b1a-130">关系</span><span class="sxs-lookup"><span data-stu-id="18b1a-130">Relationships</span></span>
| <span data-ttu-id="18b1a-131">关系</span><span class="sxs-lookup"><span data-stu-id="18b1a-131">Relationship</span></span> | <span data-ttu-id="18b1a-132">类型</span><span class="sxs-lookup"><span data-stu-id="18b1a-132">Type</span></span>   |<span data-ttu-id="18b1a-133">说明</span><span class="sxs-lookup"><span data-stu-id="18b1a-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18b1a-134">buckets</span><span class="sxs-lookup"><span data-stu-id="18b1a-134">buckets</span></span>|<span data-ttu-id="18b1a-135">[plannerBucket](plannerbucket.md) collection</span><span class="sxs-lookup"><span data-stu-id="18b1a-135">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="18b1a-p104">只读。可为 NULL。返回指定存储桶的集合</span><span class="sxs-lookup"><span data-stu-id="18b1a-p104">Read-only. Nullable. Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="18b1a-139">plans</span><span class="sxs-lookup"><span data-stu-id="18b1a-139">plans</span></span>|<span data-ttu-id="18b1a-140">[plannerPlan](plannerplan.md) collection</span><span class="sxs-lookup"><span data-stu-id="18b1a-140">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="18b1a-p105">只读。可为 NULL。返回指定计划的集合</span><span class="sxs-lookup"><span data-stu-id="18b1a-p105">Read-only. Nullable. Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="18b1a-144">tasks</span><span class="sxs-lookup"><span data-stu-id="18b1a-144">tasks</span></span>|<span data-ttu-id="18b1a-145">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="18b1a-145">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="18b1a-p106">只读。可为 NULL。返回指定任务的集合</span><span class="sxs-lookup"><span data-stu-id="18b1a-p106">Read-only. Nullable. Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="18b1a-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="18b1a-149">JSON representation</span></span>
<span data-ttu-id="18b1a-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="18b1a-150">Here is a JSON representation of the resource.</span></span>

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
