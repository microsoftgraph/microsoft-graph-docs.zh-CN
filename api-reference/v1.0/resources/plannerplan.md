---
title: plannerPlan 资源类型
description: '**PlannerPlan**资源表示 Office 365 中的计划。 规划组可以拥有和包含 plannerTasks 的集合。 它还可以具有 plannerBuckets 的集合。 每个计划对象有一个详细对象，可以包含有关计划的详细信息。 有关组、 计划和任务之间的关系的详细信息，请参阅计划程序。'
localization_priority: Priority
ms.openlocfilehash: cfcc94fab067cc76bb530edbdb8477183ebf3531
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873008"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="1550b-107">plannerPlan 资源类型</span><span class="sxs-lookup"><span data-stu-id="1550b-107">plannerPlan resource type</span></span>

<span data-ttu-id="1550b-p102">**plannerPlan** 资源表示 Office 365 中的计划。计划可以由[组](group.md)所有，并包含 [plannerTasks](plannertask.md) 集合。其也可以有 [plannerBuckets](plannerbucket.md) 集合。每个计划对象具有可以包含此计划的更多信息的[详细信息](plannerplandetails.md)对象。有关组、计划和任务之间的关系的详细信息，请参阅 [Planner](planner-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="1550b-p102">The **plannerPlan** resource represents a plan in Office 365. A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md). It can also have a collection of [plannerBuckets](plannerbucket.md). Each plan object has a [details](plannerplandetails.md) object that can contain more information about the plan. For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1550b-113">方法</span><span class="sxs-lookup"><span data-stu-id="1550b-113">Methods</span></span>

| <span data-ttu-id="1550b-114">方法</span><span class="sxs-lookup"><span data-stu-id="1550b-114">Method</span></span>           | <span data-ttu-id="1550b-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="1550b-115">Return Type</span></span>    |<span data-ttu-id="1550b-116">说明</span><span class="sxs-lookup"><span data-stu-id="1550b-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1550b-117">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="1550b-117">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="1550b-118">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="1550b-118">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="1550b-119">读取 **plannerPlan** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1550b-119">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="1550b-120">列出存储桶</span><span class="sxs-lookup"><span data-stu-id="1550b-120">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="1550b-121">[plannerBucket](plannerbucket.md) collection</span><span class="sxs-lookup"><span data-stu-id="1550b-121">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="1550b-122">获取 **plannerBucket** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1550b-122">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="1550b-123">List tasks</span><span class="sxs-lookup"><span data-stu-id="1550b-123">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="1550b-124">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="1550b-124">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="1550b-125">获取 **plannerTask** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1550b-125">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="1550b-126">Update</span><span class="sxs-lookup"><span data-stu-id="1550b-126">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="1550b-127">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="1550b-127">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="1550b-128">更新 **plannerPlan** 对象。</span><span class="sxs-lookup"><span data-stu-id="1550b-128">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1550b-129">属性</span><span class="sxs-lookup"><span data-stu-id="1550b-129">Properties</span></span>
| <span data-ttu-id="1550b-130">属性</span><span class="sxs-lookup"><span data-stu-id="1550b-130">Property</span></span>     | <span data-ttu-id="1550b-131">类型</span><span class="sxs-lookup"><span data-stu-id="1550b-131">Type</span></span>   |<span data-ttu-id="1550b-132">说明</span><span class="sxs-lookup"><span data-stu-id="1550b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1550b-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1550b-133">createdDateTime</span></span>|<span data-ttu-id="1550b-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1550b-134">DateTimeOffset</span></span>|<span data-ttu-id="1550b-p103">只读。创建计划的日期和时间时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="1550b-p103">Read-only. Date and time at which the plan is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="1550b-139">id</span><span class="sxs-lookup"><span data-stu-id="1550b-139">id</span></span>|<span data-ttu-id="1550b-140">String</span><span class="sxs-lookup"><span data-stu-id="1550b-140">String</span></span>| <span data-ttu-id="1550b-141">只读。</span><span class="sxs-lookup"><span data-stu-id="1550b-141">Read-only.</span></span> <span data-ttu-id="1550b-142">在计划的 ID。</span><span class="sxs-lookup"><span data-stu-id="1550b-142">ID of the plan.</span></span> <span data-ttu-id="1550b-143">它是 28 字符长度和区分大小写。</span><span class="sxs-lookup"><span data-stu-id="1550b-143">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="1550b-144">服务上执行[格式验证](planner-identifiers-disclaimer.md)。</span><span class="sxs-lookup"><span data-stu-id="1550b-144">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="1550b-145">owner</span><span class="sxs-lookup"><span data-stu-id="1550b-145">owner</span></span>|<span data-ttu-id="1550b-146">字符串</span><span class="sxs-lookup"><span data-stu-id="1550b-146">String</span></span>|<span data-ttu-id="1550b-147">拥有计划的[组](group.md)ID。</span><span class="sxs-lookup"><span data-stu-id="1550b-147">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="1550b-148">此字段可以设置之前，必须存在有效的组。</span><span class="sxs-lookup"><span data-stu-id="1550b-148">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="1550b-149">设置后，无法更新此属性。</span><span class="sxs-lookup"><span data-stu-id="1550b-149">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="1550b-150">title</span><span class="sxs-lookup"><span data-stu-id="1550b-150">title</span></span>|<span data-ttu-id="1550b-151">String</span><span class="sxs-lookup"><span data-stu-id="1550b-151">String</span></span>|<span data-ttu-id="1550b-p106">必填。计划的标题</span><span class="sxs-lookup"><span data-stu-id="1550b-p106">Required. Title of the plan.</span></span>|
|<span data-ttu-id="1550b-154">createdBy</span><span class="sxs-lookup"><span data-stu-id="1550b-154">createdBy</span></span>|[<span data-ttu-id="1550b-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="1550b-155">identitySet</span></span>](identityset.md)|<span data-ttu-id="1550b-p107">只读。创建计划的用户。</span><span class="sxs-lookup"><span data-stu-id="1550b-p107">Read-only. The user who created the plan.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1550b-158">关系</span><span class="sxs-lookup"><span data-stu-id="1550b-158">Relationships</span></span>
| <span data-ttu-id="1550b-159">关系</span><span class="sxs-lookup"><span data-stu-id="1550b-159">Relationship</span></span> | <span data-ttu-id="1550b-160">类型</span><span class="sxs-lookup"><span data-stu-id="1550b-160">Type</span></span>   |<span data-ttu-id="1550b-161">说明</span><span class="sxs-lookup"><span data-stu-id="1550b-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1550b-162">buckets</span><span class="sxs-lookup"><span data-stu-id="1550b-162">buckets</span></span>|<span data-ttu-id="1550b-163">[plannerBucket](plannerbucket.md) collection</span><span class="sxs-lookup"><span data-stu-id="1550b-163">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="1550b-p108">只读。可为 Null。计划中的存储桶集合。</span><span class="sxs-lookup"><span data-stu-id="1550b-p108">Read-only. Nullable. Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="1550b-167">详细信息</span><span class="sxs-lookup"><span data-stu-id="1550b-167">details</span></span>|[<span data-ttu-id="1550b-168">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="1550b-168">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="1550b-p109">只读。可为 NULL。关于计划的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="1550b-p109">Read-only. Nullable. Additional details about the plan.</span></span>|
|<span data-ttu-id="1550b-172">tasks</span><span class="sxs-lookup"><span data-stu-id="1550b-172">tasks</span></span>|<span data-ttu-id="1550b-173">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="1550b-173">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="1550b-p110">只读。可为 Null。计划中的任务集合。</span><span class="sxs-lookup"><span data-stu-id="1550b-p110">Read-only. Nullable. Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1550b-177">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1550b-177">JSON representation</span></span>

<span data-ttu-id="1550b-178">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1550b-178">Here is a JSON representation of the resource.</span></span>

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
