# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="28e21-101">plannerBucketTaskBoardTaskFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="28e21-101">plannerBucketTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="28e21-p101">**plannerBucketTaskBoardTaskFormat** 资源表示用于在“任务板”的“存储桶”视图（由被分配到的存储桶中的任务组成的视图）下正确呈现任务的信息。每个[任务](plannertask.md)均将有一个与其相关联的 **plannerBucketTaskBoardTaskFormat** 对象。</span><span class="sxs-lookup"><span data-stu-id="28e21-p101">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to). Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="28e21-104">方法</span><span class="sxs-lookup"><span data-stu-id="28e21-104">Methods</span></span>

| <span data-ttu-id="28e21-105">方法</span><span class="sxs-lookup"><span data-stu-id="28e21-105">Method</span></span>           | <span data-ttu-id="28e21-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="28e21-106">Return Type</span></span>    |<span data-ttu-id="28e21-107">说明</span><span class="sxs-lookup"><span data-stu-id="28e21-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="28e21-108">获取 plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="28e21-108">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat_get.md) | [<span data-ttu-id="28e21-109">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="28e21-109">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md) |<span data-ttu-id="28e21-110">读取 **plannerBucketTaskBoardTaskFormat** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="28e21-110">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="28e21-111">更新</span><span class="sxs-lookup"><span data-stu-id="28e21-111">Update</span></span>](../api/plannerbuckettaskboardtaskformat_update.md) | [<span data-ttu-id="28e21-112">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="28e21-112">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)  |<span data-ttu-id="28e21-113">更新 **plannerBucketTaskBoardTaskFormat** 对象</span><span class="sxs-lookup"><span data-stu-id="28e21-113">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="28e21-114">属性</span><span class="sxs-lookup"><span data-stu-id="28e21-114">Properties</span></span>
| <span data-ttu-id="28e21-115">属性</span><span class="sxs-lookup"><span data-stu-id="28e21-115">Property</span></span>     | <span data-ttu-id="28e21-116">类型</span><span class="sxs-lookup"><span data-stu-id="28e21-116">Type</span></span>   |<span data-ttu-id="28e21-117">说明</span><span class="sxs-lookup"><span data-stu-id="28e21-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28e21-118">ID</span><span class="sxs-lookup"><span data-stu-id="28e21-118">id</span></span>|<span data-ttu-id="28e21-119">字符串</span><span class="sxs-lookup"><span data-stu-id="28e21-119">String</span></span>| <span data-ttu-id="28e21-120">只读。</span><span class="sxs-lookup"><span data-stu-id="28e21-120">Read-only.</span></span> <span data-ttu-id="28e21-121">资源的ID。</span><span class="sxs-lookup"><span data-stu-id="28e21-121">The ID of the resource.</span></span> <span data-ttu-id="28e21-122">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="28e21-122">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="28e21-123">[格式验证](planner_identifiers_disclaimer.md)由服务执行。</span><span class="sxs-lookup"><span data-stu-id="28e21-123">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="28e21-124">orderHint</span><span class="sxs-lookup"><span data-stu-id="28e21-124">orderHint</span></span>|<span data-ttu-id="28e21-125">字符串</span><span class="sxs-lookup"><span data-stu-id="28e21-125">String</span></span>|<span data-ttu-id="28e21-p103">用于对任务板存储桶视图中的任务进行排序的提示。[此处](planner_order_hint_format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="28e21-p103">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](planner_order_hint_format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="28e21-128">关系</span><span class="sxs-lookup"><span data-stu-id="28e21-128">Relationships</span></span>
<span data-ttu-id="28e21-129">无</span><span class="sxs-lookup"><span data-stu-id="28e21-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="28e21-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="28e21-130">JSON representation</span></span>
<span data-ttu-id="28e21-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28e21-131">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
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
  "description": "plannerBucketTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->