# <a name="planneruser-resource-type"></a><span data-ttu-id="07f39-101">plannerUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="07f39-101">plannerUser resource type</span></span>

<span data-ttu-id="07f39-p101">**plannerUser** 资源提供[用户](user.md)的 Planner 资源的访问权限。它不包含任何可用属性。</span><span class="sxs-lookup"><span data-stu-id="07f39-p101">The **plannerUser** resource provide access to Planner resources for a [user](user.md). It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="07f39-104">方法</span><span class="sxs-lookup"><span data-stu-id="07f39-104">Methods</span></span>

| <span data-ttu-id="07f39-105">方法</span><span class="sxs-lookup"><span data-stu-id="07f39-105">Method</span></span>           | <span data-ttu-id="07f39-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="07f39-106">Return Type</span></span>    |<span data-ttu-id="07f39-107">说明</span><span class="sxs-lookup"><span data-stu-id="07f39-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="07f39-108">List plans</span><span class="sxs-lookup"><span data-stu-id="07f39-108">List plans</span></span>](../api/planneruser_list_plans.md) |<span data-ttu-id="07f39-109">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="07f39-109">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="07f39-110">获取 **plannerPlan** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="07f39-110">Get a **plannerPlan** object collection.</span></span>|
|[<span data-ttu-id="07f39-111">List tasks</span><span class="sxs-lookup"><span data-stu-id="07f39-111">List tasks</span></span>](../api/planneruser_list_tasks.md) |<span data-ttu-id="07f39-112">[plannerTask](plannertask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="07f39-112">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="07f39-113">获取 **plannerTask** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="07f39-113">Get a **plannerTask** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="07f39-114">属性</span><span class="sxs-lookup"><span data-stu-id="07f39-114">Properties</span></span>
| <span data-ttu-id="07f39-115">属性</span><span class="sxs-lookup"><span data-stu-id="07f39-115">Property</span></span>     | <span data-ttu-id="07f39-116">类型</span><span class="sxs-lookup"><span data-stu-id="07f39-116">Type</span></span>   |<span data-ttu-id="07f39-117">说明</span><span class="sxs-lookup"><span data-stu-id="07f39-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07f39-118">id</span><span class="sxs-lookup"><span data-stu-id="07f39-118">id</span></span>|<span data-ttu-id="07f39-119">String</span><span class="sxs-lookup"><span data-stu-id="07f39-119">String</span></span>| <span data-ttu-id="07f39-p102">只读。planenrUser 的标识符</span><span class="sxs-lookup"><span data-stu-id="07f39-p102">Read-only. Identifier of the planenrUser</span></span>|

## <a name="relationships"></a><span data-ttu-id="07f39-122">关系</span><span class="sxs-lookup"><span data-stu-id="07f39-122">Relationships</span></span>
| <span data-ttu-id="07f39-123">关系</span><span class="sxs-lookup"><span data-stu-id="07f39-123">Relationship</span></span> | <span data-ttu-id="07f39-124">类型</span><span class="sxs-lookup"><span data-stu-id="07f39-124">Type</span></span>   |<span data-ttu-id="07f39-125">说明</span><span class="sxs-lookup"><span data-stu-id="07f39-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07f39-126">plans</span><span class="sxs-lookup"><span data-stu-id="07f39-126">plans</span></span>|<span data-ttu-id="07f39-127">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="07f39-127">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="07f39-p103">只读。可为 NULL。返回分配给用户的 [plannerTasks](plannertask.md)。</span><span class="sxs-lookup"><span data-stu-id="07f39-p103">Read-only. Nullable. Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="07f39-131">tasks</span><span class="sxs-lookup"><span data-stu-id="07f39-131">tasks</span></span>|<span data-ttu-id="07f39-132">[plannerTask](plannertask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="07f39-132">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="07f39-p104">只读。可为 NULL。返回与用户共享的 [plannerPlans](plannerplan.md)。</span><span class="sxs-lookup"><span data-stu-id="07f39-p104">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) shared with the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="07f39-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="07f39-136">JSON representation</span></span>
<span data-ttu-id="07f39-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07f39-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUser"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->