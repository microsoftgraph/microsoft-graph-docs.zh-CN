---
title: plannerPlan 资源类型
description: '**plannerPlan** 资源表示 Office 365 中的计划。 计划可以由组所有，并包含 plannerTasks 集合。 其也可以有 plannerBuckets 集合。 每个计划对象具有可以包含此计划的更多信息的详细信息对象。 有关组、计划和任务之间的关系的详细信息，请参阅“Planner”。'
localization_priority: Priority
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 1f928252963c7796a396e1e342b413d135fb1764
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035180"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="91d53-107">plannerPlan 资源类型</span><span class="sxs-lookup"><span data-stu-id="91d53-107">plannerPlan resource type</span></span>

<span data-ttu-id="91d53-108">**plannerPlan** 资源表示 Office 365 中的计划。</span><span class="sxs-lookup"><span data-stu-id="91d53-108">The **plannerPlan** resource represents a plan in Office 365.</span></span> <span data-ttu-id="91d53-109">计划可以由[组](group.md)所有，并包含 [plannerTasks](plannertask.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="91d53-109">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="91d53-110">其也可以有 [plannerBuckets](plannerbucket.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="91d53-110">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="91d53-111">每个计划对象具有可以包含此计划的更多信息的[详细信息](plannerplandetails.md)对象。</span><span class="sxs-lookup"><span data-stu-id="91d53-111">Each plan object has a [details](plannerplandetails.md) object that can contain more information about the plan.</span></span> <span data-ttu-id="91d53-112">有关组、计划和任务之间的关系的详细信息，请参阅 [Planner](planner-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="91d53-112">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="91d53-113">方法</span><span class="sxs-lookup"><span data-stu-id="91d53-113">Methods</span></span>

| <span data-ttu-id="91d53-114">方法</span><span class="sxs-lookup"><span data-stu-id="91d53-114">Method</span></span>           | <span data-ttu-id="91d53-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="91d53-115">Return Type</span></span>    |<span data-ttu-id="91d53-116">说明</span><span class="sxs-lookup"><span data-stu-id="91d53-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="91d53-117">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="91d53-117">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="91d53-118">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="91d53-118">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="91d53-119">读取 **plannerPlan** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="91d53-119">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="91d53-120">List buckets</span><span class="sxs-lookup"><span data-stu-id="91d53-120">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="91d53-121">[plannerBucket](plannerbucket.md) collection</span><span class="sxs-lookup"><span data-stu-id="91d53-121">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="91d53-122">获取 **plannerBucket** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="91d53-122">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="91d53-123">List tasks</span><span class="sxs-lookup"><span data-stu-id="91d53-123">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="91d53-124">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="91d53-124">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="91d53-125">获取 **plannerTask** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="91d53-125">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="91d53-126">Update</span><span class="sxs-lookup"><span data-stu-id="91d53-126">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="91d53-127">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="91d53-127">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="91d53-128">更新 **plannerPlan** 对象。</span><span class="sxs-lookup"><span data-stu-id="91d53-128">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="91d53-129">属性</span><span class="sxs-lookup"><span data-stu-id="91d53-129">Properties</span></span>
| <span data-ttu-id="91d53-130">属性</span><span class="sxs-lookup"><span data-stu-id="91d53-130">Property</span></span>     | <span data-ttu-id="91d53-131">类型</span><span class="sxs-lookup"><span data-stu-id="91d53-131">Type</span></span>   |<span data-ttu-id="91d53-132">说明</span><span class="sxs-lookup"><span data-stu-id="91d53-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91d53-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="91d53-133">createdDateTime</span></span>|<span data-ttu-id="91d53-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91d53-134">DateTimeOffset</span></span>|<span data-ttu-id="91d53-p103">只读。创建计划的日期和时间时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="91d53-p103">Read-only. Date and time at which the plan is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="91d53-139">id</span><span class="sxs-lookup"><span data-stu-id="91d53-139">id</span></span>|<span data-ttu-id="91d53-140">String</span><span class="sxs-lookup"><span data-stu-id="91d53-140">String</span></span>| <span data-ttu-id="91d53-141">只读。</span><span class="sxs-lookup"><span data-stu-id="91d53-141">Read-only.</span></span> <span data-ttu-id="91d53-142">计划的 ID。</span><span class="sxs-lookup"><span data-stu-id="91d53-142">ID of the plan.</span></span> <span data-ttu-id="91d53-143">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="91d53-143">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="91d53-144">[格式验证](planner-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="91d53-144">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="91d53-145">Owner</span><span class="sxs-lookup"><span data-stu-id="91d53-145">owner</span></span>|<span data-ttu-id="91d53-146">String</span><span class="sxs-lookup"><span data-stu-id="91d53-146">String</span></span>|<span data-ttu-id="91d53-147">拥有计划的[组](group.md)的 ID。</span><span class="sxs-lookup"><span data-stu-id="91d53-147">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="91d53-148">必须存在有效的组才能设置此字段。</span><span class="sxs-lookup"><span data-stu-id="91d53-148">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="91d53-149">设置后，此属性无法更新。</span><span class="sxs-lookup"><span data-stu-id="91d53-149">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="91d53-150">title</span><span class="sxs-lookup"><span data-stu-id="91d53-150">title</span></span>|<span data-ttu-id="91d53-151">String</span><span class="sxs-lookup"><span data-stu-id="91d53-151">String</span></span>|<span data-ttu-id="91d53-152">必填。</span><span class="sxs-lookup"><span data-stu-id="91d53-152">Required.</span></span> <span data-ttu-id="91d53-153">计划的标题</span><span class="sxs-lookup"><span data-stu-id="91d53-153">Title of the plan.</span></span>|
|<span data-ttu-id="91d53-154">createdBy</span><span class="sxs-lookup"><span data-stu-id="91d53-154">createdBy</span></span>|[<span data-ttu-id="91d53-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="91d53-155">identitySet</span></span>](identityset.md)|<span data-ttu-id="91d53-156">只读。</span><span class="sxs-lookup"><span data-stu-id="91d53-156">Read-only.</span></span> <span data-ttu-id="91d53-157">创建计划的用户。</span><span class="sxs-lookup"><span data-stu-id="91d53-157">The user who created the plan.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91d53-158">关系</span><span class="sxs-lookup"><span data-stu-id="91d53-158">Relationships</span></span>
| <span data-ttu-id="91d53-159">关系</span><span class="sxs-lookup"><span data-stu-id="91d53-159">Relationship</span></span> | <span data-ttu-id="91d53-160">类型</span><span class="sxs-lookup"><span data-stu-id="91d53-160">Type</span></span>   |<span data-ttu-id="91d53-161">说明</span><span class="sxs-lookup"><span data-stu-id="91d53-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91d53-162">buckets</span><span class="sxs-lookup"><span data-stu-id="91d53-162">buckets</span></span>|<span data-ttu-id="91d53-163">[plannerBucket](plannerbucket.md) collection</span><span class="sxs-lookup"><span data-stu-id="91d53-163">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="91d53-p108">只读。可为 Null。计划中的存储桶集合。</span><span class="sxs-lookup"><span data-stu-id="91d53-p108">Read-only. Nullable. Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="91d53-167">详细信息</span><span class="sxs-lookup"><span data-stu-id="91d53-167">details</span></span>|[<span data-ttu-id="91d53-168">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="91d53-168">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="91d53-169">只读。</span><span class="sxs-lookup"><span data-stu-id="91d53-169">Read-only.</span></span> <span data-ttu-id="91d53-170">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="91d53-170">Nullable.</span></span> <span data-ttu-id="91d53-171">关于计划的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="91d53-171">Additional details about the plan.</span></span>|
|<span data-ttu-id="91d53-172">tasks</span><span class="sxs-lookup"><span data-stu-id="91d53-172">tasks</span></span>|<span data-ttu-id="91d53-173">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="91d53-173">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="91d53-174">只读。</span><span class="sxs-lookup"><span data-stu-id="91d53-174">Read-only.</span></span> <span data-ttu-id="91d53-175">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="91d53-175">Nullable.</span></span> <span data-ttu-id="91d53-176">计划中的任务集合。</span><span class="sxs-lookup"><span data-stu-id="91d53-176">Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="91d53-177">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="91d53-177">JSON representation</span></span>

<span data-ttu-id="91d53-178">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91d53-178">Here is a JSON representation of the resource.</span></span>

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
