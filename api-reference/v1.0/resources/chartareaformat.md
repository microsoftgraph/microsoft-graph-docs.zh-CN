# <a name="chartareaformat-resource-type"></a><span data-ttu-id="47e5e-101">ChartAreaFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="47e5e-101">ChartAreaFormat resource type</span></span>

<span data-ttu-id="47e5e-102">封装整个图表区域的格式属性。</span><span class="sxs-lookup"><span data-stu-id="47e5e-102">Encapsulates the format properties for the overall chart area.</span></span>


## <a name="methods"></a><span data-ttu-id="47e5e-103">方法</span><span class="sxs-lookup"><span data-stu-id="47e5e-103">Methods</span></span>
<span data-ttu-id="47e5e-104">无</span><span class="sxs-lookup"><span data-stu-id="47e5e-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="47e5e-105">属性</span><span class="sxs-lookup"><span data-stu-id="47e5e-105">Properties</span></span>
<span data-ttu-id="47e5e-106">无</span><span class="sxs-lookup"><span data-stu-id="47e5e-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="47e5e-107">关系</span><span class="sxs-lookup"><span data-stu-id="47e5e-107">Relationships</span></span>
| <span data-ttu-id="47e5e-108">关系</span><span class="sxs-lookup"><span data-stu-id="47e5e-108">Relationship</span></span> | <span data-ttu-id="47e5e-109">类型</span><span class="sxs-lookup"><span data-stu-id="47e5e-109">Type</span></span>   |<span data-ttu-id="47e5e-110">说明</span><span class="sxs-lookup"><span data-stu-id="47e5e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47e5e-111">fill</span><span class="sxs-lookup"><span data-stu-id="47e5e-111">fill</span></span>|[<span data-ttu-id="47e5e-112">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="47e5e-112">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="47e5e-p101">表示对象的填充格式，包括背景格式信息。只读。</span><span class="sxs-lookup"><span data-stu-id="47e5e-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="47e5e-115">font</span><span class="sxs-lookup"><span data-stu-id="47e5e-115">font</span></span>|[<span data-ttu-id="47e5e-116">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="47e5e-116">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="47e5e-p102">表示当前对象的字体属性（字体名称、字体大小、颜色等）。只读。</span><span class="sxs-lookup"><span data-stu-id="47e5e-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="47e5e-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="47e5e-119">JSON representation</span></span>

<span data-ttu-id="47e5e-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="47e5e-120">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAreaFormat"
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
  "description": "ChartAreaFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->