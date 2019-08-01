---
title: plannerBucket 资源类型
description: ) 用于 Office 365 中的计划中的任务。 它包含在 plannerPlan 中, 并且可以具有 plannerTasks 的集合。
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: b6810a62ecab5209ca1c17aa7f3ca9e4753a50a9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035321"
---
# <a name="plannerbucket-resource-type"></a><span data-ttu-id="5b76a-104">plannerBucket 资源类型</span><span class="sxs-lookup"><span data-stu-id="5b76a-104">plannerBucket resource type</span></span>

<span data-ttu-id="5b76a-105">**PlannerBucket**资源表示 Office 365 中的计划中的任务的存储桶 (或 "自定义列")。</span><span class="sxs-lookup"><span data-stu-id="5b76a-105">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Office 365.</span></span> <span data-ttu-id="5b76a-106">它包含在[plannerPlan](plannerplan.md)中, 并且可以具有[plannerTasks](plannertask.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="5b76a-106">It is contained in a [plannerPlan](plannerplan.md) and can have a collection of [plannerTasks](plannertask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="5b76a-107">方法</span><span class="sxs-lookup"><span data-stu-id="5b76a-107">Methods</span></span>

| <span data-ttu-id="5b76a-108">方法</span><span class="sxs-lookup"><span data-stu-id="5b76a-108">Method</span></span>           | <span data-ttu-id="5b76a-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="5b76a-109">Return Type</span></span>    |<span data-ttu-id="5b76a-110">说明</span><span class="sxs-lookup"><span data-stu-id="5b76a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5b76a-111">获取 plannerBucket</span><span class="sxs-lookup"><span data-stu-id="5b76a-111">Get plannerBucket</span></span>](../api/plannerbucket-get.md) | [<span data-ttu-id="5b76a-112">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="5b76a-112">plannerBucket</span></span>](plannerbucket.md) |<span data-ttu-id="5b76a-113">读取**plannerBucket**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5b76a-113">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="5b76a-114">List plannerTasks</span><span class="sxs-lookup"><span data-stu-id="5b76a-114">List plannerTasks</span></span>](../api/plannerbucket-list-tasks.md) |<span data-ttu-id="5b76a-115">[plannerTask](plannertask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5b76a-115">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="5b76a-116">获取 **plannerTask** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5b76a-116">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="5b76a-117">创建</span><span class="sxs-lookup"><span data-stu-id="5b76a-117">Create</span></span>](../api/planner-post-buckets.md) | [<span data-ttu-id="5b76a-118">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="5b76a-118">plannerBucket</span></span>](plannerbucket.md)   | <span data-ttu-id="5b76a-119">创建新的**plannerBucket**对象。</span><span class="sxs-lookup"><span data-stu-id="5b76a-119">Create a new **plannerBucket** object.</span></span> |
|[<span data-ttu-id="5b76a-120">更新</span><span class="sxs-lookup"><span data-stu-id="5b76a-120">Update</span></span>](../api/plannerbucket-update.md) | [<span data-ttu-id="5b76a-121">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="5b76a-121">plannerBucket</span></span>](plannerbucket.md)   |<span data-ttu-id="5b76a-122">更新**plannerBucket**对象。</span><span class="sxs-lookup"><span data-stu-id="5b76a-122">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="5b76a-123">删除</span><span class="sxs-lookup"><span data-stu-id="5b76a-123">Delete</span></span>](../api/plannerbucket-delete.md) | <span data-ttu-id="5b76a-124">无</span><span class="sxs-lookup"><span data-stu-id="5b76a-124">None</span></span> |<span data-ttu-id="5b76a-125">删除**plannerBucket**对象。</span><span class="sxs-lookup"><span data-stu-id="5b76a-125">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5b76a-126">属性</span><span class="sxs-lookup"><span data-stu-id="5b76a-126">Properties</span></span>
| <span data-ttu-id="5b76a-127">属性</span><span class="sxs-lookup"><span data-stu-id="5b76a-127">Property</span></span>     | <span data-ttu-id="5b76a-128">类型</span><span class="sxs-lookup"><span data-stu-id="5b76a-128">Type</span></span>   |<span data-ttu-id="5b76a-129">说明</span><span class="sxs-lookup"><span data-stu-id="5b76a-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b76a-130">id</span><span class="sxs-lookup"><span data-stu-id="5b76a-130">id</span></span>|<span data-ttu-id="5b76a-131">String</span><span class="sxs-lookup"><span data-stu-id="5b76a-131">String</span></span>| <span data-ttu-id="5b76a-132">只读。</span><span class="sxs-lookup"><span data-stu-id="5b76a-132">Read-only.</span></span> <span data-ttu-id="5b76a-133">存储桶的 ID。</span><span class="sxs-lookup"><span data-stu-id="5b76a-133">ID of the bucket.</span></span> <span data-ttu-id="5b76a-134">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="5b76a-134">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="5b76a-135">[格式验证](planner-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="5b76a-135">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="5b76a-136">name</span><span class="sxs-lookup"><span data-stu-id="5b76a-136">name</span></span>|<span data-ttu-id="5b76a-137">字符串</span><span class="sxs-lookup"><span data-stu-id="5b76a-137">String</span></span>|<span data-ttu-id="5b76a-138">存储桶的名称。</span><span class="sxs-lookup"><span data-stu-id="5b76a-138">Name of the bucket.</span></span>|
|<span data-ttu-id="5b76a-139">orderHint</span><span class="sxs-lookup"><span data-stu-id="5b76a-139">orderHint</span></span>|<span data-ttu-id="5b76a-140">String</span><span class="sxs-lookup"><span data-stu-id="5b76a-140">String</span></span>|<span data-ttu-id="5b76a-p104">用于为列表视图中的此类型项目排序的提示。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="5b76a-p104">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="5b76a-143">planId</span><span class="sxs-lookup"><span data-stu-id="5b76a-143">planId</span></span>|<span data-ttu-id="5b76a-144">String</span><span class="sxs-lookup"><span data-stu-id="5b76a-144">String</span></span>|<span data-ttu-id="5b76a-145">存储桶所属的计划 ID。</span><span class="sxs-lookup"><span data-stu-id="5b76a-145">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b76a-146">关系</span><span class="sxs-lookup"><span data-stu-id="5b76a-146">Relationships</span></span>
| <span data-ttu-id="5b76a-147">关系</span><span class="sxs-lookup"><span data-stu-id="5b76a-147">Relationship</span></span> | <span data-ttu-id="5b76a-148">类型</span><span class="sxs-lookup"><span data-stu-id="5b76a-148">Type</span></span>   |<span data-ttu-id="5b76a-149">说明</span><span class="sxs-lookup"><span data-stu-id="5b76a-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b76a-150">tasks</span><span class="sxs-lookup"><span data-stu-id="5b76a-150">tasks</span></span>|<span data-ttu-id="5b76a-151">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="5b76a-151">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="5b76a-152">只读。</span><span class="sxs-lookup"><span data-stu-id="5b76a-152">Read-only.</span></span> <span data-ttu-id="5b76a-153">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="5b76a-153">Nullable.</span></span> <span data-ttu-id="5b76a-154">存储桶中的任务的集合。</span><span class="sxs-lookup"><span data-stu-id="5b76a-154">The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5b76a-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5b76a-155">JSON representation</span></span>
<span data-ttu-id="5b76a-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5b76a-156">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
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
