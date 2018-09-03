# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a><span data-ttu-id="c66cd-101">plannerAssignedToTaskBoardTaskFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="c66cd-101">plannerAssignedToTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="c66cd-p101">**plannerAssignedToTaskBoardTaskFormat** 资源表示用于在“任务板”的“AssignedTo”视图（由已向其分配任务的用户组成的视图）下正确呈现任务的信息。每个[任务](plannertask.md)均将有一个与其相关联的 **plannerAssignedToTaskBoardTaskFormat** 对象。</span><span class="sxs-lookup"><span data-stu-id="c66cd-p101">The **plannerAssignedToTaskBoardTaskFormat** resource represents the information used to render a task correctly in the AssignedTo view of the Task Board (a view organized by users to whom tasks are assigned to). Each [task](plannertask.md) will have one **plannerAssignedToTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="c66cd-104">方法</span><span class="sxs-lookup"><span data-stu-id="c66cd-104">Methods</span></span>

| <span data-ttu-id="c66cd-105">方法</span><span class="sxs-lookup"><span data-stu-id="c66cd-105">Method</span></span>           | <span data-ttu-id="c66cd-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="c66cd-106">Return Type</span></span>    |<span data-ttu-id="c66cd-107">说明</span><span class="sxs-lookup"><span data-stu-id="c66cd-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c66cd-108">获取 plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="c66cd-108">Get plannerAssignedToTaskBoardTaskFormat</span></span>](../api/plannerassignedtotaskboardtaskformat_get.md) | [<span data-ttu-id="c66cd-109">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="c66cd-109">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md) |<span data-ttu-id="c66cd-110">读取 **plannerAssignedToTaskBoardTaskFormat** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c66cd-110">Read properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="c66cd-111">更新</span><span class="sxs-lookup"><span data-stu-id="c66cd-111">Update</span></span>](../api/plannerassignedtotaskboardtaskformat_update.md) | [<span data-ttu-id="c66cd-112">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="c66cd-112">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)  |<span data-ttu-id="c66cd-113">更新 **plannerAssignedToTaskBoardTaskFormat** 对象。</span><span class="sxs-lookup"><span data-stu-id="c66cd-113">Update **plannerAssignedToTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c66cd-114">属性</span><span class="sxs-lookup"><span data-stu-id="c66cd-114">Properties</span></span>
| <span data-ttu-id="c66cd-115">属性</span><span class="sxs-lookup"><span data-stu-id="c66cd-115">Property</span></span>     | <span data-ttu-id="c66cd-116">类型</span><span class="sxs-lookup"><span data-stu-id="c66cd-116">Type</span></span>   |<span data-ttu-id="c66cd-117">说明</span><span class="sxs-lookup"><span data-stu-id="c66cd-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c66cd-118">id</span><span class="sxs-lookup"><span data-stu-id="c66cd-118">id</span></span>|<span data-ttu-id="c66cd-119">字符串</span><span class="sxs-lookup"><span data-stu-id="c66cd-119">String</span></span>| <span data-ttu-id="c66cd-120">只读。</span><span class="sxs-lookup"><span data-stu-id="c66cd-120">Read-only.</span></span> <span data-ttu-id="c66cd-121">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="c66cd-121">The ID of the resource.</span></span> <span data-ttu-id="c66cd-122">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="c66cd-122">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="c66cd-123">[格式验证](planner_identifiers_disclaimer.md)由服务执行。</span><span class="sxs-lookup"><span data-stu-id="c66cd-123">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="c66cd-124">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="c66cd-124">orderHintsByAssignee</span></span>|[<span data-ttu-id="c66cd-125">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="c66cd-125">plannerOrderHintsByAssignee</span></span>](plannerorderhintsbyassignee.md)|<span data-ttu-id="c66cd-p103">用于为任务板 AssignedTo 视图上的任务进行排序的提示字典。每个条目的键是任务分配到的用户之一，值为排序提示。[此处](planner_order_hint_format.md)概述了各值的格式。</span><span class="sxs-lookup"><span data-stu-id="c66cd-p103">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board. The key of each entry is one of the users the task is assigned to and the value is the order hint. The format of each value is defined as outlined [here](planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="c66cd-129">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="c66cd-129">unassignedOrderHint</span></span>|<span data-ttu-id="c66cd-130">字符串</span><span class="sxs-lookup"><span data-stu-id="c66cd-130">String</span></span>|<span data-ttu-id="c66cd-p104">当任务未分配给任何人，或 orderHintsByAssignee 字典未向分配到任务的用户提供排序提示时，提示值用于为任务板 AssignedTo 视图上的任务排序。[此处](planner_order_hint_format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="c66cd-p104">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](planner_order_hint_format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="c66cd-133">关系</span><span class="sxs-lookup"><span data-stu-id="c66cd-133">Relationships</span></span>
<span data-ttu-id="c66cd-134">无</span><span class="sxs-lookup"><span data-stu-id="c66cd-134">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c66cd-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c66cd-135">JSON representation</span></span>
<span data-ttu-id="c66cd-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c66cd-136">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHintsByAssignee": {"@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"},
  "unassignedOrderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignedToTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->