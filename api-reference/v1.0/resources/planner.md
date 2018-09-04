# <a name="planner-resource-type"></a><span data-ttu-id="fa5df-101">planner 资源类型</span><span class="sxs-lookup"><span data-stu-id="fa5df-101">planner resource type</span></span>

<span data-ttu-id="fa5df-p101">**planner** 资源是 Planner 对象模型的入口点。其返回单一的 **planner** 资源。它不包含任何可用属性。</span><span class="sxs-lookup"><span data-stu-id="fa5df-p101">The **planner** resource is the entry point for the Planner object model. It returns a singleton **planner** resource.  It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="fa5df-105">方法</span><span class="sxs-lookup"><span data-stu-id="fa5df-105">Methods</span></span>

| <span data-ttu-id="fa5df-106">方法</span><span class="sxs-lookup"><span data-stu-id="fa5df-106">Method</span></span>           | <span data-ttu-id="fa5df-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="fa5df-107">Return Type</span></span>    |<span data-ttu-id="fa5df-108">说明</span><span class="sxs-lookup"><span data-stu-id="fa5df-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fa5df-109">Create plannerBucket</span><span class="sxs-lookup"><span data-stu-id="fa5df-109">Create plannerBucket</span></span>](../api/planner_post_buckets.md) |[<span data-ttu-id="fa5df-110">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="fa5df-110">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="fa5df-111">通过发布到存储桶集合新建 **plannerBucket**。</span><span class="sxs-lookup"><span data-stu-id="fa5df-111">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="fa5df-112">Create plannerPlan</span><span class="sxs-lookup"><span data-stu-id="fa5df-112">Create plannerPlan</span></span>](../api/planner_post_plans.md) |[<span data-ttu-id="fa5df-113">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="fa5df-113">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="fa5df-114">通过发布到计划集合新建 **plannerPlan**。</span><span class="sxs-lookup"><span data-stu-id="fa5df-114">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="fa5df-115">Create plannerTask</span><span class="sxs-lookup"><span data-stu-id="fa5df-115">Create plannerTask</span></span>](../api/planner_post_tasks.md) |[<span data-ttu-id="fa5df-116">plannerTask</span><span class="sxs-lookup"><span data-stu-id="fa5df-116">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="fa5df-117">通过发布到任务集合新建 **plannerTask**。</span><span class="sxs-lookup"><span data-stu-id="fa5df-117">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa5df-118">关系</span><span class="sxs-lookup"><span data-stu-id="fa5df-118">Relationships</span></span>
| <span data-ttu-id="fa5df-119">关系</span><span class="sxs-lookup"><span data-stu-id="fa5df-119">Relationship</span></span> | <span data-ttu-id="fa5df-120">类型</span><span class="sxs-lookup"><span data-stu-id="fa5df-120">Type</span></span>   |<span data-ttu-id="fa5df-121">说明</span><span class="sxs-lookup"><span data-stu-id="fa5df-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa5df-122">buckets</span><span class="sxs-lookup"><span data-stu-id="fa5df-122">buckets</span></span>|<span data-ttu-id="fa5df-123">[plannerBucket](plannerbucket.md) collection</span><span class="sxs-lookup"><span data-stu-id="fa5df-123">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="fa5df-p102">只读。可为 NULL。返回指定存储桶的集合</span><span class="sxs-lookup"><span data-stu-id="fa5df-p102">Read-only. Nullable. Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="fa5df-127">plans</span><span class="sxs-lookup"><span data-stu-id="fa5df-127">plans</span></span>|<span data-ttu-id="fa5df-128">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fa5df-128">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="fa5df-p103">只读。可为 NULL。返回指定计划的集合</span><span class="sxs-lookup"><span data-stu-id="fa5df-p103">Read-only. Nullable. Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="fa5df-132">tasks</span><span class="sxs-lookup"><span data-stu-id="fa5df-132">tasks</span></span>|<span data-ttu-id="fa5df-133">[plannerTask](plannertask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fa5df-133">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="fa5df-p104">只读。可为 NULL。返回指定任务的集合</span><span class="sxs-lookup"><span data-stu-id="fa5df-p104">Read-only. Nullable. Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fa5df-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fa5df-137">JSON representation</span></span>
<span data-ttu-id="fa5df-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa5df-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="fa5df-139">示例</span><span class="sxs-lookup"><span data-stu-id="fa5df-139">Example</span></span>

<span data-ttu-id="fa5df-140"> **planner** 资源位于图表的根节点。</span><span class="sxs-lookup"><span data-stu-id="fa5df-140">The **planner** resource is available at the root of the graph.</span></span>

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.planner"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->