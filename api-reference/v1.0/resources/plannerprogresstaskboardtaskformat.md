# <a name="plannerprogresstaskboardtaskformat-resource-type"></a><span data-ttu-id="dd799-101">plannerProgressTaskBoardTaskFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="dd799-101">plannerProgressTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="dd799-p101">**plannerProgressTaskBoardTaskFormat** 资源表示用于在“任务板”的“进度”视图（由任务对象上的 PercentComplete 字段的状态组成的视图，包含“未启动”、“正在进行”和“完成”列）下正确呈现任务的信息。每个[任务](plannertask.md)均将有一个与其相关联的 **plannerProgressTaskBoardTaskFormat** 对象。</span><span class="sxs-lookup"><span data-stu-id="dd799-p101">The **plannerProgressTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Progress view of the Task Board (a view organized by the state of the PercentComplete field on the task object, with columns for Not Started, In Progress and Complete). Each [task](plannertask.md) will have one **plannerProgressTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="dd799-104">方法</span><span class="sxs-lookup"><span data-stu-id="dd799-104">Methods</span></span>

| <span data-ttu-id="dd799-105">方法</span><span class="sxs-lookup"><span data-stu-id="dd799-105">Method</span></span>           | <span data-ttu-id="dd799-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="dd799-106">Return Type</span></span>    |<span data-ttu-id="dd799-107">说明</span><span class="sxs-lookup"><span data-stu-id="dd799-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dd799-108">获取 plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="dd799-108">Get plannerProgressTaskBoardTaskFormat</span></span>](../api/plannerprogresstaskboardtaskformat_get.md) | [<span data-ttu-id="dd799-109">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="dd799-109">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md) |<span data-ttu-id="dd799-110">读取 **plannerProgressTaskBoardTaskFormat** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dd799-110">Read properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="dd799-111">更新</span><span class="sxs-lookup"><span data-stu-id="dd799-111">Update</span></span>](../api/plannerprogresstaskboardtaskformat_update.md) | [<span data-ttu-id="dd799-112">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="dd799-112">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)    |<span data-ttu-id="dd799-113">更新 **plannerProgressTaskBoardTaskFormat** 对象。</span><span class="sxs-lookup"><span data-stu-id="dd799-113">Update **plannerProgressTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="dd799-114">属性</span><span class="sxs-lookup"><span data-stu-id="dd799-114">Properties</span></span>
| <span data-ttu-id="dd799-115">属性</span><span class="sxs-lookup"><span data-stu-id="dd799-115">Property</span></span>     | <span data-ttu-id="dd799-116">类型</span><span class="sxs-lookup"><span data-stu-id="dd799-116">Type</span></span>   |<span data-ttu-id="dd799-117">说明</span><span class="sxs-lookup"><span data-stu-id="dd799-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd799-118">ID</span><span class="sxs-lookup"><span data-stu-id="dd799-118">id</span></span>|<span data-ttu-id="dd799-119">字符串</span><span class="sxs-lookup"><span data-stu-id="dd799-119">String</span></span>| <span data-ttu-id="dd799-120">只读。</span><span class="sxs-lookup"><span data-stu-id="dd799-120">Read-only.</span></span> <span data-ttu-id="dd799-121">只读。</span><span class="sxs-lookup"><span data-stu-id="dd799-121">The ID of the resource.</span></span> <span data-ttu-id="dd799-122">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="dd799-122">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="dd799-123">[格式验证](planner_identifiers_disclaimer.md)由服务执行。</span><span class="sxs-lookup"><span data-stu-id="dd799-123">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="dd799-124">orderHint</span><span class="sxs-lookup"><span data-stu-id="dd799-124">orderHint</span></span>|<span data-ttu-id="dd799-125">字符串</span><span class="sxs-lookup"><span data-stu-id="dd799-125">String</span></span>|<span data-ttu-id="dd799-p103">用于对任务板进度视图上的任务进行排序的提示值。[此处](planner_order_hint_format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="dd799-p103">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](planner_order_hint_format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd799-128">关系</span><span class="sxs-lookup"><span data-stu-id="dd799-128">Relationships</span></span>
<span data-ttu-id="dd799-129">无</span><span class="sxs-lookup"><span data-stu-id="dd799-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="dd799-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dd799-130">JSON representation</span></span>
<span data-ttu-id="dd799-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd799-131">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerProgressTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->