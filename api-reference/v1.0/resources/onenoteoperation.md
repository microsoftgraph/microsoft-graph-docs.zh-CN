# <a name="onenoteoperation-resource-type"></a><span data-ttu-id="07078-101">onenoteOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="07078-101">onenoteOperation resource type</span></span>

<span data-ttu-id="07078-102">某些长时间运行的 OneNote 操作的状态。</span><span class="sxs-lookup"><span data-stu-id="07078-102">The status of certain long-running OneNote operations.</span></span>

## <a name="json-representation"></a><span data-ttu-id="07078-103">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="07078-103">JSON representation</span></span>

<span data-ttu-id="07078-104">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07078-104">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.operation",
  "@odata.type": "microsoft.graph.onenoteOperation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "error": {"@odata.type": "microsoft.graph.onenoteOperationError"},
  "id": "string (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resourceId": "string",
  "resourceLocation": "string",
  "status": "string",
  "percentComplete": "string"
}

```
## <a name="properties"></a><span data-ttu-id="07078-105">属性</span><span class="sxs-lookup"><span data-stu-id="07078-105">Properties</span></span>
| <span data-ttu-id="07078-106">属性</span><span class="sxs-lookup"><span data-stu-id="07078-106">Property</span></span>     | <span data-ttu-id="07078-107">类型</span><span class="sxs-lookup"><span data-stu-id="07078-107">Type</span></span>   |<span data-ttu-id="07078-108">说明</span><span class="sxs-lookup"><span data-stu-id="07078-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07078-109">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="07078-109">createdDateTime</span></span>| <span data-ttu-id="07078-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07078-110">DateTimeOffset</span></span> |<span data-ttu-id="07078-111">操作的开始时间。</span><span class="sxs-lookup"><span data-stu-id="07078-111">The start time of the operation.</span></span>|
|<span data-ttu-id="07078-112">错误</span><span class="sxs-lookup"><span data-stu-id="07078-112">error</span></span>|[<span data-ttu-id="07078-113">onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="07078-113">onenoteOperationError</span></span>](onenoteoperationerror.md)|<span data-ttu-id="07078-114">操作返回的错误。</span><span class="sxs-lookup"><span data-stu-id="07078-114">The error returned by the operation.</span></span>|
|<span data-ttu-id="07078-115">id</span><span class="sxs-lookup"><span data-stu-id="07078-115">id</span></span>|<span data-ttu-id="07078-116">string</span><span class="sxs-lookup"><span data-stu-id="07078-116">string</span></span>|<span data-ttu-id="07078-117">操作 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="07078-117">The operation id. Read-only.</span></span>|
|<span data-ttu-id="07078-118">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="07078-118">lastActionDateTime</span></span>| <span data-ttu-id="07078-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07078-119">DateTimeOffset</span></span> |<span data-ttu-id="07078-120">操作的上次活动时间。</span><span class="sxs-lookup"><span data-stu-id="07078-120">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="07078-121">resourceId</span><span class="sxs-lookup"><span data-stu-id="07078-121">resourceId</span></span>|<span data-ttu-id="07078-122">string</span><span class="sxs-lookup"><span data-stu-id="07078-122">string</span></span>|<span data-ttu-id="07078-123">资源 ID。</span><span class="sxs-lookup"><span data-stu-id="07078-123">The resource id.</span></span>|
|<span data-ttu-id="07078-124">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="07078-124">resourceLocation</span></span>|<span data-ttu-id="07078-125">string</span><span class="sxs-lookup"><span data-stu-id="07078-125">string</span></span>|<span data-ttu-id="07078-p101">对象的资源 URI。例如，复制页面或分区的资源 URI。</span><span class="sxs-lookup"><span data-stu-id="07078-p101">The resource URI for the object. For example, the resource URI for a copied page or section.</span></span> |
|<span data-ttu-id="07078-128">status</span><span class="sxs-lookup"><span data-stu-id="07078-128">status</span></span>|<span data-ttu-id="07078-129">string</span><span class="sxs-lookup"><span data-stu-id="07078-129">string</span></span>|<span data-ttu-id="07078-130">操作的当前状态：`notstarted`、`running`、`completed`、 `failed`</span><span class="sxs-lookup"><span data-stu-id="07078-130">The current status of the operation: `notstarted`, `running`, `completed`, `failed`</span></span> |
|<span data-ttu-id="07078-131">percentComplete</span><span class="sxs-lookup"><span data-stu-id="07078-131">percentComplete</span></span>|<span data-ttu-id="07078-132">string</span><span class="sxs-lookup"><span data-stu-id="07078-132">string</span></span>|<span data-ttu-id="07078-133">操作仍处于 `running` 状态时操作的完成百分比</span><span class="sxs-lookup"><span data-stu-id="07078-133">The operation percent complete if the operation is still in `running` status</span></span>

## <a name="relationships"></a><span data-ttu-id="07078-134">关系</span><span class="sxs-lookup"><span data-stu-id="07078-134">Relationships</span></span>
<span data-ttu-id="07078-135">无</span><span class="sxs-lookup"><span data-stu-id="07078-135">None</span></span>


## <a name="methods"></a><span data-ttu-id="07078-136">方法</span><span class="sxs-lookup"><span data-stu-id="07078-136">Methods</span></span>

| <span data-ttu-id="07078-137">方法</span><span class="sxs-lookup"><span data-stu-id="07078-137">Method</span></span>           | <span data-ttu-id="07078-138">返回类型</span><span class="sxs-lookup"><span data-stu-id="07078-138">Return Type</span></span>    |<span data-ttu-id="07078-139">说明</span><span class="sxs-lookup"><span data-stu-id="07078-139">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="07078-140">Get operation</span><span class="sxs-lookup"><span data-stu-id="07078-140">Get operation</span></span>](../api/onenoteoperation_get.md) | [<span data-ttu-id="07078-141">onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="07078-141">onenoteOperation</span></span>](onenoteoperation.md) |<span data-ttu-id="07078-142">获取操作状态。</span><span class="sxs-lookup"><span data-stu-id="07078-142">Get the status of the operation.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
