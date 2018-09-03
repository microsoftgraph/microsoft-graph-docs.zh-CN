# <a name="chartlineformat-resource-type"></a><span data-ttu-id="8fbb6-101">ChartLineFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="8fbb6-101">ChartLineFormat resource type</span></span>

<span data-ttu-id="8fbb6-102">封装线条元素的格式选项。</span><span class="sxs-lookup"><span data-stu-id="8fbb6-102">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="8fbb6-103">方法</span><span class="sxs-lookup"><span data-stu-id="8fbb6-103">Methods</span></span>

| <span data-ttu-id="8fbb6-104">方法</span><span class="sxs-lookup"><span data-stu-id="8fbb6-104">Method</span></span>           | <span data-ttu-id="8fbb6-105">返回类型</span><span class="sxs-lookup"><span data-stu-id="8fbb6-105">Return Type</span></span>    |<span data-ttu-id="8fbb6-106">说明</span><span class="sxs-lookup"><span data-stu-id="8fbb6-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8fbb6-107">Get ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="8fbb6-107">Get ChartLineFormat</span></span>](../api/chartlineformat_get.md) | [<span data-ttu-id="8fbb6-108">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="8fbb6-108">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="8fbb6-109">读取 chartLineFormat 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8fbb6-109">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="8fbb6-110">Update</span><span class="sxs-lookup"><span data-stu-id="8fbb6-110">Update</span></span>](../api/chartlineformat_update.md) | [<span data-ttu-id="8fbb6-111">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="8fbb6-111">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="8fbb6-112">更新 ChartLineFormat 对象。</span><span class="sxs-lookup"><span data-stu-id="8fbb6-112">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="8fbb6-113">Clear</span><span class="sxs-lookup"><span data-stu-id="8fbb6-113">Clear</span></span>](../api/chartlineformat_clear.md)|<span data-ttu-id="8fbb6-114">无</span><span class="sxs-lookup"><span data-stu-id="8fbb6-114">None</span></span>|<span data-ttu-id="8fbb6-115">清除图表元素的线条格式。</span><span class="sxs-lookup"><span data-stu-id="8fbb6-115">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="8fbb6-116">属性</span><span class="sxs-lookup"><span data-stu-id="8fbb6-116">Properties</span></span>
| <span data-ttu-id="8fbb6-117">属性</span><span class="sxs-lookup"><span data-stu-id="8fbb6-117">Property</span></span>     | <span data-ttu-id="8fbb6-118">类型</span><span class="sxs-lookup"><span data-stu-id="8fbb6-118">Type</span></span>   |<span data-ttu-id="8fbb6-119">说明</span><span class="sxs-lookup"><span data-stu-id="8fbb6-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8fbb6-120">color</span><span class="sxs-lookup"><span data-stu-id="8fbb6-120">color</span></span>|<span data-ttu-id="8fbb6-121">字符串</span><span class="sxs-lookup"><span data-stu-id="8fbb6-121">string</span></span>|<span data-ttu-id="8fbb6-122">表示图表中的线条颜色的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="8fbb6-122">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8fbb6-123">关系</span><span class="sxs-lookup"><span data-stu-id="8fbb6-123">Relationships</span></span>
<span data-ttu-id="8fbb6-124">无</span><span class="sxs-lookup"><span data-stu-id="8fbb6-124">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8fbb6-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8fbb6-125">JSON representation</span></span>

<span data-ttu-id="8fbb6-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8fbb6-126">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartLineFormat"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->