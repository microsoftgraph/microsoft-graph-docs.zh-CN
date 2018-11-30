---
title: plannerPlan 资源类型
description: '**PlannerPlan**资源表示 Office 365 中的计划。 规划组可以拥有和包含 plannerTasks 的集合。 它还可以具有 plannerBuckets 的集合。 每个计划对象都可以包含有关计划的详细信息的详细信息对象。 有关组、 计划和任务之间的关系的详细信息，请参阅计划程序。'
ms.openlocfilehash: 236b6cb5d35e11a30bcb4371e0563b56ac93de8f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043678"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="645c5-107">plannerPlan 资源类型</span><span class="sxs-lookup"><span data-stu-id="645c5-107">plannerPlan resource type</span></span>

> <span data-ttu-id="645c5-108">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="645c5-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="645c5-109">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="645c5-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="645c5-110">**PlannerPlan**资源表示 Office 365 中的计划。</span><span class="sxs-lookup"><span data-stu-id="645c5-110">The **plannerPlan** resource represents a plan in Office 365.</span></span> <span data-ttu-id="645c5-111">规划[组](group.md)可以拥有和包含[plannerTasks](plannertask.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="645c5-111">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="645c5-112">它还可以具有的[plannerBuckets](plannerbucket.md)集合。</span><span class="sxs-lookup"><span data-stu-id="645c5-112">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="645c5-113">每个计划对象都可以包含有关计划的详细信息的[详细信息](plannerplandetails.md)对象。</span><span class="sxs-lookup"><span data-stu-id="645c5-113">Each plan object has a [details](plannerplandetails.md) object which can contain more information about the plan.</span></span> <span data-ttu-id="645c5-114">有关组、 计划和任务之间的关系的详细信息，请参阅[计划程序](planner-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="645c5-114">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>



## <a name="methods"></a><span data-ttu-id="645c5-115">方法</span><span class="sxs-lookup"><span data-stu-id="645c5-115">Methods</span></span>

| <span data-ttu-id="645c5-116">方法</span><span class="sxs-lookup"><span data-stu-id="645c5-116">Method</span></span>           | <span data-ttu-id="645c5-117">返回类型</span><span class="sxs-lookup"><span data-stu-id="645c5-117">Return Type</span></span>    |<span data-ttu-id="645c5-118">说明</span><span class="sxs-lookup"><span data-stu-id="645c5-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="645c5-119">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="645c5-119">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="645c5-120">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="645c5-120">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="645c5-121">读取 **plannerPlan** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="645c5-121">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="645c5-122">列出存储桶</span><span class="sxs-lookup"><span data-stu-id="645c5-122">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="645c5-123">[plannerBucket](plannerbucket.md) collection</span><span class="sxs-lookup"><span data-stu-id="645c5-123">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="645c5-124">获取 **plannerBucket** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="645c5-124">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="645c5-125">List tasks</span><span class="sxs-lookup"><span data-stu-id="645c5-125">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="645c5-126">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="645c5-126">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="645c5-127">获取 **plannerTask** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="645c5-127">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="645c5-128">Update</span><span class="sxs-lookup"><span data-stu-id="645c5-128">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="645c5-129">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="645c5-129">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="645c5-130">更新 **plannerPlan** 对象。</span><span class="sxs-lookup"><span data-stu-id="645c5-130">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="645c5-131">属性</span><span class="sxs-lookup"><span data-stu-id="645c5-131">Properties</span></span>
| <span data-ttu-id="645c5-132">属性</span><span class="sxs-lookup"><span data-stu-id="645c5-132">Property</span></span>     | <span data-ttu-id="645c5-133">类型</span><span class="sxs-lookup"><span data-stu-id="645c5-133">Type</span></span>   |<span data-ttu-id="645c5-134">说明</span><span class="sxs-lookup"><span data-stu-id="645c5-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="645c5-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="645c5-135">createdDateTime</span></span>|<span data-ttu-id="645c5-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="645c5-136">DateTimeOffset</span></span>|<span data-ttu-id="645c5-p104">只读。创建计划的日期和时间时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="645c5-p104">Read-only. Date and time at which the plan is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="645c5-141">id</span><span class="sxs-lookup"><span data-stu-id="645c5-141">id</span></span>|<span data-ttu-id="645c5-142">String</span><span class="sxs-lookup"><span data-stu-id="645c5-142">String</span></span>| <span data-ttu-id="645c5-143">只读。</span><span class="sxs-lookup"><span data-stu-id="645c5-143">Read-only.</span></span> <span data-ttu-id="645c5-144">在计划的 ID。</span><span class="sxs-lookup"><span data-stu-id="645c5-144">ID of the plan.</span></span> <span data-ttu-id="645c5-145">它是 28 字符长度和区分大小写。</span><span class="sxs-lookup"><span data-stu-id="645c5-145">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="645c5-146">服务上执行[格式验证](tasks-identifiers-disclaimer.md)。</span><span class="sxs-lookup"><span data-stu-id="645c5-146">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="645c5-147">owner</span><span class="sxs-lookup"><span data-stu-id="645c5-147">owner</span></span>|<span data-ttu-id="645c5-148">字符串</span><span class="sxs-lookup"><span data-stu-id="645c5-148">String</span></span>|<span data-ttu-id="645c5-149">拥有计划的[组](group.md)ID。</span><span class="sxs-lookup"><span data-stu-id="645c5-149">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="645c5-150">此字段可以设置之前，必须存在有效的组。</span><span class="sxs-lookup"><span data-stu-id="645c5-150">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="645c5-151">设置后，无法更新此属性。</span><span class="sxs-lookup"><span data-stu-id="645c5-151">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="645c5-152">title</span><span class="sxs-lookup"><span data-stu-id="645c5-152">title</span></span>|<span data-ttu-id="645c5-153">String</span><span class="sxs-lookup"><span data-stu-id="645c5-153">String</span></span>|<span data-ttu-id="645c5-p107">必填。计划的标题</span><span class="sxs-lookup"><span data-stu-id="645c5-p107">Required. Title of the plan.</span></span>|
|<span data-ttu-id="645c5-156">createdBy</span><span class="sxs-lookup"><span data-stu-id="645c5-156">createdBy</span></span>|[<span data-ttu-id="645c5-157">identitySet</span><span class="sxs-lookup"><span data-stu-id="645c5-157">identitySet</span></span>](identityset.md)|<span data-ttu-id="645c5-p108">只读。创建计划的用户。</span><span class="sxs-lookup"><span data-stu-id="645c5-p108">Read-only. The user who created the plan.</span></span>|
|<span data-ttu-id="645c5-160">上下文</span><span class="sxs-lookup"><span data-stu-id="645c5-160">contexts</span></span>|[<span data-ttu-id="645c5-161">plannerPlanContextCollection</span><span class="sxs-lookup"><span data-stu-id="645c5-161">plannerPlanContextCollection</span></span>](plannerplancontextcollection.md)| <span data-ttu-id="645c5-162">只读。</span><span class="sxs-lookup"><span data-stu-id="645c5-162">Read-only.</span></span> <span data-ttu-id="645c5-163">使用此计划的其他用户体验表示为[plannerPlanContext](plannerplancontext.md)条目。</span><span class="sxs-lookup"><span data-stu-id="645c5-163">Additional user experiences in which this plan is used, represented as [plannerPlanContext](plannerplancontext.md) entries.</span></span>|

## <a name="relationships"></a><span data-ttu-id="645c5-164">Relationships</span><span class="sxs-lookup"><span data-stu-id="645c5-164">Relationships</span></span>
| <span data-ttu-id="645c5-165">关系</span><span class="sxs-lookup"><span data-stu-id="645c5-165">Relationship</span></span> | <span data-ttu-id="645c5-166">类型</span><span class="sxs-lookup"><span data-stu-id="645c5-166">Type</span></span>   |<span data-ttu-id="645c5-167">说明</span><span class="sxs-lookup"><span data-stu-id="645c5-167">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="645c5-168">buckets</span><span class="sxs-lookup"><span data-stu-id="645c5-168">buckets</span></span>|<span data-ttu-id="645c5-169">[plannerBucket](plannerbucket.md) collection</span><span class="sxs-lookup"><span data-stu-id="645c5-169">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="645c5-p110">只读。可为 Null。计划中的存储桶集合。</span><span class="sxs-lookup"><span data-stu-id="645c5-p110">Read-only. Nullable. Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="645c5-173">详细信息</span><span class="sxs-lookup"><span data-stu-id="645c5-173">details</span></span>|[<span data-ttu-id="645c5-174">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="645c5-174">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="645c5-p111">只读。可为 NULL。关于计划的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="645c5-p111">Read-only. Nullable. Additional details about the plan.</span></span>|
|<span data-ttu-id="645c5-178">tasks</span><span class="sxs-lookup"><span data-stu-id="645c5-178">tasks</span></span>|<span data-ttu-id="645c5-179">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="645c5-179">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="645c5-p112">只读。可为 Null。计划中的任务集合。</span><span class="sxs-lookup"><span data-stu-id="645c5-p112">Read-only. Nullable. Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="645c5-183">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="645c5-183">JSON representation</span></span>

<span data-ttu-id="645c5-184">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="645c5-184">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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