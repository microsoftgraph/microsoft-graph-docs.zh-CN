# <a name="chartpointformat-resource-type"></a><span data-ttu-id="961e5-101">ChartPointFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="961e5-101">ChartPointFormat resource type</span></span>

<span data-ttu-id="961e5-102">表示图表点的格式化对象。</span><span class="sxs-lookup"><span data-stu-id="961e5-102">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="961e5-103">方法</span><span class="sxs-lookup"><span data-stu-id="961e5-103">Methods</span></span>
<span data-ttu-id="961e5-104">无</span><span class="sxs-lookup"><span data-stu-id="961e5-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="961e5-105">属性</span><span class="sxs-lookup"><span data-stu-id="961e5-105">Properties</span></span>
<span data-ttu-id="961e5-106">无</span><span class="sxs-lookup"><span data-stu-id="961e5-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="961e5-107">关系</span><span class="sxs-lookup"><span data-stu-id="961e5-107">Relationships</span></span>
| <span data-ttu-id="961e5-108">关系</span><span class="sxs-lookup"><span data-stu-id="961e5-108">Relationship</span></span> | <span data-ttu-id="961e5-109">类型</span><span class="sxs-lookup"><span data-stu-id="961e5-109">Type</span></span>   |<span data-ttu-id="961e5-110">说明</span><span class="sxs-lookup"><span data-stu-id="961e5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="961e5-111">fill</span><span class="sxs-lookup"><span data-stu-id="961e5-111">fill</span></span>|[<span data-ttu-id="961e5-112">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="961e5-112">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="961e5-p101">表示图表的填充格式，包括背景格式信息。只读。</span><span class="sxs-lookup"><span data-stu-id="961e5-p101">Represents the fill format of a chart, which includes background formating information. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="961e5-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="961e5-115">JSON representation</span></span>

<span data-ttu-id="961e5-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="961e5-116">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPointFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPointFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->