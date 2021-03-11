---
title: plannerPlan 资源类型
description: '**plannerPlan** 资源表示 Microsoft 365 中的计划。 计划可以由组所有，并包含 plannerTasks 集合。 其也可以有 plannerBuckets 集合。 每个计划对象具有可以包含此计划的更多信息的 details 对象。 有关组、计划和任务之间的关系的详细信息，请参阅“Planner”。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 4763f268628a4609ac91d0597aeb4f55a2d406ce
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720989"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="945b9-107">plannerPlan 资源类型</span><span class="sxs-lookup"><span data-stu-id="945b9-107">plannerPlan resource type</span></span>

<span data-ttu-id="945b9-108">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="945b9-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="945b9-109">**plannerPlan** 资源表示 Microsoft 365 中的计划。</span><span class="sxs-lookup"><span data-stu-id="945b9-109">The **plannerPlan** resource represents a plan in Microsoft 365.</span></span> <span data-ttu-id="945b9-110">计划可以由[组](group.md)所有，并包含 [plannerTasks](plannertask.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="945b9-110">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="945b9-111">其也可以有 [plannerBuckets](plannerbucket.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="945b9-111">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="945b9-112">每个计划对象具有可以包含此计划的更多信息的 [details](plannerplandetails.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="945b9-112">Each plan object has a [details](plannerplandetails.md) object which can contain more information about the plan.</span></span> <span data-ttu-id="945b9-113">有关组、计划和任务之间的关系的详细信息，请参阅 [Planner](planner-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="945b9-113">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>



## <a name="methods"></a><span data-ttu-id="945b9-114">方法</span><span class="sxs-lookup"><span data-stu-id="945b9-114">Methods</span></span>

| <span data-ttu-id="945b9-115">方法</span><span class="sxs-lookup"><span data-stu-id="945b9-115">Method</span></span>           | <span data-ttu-id="945b9-116">返回类型</span><span class="sxs-lookup"><span data-stu-id="945b9-116">Return Type</span></span>    |<span data-ttu-id="945b9-117">说明</span><span class="sxs-lookup"><span data-stu-id="945b9-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="945b9-118">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="945b9-118">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="945b9-119">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="945b9-119">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="945b9-120">读取 **plannerPlan** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="945b9-120">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="945b9-121">List buckets</span><span class="sxs-lookup"><span data-stu-id="945b9-121">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="945b9-122">[plannerBucket](plannerbucket.md) collection</span><span class="sxs-lookup"><span data-stu-id="945b9-122">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="945b9-123">获取 **plannerBucket** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="945b9-123">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="945b9-124">List tasks</span><span class="sxs-lookup"><span data-stu-id="945b9-124">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="945b9-125">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="945b9-125">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="945b9-126">获取 **plannerTask** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="945b9-126">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="945b9-127">Update</span><span class="sxs-lookup"><span data-stu-id="945b9-127">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="945b9-128">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="945b9-128">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="945b9-129">更新 **plannerPlan** 对象。</span><span class="sxs-lookup"><span data-stu-id="945b9-129">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="945b9-130">属性</span><span class="sxs-lookup"><span data-stu-id="945b9-130">Properties</span></span>
| <span data-ttu-id="945b9-131">属性</span><span class="sxs-lookup"><span data-stu-id="945b9-131">Property</span></span>     | <span data-ttu-id="945b9-132">类型</span><span class="sxs-lookup"><span data-stu-id="945b9-132">Type</span></span>   |<span data-ttu-id="945b9-133">说明</span><span class="sxs-lookup"><span data-stu-id="945b9-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="945b9-134">容器</span><span class="sxs-lookup"><span data-stu-id="945b9-134">container</span></span>|[<span data-ttu-id="945b9-135">plannerPlanContainer</span><span class="sxs-lookup"><span data-stu-id="945b9-135">plannerPlanContainer</span></span>](../resources/plannerplancontainer.md)|<span data-ttu-id="945b9-136">标识计划的容器。</span><span class="sxs-lookup"><span data-stu-id="945b9-136">Identifies the container of the plan.</span></span> <span data-ttu-id="945b9-137">设置后，此属性无法更新。</span><span class="sxs-lookup"><span data-stu-id="945b9-137">After it is set, this property can’t be updated.</span></span> <span data-ttu-id="945b9-138">必需。</span><span class="sxs-lookup"><span data-stu-id="945b9-138">Required.</span></span>|
|<span data-ttu-id="945b9-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="945b9-139">createdDateTime</span></span>|<span data-ttu-id="945b9-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="945b9-140">DateTimeOffset</span></span>|<span data-ttu-id="945b9-141">只读。</span><span class="sxs-lookup"><span data-stu-id="945b9-141">Read-only.</span></span> <span data-ttu-id="945b9-142">创建计划的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="945b9-142">Date and time at which the plan is created.</span></span> <span data-ttu-id="945b9-143">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="945b9-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="945b9-144">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="945b9-144">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="945b9-145">id</span><span class="sxs-lookup"><span data-stu-id="945b9-145">id</span></span>|<span data-ttu-id="945b9-146">String</span><span class="sxs-lookup"><span data-stu-id="945b9-146">String</span></span>| <span data-ttu-id="945b9-147">只读。</span><span class="sxs-lookup"><span data-stu-id="945b9-147">Read-only.</span></span> <span data-ttu-id="945b9-148">计划的 ID。</span><span class="sxs-lookup"><span data-stu-id="945b9-148">ID of the plan.</span></span> <span data-ttu-id="945b9-149">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="945b9-149">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="945b9-150">[格式验证](tasks-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="945b9-150">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="945b9-151">title</span><span class="sxs-lookup"><span data-stu-id="945b9-151">title</span></span>|<span data-ttu-id="945b9-152">String</span><span class="sxs-lookup"><span data-stu-id="945b9-152">String</span></span>|<span data-ttu-id="945b9-153">必填。</span><span class="sxs-lookup"><span data-stu-id="945b9-153">Required.</span></span> <span data-ttu-id="945b9-154">计划的标题</span><span class="sxs-lookup"><span data-stu-id="945b9-154">Title of the plan.</span></span>|
|<span data-ttu-id="945b9-155">createdBy</span><span class="sxs-lookup"><span data-stu-id="945b9-155">createdBy</span></span>|[<span data-ttu-id="945b9-156">identitySet</span><span class="sxs-lookup"><span data-stu-id="945b9-156">identitySet</span></span>](identityset.md)|<span data-ttu-id="945b9-157">只读。</span><span class="sxs-lookup"><span data-stu-id="945b9-157">Read-only.</span></span> <span data-ttu-id="945b9-158">创建计划的用户。</span><span class="sxs-lookup"><span data-stu-id="945b9-158">The user who created the plan.</span></span>|
|<span data-ttu-id="945b9-159">上下文</span><span class="sxs-lookup"><span data-stu-id="945b9-159">contexts</span></span>|[<span data-ttu-id="945b9-160">plannerPlanContextCollection</span><span class="sxs-lookup"><span data-stu-id="945b9-160">plannerPlanContextCollection</span></span>](plannerplancontextcollection.md)| <span data-ttu-id="945b9-161">只读。</span><span class="sxs-lookup"><span data-stu-id="945b9-161">Read-only.</span></span> <span data-ttu-id="945b9-162">在此计划中使用的其他用户体验，表示为 [plannerPlanContext](plannerplancontext.md) 条目。</span><span class="sxs-lookup"><span data-stu-id="945b9-162">Additional user experiences in which this plan is used, represented as [plannerPlanContext](plannerplancontext.md) entries.</span></span>|
|<span data-ttu-id="945b9-163">所有者 (已弃) </span><span class="sxs-lookup"><span data-stu-id="945b9-163">owner (deprecated)</span></span> |<span data-ttu-id="945b9-164">String</span><span class="sxs-lookup"><span data-stu-id="945b9-164">String</span></span>| <span data-ttu-id="945b9-165">请 **改为使用容器** 属性。</span><span class="sxs-lookup"><span data-stu-id="945b9-165">Use the **container** property instead.</span></span> <span data-ttu-id="945b9-166">拥有 [计划的](group.md) 组的 ID。</span><span class="sxs-lookup"><span data-stu-id="945b9-166">ID of the [group](group.md) that owns the plan.</span></span> <span data-ttu-id="945b9-167">设置后，此属性无法更新。</span><span class="sxs-lookup"><span data-stu-id="945b9-167">After it is set, this property can’t be updated.</span></span> <span data-ttu-id="945b9-168">如果计划的容器不是组，则此属性不会返回有效的组 ID。</span><span class="sxs-lookup"><span data-stu-id="945b9-168">This property will not return a valid group ID if the container of the plan is not a group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="945b9-169">关系</span><span class="sxs-lookup"><span data-stu-id="945b9-169">Relationships</span></span>
| <span data-ttu-id="945b9-170">关系</span><span class="sxs-lookup"><span data-stu-id="945b9-170">Relationship</span></span> | <span data-ttu-id="945b9-171">类型</span><span class="sxs-lookup"><span data-stu-id="945b9-171">Type</span></span>   |<span data-ttu-id="945b9-172">说明</span><span class="sxs-lookup"><span data-stu-id="945b9-172">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="945b9-173">buckets</span><span class="sxs-lookup"><span data-stu-id="945b9-173">buckets</span></span>|<span data-ttu-id="945b9-174">[plannerBucket](plannerbucket.md) collection</span><span class="sxs-lookup"><span data-stu-id="945b9-174">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="945b9-175">计划中的存储桶集合。</span><span class="sxs-lookup"><span data-stu-id="945b9-175">Collection of buckets in the plan.</span></span> <span data-ttu-id="945b9-176">只读。</span><span class="sxs-lookup"><span data-stu-id="945b9-176">Read-only.</span></span> <span data-ttu-id="945b9-177">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="945b9-177">Nullable.</span></span>|
|<span data-ttu-id="945b9-178">详细信息</span><span class="sxs-lookup"><span data-stu-id="945b9-178">details</span></span>|[<span data-ttu-id="945b9-179">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="945b9-179">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="945b9-180">关于计划的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="945b9-180">Additional details about the plan.</span></span> <span data-ttu-id="945b9-181">只读。</span><span class="sxs-lookup"><span data-stu-id="945b9-181">Read-only.</span></span> <span data-ttu-id="945b9-182">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="945b9-182">Nullable.</span></span> |
|<span data-ttu-id="945b9-183">tasks</span><span class="sxs-lookup"><span data-stu-id="945b9-183">tasks</span></span>|<span data-ttu-id="945b9-184">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="945b9-184">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="945b9-185">计划中的任务集合。</span><span class="sxs-lookup"><span data-stu-id="945b9-185">Collection of tasks in the plan.</span></span> <span data-ttu-id="945b9-186">只读。</span><span class="sxs-lookup"><span data-stu-id="945b9-186">Read-only.</span></span> <span data-ttu-id="945b9-187">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="945b9-187">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="945b9-188">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="945b9-188">JSON representation</span></span>

<span data-ttu-id="945b9-189">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="945b9-189">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.plannerPlan"
}-->

```json
{
  "contexts": {
    "48#19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype": {
        "@odata.type": "#microsoft.graph.plannerPlanContext",
        "associationType": "Board",
        "createdDateTime": "2015-10-14T00:57:28.4698344Z",
        "displayNameSegments": [
            "Finance Team",
            "Budget Plans"
        ],
        "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
    }
  },
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "container": {
    "@odata.type": "microsoft.graph.plannerPlanContainer",
    "url": "String",
    "containerId": "String",
    "type": "String"
  },
  "title": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


