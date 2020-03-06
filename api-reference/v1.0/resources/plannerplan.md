---
title: plannerPlan 资源类型
description: '**plannerPlan** 资源表示 Office 365 中的计划。 计划可以由组所有，并包含 plannerTasks 集合。 其也可以有 plannerBuckets 集合。 每个计划对象具有可以包含此计划的更多信息的详细信息对象。 有关组、计划和任务之间的关系的详细信息，请参阅“Planner”。'
localization_priority: Priority
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: ea9ef53ee472c9051be6baabe35dc2a0a03e620f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533989"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="fe62d-107">plannerPlan 资源类型</span><span class="sxs-lookup"><span data-stu-id="fe62d-107">plannerPlan resource type</span></span>

<span data-ttu-id="fe62d-108">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe62d-108">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fe62d-109">**plannerPlan** 资源表示 Office 365 中的计划。</span><span class="sxs-lookup"><span data-stu-id="fe62d-109">The **plannerPlan** resource represents a plan in Office 365.</span></span> <span data-ttu-id="fe62d-110">计划可以由[组](group.md)所有，并包含 [plannerTasks](plannertask.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="fe62d-110">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="fe62d-111">其也可以有 [plannerBuckets](plannerbucket.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="fe62d-111">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="fe62d-112">每个计划对象具有可以包含此计划的更多信息的[详细信息](plannerplandetails.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fe62d-112">Each plan object has a [details](plannerplandetails.md) object that can contain more information about the plan.</span></span> <span data-ttu-id="fe62d-113">有关组、计划和任务之间的关系的详细信息，请参阅 [Planner](planner-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="fe62d-113">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="fe62d-114">方法</span><span class="sxs-lookup"><span data-stu-id="fe62d-114">Methods</span></span>

| <span data-ttu-id="fe62d-115">方法</span><span class="sxs-lookup"><span data-stu-id="fe62d-115">Method</span></span>           | <span data-ttu-id="fe62d-116">返回类型</span><span class="sxs-lookup"><span data-stu-id="fe62d-116">Return Type</span></span>    |<span data-ttu-id="fe62d-117">说明</span><span class="sxs-lookup"><span data-stu-id="fe62d-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fe62d-118">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="fe62d-118">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="fe62d-119">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="fe62d-119">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="fe62d-120">读取 **plannerPlan** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fe62d-120">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="fe62d-121">List buckets</span><span class="sxs-lookup"><span data-stu-id="fe62d-121">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="fe62d-122">[plannerBucket](plannerbucket.md) collection</span><span class="sxs-lookup"><span data-stu-id="fe62d-122">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="fe62d-123">获取 **plannerBucket** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="fe62d-123">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="fe62d-124">List tasks</span><span class="sxs-lookup"><span data-stu-id="fe62d-124">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="fe62d-125">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="fe62d-125">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="fe62d-126">获取 **plannerTask** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="fe62d-126">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="fe62d-127">Update</span><span class="sxs-lookup"><span data-stu-id="fe62d-127">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="fe62d-128">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="fe62d-128">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="fe62d-129">更新 **plannerPlan** 对象。</span><span class="sxs-lookup"><span data-stu-id="fe62d-129">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="fe62d-130">属性</span><span class="sxs-lookup"><span data-stu-id="fe62d-130">Properties</span></span>
| <span data-ttu-id="fe62d-131">属性</span><span class="sxs-lookup"><span data-stu-id="fe62d-131">Property</span></span>     | <span data-ttu-id="fe62d-132">类型</span><span class="sxs-lookup"><span data-stu-id="fe62d-132">Type</span></span>   |<span data-ttu-id="fe62d-133">说明</span><span class="sxs-lookup"><span data-stu-id="fe62d-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe62d-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fe62d-134">createdDateTime</span></span>|<span data-ttu-id="fe62d-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe62d-135">DateTimeOffset</span></span>|<span data-ttu-id="fe62d-p103">只读。创建计划的日期和时间时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="fe62d-p103">Read-only. Date and time at which the plan is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="fe62d-140">id</span><span class="sxs-lookup"><span data-stu-id="fe62d-140">id</span></span>|<span data-ttu-id="fe62d-141">String</span><span class="sxs-lookup"><span data-stu-id="fe62d-141">String</span></span>| <span data-ttu-id="fe62d-142">只读。</span><span class="sxs-lookup"><span data-stu-id="fe62d-142">Read-only.</span></span> <span data-ttu-id="fe62d-143">计划的 ID。</span><span class="sxs-lookup"><span data-stu-id="fe62d-143">ID of the plan.</span></span> <span data-ttu-id="fe62d-144">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="fe62d-144">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="fe62d-145">[格式验证](planner-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="fe62d-145">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="fe62d-146">Owner</span><span class="sxs-lookup"><span data-stu-id="fe62d-146">owner</span></span>|<span data-ttu-id="fe62d-147">String</span><span class="sxs-lookup"><span data-stu-id="fe62d-147">String</span></span>|<span data-ttu-id="fe62d-148">拥有计划的[组](group.md)的 ID。</span><span class="sxs-lookup"><span data-stu-id="fe62d-148">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="fe62d-149">必须存在有效的组才能设置此字段。</span><span class="sxs-lookup"><span data-stu-id="fe62d-149">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="fe62d-150">设置后，此属性无法更新。</span><span class="sxs-lookup"><span data-stu-id="fe62d-150">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="fe62d-151">title</span><span class="sxs-lookup"><span data-stu-id="fe62d-151">title</span></span>|<span data-ttu-id="fe62d-152">String</span><span class="sxs-lookup"><span data-stu-id="fe62d-152">String</span></span>|<span data-ttu-id="fe62d-153">必填。</span><span class="sxs-lookup"><span data-stu-id="fe62d-153">Required.</span></span> <span data-ttu-id="fe62d-154">计划的标题</span><span class="sxs-lookup"><span data-stu-id="fe62d-154">Title of the plan.</span></span>|
|<span data-ttu-id="fe62d-155">createdBy</span><span class="sxs-lookup"><span data-stu-id="fe62d-155">createdBy</span></span>|[<span data-ttu-id="fe62d-156">identitySet</span><span class="sxs-lookup"><span data-stu-id="fe62d-156">identitySet</span></span>](identityset.md)|<span data-ttu-id="fe62d-157">只读。</span><span class="sxs-lookup"><span data-stu-id="fe62d-157">Read-only.</span></span> <span data-ttu-id="fe62d-158">创建计划的用户。</span><span class="sxs-lookup"><span data-stu-id="fe62d-158">The user who created the plan.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe62d-159">关系</span><span class="sxs-lookup"><span data-stu-id="fe62d-159">Relationships</span></span>
| <span data-ttu-id="fe62d-160">关系</span><span class="sxs-lookup"><span data-stu-id="fe62d-160">Relationship</span></span> | <span data-ttu-id="fe62d-161">类型</span><span class="sxs-lookup"><span data-stu-id="fe62d-161">Type</span></span>   |<span data-ttu-id="fe62d-162">说明</span><span class="sxs-lookup"><span data-stu-id="fe62d-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe62d-163">buckets</span><span class="sxs-lookup"><span data-stu-id="fe62d-163">buckets</span></span>|<span data-ttu-id="fe62d-164">[plannerBucket](plannerbucket.md) collection</span><span class="sxs-lookup"><span data-stu-id="fe62d-164">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="fe62d-p108">只读。可为 Null。计划中的存储桶集合。</span><span class="sxs-lookup"><span data-stu-id="fe62d-p108">Read-only. Nullable. Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="fe62d-168">详细信息</span><span class="sxs-lookup"><span data-stu-id="fe62d-168">details</span></span>|[<span data-ttu-id="fe62d-169">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="fe62d-169">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="fe62d-170">只读。</span><span class="sxs-lookup"><span data-stu-id="fe62d-170">Read-only.</span></span> <span data-ttu-id="fe62d-171">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="fe62d-171">Nullable.</span></span> <span data-ttu-id="fe62d-172">关于计划的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="fe62d-172">Additional details about the plan.</span></span>|
|<span data-ttu-id="fe62d-173">tasks</span><span class="sxs-lookup"><span data-stu-id="fe62d-173">tasks</span></span>|<span data-ttu-id="fe62d-174">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="fe62d-174">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="fe62d-175">只读。</span><span class="sxs-lookup"><span data-stu-id="fe62d-175">Read-only.</span></span> <span data-ttu-id="fe62d-176">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="fe62d-176">Nullable.</span></span> <span data-ttu-id="fe62d-177">计划中的任务集合。</span><span class="sxs-lookup"><span data-stu-id="fe62d-177">Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fe62d-178">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fe62d-178">JSON representation</span></span>

<span data-ttu-id="fe62d-179">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe62d-179">Here is a JSON representation of the resource.</span></span>

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
