# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="0cbee-101">ChartDataLabels 资源类型</span><span class="sxs-lookup"><span data-stu-id="0cbee-101">ChartDataLabels resource type</span></span>

<span data-ttu-id="0cbee-102">表示图表点上的所有数据标签的集合。</span><span class="sxs-lookup"><span data-stu-id="0cbee-102">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="0cbee-103">方法</span><span class="sxs-lookup"><span data-stu-id="0cbee-103">Methods</span></span>

| <span data-ttu-id="0cbee-104">方法</span><span class="sxs-lookup"><span data-stu-id="0cbee-104">Method</span></span>           | <span data-ttu-id="0cbee-105">返回类型</span><span class="sxs-lookup"><span data-stu-id="0cbee-105">Return Type</span></span>    |<span data-ttu-id="0cbee-106">说明</span><span class="sxs-lookup"><span data-stu-id="0cbee-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0cbee-107">Get ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="0cbee-107">Get ChartDataLabels</span></span>](../api/chartdatalabels_get.md) | [<span data-ttu-id="0cbee-108">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="0cbee-108">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="0cbee-109">读取 chartDataLabels 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0cbee-109">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="0cbee-110">Update</span><span class="sxs-lookup"><span data-stu-id="0cbee-110">Update</span></span>](../api/chartdatalabels_update.md) | [<span data-ttu-id="0cbee-111">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="0cbee-111">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="0cbee-112">更新 ChartDataLabels 对象。</span><span class="sxs-lookup"><span data-stu-id="0cbee-112">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0cbee-113">属性</span><span class="sxs-lookup"><span data-stu-id="0cbee-113">Properties</span></span>
| <span data-ttu-id="0cbee-114">属性</span><span class="sxs-lookup"><span data-stu-id="0cbee-114">Property</span></span>     | <span data-ttu-id="0cbee-115">类型</span><span class="sxs-lookup"><span data-stu-id="0cbee-115">Type</span></span>   |<span data-ttu-id="0cbee-116">说明</span><span class="sxs-lookup"><span data-stu-id="0cbee-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0cbee-117">position</span><span class="sxs-lookup"><span data-stu-id="0cbee-117">position</span></span>|<span data-ttu-id="0cbee-118">string</span><span class="sxs-lookup"><span data-stu-id="0cbee-118">string</span></span>|<span data-ttu-id="0cbee-119">表示数据标签位置的 DataLabelPosition 值。</span><span class="sxs-lookup"><span data-stu-id="0cbee-119">DataLabelPosition value that represents the position of the data label. Possible values are: , , , , , , , , , , .</span></span> <span data-ttu-id="0cbee-120">可取值为：`None`、`Center`、`InsideEnd`、`InsideBase`、`OutsideEnd`、`Left`、`Right`、`Top`、`Bottom`、`BestFit`、`Callout`。</span><span class="sxs-lookup"><span data-stu-id="0cbee-120">The possible values are `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`, or .</span></span>|
|<span data-ttu-id="0cbee-121">separator</span><span class="sxs-lookup"><span data-stu-id="0cbee-121">separator</span></span>|<span data-ttu-id="0cbee-122">string</span><span class="sxs-lookup"><span data-stu-id="0cbee-122">string</span></span>|<span data-ttu-id="0cbee-123">表示用于图表中数据标签的分隔符的字符串。</span><span class="sxs-lookup"><span data-stu-id="0cbee-123">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="0cbee-124">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="0cbee-124">showBubbleSize</span></span>|<span data-ttu-id="0cbee-125">boolean</span><span class="sxs-lookup"><span data-stu-id="0cbee-125">boolean</span></span>|<span data-ttu-id="0cbee-126">表示数据标签气泡大小是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="0cbee-126">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="0cbee-127">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="0cbee-127">showCategoryName</span></span>|<span data-ttu-id="0cbee-128">boolean</span><span class="sxs-lookup"><span data-stu-id="0cbee-128">boolean</span></span>|<span data-ttu-id="0cbee-129">表示数据标签类别名称是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="0cbee-129">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="0cbee-130">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="0cbee-130">showLegendKey</span></span>|<span data-ttu-id="0cbee-131">boolean</span><span class="sxs-lookup"><span data-stu-id="0cbee-131">boolean</span></span>|<span data-ttu-id="0cbee-132">表示数据标签图例标示是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="0cbee-132">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="0cbee-133">showPercentage</span><span class="sxs-lookup"><span data-stu-id="0cbee-133">showPercentage</span></span>|<span data-ttu-id="0cbee-134">boolean</span><span class="sxs-lookup"><span data-stu-id="0cbee-134">boolean</span></span>|<span data-ttu-id="0cbee-135">表示数据标签百分比是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="0cbee-135">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="0cbee-136">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="0cbee-136">showSeriesName</span></span>|<span data-ttu-id="0cbee-137">boolean</span><span class="sxs-lookup"><span data-stu-id="0cbee-137">boolean</span></span>|<span data-ttu-id="0cbee-138">表示数据标签系列名称是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="0cbee-138">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="0cbee-139">showValue</span><span class="sxs-lookup"><span data-stu-id="0cbee-139">showValue</span></span>|<span data-ttu-id="0cbee-140">boolean</span><span class="sxs-lookup"><span data-stu-id="0cbee-140">boolean</span></span>|<span data-ttu-id="0cbee-141">表示数据标签值是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="0cbee-141">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0cbee-142">关系</span><span class="sxs-lookup"><span data-stu-id="0cbee-142">Relationships</span></span>
| <span data-ttu-id="0cbee-143">关系</span><span class="sxs-lookup"><span data-stu-id="0cbee-143">Relationship</span></span> | <span data-ttu-id="0cbee-144">类型</span><span class="sxs-lookup"><span data-stu-id="0cbee-144">Type</span></span>   |<span data-ttu-id="0cbee-145">说明</span><span class="sxs-lookup"><span data-stu-id="0cbee-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0cbee-146">format</span><span class="sxs-lookup"><span data-stu-id="0cbee-146">format</span></span>|[<span data-ttu-id="0cbee-147">WorkbookChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="0cbee-147">WorkbookChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="0cbee-p102">表示图表数据标签的格式，包括填充和字体格式。只读。</span><span class="sxs-lookup"><span data-stu-id="0cbee-p102">Represents the format of chart data labels, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0cbee-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0cbee-150">JSON representation</span></span>

<span data-ttu-id="0cbee-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0cbee-151">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartDataLabels"
}-->

```json
{
  "position": "string",
  "separator": "string",
  "showBubbleSize": true,
  "showCategoryName": true,
  "showLegendKey": true,
  "showPercentage": true,
  "showSeriesName": true,
  "showValue": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartDataLabels resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->