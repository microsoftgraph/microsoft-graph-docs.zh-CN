# <a name="chartgridlinesformat-resource-type"></a><span data-ttu-id="9f0de-101">ChartGridlinesFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="9f0de-101">ChartGridlinesFormat resource type</span></span>

<span data-ttu-id="9f0de-102">封装图表网格线的格式属性。</span><span class="sxs-lookup"><span data-stu-id="9f0de-102">Encapsulates the format properties for chart gridlines.</span></span>


## <a name="methods"></a><span data-ttu-id="9f0de-103">方法</span><span class="sxs-lookup"><span data-stu-id="9f0de-103">Methods</span></span>
<span data-ttu-id="9f0de-104">无</span><span class="sxs-lookup"><span data-stu-id="9f0de-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="9f0de-105">属性</span><span class="sxs-lookup"><span data-stu-id="9f0de-105">Properties</span></span>
<span data-ttu-id="9f0de-106">无</span><span class="sxs-lookup"><span data-stu-id="9f0de-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="9f0de-107">关系</span><span class="sxs-lookup"><span data-stu-id="9f0de-107">Relationships</span></span>
| <span data-ttu-id="9f0de-108">关系</span><span class="sxs-lookup"><span data-stu-id="9f0de-108">Relationship</span></span> | <span data-ttu-id="9f0de-109">类型</span><span class="sxs-lookup"><span data-stu-id="9f0de-109">Type</span></span>   |<span data-ttu-id="9f0de-110">说明</span><span class="sxs-lookup"><span data-stu-id="9f0de-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f0de-111">line</span><span class="sxs-lookup"><span data-stu-id="9f0de-111">line</span></span>|[<span data-ttu-id="9f0de-112">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="9f0de-112">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="9f0de-p101">表示图表线条格式。只读。</span><span class="sxs-lookup"><span data-stu-id="9f0de-p101">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="9f0de-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9f0de-115">JSON representation</span></span>

<span data-ttu-id="9f0de-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9f0de-116">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartGridlinesFormat"
}-->

```json
{
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartGridlinesFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->