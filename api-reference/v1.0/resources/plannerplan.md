---
title: plannerPlan 资源类型
description: '**plannerPlan** 资源表示 Microsoft 365 中的计划。 计划可以由组所有，并包含 plannerTasks 集合。 其也可以有 plannerBuckets 集合。 每个计划对象具有可以包含此计划的更多信息的详细信息对象。 有关组、计划和任务之间的关系的详细信息，请参阅“Planner”。'
localization_priority: Priority
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: da5f4b882ad0c364d590b3db64913c170bb5a1d8
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720681"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="a0925-107">plannerPlan 资源类型</span><span class="sxs-lookup"><span data-stu-id="a0925-107">plannerPlan resource type</span></span>

<span data-ttu-id="a0925-108">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0925-108">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a0925-109">**plannerPlan** 资源表示 Microsoft 365 中的计划。</span><span class="sxs-lookup"><span data-stu-id="a0925-109">The **plannerPlan** resource represents a plan in Microsoft 365.</span></span> <span data-ttu-id="a0925-110">计划可以由[组](group.md)所有，并包含 [plannerTasks](plannertask.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="a0925-110">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="a0925-111">其也可以有 [plannerBuckets](plannerbucket.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="a0925-111">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="a0925-112">每个计划对象具有可以包含此计划的更多信息的[详细信息](plannerplandetails.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a0925-112">Each plan object has a [details](plannerplandetails.md) object that can contain more information about the plan.</span></span> <span data-ttu-id="a0925-113">有关组、计划和任务之间的关系的详细信息，请参阅 [Planner](planner-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="a0925-113">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a0925-114">方法</span><span class="sxs-lookup"><span data-stu-id="a0925-114">Methods</span></span>

| <span data-ttu-id="a0925-115">方法</span><span class="sxs-lookup"><span data-stu-id="a0925-115">Method</span></span>           | <span data-ttu-id="a0925-116">返回类型</span><span class="sxs-lookup"><span data-stu-id="a0925-116">Return Type</span></span>    |<span data-ttu-id="a0925-117">说明</span><span class="sxs-lookup"><span data-stu-id="a0925-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a0925-118">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="a0925-118">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="a0925-119">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="a0925-119">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="a0925-120">读取 **plannerPlan** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a0925-120">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="a0925-121">List buckets</span><span class="sxs-lookup"><span data-stu-id="a0925-121">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="a0925-122">[plannerBucket](plannerbucket.md) collection</span><span class="sxs-lookup"><span data-stu-id="a0925-122">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="a0925-123">获取 **plannerBucket** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a0925-123">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="a0925-124">List tasks</span><span class="sxs-lookup"><span data-stu-id="a0925-124">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="a0925-125">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="a0925-125">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="a0925-126">获取 **plannerTask** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a0925-126">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="a0925-127">Update</span><span class="sxs-lookup"><span data-stu-id="a0925-127">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="a0925-128">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="a0925-128">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="a0925-129">更新 **plannerPlan** 对象。</span><span class="sxs-lookup"><span data-stu-id="a0925-129">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a0925-130">属性</span><span class="sxs-lookup"><span data-stu-id="a0925-130">Properties</span></span>
| <span data-ttu-id="a0925-131">属性</span><span class="sxs-lookup"><span data-stu-id="a0925-131">Property</span></span>     | <span data-ttu-id="a0925-132">类型</span><span class="sxs-lookup"><span data-stu-id="a0925-132">Type</span></span>   |<span data-ttu-id="a0925-133">说明</span><span class="sxs-lookup"><span data-stu-id="a0925-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a0925-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a0925-134">createdDateTime</span></span>|<span data-ttu-id="a0925-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0925-135">DateTimeOffset</span></span>|<span data-ttu-id="a0925-136">只读。</span><span class="sxs-lookup"><span data-stu-id="a0925-136">Read-only.</span></span> <span data-ttu-id="a0925-137">创建计划的日期和时间</span><span class="sxs-lookup"><span data-stu-id="a0925-137">Date and time at which the plan is created.</span></span> <span data-ttu-id="a0925-138">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="a0925-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a0925-139">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="a0925-139">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="a0925-140">id</span><span class="sxs-lookup"><span data-stu-id="a0925-140">id</span></span>|<span data-ttu-id="a0925-141">字符串</span><span class="sxs-lookup"><span data-stu-id="a0925-141">String</span></span>| <span data-ttu-id="a0925-142">只读。</span><span class="sxs-lookup"><span data-stu-id="a0925-142">Read-only.</span></span> <span data-ttu-id="a0925-143">计划的 ID。</span><span class="sxs-lookup"><span data-stu-id="a0925-143">ID of the plan.</span></span> <span data-ttu-id="a0925-144">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="a0925-144">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="a0925-145">[格式验证](planner-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="a0925-145">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="a0925-146">Owner</span><span class="sxs-lookup"><span data-stu-id="a0925-146">owner</span></span>|<span data-ttu-id="a0925-147">String</span><span class="sxs-lookup"><span data-stu-id="a0925-147">String</span></span>|<span data-ttu-id="a0925-148">拥有计划的[组](group.md)的 ID。</span><span class="sxs-lookup"><span data-stu-id="a0925-148">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="a0925-149">必须存在有效的组才能设置此字段。</span><span class="sxs-lookup"><span data-stu-id="a0925-149">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="a0925-150">设置后，此属性无法更新。</span><span class="sxs-lookup"><span data-stu-id="a0925-150">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="a0925-151">title</span><span class="sxs-lookup"><span data-stu-id="a0925-151">title</span></span>|<span data-ttu-id="a0925-152">String</span><span class="sxs-lookup"><span data-stu-id="a0925-152">String</span></span>|<span data-ttu-id="a0925-153">必填。</span><span class="sxs-lookup"><span data-stu-id="a0925-153">Required.</span></span> <span data-ttu-id="a0925-154">计划的标题</span><span class="sxs-lookup"><span data-stu-id="a0925-154">Title of the plan.</span></span>|
|<span data-ttu-id="a0925-155">createdBy</span><span class="sxs-lookup"><span data-stu-id="a0925-155">createdBy</span></span>|[<span data-ttu-id="a0925-156">identitySet</span><span class="sxs-lookup"><span data-stu-id="a0925-156">identitySet</span></span>](identityset.md)|<span data-ttu-id="a0925-157">只读。</span><span class="sxs-lookup"><span data-stu-id="a0925-157">Read-only.</span></span> <span data-ttu-id="a0925-158">创建计划的用户。</span><span class="sxs-lookup"><span data-stu-id="a0925-158">The user who created the plan.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0925-159">关系</span><span class="sxs-lookup"><span data-stu-id="a0925-159">Relationships</span></span>
| <span data-ttu-id="a0925-160">关系</span><span class="sxs-lookup"><span data-stu-id="a0925-160">Relationship</span></span> | <span data-ttu-id="a0925-161">类型</span><span class="sxs-lookup"><span data-stu-id="a0925-161">Type</span></span>   |<span data-ttu-id="a0925-162">说明</span><span class="sxs-lookup"><span data-stu-id="a0925-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a0925-163">buckets</span><span class="sxs-lookup"><span data-stu-id="a0925-163">buckets</span></span>|<span data-ttu-id="a0925-164">[plannerBucket](plannerbucket.md) collection</span><span class="sxs-lookup"><span data-stu-id="a0925-164">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="a0925-p108">只读。可为 Null。计划中的存储桶集合。</span><span class="sxs-lookup"><span data-stu-id="a0925-p108">Read-only. Nullable. Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="a0925-168">详细信息</span><span class="sxs-lookup"><span data-stu-id="a0925-168">details</span></span>|[<span data-ttu-id="a0925-169">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="a0925-169">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="a0925-170">只读。</span><span class="sxs-lookup"><span data-stu-id="a0925-170">Read-only.</span></span> <span data-ttu-id="a0925-171">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="a0925-171">Nullable.</span></span> <span data-ttu-id="a0925-172">关于计划的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="a0925-172">Additional details about the plan.</span></span>|
|<span data-ttu-id="a0925-173">tasks</span><span class="sxs-lookup"><span data-stu-id="a0925-173">tasks</span></span>|<span data-ttu-id="a0925-174">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="a0925-174">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="a0925-175">只读。</span><span class="sxs-lookup"><span data-stu-id="a0925-175">Read-only.</span></span> <span data-ttu-id="a0925-176">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="a0925-176">Nullable.</span></span> <span data-ttu-id="a0925-177">计划中的任务集合。</span><span class="sxs-lookup"><span data-stu-id="a0925-177">Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a0925-178">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a0925-178">JSON representation</span></span>

<span data-ttu-id="a0925-179">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0925-179">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlan"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "owner": "String",
  "title": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

