# <a name="chartgridlines-resource-type"></a><span data-ttu-id="d05f2-101">ChartGridlines 资源类型</span><span class="sxs-lookup"><span data-stu-id="d05f2-101">ChartGridlines resource type</span></span>

<span data-ttu-id="d05f2-102">代表图表坐标轴的主要或次要网格线。</span><span class="sxs-lookup"><span data-stu-id="d05f2-102">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="d05f2-103">方法</span><span class="sxs-lookup"><span data-stu-id="d05f2-103">Methods</span></span>

| <span data-ttu-id="d05f2-104">方法</span><span class="sxs-lookup"><span data-stu-id="d05f2-104">Method</span></span>           | <span data-ttu-id="d05f2-105">返回类型</span><span class="sxs-lookup"><span data-stu-id="d05f2-105">Return Type</span></span>    |<span data-ttu-id="d05f2-106">说明</span><span class="sxs-lookup"><span data-stu-id="d05f2-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d05f2-107">获取 ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="d05f2-107">Get ChartGridlines</span></span>](../api/chartgridlines_get.md) | [<span data-ttu-id="d05f2-108">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="d05f2-108">WorkbookChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="d05f2-109">读取 chartGridlines 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d05f2-109">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="d05f2-110">Update</span><span class="sxs-lookup"><span data-stu-id="d05f2-110">Update</span></span>](../api/chartgridlines_update.md) | [<span data-ttu-id="d05f2-111">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="d05f2-111">WorkbookChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="d05f2-112">更新 ChartGridlines 对象。</span><span class="sxs-lookup"><span data-stu-id="d05f2-112">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d05f2-113">属性</span><span class="sxs-lookup"><span data-stu-id="d05f2-113">Properties</span></span>
| <span data-ttu-id="d05f2-114">属性</span><span class="sxs-lookup"><span data-stu-id="d05f2-114">Property</span></span>     | <span data-ttu-id="d05f2-115">类型</span><span class="sxs-lookup"><span data-stu-id="d05f2-115">Type</span></span>   |<span data-ttu-id="d05f2-116">说明</span><span class="sxs-lookup"><span data-stu-id="d05f2-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d05f2-117">可见</span><span class="sxs-lookup"><span data-stu-id="d05f2-117">visible</span></span>|<span data-ttu-id="d05f2-118">布尔值</span><span class="sxs-lookup"><span data-stu-id="d05f2-118">boolean</span></span>|<span data-ttu-id="d05f2-119">表示坐标轴网格线是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="d05f2-119">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d05f2-120">关系</span><span class="sxs-lookup"><span data-stu-id="d05f2-120">Relationships</span></span>
| <span data-ttu-id="d05f2-121">关系</span><span class="sxs-lookup"><span data-stu-id="d05f2-121">Relationship</span></span> | <span data-ttu-id="d05f2-122">类型</span><span class="sxs-lookup"><span data-stu-id="d05f2-122">Type</span></span>   |<span data-ttu-id="d05f2-123">说明</span><span class="sxs-lookup"><span data-stu-id="d05f2-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d05f2-124">format</span><span class="sxs-lookup"><span data-stu-id="d05f2-124">format</span></span>|[<span data-ttu-id="d05f2-125">WorkbookChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="d05f2-125">WorkbookChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="d05f2-p101">表示图表网格线的格式。只读。</span><span class="sxs-lookup"><span data-stu-id="d05f2-p101">Represents the formatting of chart gridlines. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d05f2-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d05f2-128">JSON representation</span></span>

<span data-ttu-id="d05f2-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d05f2-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartGridlines"
}-->

```json
{
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartGridlines resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->