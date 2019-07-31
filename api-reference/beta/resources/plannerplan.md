---
title: plannerPlan 资源类型
description: '**plannerPlan** 资源表示 Office 365 中的计划。 计划可以由组所有，并包含 plannerTasks 集合。 其也可以有 plannerBuckets 集合。 每个计划对象具有可以包含此计划的更多信息的 details 对象。 有关组、计划和任务之间的关系的详细信息，请参阅“Planner”。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 658bcbbaf8431b65565ecebd03a014776be840e9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965941"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="c6696-107">plannerPlan 资源类型</span><span class="sxs-lookup"><span data-stu-id="c6696-107">plannerPlan resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6696-108">**plannerPlan** 资源表示 Office 365 中的计划。</span><span class="sxs-lookup"><span data-stu-id="c6696-108">The **plannerPlan** resource represents a plan in Office 365.</span></span> <span data-ttu-id="c6696-109">计划可以由[组](group.md)所有，并包含 [plannerTasks](plannertask.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="c6696-109">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="c6696-110">其也可以有 [plannerBuckets](plannerbucket.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="c6696-110">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="c6696-111">每个计划对象具有可以包含此计划的更多信息的 [details](plannerplandetails.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c6696-111">Each plan object has a [details](plannerplandetails.md) object which can contain more information about the plan.</span></span> <span data-ttu-id="c6696-112">有关组、计划和任务之间的关系的详细信息，请参阅 [Planner](planner-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="c6696-112">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>



## <a name="methods"></a><span data-ttu-id="c6696-113">方法</span><span class="sxs-lookup"><span data-stu-id="c6696-113">Methods</span></span>

| <span data-ttu-id="c6696-114">方法</span><span class="sxs-lookup"><span data-stu-id="c6696-114">Method</span></span>           | <span data-ttu-id="c6696-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="c6696-115">Return Type</span></span>    |<span data-ttu-id="c6696-116">说明</span><span class="sxs-lookup"><span data-stu-id="c6696-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c6696-117">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="c6696-117">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="c6696-118">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="c6696-118">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="c6696-119">读取 **plannerPlan** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c6696-119">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="c6696-120">List buckets</span><span class="sxs-lookup"><span data-stu-id="c6696-120">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="c6696-121">[plannerBucket](plannerbucket.md) collection</span><span class="sxs-lookup"><span data-stu-id="c6696-121">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="c6696-122">获取 **plannerBucket** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c6696-122">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="c6696-123">List tasks</span><span class="sxs-lookup"><span data-stu-id="c6696-123">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="c6696-124">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="c6696-124">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="c6696-125">获取 **plannerTask** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c6696-125">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="c6696-126">Update</span><span class="sxs-lookup"><span data-stu-id="c6696-126">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="c6696-127">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="c6696-127">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="c6696-128">更新 **plannerPlan** 对象。</span><span class="sxs-lookup"><span data-stu-id="c6696-128">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c6696-129">属性</span><span class="sxs-lookup"><span data-stu-id="c6696-129">Properties</span></span>
| <span data-ttu-id="c6696-130">属性</span><span class="sxs-lookup"><span data-stu-id="c6696-130">Property</span></span>     | <span data-ttu-id="c6696-131">类型</span><span class="sxs-lookup"><span data-stu-id="c6696-131">Type</span></span>   |<span data-ttu-id="c6696-132">说明</span><span class="sxs-lookup"><span data-stu-id="c6696-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6696-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c6696-133">createdDateTime</span></span>|<span data-ttu-id="c6696-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6696-134">DateTimeOffset</span></span>|<span data-ttu-id="c6696-p103">只读。创建计划的日期和时间时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c6696-p103">Read-only. Date and time at which the plan is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c6696-139">id</span><span class="sxs-lookup"><span data-stu-id="c6696-139">id</span></span>|<span data-ttu-id="c6696-140">String</span><span class="sxs-lookup"><span data-stu-id="c6696-140">String</span></span>| <span data-ttu-id="c6696-141">只读。</span><span class="sxs-lookup"><span data-stu-id="c6696-141">Read-only.</span></span> <span data-ttu-id="c6696-142">计划的 ID。</span><span class="sxs-lookup"><span data-stu-id="c6696-142">ID of the plan.</span></span> <span data-ttu-id="c6696-143">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="c6696-143">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="c6696-144">[格式验证](tasks-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="c6696-144">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="c6696-145">Owner</span><span class="sxs-lookup"><span data-stu-id="c6696-145">owner</span></span>|<span data-ttu-id="c6696-146">String</span><span class="sxs-lookup"><span data-stu-id="c6696-146">String</span></span>|<span data-ttu-id="c6696-147">拥有计划的[组](group.md)的 ID。</span><span class="sxs-lookup"><span data-stu-id="c6696-147">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="c6696-148">必须存在有效的组才能设置此字段。</span><span class="sxs-lookup"><span data-stu-id="c6696-148">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="c6696-149">设置后，此属性无法更新。</span><span class="sxs-lookup"><span data-stu-id="c6696-149">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="c6696-150">title</span><span class="sxs-lookup"><span data-stu-id="c6696-150">title</span></span>|<span data-ttu-id="c6696-151">String</span><span class="sxs-lookup"><span data-stu-id="c6696-151">String</span></span>|<span data-ttu-id="c6696-152">必填。</span><span class="sxs-lookup"><span data-stu-id="c6696-152">Required.</span></span> <span data-ttu-id="c6696-153">计划的标题</span><span class="sxs-lookup"><span data-stu-id="c6696-153">Title of the plan.</span></span>|
|<span data-ttu-id="c6696-154">createdBy</span><span class="sxs-lookup"><span data-stu-id="c6696-154">createdBy</span></span>|[<span data-ttu-id="c6696-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="c6696-155">identitySet</span></span>](identityset.md)|<span data-ttu-id="c6696-156">只读。</span><span class="sxs-lookup"><span data-stu-id="c6696-156">Read-only.</span></span> <span data-ttu-id="c6696-157">创建计划的用户。</span><span class="sxs-lookup"><span data-stu-id="c6696-157">The user who created the plan.</span></span>|
|<span data-ttu-id="c6696-158">上下文</span><span class="sxs-lookup"><span data-stu-id="c6696-158">contexts</span></span>|[<span data-ttu-id="c6696-159">plannerPlanContextCollection</span><span class="sxs-lookup"><span data-stu-id="c6696-159">plannerPlanContextCollection</span></span>](plannerplancontextcollection.md)| <span data-ttu-id="c6696-160">只读。</span><span class="sxs-lookup"><span data-stu-id="c6696-160">Read-only.</span></span> <span data-ttu-id="c6696-161">使用此计划的其他用户体验, 表示为[plannerPlanContext](plannerplancontext.md)条目。</span><span class="sxs-lookup"><span data-stu-id="c6696-161">Additional user experiences in which this plan is used, represented as [plannerPlanContext](plannerplancontext.md) entries.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6696-162">关系</span><span class="sxs-lookup"><span data-stu-id="c6696-162">Relationships</span></span>
| <span data-ttu-id="c6696-163">关系</span><span class="sxs-lookup"><span data-stu-id="c6696-163">Relationship</span></span> | <span data-ttu-id="c6696-164">类型</span><span class="sxs-lookup"><span data-stu-id="c6696-164">Type</span></span>   |<span data-ttu-id="c6696-165">说明</span><span class="sxs-lookup"><span data-stu-id="c6696-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6696-166">buckets</span><span class="sxs-lookup"><span data-stu-id="c6696-166">buckets</span></span>|<span data-ttu-id="c6696-167">[plannerBucket](plannerbucket.md) collection</span><span class="sxs-lookup"><span data-stu-id="c6696-167">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="c6696-p109">只读。可为 Null。计划中的存储桶集合。</span><span class="sxs-lookup"><span data-stu-id="c6696-p109">Read-only. Nullable. Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="c6696-171">详细信息</span><span class="sxs-lookup"><span data-stu-id="c6696-171">details</span></span>|[<span data-ttu-id="c6696-172">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="c6696-172">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="c6696-173">只读。</span><span class="sxs-lookup"><span data-stu-id="c6696-173">Read-only.</span></span> <span data-ttu-id="c6696-174">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="c6696-174">Nullable.</span></span> <span data-ttu-id="c6696-175">关于计划的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="c6696-175">Additional details about the plan.</span></span>|
|<span data-ttu-id="c6696-176">tasks</span><span class="sxs-lookup"><span data-stu-id="c6696-176">tasks</span></span>|<span data-ttu-id="c6696-177">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="c6696-177">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="c6696-178">只读。</span><span class="sxs-lookup"><span data-stu-id="c6696-178">Read-only.</span></span> <span data-ttu-id="c6696-179">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="c6696-179">Nullable.</span></span> <span data-ttu-id="c6696-180">计划中的任务集合。</span><span class="sxs-lookup"><span data-stu-id="c6696-180">Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c6696-181">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c6696-181">JSON representation</span></span>

<span data-ttu-id="c6696-182">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6696-182">Here is a JSON representation of the resource.</span></span>

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
  "owner": "String",
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
