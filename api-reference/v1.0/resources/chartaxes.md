# <a name="chartaxes-resource-type"></a><span data-ttu-id="c4a29-101">ChartAxes 资源类型</span><span class="sxs-lookup"><span data-stu-id="c4a29-101">ChartAxes resource type</span></span>

<span data-ttu-id="c4a29-102">表示图表坐标轴。</span><span class="sxs-lookup"><span data-stu-id="c4a29-102">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="c4a29-103">方法</span><span class="sxs-lookup"><span data-stu-id="c4a29-103">Methods</span></span>
<span data-ttu-id="c4a29-104">无</span><span class="sxs-lookup"><span data-stu-id="c4a29-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="c4a29-105">属性</span><span class="sxs-lookup"><span data-stu-id="c4a29-105">Properties</span></span>
<span data-ttu-id="c4a29-106">无</span><span class="sxs-lookup"><span data-stu-id="c4a29-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="c4a29-107">关系</span><span class="sxs-lookup"><span data-stu-id="c4a29-107">Relationships</span></span>
| <span data-ttu-id="c4a29-108">关系</span><span class="sxs-lookup"><span data-stu-id="c4a29-108">Relationship</span></span> | <span data-ttu-id="c4a29-109">类型</span><span class="sxs-lookup"><span data-stu-id="c4a29-109">Type</span></span>   |<span data-ttu-id="c4a29-110">说明</span><span class="sxs-lookup"><span data-stu-id="c4a29-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4a29-111">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="c4a29-111">categoryAxis</span></span>|[<span data-ttu-id="c4a29-112">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="c4a29-112">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="c4a29-p101">表示图表中的类别轴。只读。</span><span class="sxs-lookup"><span data-stu-id="c4a29-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="c4a29-115">seriesAxis</span><span class="sxs-lookup"><span data-stu-id="c4a29-115">seriesAxis</span></span>|[<span data-ttu-id="c4a29-116">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="c4a29-116">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="c4a29-p102">表示三维图表的系列轴。只读。</span><span class="sxs-lookup"><span data-stu-id="c4a29-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="c4a29-119">valueAxis</span><span class="sxs-lookup"><span data-stu-id="c4a29-119">valueAxis</span></span>|[<span data-ttu-id="c4a29-120">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="c4a29-120">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="c4a29-p103">表示坐标轴中的数值轴。只读。</span><span class="sxs-lookup"><span data-stu-id="c4a29-p103">Represents the value axis in an axis. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c4a29-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c4a29-123">JSON representation</span></span>

<span data-ttu-id="c4a29-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c4a29-124">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxes"
}-->

```json
{
  "categoryAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"},
  "seriesAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"},
  "valueAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->