# <a name="chartdatalabelformat-resource-type"></a><span data-ttu-id="71ffe-101">ChartDataLabelFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="71ffe-101">ChartDataLabelFormat resource type</span></span>

<span data-ttu-id="71ffe-102">封装图表数据表的格式属性。</span><span class="sxs-lookup"><span data-stu-id="71ffe-102">Encapsulates the format properties for the chart data labels.</span></span>


## <a name="methods"></a><span data-ttu-id="71ffe-103">方法</span><span class="sxs-lookup"><span data-stu-id="71ffe-103">Methods</span></span>
<span data-ttu-id="71ffe-104">无</span><span class="sxs-lookup"><span data-stu-id="71ffe-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="71ffe-105">属性</span><span class="sxs-lookup"><span data-stu-id="71ffe-105">Properties</span></span>
<span data-ttu-id="71ffe-106">无</span><span class="sxs-lookup"><span data-stu-id="71ffe-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="71ffe-107">关系</span><span class="sxs-lookup"><span data-stu-id="71ffe-107">Relationships</span></span>
| <span data-ttu-id="71ffe-108">关系</span><span class="sxs-lookup"><span data-stu-id="71ffe-108">Relationship</span></span> | <span data-ttu-id="71ffe-109">类型</span><span class="sxs-lookup"><span data-stu-id="71ffe-109">Type</span></span>   |<span data-ttu-id="71ffe-110">说明</span><span class="sxs-lookup"><span data-stu-id="71ffe-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71ffe-111">fill</span><span class="sxs-lookup"><span data-stu-id="71ffe-111">fill</span></span>|[<span data-ttu-id="71ffe-112">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="71ffe-112">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="71ffe-p101">表示当前图表数据标签的填充格式。只读。</span><span class="sxs-lookup"><span data-stu-id="71ffe-p101">Represents the fill format of the current chart data label. Read-only.</span></span>|
|<span data-ttu-id="71ffe-115">font</span><span class="sxs-lookup"><span data-stu-id="71ffe-115">font</span></span>|[<span data-ttu-id="71ffe-116">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="71ffe-116">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="71ffe-p102">表示图表数据标签的字体属性（字体名称、字体大小、颜色等）。只读。</span><span class="sxs-lookup"><span data-stu-id="71ffe-p102">Represents the font attributes (font name, font size, color, etc.) for a chart data label. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="71ffe-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="71ffe-119">JSON representation</span></span>

<span data-ttu-id="71ffe-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="71ffe-120">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartDataLabelFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartDataLabelFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->