# <a name="chartaxistitle-resource-type"></a><span data-ttu-id="de81e-101">ChartAxisTitle 资源类型</span><span class="sxs-lookup"><span data-stu-id="de81e-101">ChartAxisTitle resource type</span></span>

<span data-ttu-id="de81e-102">表示图表坐标轴的标题。</span><span class="sxs-lookup"><span data-stu-id="de81e-102">Represents the title of a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="de81e-103">方法</span><span class="sxs-lookup"><span data-stu-id="de81e-103">Methods</span></span>

| <span data-ttu-id="de81e-104">方法</span><span class="sxs-lookup"><span data-stu-id="de81e-104">Method</span></span>           | <span data-ttu-id="de81e-105">返回类型</span><span class="sxs-lookup"><span data-stu-id="de81e-105">Return Type</span></span>    |<span data-ttu-id="de81e-106">说明</span><span class="sxs-lookup"><span data-stu-id="de81e-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="de81e-107">Get ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="de81e-107">Get ChartAxisTitle</span></span>](../api/chartaxistitle_get.md) | [<span data-ttu-id="de81e-108">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="de81e-108">WorkbookChartAxisTitle</span></span>](chartaxistitle.md) |<span data-ttu-id="de81e-109">读取 chartAxisTitle 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="de81e-109">Read properties and relationships of chartAxisTitle object.</span></span>|
|[<span data-ttu-id="de81e-110">Update</span><span class="sxs-lookup"><span data-stu-id="de81e-110">Update</span></span>](../api/chartaxistitle_update.md) | [<span data-ttu-id="de81e-111">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="de81e-111">WorkbookChartAxisTitle</span></span>](chartaxistitle.md)    |<span data-ttu-id="de81e-112">更新 ChartAxisTitle 对象。</span><span class="sxs-lookup"><span data-stu-id="de81e-112">Update ChartAxisTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="de81e-113">属性</span><span class="sxs-lookup"><span data-stu-id="de81e-113">Properties</span></span>
| <span data-ttu-id="de81e-114">属性</span><span class="sxs-lookup"><span data-stu-id="de81e-114">Property</span></span>     | <span data-ttu-id="de81e-115">类型</span><span class="sxs-lookup"><span data-stu-id="de81e-115">Type</span></span>   |<span data-ttu-id="de81e-116">说明</span><span class="sxs-lookup"><span data-stu-id="de81e-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de81e-117">text</span><span class="sxs-lookup"><span data-stu-id="de81e-117">text</span></span>|<span data-ttu-id="de81e-118">字符串</span><span class="sxs-lookup"><span data-stu-id="de81e-118">string</span></span>|<span data-ttu-id="de81e-119">表示坐标轴标题。</span><span class="sxs-lookup"><span data-stu-id="de81e-119">Represents the axis title.</span></span>|
|<span data-ttu-id="de81e-120">visible</span><span class="sxs-lookup"><span data-stu-id="de81e-120">visible</span></span>|<span data-ttu-id="de81e-121">布尔值</span><span class="sxs-lookup"><span data-stu-id="de81e-121">boolean</span></span>|<span data-ttu-id="de81e-122">指定坐标轴标题可见性的布尔值。</span><span class="sxs-lookup"><span data-stu-id="de81e-122">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de81e-123">关系</span><span class="sxs-lookup"><span data-stu-id="de81e-123">Relationships</span></span>
| <span data-ttu-id="de81e-124">关系</span><span class="sxs-lookup"><span data-stu-id="de81e-124">Relationship</span></span> | <span data-ttu-id="de81e-125">类型</span><span class="sxs-lookup"><span data-stu-id="de81e-125">Type</span></span>   |<span data-ttu-id="de81e-126">说明</span><span class="sxs-lookup"><span data-stu-id="de81e-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de81e-127">format</span><span class="sxs-lookup"><span data-stu-id="de81e-127">format</span></span>|[<span data-ttu-id="de81e-128">WorkbookChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="de81e-128">WorkbookChartAxisTitleFormat</span></span>](chartaxistitleformat.md)|<span data-ttu-id="de81e-p101">表示图表坐标轴标题的格式。只读。</span><span class="sxs-lookup"><span data-stu-id="de81e-p101">Represents the formatting of chart axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="de81e-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="de81e-131">JSON representation</span></span>

<span data-ttu-id="de81e-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de81e-132">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartAxisTitle"
}-->

```json
{
  "text": "string",
  "visible": true,
  "format": {"@odata.type":"microsoft.graph.workbookChartAxisTitleFormat"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->