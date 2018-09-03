# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="bfdc7-101">plannerTaskDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="bfdc7-101">plannerTaskDetails resource type</span></span>

<span data-ttu-id="bfdc7-p101">**plannerTaskDetails** 资源表示任务的其他相关信息。每个[任务](plannertask.md)对象均有一个详细信息对象。</span><span class="sxs-lookup"><span data-stu-id="bfdc7-p101">The **plannerTaskDetails** resource represents the additional information about a task. Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="bfdc7-104">方法</span><span class="sxs-lookup"><span data-stu-id="bfdc7-104">Methods</span></span>

| <span data-ttu-id="bfdc7-105">方法</span><span class="sxs-lookup"><span data-stu-id="bfdc7-105">Method</span></span>           | <span data-ttu-id="bfdc7-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="bfdc7-106">Return Type</span></span>    |<span data-ttu-id="bfdc7-107">说明</span><span class="sxs-lookup"><span data-stu-id="bfdc7-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bfdc7-108">获取 plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="bfdc7-108">Get plannerTaskDetails</span></span>](../api/plannertaskdetails_get.md) | [<span data-ttu-id="bfdc7-109">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="bfdc7-109">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="bfdc7-110">读取 **plannerTaskDetails** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bfdc7-110">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="bfdc7-111">更新</span><span class="sxs-lookup"><span data-stu-id="bfdc7-111">Update</span></span>](../api/plannertaskdetails_update.md) | [<span data-ttu-id="bfdc7-112">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="bfdc7-112">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="bfdc7-113">更新 **plannerTaskDetails** 对象。</span><span class="sxs-lookup"><span data-stu-id="bfdc7-113">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="bfdc7-114">属性</span><span class="sxs-lookup"><span data-stu-id="bfdc7-114">Properties</span></span>
| <span data-ttu-id="bfdc7-115">属性</span><span class="sxs-lookup"><span data-stu-id="bfdc7-115">Property</span></span>     | <span data-ttu-id="bfdc7-116">类型</span><span class="sxs-lookup"><span data-stu-id="bfdc7-116">Type</span></span>   |<span data-ttu-id="bfdc7-117">说明</span><span class="sxs-lookup"><span data-stu-id="bfdc7-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bfdc7-118">列表框</span><span class="sxs-lookup"><span data-stu-id="bfdc7-118">checklist</span></span>|[<span data-ttu-id="bfdc7-119">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="bfdc7-119">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="bfdc7-120">任务上的检查表项目集合。</span><span class="sxs-lookup"><span data-stu-id="bfdc7-120">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="bfdc7-121">说明</span><span class="sxs-lookup"><span data-stu-id="bfdc7-121">description</span></span>|<span data-ttu-id="bfdc7-122">字符串</span><span class="sxs-lookup"><span data-stu-id="bfdc7-122">String</span></span>|<span data-ttu-id="bfdc7-123">任务描述</span><span class="sxs-lookup"><span data-stu-id="bfdc7-123">Description of the task</span></span>|
|<span data-ttu-id="bfdc7-124">id</span><span class="sxs-lookup"><span data-stu-id="bfdc7-124">id</span></span>|<span data-ttu-id="bfdc7-125">字符串</span><span class="sxs-lookup"><span data-stu-id="bfdc7-125">String</span></span>| <span data-ttu-id="bfdc7-126">只读。</span><span class="sxs-lookup"><span data-stu-id="bfdc7-126">Read-only.</span></span> <span data-ttu-id="bfdc7-127">任务详细信息的 ID。</span><span class="sxs-lookup"><span data-stu-id="bfdc7-127">ID of the task details.</span></span> <span data-ttu-id="bfdc7-128">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="bfdc7-128">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="bfdc7-129">[格式验证](planner_identifiers_disclaimer.md) 由服务执行。</span><span class="sxs-lookup"><span data-stu-id="bfdc7-129">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="bfdc7-130">previewType</span><span class="sxs-lookup"><span data-stu-id="bfdc7-130">previewType</span></span>|<span data-ttu-id="bfdc7-131">字符串</span><span class="sxs-lookup"><span data-stu-id="bfdc7-131">string</span></span>|<span data-ttu-id="bfdc7-132">这将设置显示任务的预览类型。</span><span class="sxs-lookup"><span data-stu-id="bfdc7-132">This sets the type of preview that shows up on the task. Possible values are: , , , , .</span></span> <span data-ttu-id="bfdc7-133">可能的值为： `automatic` 、 `noPreview` 、 `checklist` 、 `description` 、 `reference` 。</span><span class="sxs-lookup"><span data-stu-id="bfdc7-133">The possible values are `automatic`, `noPreview`, `checklist`, `description`, `reference`, , , , , , , or .</span></span> <span data-ttu-id="bfdc7-134">当设置为 `automatic` 查看任务应用程序所选择的预览显示。</span><span class="sxs-lookup"><span data-stu-id="bfdc7-134">This sets the type of preview that shows up on the task. Possible values are: , , , , . When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="bfdc7-135">参考</span><span class="sxs-lookup"><span data-stu-id="bfdc7-135">references</span></span>|[<span data-ttu-id="bfdc7-136">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="bfdc7-136">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="bfdc7-137">任务上的引用集合。</span><span class="sxs-lookup"><span data-stu-id="bfdc7-137">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bfdc7-138">关系</span><span class="sxs-lookup"><span data-stu-id="bfdc7-138">Relationships</span></span>
<span data-ttu-id="bfdc7-139">无</span><span class="sxs-lookup"><span data-stu-id="bfdc7-139">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="bfdc7-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bfdc7-140">JSON representation</span></span>
<span data-ttu-id="bfdc7-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bfdc7-141">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerTaskDetails"
}-->

```json
{
  "checklist": {"@odata.type": "microsoft.graph.plannerChecklistItems"},
  "description": "String",
  "id": "String (identifier)",
  "previewType": "string",
  "references": {"@odata.type": "microsoft.graph.plannerExternalReferences"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
