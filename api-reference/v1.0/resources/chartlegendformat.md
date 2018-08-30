# <a name="chartlegendformat-resource-type"></a><span data-ttu-id="4fd02-101">ChartLegendFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="4fd02-101">ChartLegendFormat resource type</span></span>

<span data-ttu-id="4fd02-102">封装图表图例的格式属性。</span><span class="sxs-lookup"><span data-stu-id="4fd02-102">Encapsulates the format properties of a chart legend.</span></span>


## <a name="methods"></a><span data-ttu-id="4fd02-103">方法</span><span class="sxs-lookup"><span data-stu-id="4fd02-103">Methods</span></span>
<span data-ttu-id="4fd02-104">无</span><span class="sxs-lookup"><span data-stu-id="4fd02-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="4fd02-105">属性</span><span class="sxs-lookup"><span data-stu-id="4fd02-105">Properties</span></span>
<span data-ttu-id="4fd02-106">无</span><span class="sxs-lookup"><span data-stu-id="4fd02-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="4fd02-107">关系</span><span class="sxs-lookup"><span data-stu-id="4fd02-107">Relationships</span></span>
| <span data-ttu-id="4fd02-108">关系</span><span class="sxs-lookup"><span data-stu-id="4fd02-108">Relationship</span></span> | <span data-ttu-id="4fd02-109">类型</span><span class="sxs-lookup"><span data-stu-id="4fd02-109">Type</span></span>   |<span data-ttu-id="4fd02-110">说明</span><span class="sxs-lookup"><span data-stu-id="4fd02-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4fd02-111">fill</span><span class="sxs-lookup"><span data-stu-id="4fd02-111">fill</span></span>|[<span data-ttu-id="4fd02-112">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="4fd02-112">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="4fd02-p101">表示对象的填充格式，包括背景格式信息。只读。</span><span class="sxs-lookup"><span data-stu-id="4fd02-p101">Represents the fill format of an object, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="4fd02-115">font</span><span class="sxs-lookup"><span data-stu-id="4fd02-115">font</span></span>|[<span data-ttu-id="4fd02-116">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="4fd02-116">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="4fd02-p102">表示图表图例的字体属性，例如字体名称、字体大小、颜色等。只读。</span><span class="sxs-lookup"><span data-stu-id="4fd02-p102">Represents the font attributes such as font name, font size, color, etc. of a chart legend. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="4fd02-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4fd02-119">JSON representation</span></span>

<span data-ttu-id="4fd02-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4fd02-120">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartLegendFormat"
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
  "description": "ChartLegendFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->