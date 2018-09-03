# <a name="plannerplan-resource-type"></a><span data-ttu-id="cb4e9-101">plannerPlan 资源类型</span><span class="sxs-lookup"><span data-stu-id="cb4e9-101">plannerPlan resource type</span></span>

<span data-ttu-id="cb4e9-p101">**plannerPlan** 资源表示 Office 365 中的计划。计划可以由[组](group.md)所有，并包含 [plannerTasks](plannerTask.md) 集合。其也可以有 [plannerBuckets](plannerBucket.md) 集合。每个计划对象具有可以包含此计划的更多信息的[详细信息](plannerPlanDetails.md)对象。有关组、计划和任务之间的关系的详细信息，请参阅 [Planner](planner_overview.md)。</span><span class="sxs-lookup"><span data-stu-id="cb4e9-p101">The **plannerPlan** resource represents a plan in Office 365. A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannerTask.md). It can also have a collection of [plannerBuckets](plannerBucket.md). Each plan object has a [details](plannerPlanDetails.md) object that can contain more information about the plan. For more information about the relationships between groups, plans, and tasks, see [Planner](planner_overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="cb4e9-107">方法</span><span class="sxs-lookup"><span data-stu-id="cb4e9-107">Methods</span></span>

| <span data-ttu-id="cb4e9-108">方法</span><span class="sxs-lookup"><span data-stu-id="cb4e9-108">Method</span></span>           | <span data-ttu-id="cb4e9-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="cb4e9-109">Return Type</span></span>    |<span data-ttu-id="cb4e9-110">说明</span><span class="sxs-lookup"><span data-stu-id="cb4e9-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cb4e9-111">获取 plannerPlan</span><span class="sxs-lookup"><span data-stu-id="cb4e9-111">Get plannerPlan</span></span>](../api/plannerplan_get.md) | [<span data-ttu-id="cb4e9-112">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="cb4e9-112">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="cb4e9-113">读取 **plannerPlan** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cb4e9-113">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="cb4e9-114">列出存储桶</span><span class="sxs-lookup"><span data-stu-id="cb4e9-114">List buckets</span></span>](../api/plannerplan_list_buckets.md) |<span data-ttu-id="cb4e9-115">[plannerBucket](plannerbucket.md) collection</span><span class="sxs-lookup"><span data-stu-id="cb4e9-115">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="cb4e9-116">获取 **plannerBucket** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="cb4e9-116">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="cb4e9-117">List tasks</span><span class="sxs-lookup"><span data-stu-id="cb4e9-117">List tasks</span></span>](../api/plannerplan_list_tasks.md) |<span data-ttu-id="cb4e9-118">[plannerTask](plannertask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cb4e9-118">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="cb4e9-119">获取 **plannerTask** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="cb4e9-119">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="cb4e9-120">更新</span><span class="sxs-lookup"><span data-stu-id="cb4e9-120">Update</span></span>](../api/plannerplan_update.md) | [<span data-ttu-id="cb4e9-121">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="cb4e9-121">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="cb4e9-122">更新 **plannerPlan** 对象。</span><span class="sxs-lookup"><span data-stu-id="cb4e9-122">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="cb4e9-123">属性</span><span class="sxs-lookup"><span data-stu-id="cb4e9-123">Properties</span></span>
| <span data-ttu-id="cb4e9-124">属性</span><span class="sxs-lookup"><span data-stu-id="cb4e9-124">Property</span></span>     | <span data-ttu-id="cb4e9-125">类型</span><span class="sxs-lookup"><span data-stu-id="cb4e9-125">Type</span></span>   |<span data-ttu-id="cb4e9-126">说明</span><span class="sxs-lookup"><span data-stu-id="cb4e9-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cb4e9-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cb4e9-127">createdDateTime</span></span>|<span data-ttu-id="cb4e9-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb4e9-128">DateTimeOffset</span></span>|<span data-ttu-id="cb4e9-p102">只读。创建计划的日期和时间时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示： `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="cb4e9-p102">Read-only. Date and time at which the plan is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="cb4e9-133">id</span><span class="sxs-lookup"><span data-stu-id="cb4e9-133">id</span></span>|<span data-ttu-id="cb4e9-134">字符串</span><span class="sxs-lookup"><span data-stu-id="cb4e9-134">String</span></span>| <span data-ttu-id="cb4e9-135">只读。</span><span class="sxs-lookup"><span data-stu-id="cb4e9-135">Read-only.</span></span> <span data-ttu-id="cb4e9-136">计划的 ID。</span><span class="sxs-lookup"><span data-stu-id="cb4e9-136">Title of the plan.</span></span> <span data-ttu-id="cb4e9-137">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="cb4e9-137">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="cb4e9-138">[格式验证](planner_identifiers_disclaimer.md)由服务执行。</span><span class="sxs-lookup"><span data-stu-id="cb4e9-138">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="cb4e9-139">所有者</span><span class="sxs-lookup"><span data-stu-id="cb4e9-139">owner</span></span>|<span data-ttu-id="cb4e9-140">String</span><span class="sxs-lookup"><span data-stu-id="cb4e9-140">String</span></span>|<span data-ttu-id="cb4e9-p104">拥有计划的[组](group.md)的 ID。必须存在有效的组才能设置此字段。设置后，只能由所有者更新此字段。</span><span class="sxs-lookup"><span data-stu-id="cb4e9-p104">ID of the [Group](group.md) that owns the plan. A valid group must exist before this field can be set. Once set, this can only be updated by the owner.</span></span>|
|<span data-ttu-id="cb4e9-144">标题</span><span class="sxs-lookup"><span data-stu-id="cb4e9-144">title</span></span>|<span data-ttu-id="cb4e9-145">String</span><span class="sxs-lookup"><span data-stu-id="cb4e9-145">String</span></span>|<span data-ttu-id="cb4e9-p105">必填。计划的标题</span><span class="sxs-lookup"><span data-stu-id="cb4e9-p105">Required. Title of the plan.</span></span>|
|<span data-ttu-id="cb4e9-148">createdBy</span><span class="sxs-lookup"><span data-stu-id="cb4e9-148">createdBy</span></span>|[<span data-ttu-id="cb4e9-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="cb4e9-149">identitySet</span></span>](identityset.md)|<span data-ttu-id="cb4e9-p106">只读。创建计划的用户。</span><span class="sxs-lookup"><span data-stu-id="cb4e9-p106">Read-only. The user who created the plan.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb4e9-152">关系</span><span class="sxs-lookup"><span data-stu-id="cb4e9-152">Relationships</span></span>
| <span data-ttu-id="cb4e9-153">关系</span><span class="sxs-lookup"><span data-stu-id="cb4e9-153">Relationship</span></span> | <span data-ttu-id="cb4e9-154">类型</span><span class="sxs-lookup"><span data-stu-id="cb4e9-154">Type</span></span>   |<span data-ttu-id="cb4e9-155">说明</span><span class="sxs-lookup"><span data-stu-id="cb4e9-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cb4e9-156">buckets</span><span class="sxs-lookup"><span data-stu-id="cb4e9-156">buckets</span></span>|<span data-ttu-id="cb4e9-157">[plannerBucket](plannerbucket.md) collection</span><span class="sxs-lookup"><span data-stu-id="cb4e9-157">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="cb4e9-p107">只读。可为 Null。计划中的存储桶集合。</span><span class="sxs-lookup"><span data-stu-id="cb4e9-p107">Read-only. Nullable. Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="cb4e9-161">详细信息</span><span class="sxs-lookup"><span data-stu-id="cb4e9-161">details</span></span>|[<span data-ttu-id="cb4e9-162">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="cb4e9-162">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="cb4e9-p108">只读。可为 NULL。关于计划的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="cb4e9-p108">Read-only. Nullable. Additional details about the plan.</span></span>|
|<span data-ttu-id="cb4e9-166">tasks</span><span class="sxs-lookup"><span data-stu-id="cb4e9-166">tasks</span></span>|<span data-ttu-id="cb4e9-167">[plannerTask](plannertask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cb4e9-167">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="cb4e9-p109">只读。可为 Null。计划中的任务集合。</span><span class="sxs-lookup"><span data-stu-id="cb4e9-p109">Read-only. Nullable. Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cb4e9-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cb4e9-171">JSON representation</span></span>

<span data-ttu-id="cb4e9-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cb4e9-172">Here is a JSON representation of the resource.</span></span>

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