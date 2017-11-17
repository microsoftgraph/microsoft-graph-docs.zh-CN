# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="fdc50-101">plannerTaskDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="fdc50-101">plannerTaskDetails resource type</span></span>

<span data-ttu-id="fdc50-p101">**plannerTaskDetails** 资源表示任务的其他相关信息。每个[任务](plannertask.md)对象均有一个详细信息对象。</span><span class="sxs-lookup"><span data-stu-id="fdc50-p101">The **plannerTaskDetails** resource represents the additional information about a task. Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="fdc50-104">方法</span><span class="sxs-lookup"><span data-stu-id="fdc50-104">Methods</span></span>

| <span data-ttu-id="fdc50-105">方法</span><span class="sxs-lookup"><span data-stu-id="fdc50-105">Method</span></span>           | <span data-ttu-id="fdc50-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="fdc50-106">Return Type</span></span>    |<span data-ttu-id="fdc50-107">说明</span><span class="sxs-lookup"><span data-stu-id="fdc50-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fdc50-108">Get plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="fdc50-108">Get plannerTaskDetails</span></span>](../api/plannertaskdetails_get.md) | [<span data-ttu-id="fdc50-109">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="fdc50-109">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="fdc50-110">读取 **plannerTaskDetails** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fdc50-110">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="fdc50-111">Update</span><span class="sxs-lookup"><span data-stu-id="fdc50-111">Update</span></span>](../api/plannertaskdetails_update.md) | [<span data-ttu-id="fdc50-112">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="fdc50-112">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="fdc50-113">更新 **plannerTaskDetails** 对象。</span><span class="sxs-lookup"><span data-stu-id="fdc50-113">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="fdc50-114">属性</span><span class="sxs-lookup"><span data-stu-id="fdc50-114">Properties</span></span>
| <span data-ttu-id="fdc50-115">属性</span><span class="sxs-lookup"><span data-stu-id="fdc50-115">Property</span></span>     | <span data-ttu-id="fdc50-116">类型</span><span class="sxs-lookup"><span data-stu-id="fdc50-116">Type</span></span>   |<span data-ttu-id="fdc50-117">说明</span><span class="sxs-lookup"><span data-stu-id="fdc50-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fdc50-118">checklist</span><span class="sxs-lookup"><span data-stu-id="fdc50-118">checklist</span></span>|[<span data-ttu-id="fdc50-119">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="fdc50-119">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="fdc50-120">任务上的检查表项目集合。</span><span class="sxs-lookup"><span data-stu-id="fdc50-120">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="fdc50-121">description</span><span class="sxs-lookup"><span data-stu-id="fdc50-121">description</span></span>|<span data-ttu-id="fdc50-122">String</span><span class="sxs-lookup"><span data-stu-id="fdc50-122">String</span></span>|<span data-ttu-id="fdc50-123">任务描述</span><span class="sxs-lookup"><span data-stu-id="fdc50-123">Description of the task</span></span>|
|<span data-ttu-id="fdc50-124">id</span><span class="sxs-lookup"><span data-stu-id="fdc50-124">id</span></span>|<span data-ttu-id="fdc50-125">字符串</span><span class="sxs-lookup"><span data-stu-id="fdc50-125">String</span></span>| <span data-ttu-id="fdc50-p102">只读。任务详细信息 ID。长度为 28 个字符，区分大小写。[格式验证](planner_identifiers_disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="fdc50-p102">Read-only. ID of the task details. It is 28 characters long and case sensitive. [Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="fdc50-130">previewType</span><span class="sxs-lookup"><span data-stu-id="fdc50-130">previewType</span></span>|<span data-ttu-id="fdc50-131">string</span><span class="sxs-lookup"><span data-stu-id="fdc50-131">string</span></span>|<span data-ttu-id="fdc50-p103">这将设置显示在任务上的预览类型。可能的值是：`automatic`、`noPreview`、`checklist`、`description`、`reference`。当设为 `automatic` 时，由查看任务的应用选择显示的预览。</span><span class="sxs-lookup"><span data-stu-id="fdc50-p103">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="fdc50-135">references</span><span class="sxs-lookup"><span data-stu-id="fdc50-135">references</span></span>|[<span data-ttu-id="fdc50-136">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="fdc50-136">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="fdc50-137">任务上的引用集合。</span><span class="sxs-lookup"><span data-stu-id="fdc50-137">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fdc50-138">关系</span><span class="sxs-lookup"><span data-stu-id="fdc50-138">Relationships</span></span>
<span data-ttu-id="fdc50-139">无</span><span class="sxs-lookup"><span data-stu-id="fdc50-139">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="fdc50-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fdc50-140">JSON representation</span></span>
<span data-ttu-id="fdc50-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fdc50-141">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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