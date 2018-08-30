# <a name="chartaxistitleformat-resource-type"></a><span data-ttu-id="d4e3b-101">ChartAxisTitleFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4e3b-101">ChartAxisTitleFormat resource type</span></span>

<span data-ttu-id="d4e3b-102">表示图表坐标轴标题格式。</span><span class="sxs-lookup"><span data-stu-id="d4e3b-102">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="d4e3b-103">方法</span><span class="sxs-lookup"><span data-stu-id="d4e3b-103">Methods</span></span>
<span data-ttu-id="d4e3b-104">无</span><span class="sxs-lookup"><span data-stu-id="d4e3b-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="d4e3b-105">属性</span><span class="sxs-lookup"><span data-stu-id="d4e3b-105">Properties</span></span>
<span data-ttu-id="d4e3b-106">无</span><span class="sxs-lookup"><span data-stu-id="d4e3b-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="d4e3b-107">关系</span><span class="sxs-lookup"><span data-stu-id="d4e3b-107">Relationships</span></span>
| <span data-ttu-id="d4e3b-108">关系</span><span class="sxs-lookup"><span data-stu-id="d4e3b-108">Relationship</span></span> | <span data-ttu-id="d4e3b-109">类型</span><span class="sxs-lookup"><span data-stu-id="d4e3b-109">Type</span></span>   |<span data-ttu-id="d4e3b-110">说明</span><span class="sxs-lookup"><span data-stu-id="d4e3b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4e3b-111">字体</span><span class="sxs-lookup"><span data-stu-id="d4e3b-111">font</span></span>|[<span data-ttu-id="d4e3b-112">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="d4e3b-112">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="d4e3b-p101">表示图表坐标轴标题对象的字体属性，例如字体名称、字体大小、颜色等。只读。</span><span class="sxs-lookup"><span data-stu-id="d4e3b-p101">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d4e3b-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4e3b-115">JSON representation</span></span>

<span data-ttu-id="d4e3b-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4e3b-116">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisTitleFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitleFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->