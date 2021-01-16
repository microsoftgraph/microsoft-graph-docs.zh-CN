---
title: plannerPlan 资源类型
description: '**plannerPlan** 资源表示 Microsoft 365 中的计划。 计划可以由组所有，并包含 plannerTasks 集合。 其也可以有 plannerBuckets 集合。 每个计划对象具有可以包含此计划的更多信息的 details 对象。 有关组、计划和任务之间的关系的详细信息，请参阅“Planner”。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: e79b84bc77b81b02a408035acb34f89d2f990cc8
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883032"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="e450a-107">plannerPlan 资源类型</span><span class="sxs-lookup"><span data-stu-id="e450a-107">plannerPlan resource type</span></span>

<span data-ttu-id="e450a-108">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e450a-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e450a-109">**plannerPlan** 资源表示 Microsoft 365 中的计划。</span><span class="sxs-lookup"><span data-stu-id="e450a-109">The **plannerPlan** resource represents a plan in Microsoft 365.</span></span> <span data-ttu-id="e450a-110">计划可以由[组](group.md)所有，并包含 [plannerTasks](plannertask.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="e450a-110">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="e450a-111">其也可以有 [plannerBuckets](plannerbucket.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="e450a-111">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="e450a-112">每个计划对象具有可以包含此计划的更多信息的 [details](plannerplandetails.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e450a-112">Each plan object has a [details](plannerplandetails.md) object which can contain more information about the plan.</span></span> <span data-ttu-id="e450a-113">有关组、计划和任务之间的关系的详细信息，请参阅 [Planner](planner-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="e450a-113">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>



## <a name="methods"></a><span data-ttu-id="e450a-114">方法</span><span class="sxs-lookup"><span data-stu-id="e450a-114">Methods</span></span>

| <span data-ttu-id="e450a-115">方法</span><span class="sxs-lookup"><span data-stu-id="e450a-115">Method</span></span>           | <span data-ttu-id="e450a-116">返回类型</span><span class="sxs-lookup"><span data-stu-id="e450a-116">Return Type</span></span>    |<span data-ttu-id="e450a-117">说明</span><span class="sxs-lookup"><span data-stu-id="e450a-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e450a-118">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="e450a-118">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="e450a-119">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="e450a-119">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="e450a-120">读取 **plannerPlan** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e450a-120">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="e450a-121">List buckets</span><span class="sxs-lookup"><span data-stu-id="e450a-121">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="e450a-122">[plannerBucket](plannerbucket.md) collection</span><span class="sxs-lookup"><span data-stu-id="e450a-122">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="e450a-123">获取 **plannerBucket** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e450a-123">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="e450a-124">List tasks</span><span class="sxs-lookup"><span data-stu-id="e450a-124">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="e450a-125">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="e450a-125">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="e450a-126">获取 **plannerTask** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e450a-126">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="e450a-127">Update</span><span class="sxs-lookup"><span data-stu-id="e450a-127">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="e450a-128">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="e450a-128">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="e450a-129">更新 **plannerPlan** 对象。</span><span class="sxs-lookup"><span data-stu-id="e450a-129">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e450a-130">属性</span><span class="sxs-lookup"><span data-stu-id="e450a-130">Properties</span></span>
| <span data-ttu-id="e450a-131">属性</span><span class="sxs-lookup"><span data-stu-id="e450a-131">Property</span></span>     | <span data-ttu-id="e450a-132">类型</span><span class="sxs-lookup"><span data-stu-id="e450a-132">Type</span></span>   |<span data-ttu-id="e450a-133">说明</span><span class="sxs-lookup"><span data-stu-id="e450a-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e450a-134">容器</span><span class="sxs-lookup"><span data-stu-id="e450a-134">container</span></span>|[<span data-ttu-id="e450a-135">plannerPlanContainer</span><span class="sxs-lookup"><span data-stu-id="e450a-135">plannerPlanContainer</span></span>](../resources/plannerplancontainer.md)|<span data-ttu-id="e450a-136">标识计划的容器。</span><span class="sxs-lookup"><span data-stu-id="e450a-136">Identifies the container of the plan.</span></span> <span data-ttu-id="e450a-137">设置后，此属性无法更新。</span><span class="sxs-lookup"><span data-stu-id="e450a-137">After it is set, this property can’t be updated.</span></span> <span data-ttu-id="e450a-138">必需。</span><span class="sxs-lookup"><span data-stu-id="e450a-138">Required.</span></span>|
|<span data-ttu-id="e450a-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e450a-139">createdDateTime</span></span>|<span data-ttu-id="e450a-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e450a-140">DateTimeOffset</span></span>|<span data-ttu-id="e450a-p104">只读。创建计划的日期和时间时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e450a-p104">Read-only. Date and time at which the plan is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e450a-145">id</span><span class="sxs-lookup"><span data-stu-id="e450a-145">id</span></span>|<span data-ttu-id="e450a-146">String</span><span class="sxs-lookup"><span data-stu-id="e450a-146">String</span></span>| <span data-ttu-id="e450a-147">只读。</span><span class="sxs-lookup"><span data-stu-id="e450a-147">Read-only.</span></span> <span data-ttu-id="e450a-148">计划的 ID。</span><span class="sxs-lookup"><span data-stu-id="e450a-148">ID of the plan.</span></span> <span data-ttu-id="e450a-149">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="e450a-149">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="e450a-150">[格式验证](tasks-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="e450a-150">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="e450a-151">title</span><span class="sxs-lookup"><span data-stu-id="e450a-151">title</span></span>|<span data-ttu-id="e450a-152">String</span><span class="sxs-lookup"><span data-stu-id="e450a-152">String</span></span>|<span data-ttu-id="e450a-153">必填。</span><span class="sxs-lookup"><span data-stu-id="e450a-153">Required.</span></span> <span data-ttu-id="e450a-154">计划的标题</span><span class="sxs-lookup"><span data-stu-id="e450a-154">Title of the plan.</span></span>|
|<span data-ttu-id="e450a-155">createdBy</span><span class="sxs-lookup"><span data-stu-id="e450a-155">createdBy</span></span>|[<span data-ttu-id="e450a-156">identitySet</span><span class="sxs-lookup"><span data-stu-id="e450a-156">identitySet</span></span>](identityset.md)|<span data-ttu-id="e450a-157">只读。</span><span class="sxs-lookup"><span data-stu-id="e450a-157">Read-only.</span></span> <span data-ttu-id="e450a-158">创建计划的用户。</span><span class="sxs-lookup"><span data-stu-id="e450a-158">The user who created the plan.</span></span>|
|<span data-ttu-id="e450a-159">上下文</span><span class="sxs-lookup"><span data-stu-id="e450a-159">contexts</span></span>|[<span data-ttu-id="e450a-160">plannerPlanContextCollection</span><span class="sxs-lookup"><span data-stu-id="e450a-160">plannerPlanContextCollection</span></span>](plannerplancontextcollection.md)| <span data-ttu-id="e450a-161">只读。</span><span class="sxs-lookup"><span data-stu-id="e450a-161">Read-only.</span></span> <span data-ttu-id="e450a-162">在此计划中使用的其他用户体验，表示为 [plannerPlanContext](plannerplancontext.md) 条目。</span><span class="sxs-lookup"><span data-stu-id="e450a-162">Additional user experiences in which this plan is used, represented as [plannerPlanContext](plannerplancontext.md) entries.</span></span>|
|<span data-ttu-id="e450a-163">所有者 (已弃) </span><span class="sxs-lookup"><span data-stu-id="e450a-163">owner (deprecated)</span></span> |<span data-ttu-id="e450a-164">String</span><span class="sxs-lookup"><span data-stu-id="e450a-164">String</span></span>| <span data-ttu-id="e450a-165">请 **改为使用容器** 属性。</span><span class="sxs-lookup"><span data-stu-id="e450a-165">Use the **container** property instead.</span></span> <span data-ttu-id="e450a-166">拥有 [计划的](group.md) 组的 ID。</span><span class="sxs-lookup"><span data-stu-id="e450a-166">ID of the [group](group.md) that owns the plan.</span></span> <span data-ttu-id="e450a-167">设置后，此属性无法更新。</span><span class="sxs-lookup"><span data-stu-id="e450a-167">After it is set, this property can’t be updated.</span></span> <span data-ttu-id="e450a-168">如果计划的容器不是组，则此属性不会返回有效的组 ID。</span><span class="sxs-lookup"><span data-stu-id="e450a-168">This property will not return a valid group ID if the container of the plan is not a group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e450a-169">关系</span><span class="sxs-lookup"><span data-stu-id="e450a-169">Relationships</span></span>
| <span data-ttu-id="e450a-170">关系</span><span class="sxs-lookup"><span data-stu-id="e450a-170">Relationship</span></span> | <span data-ttu-id="e450a-171">类型</span><span class="sxs-lookup"><span data-stu-id="e450a-171">Type</span></span>   |<span data-ttu-id="e450a-172">说明</span><span class="sxs-lookup"><span data-stu-id="e450a-172">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e450a-173">buckets</span><span class="sxs-lookup"><span data-stu-id="e450a-173">buckets</span></span>|<span data-ttu-id="e450a-174">[plannerBucket](plannerbucket.md) collection</span><span class="sxs-lookup"><span data-stu-id="e450a-174">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="e450a-175">计划中的存储桶集合。</span><span class="sxs-lookup"><span data-stu-id="e450a-175">Collection of buckets in the plan.</span></span> <span data-ttu-id="e450a-176">只读。</span><span class="sxs-lookup"><span data-stu-id="e450a-176">Read-only.</span></span> <span data-ttu-id="e450a-177">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="e450a-177">Nullable.</span></span>|
|<span data-ttu-id="e450a-178">详细信息</span><span class="sxs-lookup"><span data-stu-id="e450a-178">details</span></span>|[<span data-ttu-id="e450a-179">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="e450a-179">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="e450a-180">关于计划的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="e450a-180">Additional details about the plan.</span></span> <span data-ttu-id="e450a-181">只读。</span><span class="sxs-lookup"><span data-stu-id="e450a-181">Read-only.</span></span> <span data-ttu-id="e450a-182">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="e450a-182">Nullable.</span></span> |
|<span data-ttu-id="e450a-183">tasks</span><span class="sxs-lookup"><span data-stu-id="e450a-183">tasks</span></span>|<span data-ttu-id="e450a-184">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="e450a-184">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="e450a-185">计划中的任务集合。</span><span class="sxs-lookup"><span data-stu-id="e450a-185">Collection of tasks in the plan.</span></span> <span data-ttu-id="e450a-186">只读。</span><span class="sxs-lookup"><span data-stu-id="e450a-186">Read-only.</span></span> <span data-ttu-id="e450a-187">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="e450a-187">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e450a-188">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e450a-188">JSON representation</span></span>

<span data-ttu-id="e450a-189">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e450a-189">Here is a JSON representation of the resource.</span></span>

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


