# <a name="plannerbucket-resource-type"></a><span data-ttu-id="b6c8a-101">plannerBucket 资源类型</span><span class="sxs-lookup"><span data-stu-id="b6c8a-101">plannerBucket resource type</span></span>

<span data-ttu-id="b6c8a-p101">**plannerBucket** 资源表示 Office 365 计划中的任务的存储桶（或“自定义列”）。它包含在 [plannerPlan](plannerPlan.md) 之中，并且可能具有 [plannerTasks](plannerTask.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="b6c8a-p101">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Office 365. It is contained in a [plannerPlan](plannerPlan.md) and can have a collection of [plannerTasks](plannerTask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="b6c8a-104">方法</span><span class="sxs-lookup"><span data-stu-id="b6c8a-104">Methods</span></span>

| <span data-ttu-id="b6c8a-105">方法</span><span class="sxs-lookup"><span data-stu-id="b6c8a-105">Method</span></span>           | <span data-ttu-id="b6c8a-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="b6c8a-106">Return Type</span></span>    |<span data-ttu-id="b6c8a-107">说明</span><span class="sxs-lookup"><span data-stu-id="b6c8a-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b6c8a-108">Get plannerBucket</span><span class="sxs-lookup"><span data-stu-id="b6c8a-108">Get plannerBucket</span></span>](../api/plannerbucket_get.md) | [<span data-ttu-id="b6c8a-109">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="b6c8a-109">plannerBucket</span></span>](plannerbucket.md) |<span data-ttu-id="b6c8a-110">读取 **plannerBucket** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b6c8a-110">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="b6c8a-111">List plannerTasks</span><span class="sxs-lookup"><span data-stu-id="b6c8a-111">List plannerTasks</span></span>](../api/plannerbucket_list_tasks.md) |<span data-ttu-id="b6c8a-112">[plannerTask](plannertask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b6c8a-112">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="b6c8a-113">获取 **plannerTask** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b6c8a-113">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="b6c8a-114">Create</span><span class="sxs-lookup"><span data-stu-id="b6c8a-114">Create</span></span>](../api/planner_post_buckets.md) | [<span data-ttu-id="b6c8a-115">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="b6c8a-115">plannerBucket</span></span>](plannerbucket.md)   | <span data-ttu-id="b6c8a-116">新建 **plannerBucket** 对象。</span><span class="sxs-lookup"><span data-stu-id="b6c8a-116">Create a new **plannerBucket** object.</span></span> |
|[<span data-ttu-id="b6c8a-117">Update</span><span class="sxs-lookup"><span data-stu-id="b6c8a-117">Update</span></span>](../api/plannerbucket_update.md) | [<span data-ttu-id="b6c8a-118">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="b6c8a-118">plannerBucket</span></span>](plannerbucket.md)   |<span data-ttu-id="b6c8a-119">更新 **plannerBucket** 对象。</span><span class="sxs-lookup"><span data-stu-id="b6c8a-119">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="b6c8a-120">Delete</span><span class="sxs-lookup"><span data-stu-id="b6c8a-120">Delete</span></span>](../api/plannerbucket_delete.md) | <span data-ttu-id="b6c8a-121">无</span><span class="sxs-lookup"><span data-stu-id="b6c8a-121">None</span></span> |<span data-ttu-id="b6c8a-122">删除 **plannerBucket** 对象。</span><span class="sxs-lookup"><span data-stu-id="b6c8a-122">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b6c8a-123">属性</span><span class="sxs-lookup"><span data-stu-id="b6c8a-123">Properties</span></span>
| <span data-ttu-id="b6c8a-124">属性</span><span class="sxs-lookup"><span data-stu-id="b6c8a-124">Property</span></span>     | <span data-ttu-id="b6c8a-125">类型</span><span class="sxs-lookup"><span data-stu-id="b6c8a-125">Type</span></span>   |<span data-ttu-id="b6c8a-126">说明</span><span class="sxs-lookup"><span data-stu-id="b6c8a-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b6c8a-127">id</span><span class="sxs-lookup"><span data-stu-id="b6c8a-127">id</span></span>|<span data-ttu-id="b6c8a-128">字符串</span><span class="sxs-lookup"><span data-stu-id="b6c8a-128">String</span></span>| <span data-ttu-id="b6c8a-129">只读。</span><span class="sxs-lookup"><span data-stu-id="b6c8a-129">Read-only.</span></span> <span data-ttu-id="b6c8a-130">存储桶的 ID。</span><span class="sxs-lookup"><span data-stu-id="b6c8a-130">Name of the bucket.</span></span> <span data-ttu-id="b6c8a-131">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="b6c8a-131">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="b6c8a-132">[格式验证](planner_identifiers_disclaimer.md)由服务执行。</span><span class="sxs-lookup"><span data-stu-id="b6c8a-132">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="b6c8a-133">name</span><span class="sxs-lookup"><span data-stu-id="b6c8a-133">name</span></span>|<span data-ttu-id="b6c8a-134">字符串</span><span class="sxs-lookup"><span data-stu-id="b6c8a-134">String</span></span>|<span data-ttu-id="b6c8a-135">存储桶的名称。</span><span class="sxs-lookup"><span data-stu-id="b6c8a-135">Name of the bucket.</span></span>|
|<span data-ttu-id="b6c8a-136">orderHint</span><span class="sxs-lookup"><span data-stu-id="b6c8a-136">orderHint</span></span>|<span data-ttu-id="b6c8a-137">字符串</span><span class="sxs-lookup"><span data-stu-id="b6c8a-137">String</span></span>|<span data-ttu-id="b6c8a-p103">用于为列表视图中的此类型项目排序的提示。[此处](planner_order_hint_format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="b6c8a-p103">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="b6c8a-140">planId</span><span class="sxs-lookup"><span data-stu-id="b6c8a-140">planId</span></span>|<span data-ttu-id="b6c8a-141">字符串</span><span class="sxs-lookup"><span data-stu-id="b6c8a-141">String</span></span>|<span data-ttu-id="b6c8a-142">此存储桶所属的计划 ID。</span><span class="sxs-lookup"><span data-stu-id="b6c8a-142">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6c8a-143">关系</span><span class="sxs-lookup"><span data-stu-id="b6c8a-143">Relationships</span></span>
| <span data-ttu-id="b6c8a-144">关系</span><span class="sxs-lookup"><span data-stu-id="b6c8a-144">Relationship</span></span> | <span data-ttu-id="b6c8a-145">类型</span><span class="sxs-lookup"><span data-stu-id="b6c8a-145">Type</span></span>   |<span data-ttu-id="b6c8a-146">说明</span><span class="sxs-lookup"><span data-stu-id="b6c8a-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b6c8a-147">tasks</span><span class="sxs-lookup"><span data-stu-id="b6c8a-147">tasks</span></span>|<span data-ttu-id="b6c8a-148">[plannerTask](plannertask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b6c8a-148">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="b6c8a-p104">只读。可为 NULL。存储桶中的任务集合。</span><span class="sxs-lookup"><span data-stu-id="b6c8a-p104">Read-only. Nullable. The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b6c8a-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b6c8a-152">JSON representation</span></span>
<span data-ttu-id="b6c8a-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6c8a-153">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerBucket"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "orderHint": "String",
  "planId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucket resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->