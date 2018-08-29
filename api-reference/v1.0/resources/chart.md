# <a name="chart-resource-type"></a><span data-ttu-id="3b949-101">图表资源类型</span><span class="sxs-lookup"><span data-stu-id="3b949-101">Chart resource type</span></span>

<span data-ttu-id="3b949-102">表示工作簿中的 chart 对象。</span><span class="sxs-lookup"><span data-stu-id="3b949-102">Represents a chart object in a workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="3b949-103">方法</span><span class="sxs-lookup"><span data-stu-id="3b949-103">Methods</span></span>

| <span data-ttu-id="3b949-104">方法</span><span class="sxs-lookup"><span data-stu-id="3b949-104">Method</span></span>           | <span data-ttu-id="3b949-105">返回类型</span><span class="sxs-lookup"><span data-stu-id="3b949-105">Return Type</span></span>    |<span data-ttu-id="3b949-106">说明</span><span class="sxs-lookup"><span data-stu-id="3b949-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3b949-107">获取图表</span><span class="sxs-lookup"><span data-stu-id="3b949-107">Get Chart</span></span>](../api/chart_get.md) | [<span data-ttu-id="3b949-108">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="3b949-108">WorkbookChart</span></span>](chart.md) |<span data-ttu-id="3b949-109">读取 chart 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3b949-109">Read properties and relationships of chart object.</span></span>|
|[<span data-ttu-id="3b949-110">创建 ChartSeries</span><span class="sxs-lookup"><span data-stu-id="3b949-110">Create ChartSeries</span></span>](../api/chart_post_series.md) |[<span data-ttu-id="3b949-111">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="3b949-111">WorkbookChartSeries</span></span>](chartseries.md)| <span data-ttu-id="3b949-112">通过发布到序列集合创建新的 ChartSeries。</span><span class="sxs-lookup"><span data-stu-id="3b949-112">Create a new ChartSeries by posting to the series collection.</span></span>|
|[<span data-ttu-id="3b949-113">列出 series</span><span class="sxs-lookup"><span data-stu-id="3b949-113">List series</span></span>](../api/chart_list_series.md) |<span data-ttu-id="3b949-114">[WorkbookChartSeries](chartseries.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3b949-114">[WorkbookChartSeries](chartseries.md) collection</span></span>| <span data-ttu-id="3b949-115">获取 ChartSeries 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3b949-115">Get a ChartSeries object collection.</span></span>|
|[<span data-ttu-id="3b949-116">更新</span><span class="sxs-lookup"><span data-stu-id="3b949-116">Update</span></span>](../api/chart_update.md) | [<span data-ttu-id="3b949-117">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="3b949-117">WorkbookChart</span></span>](chart.md)   |<span data-ttu-id="3b949-118">更新 Chart 对象。</span><span class="sxs-lookup"><span data-stu-id="3b949-118">Update Chart object.</span></span> |
|[<span data-ttu-id="3b949-119">图像</span><span class="sxs-lookup"><span data-stu-id="3b949-119">Image</span></span>](../api/chart_image.md)|<span data-ttu-id="3b949-120">图像 base64 编码字符串</span><span class="sxs-lookup"><span data-stu-id="3b949-120">Image base64 encoded string</span></span>|<span data-ttu-id="3b949-121">通过缩放图表适应指定的尺寸，将图表呈现为 base64 编码的图像。</span><span class="sxs-lookup"><span data-stu-id="3b949-121">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>|
|[<span data-ttu-id="3b949-122">删除</span><span class="sxs-lookup"><span data-stu-id="3b949-122">Delete</span></span>](../api/chart_delete.md)|<span data-ttu-id="3b949-123">无</span><span class="sxs-lookup"><span data-stu-id="3b949-123">None</span></span>|<span data-ttu-id="3b949-124">删除 chart 对象。</span><span class="sxs-lookup"><span data-stu-id="3b949-124">Deletes the chart object.</span></span>|
|[<span data-ttu-id="3b949-125">Setdata</span><span class="sxs-lookup"><span data-stu-id="3b949-125">Setdata</span></span>](../api/chart_setdata.md)|<span data-ttu-id="3b949-126">无</span><span class="sxs-lookup"><span data-stu-id="3b949-126">None</span></span>|<span data-ttu-id="3b949-127">重置图表的源数据。</span><span class="sxs-lookup"><span data-stu-id="3b949-127">Resets the source data for the chart.</span></span>|
|[<span data-ttu-id="3b949-128">Setposition</span><span class="sxs-lookup"><span data-stu-id="3b949-128">Setposition</span></span>](../api/chart_setposition.md)|<span data-ttu-id="3b949-129">无</span><span class="sxs-lookup"><span data-stu-id="3b949-129">None</span></span>|<span data-ttu-id="3b949-130">相对于工作表上的单元格放置图表。</span><span class="sxs-lookup"><span data-stu-id="3b949-130">Positions the chart relative to cells on the worksheet.</span></span>|
|[<span data-ttu-id="3b949-131">列出</span><span class="sxs-lookup"><span data-stu-id="3b949-131">List</span></span>](../api/chart_list.md) | <span data-ttu-id="3b949-132">[WorkbookChart](chart.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3b949-132">[WorkbookChart](chart.md) collection</span></span> |<span data-ttu-id="3b949-133">获取 chart 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3b949-133">Get chart object collection.</span></span> |
|[<span data-ttu-id="3b949-134">Itemat</span><span class="sxs-lookup"><span data-stu-id="3b949-134">Itemat</span></span>](../api/chartcollection_itemat.md)|[<span data-ttu-id="3b949-135">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="3b949-135">WorkbookChart</span></span>](chart.md)|<span data-ttu-id="3b949-136">根据其在集合中的位置获取图表。</span><span class="sxs-lookup"><span data-stu-id="3b949-136">Gets a chart based on its position in the collection.</span></span>|
|[<span data-ttu-id="3b949-137">添加</span><span class="sxs-lookup"><span data-stu-id="3b949-137">Add</span></span>](../api/chartcollection_add.md)|[<span data-ttu-id="3b949-138">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="3b949-138">WorkbookChart</span></span>](chart.md)|<span data-ttu-id="3b949-139">创建新图表。</span><span class="sxs-lookup"><span data-stu-id="3b949-139">Creates a new chart.</span></span>|

## <a name="properties"></a><span data-ttu-id="3b949-140">属性</span><span class="sxs-lookup"><span data-stu-id="3b949-140">Properties</span></span>
| <span data-ttu-id="3b949-141">属性</span><span class="sxs-lookup"><span data-stu-id="3b949-141">Property</span></span>     | <span data-ttu-id="3b949-142">类型</span><span class="sxs-lookup"><span data-stu-id="3b949-142">Type</span></span>   |<span data-ttu-id="3b949-143">说明</span><span class="sxs-lookup"><span data-stu-id="3b949-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b949-144">height</span><span class="sxs-lookup"><span data-stu-id="3b949-144">height</span></span>|<span data-ttu-id="3b949-145">double</span><span class="sxs-lookup"><span data-stu-id="3b949-145">double</span></span>|<span data-ttu-id="3b949-146">表示 chart 对象的高度，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="3b949-146">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="3b949-147">id</span><span class="sxs-lookup"><span data-stu-id="3b949-147">id</span></span>|<span data-ttu-id="3b949-148">string</span><span class="sxs-lookup"><span data-stu-id="3b949-148">string</span></span>|<span data-ttu-id="3b949-p101">根据其在集合中的位置获取图表。只读。</span><span class="sxs-lookup"><span data-stu-id="3b949-p101">Gets a chart based on its position in the collection. Read-only.</span></span>|
|<span data-ttu-id="3b949-151">left</span><span class="sxs-lookup"><span data-stu-id="3b949-151">left</span></span>|<span data-ttu-id="3b949-152">double</span><span class="sxs-lookup"><span data-stu-id="3b949-152">double</span></span>|<span data-ttu-id="3b949-153">从图表左侧到工作表原点的距离，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="3b949-153">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="3b949-154">name</span><span class="sxs-lookup"><span data-stu-id="3b949-154">name</span></span>|<span data-ttu-id="3b949-155">string</span><span class="sxs-lookup"><span data-stu-id="3b949-155">string</span></span>|<span data-ttu-id="3b949-156">表示 chart 对象的名称。</span><span class="sxs-lookup"><span data-stu-id="3b949-156">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="3b949-157">top</span><span class="sxs-lookup"><span data-stu-id="3b949-157">top</span></span>|<span data-ttu-id="3b949-158">double</span><span class="sxs-lookup"><span data-stu-id="3b949-158">double</span></span>|<span data-ttu-id="3b949-159">表示从对象左边界至第 1 行顶部（在工作表上）或图表区域顶部（在图表上）的距离，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="3b949-159">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="3b949-160">width</span><span class="sxs-lookup"><span data-stu-id="3b949-160">width</span></span>|<span data-ttu-id="3b949-161">double</span><span class="sxs-lookup"><span data-stu-id="3b949-161">double</span></span>|<span data-ttu-id="3b949-162">表示 chart 对象的宽度，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="3b949-162">Represents the width, in points, of the chart object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b949-163">关系</span><span class="sxs-lookup"><span data-stu-id="3b949-163">Relationships</span></span>
| <span data-ttu-id="3b949-164">关系</span><span class="sxs-lookup"><span data-stu-id="3b949-164">Relationship</span></span> | <span data-ttu-id="3b949-165">类型</span><span class="sxs-lookup"><span data-stu-id="3b949-165">Type</span></span>   |<span data-ttu-id="3b949-166">说明</span><span class="sxs-lookup"><span data-stu-id="3b949-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b949-167">axes</span><span class="sxs-lookup"><span data-stu-id="3b949-167">axes</span></span>|[<span data-ttu-id="3b949-168">WorkbookChartAxes</span><span class="sxs-lookup"><span data-stu-id="3b949-168">WorkbookChartAxes</span></span>](chartaxes.md)|<span data-ttu-id="3b949-p102">表示图表坐标轴。只读。</span><span class="sxs-lookup"><span data-stu-id="3b949-p102">Represents chart axes. Read-only.</span></span>|
|<span data-ttu-id="3b949-171">dataLabels</span><span class="sxs-lookup"><span data-stu-id="3b949-171">dataLabels</span></span>|[<span data-ttu-id="3b949-172">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="3b949-172">WorkbookChartDataLabels</span></span>](chartdatalabels.md)|<span data-ttu-id="3b949-p103">表示图表上的数据标签。只读。</span><span class="sxs-lookup"><span data-stu-id="3b949-p103">Represents the datalabels on the chart. Read-only.</span></span>|
|<span data-ttu-id="3b949-175">format</span><span class="sxs-lookup"><span data-stu-id="3b949-175">format</span></span>|[<span data-ttu-id="3b949-176">WorkbookChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="3b949-176">WorkbookChartAreaFormat</span></span>](chartareaformat.md)|<span data-ttu-id="3b949-p104">封装图表区域的格式属性。只读。</span><span class="sxs-lookup"><span data-stu-id="3b949-p104">Encapsulates the format properties for the chart area. Read-only.</span></span>|
|<span data-ttu-id="3b949-179">legend</span><span class="sxs-lookup"><span data-stu-id="3b949-179">legend</span></span>|[<span data-ttu-id="3b949-180">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="3b949-180">WorkbookChartLegend</span></span>](chartlegend.md)|<span data-ttu-id="3b949-p105">表示图表的图例。只读。</span><span class="sxs-lookup"><span data-stu-id="3b949-p105">Represents the legend for the chart. Read-only.</span></span>|
|<span data-ttu-id="3b949-183">series</span><span class="sxs-lookup"><span data-stu-id="3b949-183">series</span></span>|<span data-ttu-id="3b949-184">[WorkbookChartSeries](chartseries.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3b949-184">[WorkbookChartSeries](chartseries.md) collection</span></span>|<span data-ttu-id="3b949-p106">表示单个系列或图表中的系列集合。只读。</span><span class="sxs-lookup"><span data-stu-id="3b949-p106">Represents either a single series or collection of series in the chart. Read-only.</span></span>|
|<span data-ttu-id="3b949-187">title</span><span class="sxs-lookup"><span data-stu-id="3b949-187">title</span></span>|[<span data-ttu-id="3b949-188">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="3b949-188">WorkbookChartTitle</span></span>](charttitle.md)|<span data-ttu-id="3b949-p107">表示指定图表的标题，包括标题的文本、可见性、位置和格式。只读。</span><span class="sxs-lookup"><span data-stu-id="3b949-p107">Represents the title of the specified chart, including the text, visibility, position and formating of the title. Read-only.</span></span>|
|<span data-ttu-id="3b949-191">worksheet</span><span class="sxs-lookup"><span data-stu-id="3b949-191">worksheet</span></span>|[<span data-ttu-id="3b949-192">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="3b949-192">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="3b949-p108">包含当前 chart 的 worksheet 对象。只读。</span><span class="sxs-lookup"><span data-stu-id="3b949-p108">The worksheet containing the current chart. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3b949-195">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3b949-195">JSON representation</span></span>

<span data-ttu-id="3b949-196">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3b949-196">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChart"
}-->

```json
{
  "height": 1024,
  "id": "string",
  "left": 1024,
  "name": "string",
  "top": 1024,
  "width": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->