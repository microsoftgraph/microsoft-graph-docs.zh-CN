---
title: plannerBucket 资源类型
description: ）用于 Microsoft 365 中的计划中的任务。 它包含在 plannerPlan 中，并且可以具有 plannerTasks 的集合。
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: b424a5ed3aba8bf287ad4d7fe6319504e18b4828
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895564"
---
# <a name="plannerbucket-resource-type"></a><span data-ttu-id="d4a39-104">plannerBucket 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4a39-104">plannerBucket resource type</span></span>

<span data-ttu-id="d4a39-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4a39-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d4a39-106">**PlannerBucket**资源表示 Microsoft 365 中的计划中的任务的存储桶（或 "自定义列"）。</span><span class="sxs-lookup"><span data-stu-id="d4a39-106">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Microsoft 365.</span></span> <span data-ttu-id="d4a39-107">它包含在[plannerPlan](plannerplan.md)中，并且可以具有[plannerTasks](plannertask.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="d4a39-107">It is contained in a [plannerPlan](plannerplan.md) and can have a collection of [plannerTasks](plannertask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="d4a39-108">方法</span><span class="sxs-lookup"><span data-stu-id="d4a39-108">Methods</span></span>

| <span data-ttu-id="d4a39-109">方法</span><span class="sxs-lookup"><span data-stu-id="d4a39-109">Method</span></span>           | <span data-ttu-id="d4a39-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d4a39-110">Return Type</span></span>    |<span data-ttu-id="d4a39-111">说明</span><span class="sxs-lookup"><span data-stu-id="d4a39-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d4a39-112">获取 plannerBucket</span><span class="sxs-lookup"><span data-stu-id="d4a39-112">Get plannerBucket</span></span>](../api/plannerbucket-get.md) | [<span data-ttu-id="d4a39-113">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="d4a39-113">plannerBucket</span></span>](plannerbucket.md) |<span data-ttu-id="d4a39-114">读取**plannerBucket**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d4a39-114">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="d4a39-115">List plannerTasks</span><span class="sxs-lookup"><span data-stu-id="d4a39-115">List plannerTasks</span></span>](../api/plannerbucket-list-tasks.md) |<span data-ttu-id="d4a39-116">[plannerTask](plannertask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d4a39-116">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="d4a39-117">获取 **plannerTask** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d4a39-117">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="d4a39-118">创建</span><span class="sxs-lookup"><span data-stu-id="d4a39-118">Create</span></span>](../api/planner-post-buckets.md) | [<span data-ttu-id="d4a39-119">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="d4a39-119">plannerBucket</span></span>](plannerbucket.md)   | <span data-ttu-id="d4a39-120">创建新的**plannerBucket**对象。</span><span class="sxs-lookup"><span data-stu-id="d4a39-120">Create a new **plannerBucket** object.</span></span> |
|[<span data-ttu-id="d4a39-121">更新</span><span class="sxs-lookup"><span data-stu-id="d4a39-121">Update</span></span>](../api/plannerbucket-update.md) | [<span data-ttu-id="d4a39-122">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="d4a39-122">plannerBucket</span></span>](plannerbucket.md)   |<span data-ttu-id="d4a39-123">更新**plannerBucket**对象。</span><span class="sxs-lookup"><span data-stu-id="d4a39-123">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="d4a39-124">删除</span><span class="sxs-lookup"><span data-stu-id="d4a39-124">Delete</span></span>](../api/plannerbucket-delete.md) | <span data-ttu-id="d4a39-125">无</span><span class="sxs-lookup"><span data-stu-id="d4a39-125">None</span></span> |<span data-ttu-id="d4a39-126">删除**plannerBucket**对象。</span><span class="sxs-lookup"><span data-stu-id="d4a39-126">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d4a39-127">属性</span><span class="sxs-lookup"><span data-stu-id="d4a39-127">Properties</span></span>
| <span data-ttu-id="d4a39-128">属性</span><span class="sxs-lookup"><span data-stu-id="d4a39-128">Property</span></span>     | <span data-ttu-id="d4a39-129">类型</span><span class="sxs-lookup"><span data-stu-id="d4a39-129">Type</span></span>   |<span data-ttu-id="d4a39-130">说明</span><span class="sxs-lookup"><span data-stu-id="d4a39-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4a39-131">id</span><span class="sxs-lookup"><span data-stu-id="d4a39-131">id</span></span>|<span data-ttu-id="d4a39-132">字符串</span><span class="sxs-lookup"><span data-stu-id="d4a39-132">String</span></span>| <span data-ttu-id="d4a39-133">只读。</span><span class="sxs-lookup"><span data-stu-id="d4a39-133">Read-only.</span></span> <span data-ttu-id="d4a39-134">存储桶的 ID。</span><span class="sxs-lookup"><span data-stu-id="d4a39-134">ID of the bucket.</span></span> <span data-ttu-id="d4a39-135">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="d4a39-135">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="d4a39-136">[格式验证](planner-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="d4a39-136">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="d4a39-137">name</span><span class="sxs-lookup"><span data-stu-id="d4a39-137">name</span></span>|<span data-ttu-id="d4a39-138">字符串</span><span class="sxs-lookup"><span data-stu-id="d4a39-138">String</span></span>|<span data-ttu-id="d4a39-139">存储桶的名称。</span><span class="sxs-lookup"><span data-stu-id="d4a39-139">Name of the bucket.</span></span>|
|<span data-ttu-id="d4a39-140">orderHint</span><span class="sxs-lookup"><span data-stu-id="d4a39-140">orderHint</span></span>|<span data-ttu-id="d4a39-141">String</span><span class="sxs-lookup"><span data-stu-id="d4a39-141">String</span></span>|<span data-ttu-id="d4a39-p104">用于为列表视图中的此类型项目排序的提示。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="d4a39-p104">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="d4a39-144">planId</span><span class="sxs-lookup"><span data-stu-id="d4a39-144">planId</span></span>|<span data-ttu-id="d4a39-145">String</span><span class="sxs-lookup"><span data-stu-id="d4a39-145">String</span></span>|<span data-ttu-id="d4a39-146">存储桶所属的计划 ID。</span><span class="sxs-lookup"><span data-stu-id="d4a39-146">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4a39-147">关系</span><span class="sxs-lookup"><span data-stu-id="d4a39-147">Relationships</span></span>
| <span data-ttu-id="d4a39-148">关系</span><span class="sxs-lookup"><span data-stu-id="d4a39-148">Relationship</span></span> | <span data-ttu-id="d4a39-149">类型</span><span class="sxs-lookup"><span data-stu-id="d4a39-149">Type</span></span>   |<span data-ttu-id="d4a39-150">说明</span><span class="sxs-lookup"><span data-stu-id="d4a39-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4a39-151">tasks</span><span class="sxs-lookup"><span data-stu-id="d4a39-151">tasks</span></span>|<span data-ttu-id="d4a39-152">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="d4a39-152">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="d4a39-153">只读。</span><span class="sxs-lookup"><span data-stu-id="d4a39-153">Read-only.</span></span> <span data-ttu-id="d4a39-154">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="d4a39-154">Nullable.</span></span> <span data-ttu-id="d4a39-155">存储桶中的任务的集合。</span><span class="sxs-lookup"><span data-stu-id="d4a39-155">The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d4a39-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4a39-156">JSON representation</span></span>
<span data-ttu-id="d4a39-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4a39-157">Here is a JSON representation of the resource.</span></span>

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
