---
title: plannerPlan 资源类型
description: '**plannerPlan** 资源表示 Office 365 中的计划。 计划可以由组所有，并包含 plannerTasks 集合。 其也可以有 plannerBuckets 集合。 每个计划对象具有可以包含此计划的更多信息的 details 对象。 有关组、计划和任务之间的关系的详细信息，请参阅“Planner”。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 973d6dfd9bed1bfef2c607276b9aaa0512f0fe9a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521711"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="e252f-107">plannerPlan 资源类型</span><span class="sxs-lookup"><span data-stu-id="e252f-107">plannerPlan resource type</span></span>

<span data-ttu-id="e252f-108">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e252f-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e252f-109">**plannerPlan** 资源表示 Office 365 中的计划。</span><span class="sxs-lookup"><span data-stu-id="e252f-109">The **plannerPlan** resource represents a plan in Office 365.</span></span> <span data-ttu-id="e252f-110">计划可以由[组](group.md)所有，并包含 [plannerTasks](plannertask.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="e252f-110">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="e252f-111">其也可以有 [plannerBuckets](plannerbucket.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="e252f-111">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="e252f-112">每个计划对象具有可以包含此计划的更多信息的 [details](plannerplandetails.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e252f-112">Each plan object has a [details](plannerplandetails.md) object which can contain more information about the plan.</span></span> <span data-ttu-id="e252f-113">有关组、计划和任务之间的关系的详细信息，请参阅 [Planner](planner-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="e252f-113">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>



## <a name="methods"></a><span data-ttu-id="e252f-114">方法</span><span class="sxs-lookup"><span data-stu-id="e252f-114">Methods</span></span>

| <span data-ttu-id="e252f-115">方法</span><span class="sxs-lookup"><span data-stu-id="e252f-115">Method</span></span>           | <span data-ttu-id="e252f-116">返回类型</span><span class="sxs-lookup"><span data-stu-id="e252f-116">Return Type</span></span>    |<span data-ttu-id="e252f-117">说明</span><span class="sxs-lookup"><span data-stu-id="e252f-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e252f-118">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="e252f-118">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="e252f-119">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="e252f-119">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="e252f-120">读取 **plannerPlan** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e252f-120">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="e252f-121">List buckets</span><span class="sxs-lookup"><span data-stu-id="e252f-121">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="e252f-122">[plannerBucket](plannerbucket.md) collection</span><span class="sxs-lookup"><span data-stu-id="e252f-122">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="e252f-123">获取 **plannerBucket** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e252f-123">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="e252f-124">List tasks</span><span class="sxs-lookup"><span data-stu-id="e252f-124">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="e252f-125">[plannerTask](plannertask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e252f-125">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="e252f-126">获取 **plannerTask** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e252f-126">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="e252f-127">Update</span><span class="sxs-lookup"><span data-stu-id="e252f-127">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="e252f-128">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="e252f-128">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="e252f-129">更新 **plannerPlan** 对象。</span><span class="sxs-lookup"><span data-stu-id="e252f-129">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e252f-130">属性</span><span class="sxs-lookup"><span data-stu-id="e252f-130">Properties</span></span>
| <span data-ttu-id="e252f-131">属性</span><span class="sxs-lookup"><span data-stu-id="e252f-131">Property</span></span>     | <span data-ttu-id="e252f-132">类型</span><span class="sxs-lookup"><span data-stu-id="e252f-132">Type</span></span>   |<span data-ttu-id="e252f-133">说明</span><span class="sxs-lookup"><span data-stu-id="e252f-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e252f-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e252f-134">createdDateTime</span></span>|<span data-ttu-id="e252f-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e252f-135">DateTimeOffset</span></span>|<span data-ttu-id="e252f-p103">只读。创建计划的日期和时间时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e252f-p103">Read-only. Date and time at which the plan is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e252f-140">id</span><span class="sxs-lookup"><span data-stu-id="e252f-140">id</span></span>|<span data-ttu-id="e252f-141">字符串</span><span class="sxs-lookup"><span data-stu-id="e252f-141">String</span></span>| <span data-ttu-id="e252f-142">只读。</span><span class="sxs-lookup"><span data-stu-id="e252f-142">Read-only.</span></span> <span data-ttu-id="e252f-143">计划的 ID。</span><span class="sxs-lookup"><span data-stu-id="e252f-143">ID of the plan.</span></span> <span data-ttu-id="e252f-144">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="e252f-144">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="e252f-145">[格式验证](tasks-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="e252f-145">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="e252f-146">Owner</span><span class="sxs-lookup"><span data-stu-id="e252f-146">owner</span></span>|<span data-ttu-id="e252f-147">String</span><span class="sxs-lookup"><span data-stu-id="e252f-147">String</span></span>|<span data-ttu-id="e252f-148">拥有计划的[组](group.md)的 ID。</span><span class="sxs-lookup"><span data-stu-id="e252f-148">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="e252f-149">必须存在有效的组才能设置此字段。</span><span class="sxs-lookup"><span data-stu-id="e252f-149">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="e252f-150">设置后，此属性无法更新。</span><span class="sxs-lookup"><span data-stu-id="e252f-150">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="e252f-151">title</span><span class="sxs-lookup"><span data-stu-id="e252f-151">title</span></span>|<span data-ttu-id="e252f-152">String</span><span class="sxs-lookup"><span data-stu-id="e252f-152">String</span></span>|<span data-ttu-id="e252f-153">必填。</span><span class="sxs-lookup"><span data-stu-id="e252f-153">Required.</span></span> <span data-ttu-id="e252f-154">计划的标题</span><span class="sxs-lookup"><span data-stu-id="e252f-154">Title of the plan.</span></span>|
|<span data-ttu-id="e252f-155">createdBy</span><span class="sxs-lookup"><span data-stu-id="e252f-155">createdBy</span></span>|[<span data-ttu-id="e252f-156">identitySet</span><span class="sxs-lookup"><span data-stu-id="e252f-156">identitySet</span></span>](identityset.md)|<span data-ttu-id="e252f-157">只读。</span><span class="sxs-lookup"><span data-stu-id="e252f-157">Read-only.</span></span> <span data-ttu-id="e252f-158">创建计划的用户。</span><span class="sxs-lookup"><span data-stu-id="e252f-158">The user who created the plan.</span></span>|
|<span data-ttu-id="e252f-159">上下文</span><span class="sxs-lookup"><span data-stu-id="e252f-159">contexts</span></span>|[<span data-ttu-id="e252f-160">plannerPlanContextCollection</span><span class="sxs-lookup"><span data-stu-id="e252f-160">plannerPlanContextCollection</span></span>](plannerplancontextcollection.md)| <span data-ttu-id="e252f-161">只读。</span><span class="sxs-lookup"><span data-stu-id="e252f-161">Read-only.</span></span> <span data-ttu-id="e252f-162">使用此计划的其他用户体验，表示为[plannerPlanContext](plannerplancontext.md)条目。</span><span class="sxs-lookup"><span data-stu-id="e252f-162">Additional user experiences in which this plan is used, represented as [plannerPlanContext](plannerplancontext.md) entries.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e252f-163">关系</span><span class="sxs-lookup"><span data-stu-id="e252f-163">Relationships</span></span>
| <span data-ttu-id="e252f-164">关系</span><span class="sxs-lookup"><span data-stu-id="e252f-164">Relationship</span></span> | <span data-ttu-id="e252f-165">类型</span><span class="sxs-lookup"><span data-stu-id="e252f-165">Type</span></span>   |<span data-ttu-id="e252f-166">说明</span><span class="sxs-lookup"><span data-stu-id="e252f-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e252f-167">buckets</span><span class="sxs-lookup"><span data-stu-id="e252f-167">buckets</span></span>|<span data-ttu-id="e252f-168">[plannerBucket](plannerbucket.md) collection</span><span class="sxs-lookup"><span data-stu-id="e252f-168">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="e252f-p109">只读。可为 Null。计划中的存储桶集合。</span><span class="sxs-lookup"><span data-stu-id="e252f-p109">Read-only. Nullable. Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="e252f-172">详细信息</span><span class="sxs-lookup"><span data-stu-id="e252f-172">details</span></span>|[<span data-ttu-id="e252f-173">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="e252f-173">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="e252f-174">只读。</span><span class="sxs-lookup"><span data-stu-id="e252f-174">Read-only.</span></span> <span data-ttu-id="e252f-175">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="e252f-175">Nullable.</span></span> <span data-ttu-id="e252f-176">关于计划的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="e252f-176">Additional details about the plan.</span></span>|
|<span data-ttu-id="e252f-177">tasks</span><span class="sxs-lookup"><span data-stu-id="e252f-177">tasks</span></span>|<span data-ttu-id="e252f-178">[plannerTask](plannertask.md) collection</span><span class="sxs-lookup"><span data-stu-id="e252f-178">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="e252f-179">只读。</span><span class="sxs-lookup"><span data-stu-id="e252f-179">Read-only.</span></span> <span data-ttu-id="e252f-180">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="e252f-180">Nullable.</span></span> <span data-ttu-id="e252f-181">计划中的任务集合。</span><span class="sxs-lookup"><span data-stu-id="e252f-181">Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e252f-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e252f-182">JSON representation</span></span>

<span data-ttu-id="e252f-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e252f-183">Here is a JSON representation of the resource.</span></span>

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
