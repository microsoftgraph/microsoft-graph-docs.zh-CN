# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="437e4-101">plannerPlanDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="437e4-101">plannerPlanDetails resource type</span></span>


<span data-ttu-id="437e4-p101">**plannerPlanDetails** 资源表示计划的其他相关信息。每个[计划](plannerplan.md)对象均有一个详细信息对象。</span><span class="sxs-lookup"><span data-stu-id="437e4-p101">The **plannerPlanDetails** resource represents the additional information about a plan. Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="437e4-104">方法</span><span class="sxs-lookup"><span data-stu-id="437e4-104">Methods</span></span>

| <span data-ttu-id="437e4-105">方法</span><span class="sxs-lookup"><span data-stu-id="437e4-105">Method</span></span>           | <span data-ttu-id="437e4-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="437e4-106">Return Type</span></span>    |<span data-ttu-id="437e4-107">说明</span><span class="sxs-lookup"><span data-stu-id="437e4-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="437e4-108">Get plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="437e4-108">Get plannerPlanDetails</span></span>](../api/plannerplandetails_get.md) | [<span data-ttu-id="437e4-109">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="437e4-109">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="437e4-110">读取 **plannerPlanDetails** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="437e4-110">Read properties and relationships of **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="437e4-111">Update</span><span class="sxs-lookup"><span data-stu-id="437e4-111">Update</span></span>](../api/plannerplandetails_update.md) | [<span data-ttu-id="437e4-112">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="437e4-112">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="437e4-113">更新 **plannerPlanDetails** 对象。</span><span class="sxs-lookup"><span data-stu-id="437e4-113">Update **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="437e4-114">属性</span><span class="sxs-lookup"><span data-stu-id="437e4-114">Properties</span></span>
| <span data-ttu-id="437e4-115">属性</span><span class="sxs-lookup"><span data-stu-id="437e4-115">Property</span></span>     | <span data-ttu-id="437e4-116">类型</span><span class="sxs-lookup"><span data-stu-id="437e4-116">Type</span></span>   |<span data-ttu-id="437e4-117">说明</span><span class="sxs-lookup"><span data-stu-id="437e4-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="437e4-118">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="437e4-118">categoryDescriptions</span></span>|[<span data-ttu-id="437e4-119">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="437e4-119">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="437e4-120">指定可与计划中的任务相关联的六个类别的描述的对象</span><span class="sxs-lookup"><span data-stu-id="437e4-120">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="437e4-121">id</span><span class="sxs-lookup"><span data-stu-id="437e4-121">id</span></span>|<span data-ttu-id="437e4-122">字符串</span><span class="sxs-lookup"><span data-stu-id="437e4-122">String</span></span>| <span data-ttu-id="437e4-123">只读。</span><span class="sxs-lookup"><span data-stu-id="437e4-123">Read-only.</span></span> <span data-ttu-id="437e4-124">计划详细信息的 ID。</span><span class="sxs-lookup"><span data-stu-id="437e4-124">ID of the plan details.</span></span> <span data-ttu-id="437e4-125">其长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="437e4-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="437e4-126">[格式验证](planner_identifiers_disclaimer.md)在服务上执行。</span><span class="sxs-lookup"><span data-stu-id="437e4-126">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="437e4-127">sharedWith</span><span class="sxs-lookup"><span data-stu-id="437e4-127">sharedWith</span></span>|[<span data-ttu-id="437e4-128">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="437e4-128">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="437e4-p103">此计划共享的用户 id 集合。如果你正在利用 Office 365 组，使用组 API 管理组成员身份以共享[组的](group.md)计划。你还可以将现有的组成员添加到此集合，尽管他们无需访问组拥有的计划。</span><span class="sxs-lookup"><span data-stu-id="437e4-p103">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span> |

## <a name="relationships"></a><span data-ttu-id="437e4-132">关系</span><span class="sxs-lookup"><span data-stu-id="437e4-132">Relationships</span></span>
<span data-ttu-id="437e4-133">无</span><span class="sxs-lookup"><span data-stu-id="437e4-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="437e4-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="437e4-134">JSON representation</span></span>
<span data-ttu-id="437e4-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="437e4-135">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}-->

```json
{
  "categoryDescriptions": {"@odata.type": "microsoft.graph.plannerCategoryDescriptions"},
  "id": "String (identifier)",
  "sharedWith": {"@odata.type": "microsoft.graph.plannerUserIds"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->