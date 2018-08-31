# <a name="chartaxisformat-resource-type"></a><span data-ttu-id="ea294-101">ChartAxisFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="ea294-101">ChartAxisFormat resource type</span></span>

<span data-ttu-id="ea294-102">封装图表坐标轴的格式属性。</span><span class="sxs-lookup"><span data-stu-id="ea294-102">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="ea294-103">方法</span><span class="sxs-lookup"><span data-stu-id="ea294-103">Methods</span></span>
<span data-ttu-id="ea294-104">无</span><span class="sxs-lookup"><span data-stu-id="ea294-104">None</span></span>
## <a name="properties"></a><span data-ttu-id="ea294-105">属性</span><span class="sxs-lookup"><span data-stu-id="ea294-105">Properties</span></span>
<span data-ttu-id="ea294-106">无</span><span class="sxs-lookup"><span data-stu-id="ea294-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="ea294-107">关系</span><span class="sxs-lookup"><span data-stu-id="ea294-107">Relationships</span></span>
| <span data-ttu-id="ea294-108">关系</span><span class="sxs-lookup"><span data-stu-id="ea294-108">Relationship</span></span> | <span data-ttu-id="ea294-109">类型</span><span class="sxs-lookup"><span data-stu-id="ea294-109">Type</span></span>   |<span data-ttu-id="ea294-110">说明</span><span class="sxs-lookup"><span data-stu-id="ea294-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea294-111">font</span><span class="sxs-lookup"><span data-stu-id="ea294-111">font</span></span>|[<span data-ttu-id="ea294-112">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="ea294-112">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="ea294-p101">表示图表坐标轴元素的字体属性（字体名称、字体大小、颜色等）。只读。</span><span class="sxs-lookup"><span data-stu-id="ea294-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="ea294-115">line</span><span class="sxs-lookup"><span data-stu-id="ea294-115">line</span></span>|[<span data-ttu-id="ea294-116">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="ea294-116">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="ea294-p102">表示图表线条格式。只读。</span><span class="sxs-lookup"><span data-stu-id="ea294-p102">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="ea294-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ea294-119">JSON representation</span></span>

<span data-ttu-id="ea294-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea294-120">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"},
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->