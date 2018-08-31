# <a name="chartseries-resource-type"></a><span data-ttu-id="0595e-101">ChartSeries 资源类型</span><span class="sxs-lookup"><span data-stu-id="0595e-101">ChartSeries resource type</span></span>

<span data-ttu-id="0595e-102">代表图表上的系列。</span><span class="sxs-lookup"><span data-stu-id="0595e-102">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="0595e-103">方法</span><span class="sxs-lookup"><span data-stu-id="0595e-103">Methods</span></span>

| <span data-ttu-id="0595e-104">方法</span><span class="sxs-lookup"><span data-stu-id="0595e-104">Method</span></span>           | <span data-ttu-id="0595e-105">返回类型</span><span class="sxs-lookup"><span data-stu-id="0595e-105">Return Type</span></span>    |<span data-ttu-id="0595e-106">说明</span><span class="sxs-lookup"><span data-stu-id="0595e-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0595e-107">获取 ChartSeries</span><span class="sxs-lookup"><span data-stu-id="0595e-107">Get ChartSeries</span></span>](../api/chartseries_get.md) | [<span data-ttu-id="0595e-108">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="0595e-108">WorkbookChartSeries</span></span>](chartseries.md) |<span data-ttu-id="0595e-109">读取 chartSeries 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0595e-109">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="0595e-110">创建 ChartPoints</span><span class="sxs-lookup"><span data-stu-id="0595e-110">Create ChartPoints</span></span>](../api/chartseries_post_points.md) |[<span data-ttu-id="0595e-111">ChartPoints</span><span class="sxs-lookup"><span data-stu-id="0595e-111">ChartPoints</span></span>](chartpoint.md)| <span data-ttu-id="0595e-112">通过发布到点集合创建新的 ChartPoints。</span><span class="sxs-lookup"><span data-stu-id="0595e-112">Create a new ChartPoints by posting to the points collection.</span></span>|
|[<span data-ttu-id="0595e-113">列举数据点</span><span class="sxs-lookup"><span data-stu-id="0595e-113">List points</span></span>](../api/chartseries_list_points.md) |<span data-ttu-id="0595e-114">[ChartPoints](chartpoint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0595e-114">[ChartPoints](chartpoint.md) collection</span></span>| <span data-ttu-id="0595e-115">获取 ChartPoints 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0595e-115">Get a ChartPoints object collection.</span></span>|
|[<span data-ttu-id="0595e-116">更新</span><span class="sxs-lookup"><span data-stu-id="0595e-116">Update</span></span>](../api/chartseries_update.md) | [<span data-ttu-id="0595e-117">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="0595e-117">WorkbookChartSeries</span></span>](chartseries.md) |<span data-ttu-id="0595e-118">更新 ChartSeries 对象。</span><span class="sxs-lookup"><span data-stu-id="0595e-118">Update ChartSeries object.</span></span> |
|[<span data-ttu-id="0595e-119">列表</span><span class="sxs-lookup"><span data-stu-id="0595e-119">List</span></span>](../api/chartseries_list.md) | <span data-ttu-id="0595e-120">[WorkbookChartSeries](chartseries.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0595e-120">[WorkbookChartSeries](chartseries.md) collection</span></span> |<span data-ttu-id="0595e-121">获取 chartSeries 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0595e-121">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="0595e-122">ItemAt</span><span class="sxs-lookup"><span data-stu-id="0595e-122">Itemat</span></span>](../api/chartseriescollection_itemat.md)|[<span data-ttu-id="0595e-123">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="0595e-123">WorkbookChartSeries</span></span>](chartseries.md)|<span data-ttu-id="0595e-124">根据集合中的位置检索系列</span><span class="sxs-lookup"><span data-stu-id="0595e-124">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="0595e-125">属性</span><span class="sxs-lookup"><span data-stu-id="0595e-125">Properties</span></span>
| <span data-ttu-id="0595e-126">属性</span><span class="sxs-lookup"><span data-stu-id="0595e-126">Property</span></span>     | <span data-ttu-id="0595e-127">类型</span><span class="sxs-lookup"><span data-stu-id="0595e-127">Type</span></span>   |<span data-ttu-id="0595e-128">说明</span><span class="sxs-lookup"><span data-stu-id="0595e-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0595e-129">名称</span><span class="sxs-lookup"><span data-stu-id="0595e-129">name</span></span>|<span data-ttu-id="0595e-130">字符串</span><span class="sxs-lookup"><span data-stu-id="0595e-130">string</span></span>|<span data-ttu-id="0595e-131">表示图表中某个系列的名称。</span><span class="sxs-lookup"><span data-stu-id="0595e-131">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0595e-132">关系</span><span class="sxs-lookup"><span data-stu-id="0595e-132">Relationships</span></span>
| <span data-ttu-id="0595e-133">关系</span><span class="sxs-lookup"><span data-stu-id="0595e-133">Relationship</span></span> | <span data-ttu-id="0595e-134">类型</span><span class="sxs-lookup"><span data-stu-id="0595e-134">Type</span></span>   |<span data-ttu-id="0595e-135">说明</span><span class="sxs-lookup"><span data-stu-id="0595e-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0595e-136">格式</span><span class="sxs-lookup"><span data-stu-id="0595e-136">format</span></span>|[<span data-ttu-id="0595e-137">WorkbookChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="0595e-137">WorkbookChartSeriesFormat</span></span>](chartseriesformat.md)|<span data-ttu-id="0595e-p101">表示图表系列的格式，包括填充和线条格式。只读。</span><span class="sxs-lookup"><span data-stu-id="0595e-p101">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="0595e-140">数据点</span><span class="sxs-lookup"><span data-stu-id="0595e-140">points</span></span>|<span data-ttu-id="0595e-141">[WorkbookChartPoint](chartpoint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0595e-141">[WorkbookChartPoint](chartpoint.md) collection</span></span>|<span data-ttu-id="0595e-p102">表示系列中所有数据点的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="0595e-p102">Represents a collection of all points in the series. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0595e-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0595e-144">JSON representation</span></span>

<span data-ttu-id="0595e-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0595e-145">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartSeries"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeries resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->