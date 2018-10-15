# <a name="chartaxis-resource-type"></a><span data-ttu-id="c6a38-101">ChartAxis 资源类型</span><span class="sxs-lookup"><span data-stu-id="c6a38-101">ChartAxis resource type</span></span>

<span data-ttu-id="c6a38-102">表示图表中的单个坐标轴。</span><span class="sxs-lookup"><span data-stu-id="c6a38-102">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="c6a38-103">方法</span><span class="sxs-lookup"><span data-stu-id="c6a38-103">Methods</span></span>

| <span data-ttu-id="c6a38-104">方法</span><span class="sxs-lookup"><span data-stu-id="c6a38-104">Method</span></span>           | <span data-ttu-id="c6a38-105">返回类型</span><span class="sxs-lookup"><span data-stu-id="c6a38-105">Return Type</span></span>    |<span data-ttu-id="c6a38-106">说明</span><span class="sxs-lookup"><span data-stu-id="c6a38-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c6a38-107">Get ChartAxis</span><span class="sxs-lookup"><span data-stu-id="c6a38-107">Get ChartAxis</span></span>](../api/chartaxis_get.md) | [<span data-ttu-id="c6a38-108">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="c6a38-108">WorkbookChartAxis</span></span>](chartaxis.md) |<span data-ttu-id="c6a38-109">读取 chartAxis 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c6a38-109">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="c6a38-110">Update</span><span class="sxs-lookup"><span data-stu-id="c6a38-110">Update</span></span>](../api/chartaxis_update.md) | [<span data-ttu-id="c6a38-111">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="c6a38-111">WorkbookChartAxis</span></span>](chartaxis.md)   |<span data-ttu-id="c6a38-112">更新 ChartAxis 对象</span><span class="sxs-lookup"><span data-stu-id="c6a38-112">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c6a38-113">属性</span><span class="sxs-lookup"><span data-stu-id="c6a38-113">Properties</span></span>
| <span data-ttu-id="c6a38-114">属性</span><span class="sxs-lookup"><span data-stu-id="c6a38-114">Property</span></span>     | <span data-ttu-id="c6a38-115">类型</span><span class="sxs-lookup"><span data-stu-id="c6a38-115">Type</span></span>   |<span data-ttu-id="c6a38-116">说明</span><span class="sxs-lookup"><span data-stu-id="c6a38-116">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c6a38-117">id</span><span class="sxs-lookup"><span data-stu-id="c6a38-117">id</span></span>       |<span data-ttu-id="c6a38-118">字符串</span><span class="sxs-lookup"><span data-stu-id="c6a38-118">string</span></span>   | <span data-ttu-id="c6a38-119">唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c6a38-119">Unique Identifier</span></span> <span data-ttu-id="c6a38-120">只读。</span><span class="sxs-lookup"><span data-stu-id="c6a38-120">Read-only.</span></span>|
|<span data-ttu-id="c6a38-121">majorUnit</span><span class="sxs-lookup"><span data-stu-id="c6a38-121">majorUnit</span></span>|<span data-ttu-id="c6a38-122">Json</span><span class="sxs-lookup"><span data-stu-id="c6a38-122">Json</span></span>|<span data-ttu-id="c6a38-p102">表示两个主要刻度标记之间的间隔。可以设置为数字值或空字符串。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="c6a38-p102">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="c6a38-126">maximum</span><span class="sxs-lookup"><span data-stu-id="c6a38-126">maximum</span></span>|<span data-ttu-id="c6a38-127">Json</span><span class="sxs-lookup"><span data-stu-id="c6a38-127">Json</span></span>|<span data-ttu-id="c6a38-p103">表示数值轴上的最大值。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="c6a38-p103">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="c6a38-131">minimum</span><span class="sxs-lookup"><span data-stu-id="c6a38-131">minimum</span></span>|<span data-ttu-id="c6a38-132">Json</span><span class="sxs-lookup"><span data-stu-id="c6a38-132">Json</span></span>|<span data-ttu-id="c6a38-p104">表示数值轴上的最小值。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="c6a38-p104">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="c6a38-136">minorUnit</span><span class="sxs-lookup"><span data-stu-id="c6a38-136">minorUnit</span></span>|<span data-ttu-id="c6a38-137">Json</span><span class="sxs-lookup"><span data-stu-id="c6a38-137">Json</span></span>|<span data-ttu-id="c6a38-p105">表示两个次要刻度标记之间的间隔。可以设置为数字值或空字符串（对于自动坐标轴值）。返回的值始终为数字。</span><span class="sxs-lookup"><span data-stu-id="c6a38-p105">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6a38-141">关系</span><span class="sxs-lookup"><span data-stu-id="c6a38-141">Relationships</span></span>
| <span data-ttu-id="c6a38-142">关系</span><span class="sxs-lookup"><span data-stu-id="c6a38-142">Relationship</span></span> | <span data-ttu-id="c6a38-143">类型</span><span class="sxs-lookup"><span data-stu-id="c6a38-143">Type</span></span>   |<span data-ttu-id="c6a38-144">说明</span><span class="sxs-lookup"><span data-stu-id="c6a38-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6a38-145">format</span><span class="sxs-lookup"><span data-stu-id="c6a38-145">format</span></span>|[<span data-ttu-id="c6a38-146">WorkbookChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="c6a38-146">WorkbookChartAxisFormat</span></span>](chartaxisformat.md)|<span data-ttu-id="c6a38-p106">表示 chart 对象的格式，包括线条和字体格式。只读。</span><span class="sxs-lookup"><span data-stu-id="c6a38-p106">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="c6a38-149">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="c6a38-149">majorGridlines</span></span>|[<span data-ttu-id="c6a38-150">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="c6a38-150">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="c6a38-p107">返回一个表示指定坐标轴的主要网格线的 gridline 对象。只读。</span><span class="sxs-lookup"><span data-stu-id="c6a38-p107">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="c6a38-153">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="c6a38-153">minorGridlines</span></span>|[<span data-ttu-id="c6a38-154">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="c6a38-154">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="c6a38-p108">返回一个表示指定坐标轴的次要网格线的网格线对象。只读。</span><span class="sxs-lookup"><span data-stu-id="c6a38-p108">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="c6a38-157">title</span><span class="sxs-lookup"><span data-stu-id="c6a38-157">title</span></span>|[<span data-ttu-id="c6a38-158">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="c6a38-158">WorkbookChartAxisTitle</span></span>](chartaxistitle.md)|<span data-ttu-id="c6a38-p109">表示坐标轴标题。只读。</span><span class="sxs-lookup"><span data-stu-id="c6a38-p109">Represents the axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c6a38-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c6a38-161">JSON representation</span></span>

<span data-ttu-id="c6a38-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6a38-162">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxis"
}-->

```json
{
  "id": "string",
  "majorUnit": "string",
  "maximum": "string",
  "minimum": "string",
  "minorUnit": "string",
   "format": {"@odata.type": "microsoft.graph.workbookChartAxisFormat"},
  "majorGridlines": {"@odata.type": "microsoft.graph.workbookChartGridlines"},
  "minorGridlines": {"@odata.type": "microsoft.graph.workbookChartGridlines"},
  "title": {"@odata.type": "microsoft.graph.workbookChartAxisTitle"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxis resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->