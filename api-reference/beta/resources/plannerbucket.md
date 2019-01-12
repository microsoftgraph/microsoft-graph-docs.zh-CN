---
title: plannerBucket 资源类型
description: ) 中的 Office 365 中的计划任务。 它包含在 plannerPlan，并且可以具有的 plannerTasks 集合。
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: 4ed1cbe51ca22fbabce6dfd030747e728299190f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929709"
---
# <a name="plannerbucket-resource-type"></a><span data-ttu-id="5fc62-104">plannerBucket 资源类型</span><span class="sxs-lookup"><span data-stu-id="5fc62-104">plannerBucket resource type</span></span>

> <span data-ttu-id="5fc62-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5fc62-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5fc62-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5fc62-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5fc62-p103">**plannerBucket** 资源表示 Office 365 计划中的任务的存储桶（或“自定义列”）。它包含在 [plannerPlan](plannerplan.md) 之中，并且可能具有 [plannerTasks](plannertask.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="5fc62-p103">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Office 365. It is contained in a [plannerPlan](plannerplan.md) and can have a collection of [plannerTasks](plannertask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="5fc62-109">方法</span><span class="sxs-lookup"><span data-stu-id="5fc62-109">Methods</span></span>

| <span data-ttu-id="5fc62-110">方法</span><span class="sxs-lookup"><span data-stu-id="5fc62-110">Method</span></span>           | <span data-ttu-id="5fc62-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="5fc62-111">Return Type</span></span>    |<span data-ttu-id="5fc62-112">说明</span><span class="sxs-lookup"><span data-stu-id="5fc62-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5fc62-113">Get plannerBucket</span><span class="sxs-lookup"><span data-stu-id="5fc62-113">Get plannerBucket</span></span>](../api/plannerbucket-get.md) | [<span data-ttu-id="5fc62-114">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="5fc62-114">plannerBucket</span></span>](plannerbucket.md) |<span data-ttu-id="5fc62-115">读取 **plannerBucket** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5fc62-115">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="5fc62-116">List plannerTasks</span><span class="sxs-lookup"><span data-stu-id="5fc62-116">List plannerTasks</span></span>](../api/plannerbucket-list-tasks.md) |<span data-ttu-id="5fc62-117">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="5fc62-117">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="5fc62-118">获取 **plannerTask** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5fc62-118">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="5fc62-119">Create</span><span class="sxs-lookup"><span data-stu-id="5fc62-119">Create</span></span>](../api/planner-post-buckets.md) | [<span data-ttu-id="5fc62-120">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="5fc62-120">plannerBucket</span></span>](plannerbucket.md)   | <span data-ttu-id="5fc62-121">新建 **plannerBucket** 对象。</span><span class="sxs-lookup"><span data-stu-id="5fc62-121">Create a new **plannerBucket** object.</span></span> |
|[<span data-ttu-id="5fc62-122">Update</span><span class="sxs-lookup"><span data-stu-id="5fc62-122">Update</span></span>](../api/plannerbucket-update.md) | [<span data-ttu-id="5fc62-123">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="5fc62-123">plannerBucket</span></span>](plannerbucket.md)   |<span data-ttu-id="5fc62-124">更新 **plannerBucket** 对象。</span><span class="sxs-lookup"><span data-stu-id="5fc62-124">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="5fc62-125">Delete</span><span class="sxs-lookup"><span data-stu-id="5fc62-125">Delete</span></span>](../api/plannerbucket-delete.md) | <span data-ttu-id="5fc62-126">无</span><span class="sxs-lookup"><span data-stu-id="5fc62-126">None</span></span> |<span data-ttu-id="5fc62-127">删除 **plannerBucket** 对象。</span><span class="sxs-lookup"><span data-stu-id="5fc62-127">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5fc62-128">属性</span><span class="sxs-lookup"><span data-stu-id="5fc62-128">Properties</span></span>
| <span data-ttu-id="5fc62-129">属性</span><span class="sxs-lookup"><span data-stu-id="5fc62-129">Property</span></span>     | <span data-ttu-id="5fc62-130">类型</span><span class="sxs-lookup"><span data-stu-id="5fc62-130">Type</span></span>   |<span data-ttu-id="5fc62-131">说明</span><span class="sxs-lookup"><span data-stu-id="5fc62-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5fc62-132">id</span><span class="sxs-lookup"><span data-stu-id="5fc62-132">id</span></span>|<span data-ttu-id="5fc62-133">String</span><span class="sxs-lookup"><span data-stu-id="5fc62-133">String</span></span>| <span data-ttu-id="5fc62-134">只读。</span><span class="sxs-lookup"><span data-stu-id="5fc62-134">Read-only.</span></span> <span data-ttu-id="5fc62-135">存储桶的 ID。</span><span class="sxs-lookup"><span data-stu-id="5fc62-135">ID of the bucket.</span></span> <span data-ttu-id="5fc62-136">它是 28 字符长度和区分大小写。</span><span class="sxs-lookup"><span data-stu-id="5fc62-136">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="5fc62-137">服务上执行[格式验证](tasks-identifiers-disclaimer.md)。</span><span class="sxs-lookup"><span data-stu-id="5fc62-137">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="5fc62-138">name</span><span class="sxs-lookup"><span data-stu-id="5fc62-138">name</span></span>|<span data-ttu-id="5fc62-139">String</span><span class="sxs-lookup"><span data-stu-id="5fc62-139">String</span></span>|<span data-ttu-id="5fc62-140">存储桶的名称。</span><span class="sxs-lookup"><span data-stu-id="5fc62-140">Name of the bucket.</span></span>|
|<span data-ttu-id="5fc62-141">orderHint</span><span class="sxs-lookup"><span data-stu-id="5fc62-141">orderHint</span></span>|<span data-ttu-id="5fc62-142">String</span><span class="sxs-lookup"><span data-stu-id="5fc62-142">String</span></span>|<span data-ttu-id="5fc62-p105">用于为列表视图中的此类型项目排序的提示。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="5fc62-p105">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="5fc62-145">planId</span><span class="sxs-lookup"><span data-stu-id="5fc62-145">planId</span></span>|<span data-ttu-id="5fc62-146">String</span><span class="sxs-lookup"><span data-stu-id="5fc62-146">String</span></span>|<span data-ttu-id="5fc62-147">此存储桶所属的计划 ID。</span><span class="sxs-lookup"><span data-stu-id="5fc62-147">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5fc62-148">关系</span><span class="sxs-lookup"><span data-stu-id="5fc62-148">Relationships</span></span>
| <span data-ttu-id="5fc62-149">关系</span><span class="sxs-lookup"><span data-stu-id="5fc62-149">Relationship</span></span> | <span data-ttu-id="5fc62-150">类型</span><span class="sxs-lookup"><span data-stu-id="5fc62-150">Type</span></span>   |<span data-ttu-id="5fc62-151">说明</span><span class="sxs-lookup"><span data-stu-id="5fc62-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5fc62-152">tasks</span><span class="sxs-lookup"><span data-stu-id="5fc62-152">tasks</span></span>|<span data-ttu-id="5fc62-153">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="5fc62-153">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="5fc62-p106">只读。可为 NULL。存储桶中的任务集合。</span><span class="sxs-lookup"><span data-stu-id="5fc62-p106">Read-only. Nullable. The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5fc62-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5fc62-157">JSON representation</span></span>
<span data-ttu-id="5fc62-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5fc62-158">Here is a JSON representation of the resource.</span></span>

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
