# <a name="charttitle-resource-type"></a><span data-ttu-id="7e52d-101">ChartTitle 资源类型</span><span class="sxs-lookup"><span data-stu-id="7e52d-101">ChartTitle resource type</span></span>

<span data-ttu-id="7e52d-102">表示图表的 chart title 对象。</span><span class="sxs-lookup"><span data-stu-id="7e52d-102">Represents a chart title object of a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="7e52d-103">方法</span><span class="sxs-lookup"><span data-stu-id="7e52d-103">Methods</span></span>

| <span data-ttu-id="7e52d-104">方法</span><span class="sxs-lookup"><span data-stu-id="7e52d-104">Method</span></span>           | <span data-ttu-id="7e52d-105">返回类型</span><span class="sxs-lookup"><span data-stu-id="7e52d-105">Return Type</span></span>    |<span data-ttu-id="7e52d-106">说明</span><span class="sxs-lookup"><span data-stu-id="7e52d-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7e52d-107">获取 ChartTitle</span><span class="sxs-lookup"><span data-stu-id="7e52d-107">Get ChartTitle</span></span>](../api/charttitle_get.md) | [<span data-ttu-id="7e52d-108">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="7e52d-108">WorkbookChartTitle</span></span>](charttitle.md) |<span data-ttu-id="7e52d-109">读取 chartTitle 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7e52d-109">Read properties and relationships of chartTitle object.</span></span>|
|[<span data-ttu-id="7e52d-110">更新</span><span class="sxs-lookup"><span data-stu-id="7e52d-110">Update</span></span>](../api/charttitle_update.md) | [<span data-ttu-id="7e52d-111">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="7e52d-111">WorkbookChartTitle</span></span>](charttitle.md)    |<span data-ttu-id="7e52d-112">更新 ChartTitle 对象。</span><span class="sxs-lookup"><span data-stu-id="7e52d-112">Update ChartTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7e52d-113">属性</span><span class="sxs-lookup"><span data-stu-id="7e52d-113">Properties</span></span>
| <span data-ttu-id="7e52d-114">属性</span><span class="sxs-lookup"><span data-stu-id="7e52d-114">Property</span></span>     | <span data-ttu-id="7e52d-115">类型</span><span class="sxs-lookup"><span data-stu-id="7e52d-115">Type</span></span>   |<span data-ttu-id="7e52d-116">说明</span><span class="sxs-lookup"><span data-stu-id="7e52d-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e52d-117">overlay</span><span class="sxs-lookup"><span data-stu-id="7e52d-117">overlay</span></span>|<span data-ttu-id="7e52d-118">布尔值</span><span class="sxs-lookup"><span data-stu-id="7e52d-118">boolean</span></span>|<span data-ttu-id="7e52d-119">表示图表标题是否将叠加在图表上的布尔值。</span><span class="sxs-lookup"><span data-stu-id="7e52d-119">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="7e52d-120">text</span><span class="sxs-lookup"><span data-stu-id="7e52d-120">text</span></span>|<span data-ttu-id="7e52d-121">字符串</span><span class="sxs-lookup"><span data-stu-id="7e52d-121">string</span></span>|<span data-ttu-id="7e52d-122">表示图表的标题文本。</span><span class="sxs-lookup"><span data-stu-id="7e52d-122">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="7e52d-123">visible</span><span class="sxs-lookup"><span data-stu-id="7e52d-123">visible</span></span>|<span data-ttu-id="7e52d-124">布尔值</span><span class="sxs-lookup"><span data-stu-id="7e52d-124">boolean</span></span>|<span data-ttu-id="7e52d-125">表示 chart title 对象的可见性的布尔值。</span><span class="sxs-lookup"><span data-stu-id="7e52d-125">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e52d-126">关系</span><span class="sxs-lookup"><span data-stu-id="7e52d-126">Relationships</span></span>
| <span data-ttu-id="7e52d-127">关系</span><span class="sxs-lookup"><span data-stu-id="7e52d-127">Relationship</span></span> | <span data-ttu-id="7e52d-128">类型</span><span class="sxs-lookup"><span data-stu-id="7e52d-128">Type</span></span>   |<span data-ttu-id="7e52d-129">说明</span><span class="sxs-lookup"><span data-stu-id="7e52d-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e52d-130">format</span><span class="sxs-lookup"><span data-stu-id="7e52d-130">format</span></span>|[<span data-ttu-id="7e52d-131">WorkbookChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="7e52d-131">WorkbookChartTitleFormat</span></span>](charttitleformat.md)|<span data-ttu-id="7e52d-p101">表示图表标题的格式，包括填充和字体格式。只读。</span><span class="sxs-lookup"><span data-stu-id="7e52d-p101">Represents the formatting of a chart title, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7e52d-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7e52d-134">JSON representation</span></span>

<span data-ttu-id="7e52d-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e52d-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartTitle"
}-->

```json
{
  "overlay": true,
  "text": "string",
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->