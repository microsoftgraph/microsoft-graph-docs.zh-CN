# <a name="chartlegend-resource-type"></a><span data-ttu-id="51077-101">ChartLegend 资源类型</span><span class="sxs-lookup"><span data-stu-id="51077-101">ChartLegend resource type</span></span>

<span data-ttu-id="51077-102">表示图表中的图例。</span><span class="sxs-lookup"><span data-stu-id="51077-102">Represents the legend in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="51077-103">方法</span><span class="sxs-lookup"><span data-stu-id="51077-103">Methods</span></span>

| <span data-ttu-id="51077-104">方法</span><span class="sxs-lookup"><span data-stu-id="51077-104">Method</span></span>           | <span data-ttu-id="51077-105">返回类型</span><span class="sxs-lookup"><span data-stu-id="51077-105">Return Type</span></span>    |<span data-ttu-id="51077-106">说明</span><span class="sxs-lookup"><span data-stu-id="51077-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="51077-107">获取 ChartLegend</span><span class="sxs-lookup"><span data-stu-id="51077-107">Get ChartLegend</span></span>](../api/chartlegend_get.md) | [<span data-ttu-id="51077-108">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="51077-108">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="51077-109">读取 chartLegend 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="51077-109">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="51077-110">更新</span><span class="sxs-lookup"><span data-stu-id="51077-110">Update</span></span>](../api/chartlegend_update.md) | [<span data-ttu-id="51077-111">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="51077-111">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="51077-112">更新 ChartLegend 对象。</span><span class="sxs-lookup"><span data-stu-id="51077-112">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="51077-113">属性</span><span class="sxs-lookup"><span data-stu-id="51077-113">Properties</span></span>
| <span data-ttu-id="51077-114">属性</span><span class="sxs-lookup"><span data-stu-id="51077-114">Property</span></span>     | <span data-ttu-id="51077-115">类型</span><span class="sxs-lookup"><span data-stu-id="51077-115">Type</span></span>   |<span data-ttu-id="51077-116">说明</span><span class="sxs-lookup"><span data-stu-id="51077-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51077-117">overlay</span><span class="sxs-lookup"><span data-stu-id="51077-117">overlay</span></span>|<span data-ttu-id="51077-118">boolean</span><span class="sxs-lookup"><span data-stu-id="51077-118">boolean</span></span>|<span data-ttu-id="51077-119">表示图表图例是否应该与图表主体重叠的布尔值。</span><span class="sxs-lookup"><span data-stu-id="51077-119">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="51077-120">position</span><span class="sxs-lookup"><span data-stu-id="51077-120">position</span></span>|<span data-ttu-id="51077-121">string</span><span class="sxs-lookup"><span data-stu-id="51077-121">string</span></span>|<span data-ttu-id="51077-122">代表图表上图例的位置。</span><span class="sxs-lookup"><span data-stu-id="51077-122">Represents the position of the legend on the chart. Possible values are: , , , , , .</span></span> <span data-ttu-id="51077-123">可取值为：`Top`、`Bottom`、`Left`、`Right`、`Corner`、`Custom`。</span><span class="sxs-lookup"><span data-stu-id="51077-123">The possible values are `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`, , , , , , or .</span></span>|
|<span data-ttu-id="51077-124">visible</span><span class="sxs-lookup"><span data-stu-id="51077-124">visible</span></span>|<span data-ttu-id="51077-125">boolean</span><span class="sxs-lookup"><span data-stu-id="51077-125">boolean</span></span>|<span data-ttu-id="51077-126">表示 ChartLegend 对象的可见性的布尔值。</span><span class="sxs-lookup"><span data-stu-id="51077-126">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51077-127">关系</span><span class="sxs-lookup"><span data-stu-id="51077-127">Relationships</span></span>
| <span data-ttu-id="51077-128">关系</span><span class="sxs-lookup"><span data-stu-id="51077-128">Relationship</span></span> | <span data-ttu-id="51077-129">类型</span><span class="sxs-lookup"><span data-stu-id="51077-129">Type</span></span>   |<span data-ttu-id="51077-130">说明</span><span class="sxs-lookup"><span data-stu-id="51077-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51077-131">format</span><span class="sxs-lookup"><span data-stu-id="51077-131">format</span></span>|[<span data-ttu-id="51077-132">WorkbookChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="51077-132">WorkbookChartLegendFormat</span></span>](chartlegendformat.md)|<span data-ttu-id="51077-p102">表示图表图例的格式，包括填充和字体格式。只读。</span><span class="sxs-lookup"><span data-stu-id="51077-p102">Represents the formatting of a chart legend, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="51077-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="51077-135">JSON representation</span></span>

<span data-ttu-id="51077-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51077-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartLegend"
}-->

```json
{
  "overlay": true,
  "position": "string",
  "visible": true,
  "format": {"@odata.type":"microsoft.graph.workbookChartLegendFormat"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLegend resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->