# <a name="chartpoint-resource-type"></a><span data-ttu-id="724a8-101">ChartPoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="724a8-101">ChartPoint resource type</span></span>

<span data-ttu-id="724a8-102">表示图表中某个系列的点。</span><span class="sxs-lookup"><span data-stu-id="724a8-102">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="724a8-103">方法</span><span class="sxs-lookup"><span data-stu-id="724a8-103">Methods</span></span>

| <span data-ttu-id="724a8-104">方法</span><span class="sxs-lookup"><span data-stu-id="724a8-104">Method</span></span>           | <span data-ttu-id="724a8-105">返回类型</span><span class="sxs-lookup"><span data-stu-id="724a8-105">Return Type</span></span>    |<span data-ttu-id="724a8-106">说明</span><span class="sxs-lookup"><span data-stu-id="724a8-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="724a8-107">获取 ChartPoint</span><span class="sxs-lookup"><span data-stu-id="724a8-107">Get ChartPoint</span></span>](../api/chartpoint_get.md) | [<span data-ttu-id="724a8-108">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="724a8-108">WorkbookChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="724a8-109">读取 chartPoint 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="724a8-109">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="724a8-110">列表</span><span class="sxs-lookup"><span data-stu-id="724a8-110">List</span></span>](../api/chartpoint_list.md) | <span data-ttu-id="724a8-111">[WorkbookChartPoint](chartpoint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="724a8-111">[WorkbookChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="724a8-112">获取 chartPoint 对象集合。</span><span class="sxs-lookup"><span data-stu-id="724a8-112">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="724a8-113">ItemAt</span><span class="sxs-lookup"><span data-stu-id="724a8-113">Itemat</span></span>](../api/chartpointscollection_itemat.md)|[<span data-ttu-id="724a8-114">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="724a8-114">WorkbookChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="724a8-115">根据其在系列中的位置检索点。</span><span class="sxs-lookup"><span data-stu-id="724a8-115">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="724a8-116">属性</span><span class="sxs-lookup"><span data-stu-id="724a8-116">Properties</span></span>
| <span data-ttu-id="724a8-117">属性</span><span class="sxs-lookup"><span data-stu-id="724a8-117">Property</span></span>     | <span data-ttu-id="724a8-118">类型</span><span class="sxs-lookup"><span data-stu-id="724a8-118">Type</span></span>   |<span data-ttu-id="724a8-119">说明</span><span class="sxs-lookup"><span data-stu-id="724a8-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="724a8-120">value</span><span class="sxs-lookup"><span data-stu-id="724a8-120">value</span></span>|<span data-ttu-id="724a8-121">Json</span><span class="sxs-lookup"><span data-stu-id="724a8-121">Json</span></span>|<span data-ttu-id="724a8-p101">返回图表点的值。只读。</span><span class="sxs-lookup"><span data-stu-id="724a8-p101">Returns the value of a chart point. Read-only.</span></span>|
|<span data-ttu-id="724a8-124">id</span><span class="sxs-lookup"><span data-stu-id="724a8-124">id</span></span>|<span data-ttu-id="724a8-125">string</span><span class="sxs-lookup"><span data-stu-id="724a8-125">string</span></span>|<span data-ttu-id="724a8-126">唯一标识符</span><span class="sxs-lookup"><span data-stu-id="724a8-126">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="724a8-127">关系</span><span class="sxs-lookup"><span data-stu-id="724a8-127">Relationships</span></span>
| <span data-ttu-id="724a8-128">关系</span><span class="sxs-lookup"><span data-stu-id="724a8-128">Relationship</span></span> | <span data-ttu-id="724a8-129">类型</span><span class="sxs-lookup"><span data-stu-id="724a8-129">Type</span></span>   |<span data-ttu-id="724a8-130">说明</span><span class="sxs-lookup"><span data-stu-id="724a8-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="724a8-131">format</span><span class="sxs-lookup"><span data-stu-id="724a8-131">format</span></span>|[<span data-ttu-id="724a8-132">WorkbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="724a8-132">WorkbookChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="724a8-p102">封装图表点的格式属性。只读。</span><span class="sxs-lookup"><span data-stu-id="724a8-p102">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="724a8-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="724a8-135">JSON representation</span></span>

<span data-ttu-id="724a8-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="724a8-136">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPoint"
}-->

```json
{
  "value": "string",
  "id": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->