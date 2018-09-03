# <a name="chartseriesformat-resource-type"></a><span data-ttu-id="a4907-101">ChartSeriesFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="a4907-101">ChartSeriesFormat resource type</span></span>

<span data-ttu-id="a4907-102">封装图表系列的格式属性</span><span class="sxs-lookup"><span data-stu-id="a4907-102">encapsulates the format properties for the chart series</span></span>


## <a name="methods"></a><span data-ttu-id="a4907-103">方法</span><span class="sxs-lookup"><span data-stu-id="a4907-103">Methods</span></span>
<span data-ttu-id="a4907-104">无</span><span class="sxs-lookup"><span data-stu-id="a4907-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="a4907-105">属性</span><span class="sxs-lookup"><span data-stu-id="a4907-105">Properties</span></span>
<span data-ttu-id="a4907-106">无</span><span class="sxs-lookup"><span data-stu-id="a4907-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="a4907-107">关系</span><span class="sxs-lookup"><span data-stu-id="a4907-107">Relationships</span></span>
| <span data-ttu-id="a4907-108">关系</span><span class="sxs-lookup"><span data-stu-id="a4907-108">Relationship</span></span> | <span data-ttu-id="a4907-109">类型</span><span class="sxs-lookup"><span data-stu-id="a4907-109">Type</span></span>   |<span data-ttu-id="a4907-110">说明</span><span class="sxs-lookup"><span data-stu-id="a4907-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4907-111">填充</span><span class="sxs-lookup"><span data-stu-id="a4907-111">fill</span></span>|[<span data-ttu-id="a4907-112">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="a4907-112">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="a4907-p101">表示图表序列的填充格式，包括背景格式化信息。只读。</span><span class="sxs-lookup"><span data-stu-id="a4907-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="a4907-115">line</span><span class="sxs-lookup"><span data-stu-id="a4907-115">line</span></span>|[<span data-ttu-id="a4907-116">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="a4907-116">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="a4907-p102">表示线条格式化。只读。</span><span class="sxs-lookup"><span data-stu-id="a4907-p102">Represents line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="a4907-119">JSON 表示</span><span class="sxs-lookup"><span data-stu-id="a4907-119">JSON representation</span></span>

<span data-ttu-id="a4907-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4907-120">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartSeriesFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeriesFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->