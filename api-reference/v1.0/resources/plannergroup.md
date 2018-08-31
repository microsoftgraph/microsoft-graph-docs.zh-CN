# <a name="plannergroup-resource-type"></a><span data-ttu-id="b16cc-101">plannerGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="b16cc-101">plannerGroup resource type</span></span>

<span data-ttu-id="b16cc-p101">**plannerGroup** 资源提供[组](group.md)的 Planner 资源的访问权限。它不包含任何可用属性。</span><span class="sxs-lookup"><span data-stu-id="b16cc-p101">The **plannerGroup** resource provides access to Planner resources for a [group](group.md). It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="b16cc-104">方法</span><span class="sxs-lookup"><span data-stu-id="b16cc-104">Methods</span></span>

| <span data-ttu-id="b16cc-105">方法</span><span class="sxs-lookup"><span data-stu-id="b16cc-105">Method</span></span>           | <span data-ttu-id="b16cc-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="b16cc-106">Return Type</span></span>    |<span data-ttu-id="b16cc-107">说明</span><span class="sxs-lookup"><span data-stu-id="b16cc-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b16cc-108">List plans</span><span class="sxs-lookup"><span data-stu-id="b16cc-108">List plans</span></span>](../api/plannergroup_list_plans.md) |<span data-ttu-id="b16cc-109">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b16cc-109">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="b16cc-110">获取 **plannerPlan** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b16cc-110">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="b16cc-111">属性</span><span class="sxs-lookup"><span data-stu-id="b16cc-111">Properties</span></span>
| <span data-ttu-id="b16cc-112">属性</span><span class="sxs-lookup"><span data-stu-id="b16cc-112">Property</span></span>     | <span data-ttu-id="b16cc-113">类型</span><span class="sxs-lookup"><span data-stu-id="b16cc-113">Type</span></span>   |<span data-ttu-id="b16cc-114">说明</span><span class="sxs-lookup"><span data-stu-id="b16cc-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b16cc-115">id</span><span class="sxs-lookup"><span data-stu-id="b16cc-115">id</span></span>|<span data-ttu-id="b16cc-116">String</span><span class="sxs-lookup"><span data-stu-id="b16cc-116">String</span></span>| <span data-ttu-id="b16cc-p102">只读。**plannerGroup** 的标识符</span><span class="sxs-lookup"><span data-stu-id="b16cc-p102">Read-only. Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="b16cc-119">关系</span><span class="sxs-lookup"><span data-stu-id="b16cc-119">Relationships</span></span>
| <span data-ttu-id="b16cc-120">关系</span><span class="sxs-lookup"><span data-stu-id="b16cc-120">Relationship</span></span> | <span data-ttu-id="b16cc-121">类型</span><span class="sxs-lookup"><span data-stu-id="b16cc-121">Type</span></span>   |<span data-ttu-id="b16cc-122">说明</span><span class="sxs-lookup"><span data-stu-id="b16cc-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b16cc-123">plans</span><span class="sxs-lookup"><span data-stu-id="b16cc-123">plans</span></span>|<span data-ttu-id="b16cc-124">[plannerPlan](plannerplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b16cc-124">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="b16cc-p103">只读。可为 NULL。返回组拥有的 [plannerPlans](plannerplan.md)。</span><span class="sxs-lookup"><span data-stu-id="b16cc-p103">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b16cc-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b16cc-128">JSON representation</span></span>
<span data-ttu-id="b16cc-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b16cc-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerGroup"
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
  "description": "plannerGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->