---
title: plannerBucket 资源类型
description: ) 中的 Office 365 中的计划任务。 它包含在 plannerPlan，并且可以具有的 plannerTasks 集合。
ms.openlocfilehash: 4ccf4d683fd11caeb4a0f9800afd9811a137eefb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045633"
---
# <a name="plannerbucket-resource-type"></a><span data-ttu-id="0170e-104">plannerBucket 资源类型</span><span class="sxs-lookup"><span data-stu-id="0170e-104">plannerBucket resource type</span></span>

> <span data-ttu-id="0170e-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0170e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0170e-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0170e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0170e-p103">**plannerBucket** 资源表示 Office 365 计划中的任务的存储桶（或“自定义列”）。它包含在 [plannerPlan](plannerplan.md) 之中，并且可能具有 [plannerTasks](plannertask.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="0170e-p103">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Office 365. It is contained in a [plannerPlan](plannerplan.md) and can have a collection of [plannerTasks](plannertask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="0170e-109">方法</span><span class="sxs-lookup"><span data-stu-id="0170e-109">Methods</span></span>

| <span data-ttu-id="0170e-110">方法</span><span class="sxs-lookup"><span data-stu-id="0170e-110">Method</span></span>           | <span data-ttu-id="0170e-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="0170e-111">Return Type</span></span>    |<span data-ttu-id="0170e-112">说明</span><span class="sxs-lookup"><span data-stu-id="0170e-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0170e-113">Get plannerBucket</span><span class="sxs-lookup"><span data-stu-id="0170e-113">Get plannerBucket</span></span>](../api/plannerbucket-get.md) | [<span data-ttu-id="0170e-114">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="0170e-114">plannerBucket</span></span>](plannerbucket.md) |<span data-ttu-id="0170e-115">读取 **plannerBucket** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0170e-115">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="0170e-116">List plannerTasks</span><span class="sxs-lookup"><span data-stu-id="0170e-116">List plannerTasks</span></span>](../api/plannerbucket-list-tasks.md) |<span data-ttu-id="0170e-117">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="0170e-117">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="0170e-118">获取 **plannerTask** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0170e-118">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="0170e-119">Create</span><span class="sxs-lookup"><span data-stu-id="0170e-119">Create</span></span>](../api/planner-post-buckets.md) | [<span data-ttu-id="0170e-120">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="0170e-120">plannerBucket</span></span>](plannerbucket.md)   | <span data-ttu-id="0170e-121">新建 **plannerBucket** 对象。</span><span class="sxs-lookup"><span data-stu-id="0170e-121">Create a new **plannerBucket** object.</span></span> |
|[<span data-ttu-id="0170e-122">Update</span><span class="sxs-lookup"><span data-stu-id="0170e-122">Update</span></span>](../api/plannerbucket-update.md) | [<span data-ttu-id="0170e-123">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="0170e-123">plannerBucket</span></span>](plannerbucket.md)   |<span data-ttu-id="0170e-124">更新 **plannerBucket** 对象。</span><span class="sxs-lookup"><span data-stu-id="0170e-124">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="0170e-125">Delete</span><span class="sxs-lookup"><span data-stu-id="0170e-125">Delete</span></span>](../api/plannerbucket-delete.md) | <span data-ttu-id="0170e-126">无</span><span class="sxs-lookup"><span data-stu-id="0170e-126">None</span></span> |<span data-ttu-id="0170e-127">删除 **plannerBucket** 对象。</span><span class="sxs-lookup"><span data-stu-id="0170e-127">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0170e-128">属性</span><span class="sxs-lookup"><span data-stu-id="0170e-128">Properties</span></span>
| <span data-ttu-id="0170e-129">属性</span><span class="sxs-lookup"><span data-stu-id="0170e-129">Property</span></span>     | <span data-ttu-id="0170e-130">类型</span><span class="sxs-lookup"><span data-stu-id="0170e-130">Type</span></span>   |<span data-ttu-id="0170e-131">说明</span><span class="sxs-lookup"><span data-stu-id="0170e-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0170e-132">id</span><span class="sxs-lookup"><span data-stu-id="0170e-132">id</span></span>|<span data-ttu-id="0170e-133">String</span><span class="sxs-lookup"><span data-stu-id="0170e-133">String</span></span>| <span data-ttu-id="0170e-134">只读。</span><span class="sxs-lookup"><span data-stu-id="0170e-134">Read-only.</span></span> <span data-ttu-id="0170e-135">存储桶的 ID。</span><span class="sxs-lookup"><span data-stu-id="0170e-135">ID of the bucket.</span></span> <span data-ttu-id="0170e-136">它是 28 字符长度和区分大小写。</span><span class="sxs-lookup"><span data-stu-id="0170e-136">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="0170e-137">服务上执行[格式验证](tasks-identifiers-disclaimer.md)。</span><span class="sxs-lookup"><span data-stu-id="0170e-137">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="0170e-138">name</span><span class="sxs-lookup"><span data-stu-id="0170e-138">name</span></span>|<span data-ttu-id="0170e-139">String</span><span class="sxs-lookup"><span data-stu-id="0170e-139">String</span></span>|<span data-ttu-id="0170e-140">存储桶的名称。</span><span class="sxs-lookup"><span data-stu-id="0170e-140">Name of the bucket.</span></span>|
|<span data-ttu-id="0170e-141">orderHint</span><span class="sxs-lookup"><span data-stu-id="0170e-141">orderHint</span></span>|<span data-ttu-id="0170e-142">String</span><span class="sxs-lookup"><span data-stu-id="0170e-142">String</span></span>|<span data-ttu-id="0170e-p105">用于为列表视图中的此类型项目排序的提示。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="0170e-p105">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="0170e-145">planId</span><span class="sxs-lookup"><span data-stu-id="0170e-145">planId</span></span>|<span data-ttu-id="0170e-146">String</span><span class="sxs-lookup"><span data-stu-id="0170e-146">String</span></span>|<span data-ttu-id="0170e-147">此存储桶所属的计划 ID。</span><span class="sxs-lookup"><span data-stu-id="0170e-147">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0170e-148">关系</span><span class="sxs-lookup"><span data-stu-id="0170e-148">Relationships</span></span>
| <span data-ttu-id="0170e-149">关系</span><span class="sxs-lookup"><span data-stu-id="0170e-149">Relationship</span></span> | <span data-ttu-id="0170e-150">类型</span><span class="sxs-lookup"><span data-stu-id="0170e-150">Type</span></span>   |<span data-ttu-id="0170e-151">说明</span><span class="sxs-lookup"><span data-stu-id="0170e-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0170e-152">tasks</span><span class="sxs-lookup"><span data-stu-id="0170e-152">tasks</span></span>|<span data-ttu-id="0170e-153">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="0170e-153">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="0170e-p106">只读。可为 NULL。存储桶中的任务集合。</span><span class="sxs-lookup"><span data-stu-id="0170e-p106">Read-only. Nullable. The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0170e-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0170e-157">JSON representation</span></span>
<span data-ttu-id="0170e-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0170e-158">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerBucket"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "orderHint": "String",
  "planId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucket resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->