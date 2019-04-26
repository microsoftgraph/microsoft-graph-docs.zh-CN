---
title: plannerPlan 资源类型
description: '**plannerPlan** 资源表示 Office 365 中的计划。 计划可以由组所有，并包含 plannerTasks 集合。 其也可以有 plannerBuckets 集合。 每个计划对象具有可以包含此计划的更多信息的详细信息对象。 有关组、计划和任务之间的关系的详细信息，请参阅“Planner”。'
localization_priority: Priority
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 9e77f2c0163f9093d931c46098498caa8c43f42c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462289"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="fbd8a-107">plannerPlan 资源类型</span><span class="sxs-lookup"><span data-stu-id="fbd8a-107">plannerPlan resource type</span></span>

<span data-ttu-id="fbd8a-108">**plannerPlan** 资源表示 Office 365 中的计划。</span><span class="sxs-lookup"><span data-stu-id="fbd8a-108">The Plan resource represents a plan in Office 365.</span></span> <span data-ttu-id="fbd8a-109">计划可以由[组](group.md)所有，并包含 [plannerTasks](plannertask.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="fbd8a-109">A plan can be owned by a [group](group.md) and contains a collection of [tasks](plannertask.md).</span></span> <span data-ttu-id="fbd8a-110">其也可以有 [plannerBuckets](plannerbucket.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="fbd8a-110">It also can have a collection of [buckets](plannerbucket.md).</span></span> <span data-ttu-id="fbd8a-111">每个计划对象具有可以包含此计划的更多信息的[详细信息](plannerplandetails.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fbd8a-111">Each plan object has a [details](plannerplandetails.md) object which can contain more information about the plan.</span></span> <span data-ttu-id="fbd8a-112">有关组、计划和任务之间的关系的详细信息，请参阅 [Planner](planner-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="fbd8a-112">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="fbd8a-113">方法</span><span class="sxs-lookup"><span data-stu-id="fbd8a-113">Methods</span></span>

| <span data-ttu-id="fbd8a-114">方法</span><span class="sxs-lookup"><span data-stu-id="fbd8a-114">Method</span></span>           | <span data-ttu-id="fbd8a-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="fbd8a-115">Return Type</span></span>    |<span data-ttu-id="fbd8a-116">说明</span><span class="sxs-lookup"><span data-stu-id="fbd8a-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fbd8a-117">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="fbd8a-117">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="fbd8a-118">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="fbd8a-118">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="fbd8a-119">读取 **plannerPlan** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fbd8a-119">Read properties and relationships of user object.</span></span>|
|[<span data-ttu-id="fbd8a-120">List buckets</span><span class="sxs-lookup"><span data-stu-id="fbd8a-120">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="fbd8a-121">[plannerBucket](plannerbucket.md) collection</span><span class="sxs-lookup"><span data-stu-id="fbd8a-121">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="fbd8a-122">获取 **plannerBucket** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="fbd8a-122">Get a CalendarGroup object collection.</span></span>|
|[<span data-ttu-id="fbd8a-123">List tasks</span><span class="sxs-lookup"><span data-stu-id="fbd8a-123">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="fbd8a-124">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="fbd8a-124">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="fbd8a-125">获取 **plannerTask** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="fbd8a-125">Get a Calendar object collection.</span></span>|
|[<span data-ttu-id="fbd8a-126">Update</span><span class="sxs-lookup"><span data-stu-id="fbd8a-126">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="fbd8a-127">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="fbd8a-127">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="fbd8a-128">更新 **plannerPlan** 对象。</span><span class="sxs-lookup"><span data-stu-id="fbd8a-128">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="fbd8a-129">属性</span><span class="sxs-lookup"><span data-stu-id="fbd8a-129">Properties</span></span>
| <span data-ttu-id="fbd8a-130">属性</span><span class="sxs-lookup"><span data-stu-id="fbd8a-130">Property</span></span>     | <span data-ttu-id="fbd8a-131">类型</span><span class="sxs-lookup"><span data-stu-id="fbd8a-131">Type</span></span>   |<span data-ttu-id="fbd8a-132">说明</span><span class="sxs-lookup"><span data-stu-id="fbd8a-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fbd8a-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fbd8a-133">createdDateTime</span></span>|<span data-ttu-id="fbd8a-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbd8a-134">DateTimeOffset</span></span>|<span data-ttu-id="fbd8a-p103">只读。创建计划的日期和时间时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="fbd8a-p103">Read-only. Date and time at which the plan is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="fbd8a-139">id</span><span class="sxs-lookup"><span data-stu-id="fbd8a-139">id</span></span>|<span data-ttu-id="fbd8a-140">String</span><span class="sxs-lookup"><span data-stu-id="fbd8a-140">String</span></span>| <span data-ttu-id="fbd8a-141">只读。</span><span class="sxs-lookup"><span data-stu-id="fbd8a-141">Read-only.</span></span> <span data-ttu-id="fbd8a-142">计划的 ID。</span><span class="sxs-lookup"><span data-stu-id="fbd8a-142">ID of the message</span></span> <span data-ttu-id="fbd8a-143">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="fbd8a-143">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="fbd8a-144">[格式验证](planner-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="fbd8a-144">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="fbd8a-145">Owner</span><span class="sxs-lookup"><span data-stu-id="fbd8a-145">owner</span></span>|<span data-ttu-id="fbd8a-146">String</span><span class="sxs-lookup"><span data-stu-id="fbd8a-146">String</span></span>|<span data-ttu-id="fbd8a-147">拥有计划的[组](group.md)的 ID。</span><span class="sxs-lookup"><span data-stu-id="fbd8a-147">ID of the principal that owns the lock.</span></span> <span data-ttu-id="fbd8a-148">必须存在有效的组才能设置此字段。</span><span class="sxs-lookup"><span data-stu-id="fbd8a-148">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="fbd8a-149">设置后，此属性无法更新。</span><span class="sxs-lookup"><span data-stu-id="fbd8a-149">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="fbd8a-150">title</span><span class="sxs-lookup"><span data-stu-id="fbd8a-150">title</span></span>|<span data-ttu-id="fbd8a-151">String</span><span class="sxs-lookup"><span data-stu-id="fbd8a-151">String</span></span>|<span data-ttu-id="fbd8a-152">必填。</span><span class="sxs-lookup"><span data-stu-id="fbd8a-152">Required.</span></span> <span data-ttu-id="fbd8a-153">计划的标题</span><span class="sxs-lookup"><span data-stu-id="fbd8a-153">Title of the plan.</span></span>|
|<span data-ttu-id="fbd8a-154">createdBy</span><span class="sxs-lookup"><span data-stu-id="fbd8a-154">createdBy</span></span>|[<span data-ttu-id="fbd8a-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="fbd8a-155">identitySet</span></span>](identityset.md)|<span data-ttu-id="fbd8a-156">只读。</span><span class="sxs-lookup"><span data-stu-id="fbd8a-156">Read-only.</span></span> <span data-ttu-id="fbd8a-157">创建计划的用户。</span><span class="sxs-lookup"><span data-stu-id="fbd8a-157">The user who created the Timesheet is listed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fbd8a-158">关系</span><span class="sxs-lookup"><span data-stu-id="fbd8a-158">Relationships</span></span>
| <span data-ttu-id="fbd8a-159">关系</span><span class="sxs-lookup"><span data-stu-id="fbd8a-159">Relationship</span></span> | <span data-ttu-id="fbd8a-160">类型</span><span class="sxs-lookup"><span data-stu-id="fbd8a-160">Type</span></span>   |<span data-ttu-id="fbd8a-161">说明</span><span class="sxs-lookup"><span data-stu-id="fbd8a-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fbd8a-162">buckets</span><span class="sxs-lookup"><span data-stu-id="fbd8a-162">buckets</span></span>|<span data-ttu-id="fbd8a-163">[plannerBucket](plannerbucket.md) collection</span><span class="sxs-lookup"><span data-stu-id="fbd8a-163">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="fbd8a-p108">只读。可为 Null。计划中的存储桶集合。</span><span class="sxs-lookup"><span data-stu-id="fbd8a-p108">Read-only. Nullable. Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="fbd8a-167">详细信息</span><span class="sxs-lookup"><span data-stu-id="fbd8a-167">details</span></span>|[<span data-ttu-id="fbd8a-168">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="fbd8a-168">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="fbd8a-169">只读。</span><span class="sxs-lookup"><span data-stu-id="fbd8a-169">Read-only.</span></span> <span data-ttu-id="fbd8a-170">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="fbd8a-170">Nullable.</span></span> <span data-ttu-id="fbd8a-171">关于计划的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="fbd8a-171">Additional details about the plan.</span></span>|
|<span data-ttu-id="fbd8a-172">tasks</span><span class="sxs-lookup"><span data-stu-id="fbd8a-172">tasks</span></span>|<span data-ttu-id="fbd8a-173">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="fbd8a-173">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="fbd8a-174">只读。</span><span class="sxs-lookup"><span data-stu-id="fbd8a-174">Read-only.</span></span> <span data-ttu-id="fbd8a-175">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="fbd8a-175">Nullable.</span></span> <span data-ttu-id="fbd8a-176">计划中的任务集合。</span><span class="sxs-lookup"><span data-stu-id="fbd8a-176">Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fbd8a-177">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fbd8a-177">JSON representation</span></span>

<span data-ttu-id="fbd8a-178">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fbd8a-178">Here is a JSON representation of the resource.</span></span>

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
