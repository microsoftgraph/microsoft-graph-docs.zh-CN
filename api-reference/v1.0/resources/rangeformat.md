# <a name="rangeformat-resource-type"></a><span data-ttu-id="c0829-101">RangeFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="c0829-101">RangeFormat resource type</span></span>

<span data-ttu-id="c0829-102">一个格式对象，其中封装了区域的字体、填充、边框、对齐方式和其他属性。</span><span class="sxs-lookup"><span data-stu-id="c0829-102">A format object encapsulating the range's font, fill, borders, alignment, and other properties.</span></span>


## <a name="methods"></a><span data-ttu-id="c0829-103">方法</span><span class="sxs-lookup"><span data-stu-id="c0829-103">Methods</span></span>

| <span data-ttu-id="c0829-104">方法</span><span class="sxs-lookup"><span data-stu-id="c0829-104">Method</span></span>           | <span data-ttu-id="c0829-105">返回类型</span><span class="sxs-lookup"><span data-stu-id="c0829-105">Return Type</span></span>    |<span data-ttu-id="c0829-106">说明</span><span class="sxs-lookup"><span data-stu-id="c0829-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c0829-107">获取 RangeFormat</span><span class="sxs-lookup"><span data-stu-id="c0829-107">Get RangeFormat</span></span>](../api/rangeformat_get.md) | [<span data-ttu-id="c0829-108">WorkbookRangeFormat</span><span class="sxs-lookup"><span data-stu-id="c0829-108">WorkbookRangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="c0829-109">读取 rangeFormat 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c0829-109">Read properties and relationships of rangeFormat object.</span></span>|
|[<span data-ttu-id="c0829-110">创建 RangeBorder</span><span class="sxs-lookup"><span data-stu-id="c0829-110">Create RangeBorder</span></span>](../api/rangeformat_post_borders.md) |[<span data-ttu-id="c0829-111">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="c0829-111">WorkbookRangeBorder</span></span>](rangeborder.md)| <span data-ttu-id="c0829-112">通过发布到边框集合创建新的 RangeBorder。</span><span class="sxs-lookup"><span data-stu-id="c0829-112">Create a new RangeBorder by posting to the borders collection.</span></span>|
|[<span data-ttu-id="c0829-113">列举边框</span><span class="sxs-lookup"><span data-stu-id="c0829-113">List borders</span></span>](../api/rangeformat_list_borders.md) |<span data-ttu-id="c0829-114">[WorkbookRangeBorder](rangeborder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c0829-114">[WorkbookRangeBorder](rangeborder.md) collection</span></span>| <span data-ttu-id="c0829-115">获取 RangeBorder 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c0829-115">Get a RangeBorder object collection.</span></span>|
|[<span data-ttu-id="c0829-116">更新</span><span class="sxs-lookup"><span data-stu-id="c0829-116">Update</span></span>](../api/rangeformat_update.md) | [<span data-ttu-id="c0829-117">WorkbookRangeFormat</span><span class="sxs-lookup"><span data-stu-id="c0829-117">WorkbookRangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="c0829-118">更新 RangeFormat 对象。</span><span class="sxs-lookup"><span data-stu-id="c0829-118">Update RangeFormat object.</span></span> |
|[<span data-ttu-id="c0829-119">Autofitcolumns</span><span class="sxs-lookup"><span data-stu-id="c0829-119">Autofitcolumns</span></span>](../api/rangeformat_autofitcolumns.md)|<span data-ttu-id="c0829-120">无</span><span class="sxs-lookup"><span data-stu-id="c0829-120">None</span></span>|<span data-ttu-id="c0829-121">根据列中的当前数据更改当前区域的列宽，以达到最佳宽度。</span><span class="sxs-lookup"><span data-stu-id="c0829-121">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>|
|[<span data-ttu-id="c0829-122">Autofitrows</span><span class="sxs-lookup"><span data-stu-id="c0829-122">Autofitrows</span></span>](../api/rangeformat_autofitrows.md)|<span data-ttu-id="c0829-123">无</span><span class="sxs-lookup"><span data-stu-id="c0829-123">None</span></span>|<span data-ttu-id="c0829-124">根据列中的当前数据更改当前区域的行高，以达到最佳高度。</span><span class="sxs-lookup"><span data-stu-id="c0829-124">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>|

## <a name="properties"></a><span data-ttu-id="c0829-125">属性</span><span class="sxs-lookup"><span data-stu-id="c0829-125">Properties</span></span>
| <span data-ttu-id="c0829-126">属性</span><span class="sxs-lookup"><span data-stu-id="c0829-126">Property</span></span>     | <span data-ttu-id="c0829-127">类型</span><span class="sxs-lookup"><span data-stu-id="c0829-127">Type</span></span>   |<span data-ttu-id="c0829-128">说明</span><span class="sxs-lookup"><span data-stu-id="c0829-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0829-129">columnWidth</span><span class="sxs-lookup"><span data-stu-id="c0829-129">columnWidth</span></span>|<span data-ttu-id="c0829-130">翻倍</span><span class="sxs-lookup"><span data-stu-id="c0829-130">double</span></span>|<span data-ttu-id="c0829-p101">获取或设置区域内的所有列的宽度。如果列宽不统一，则返回 NULL。</span><span class="sxs-lookup"><span data-stu-id="c0829-p101">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="c0829-133">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="c0829-133">horizontalAlignment</span></span>|<span data-ttu-id="c0829-134">字符串</span><span class="sxs-lookup"><span data-stu-id="c0829-134">string</span></span>|<span data-ttu-id="c0829-135">代表指定对象的水平对齐方式。</span><span class="sxs-lookup"><span data-stu-id="c0829-135">Returns or sets the horizontal alignment for the specified object.</span></span> <span data-ttu-id="c0829-136">可取值为：`General`、`Left`、`Center`、`Right`、`Fill`、`Justify`、`CenterAcrossSelection`、`Distributed`。</span><span class="sxs-lookup"><span data-stu-id="c0829-136">The possible values are `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`, , , , or .</span></span>|
|<span data-ttu-id="c0829-137">rowHeight</span><span class="sxs-lookup"><span data-stu-id="c0829-137">rowHeight</span></span>|<span data-ttu-id="c0829-138">翻倍</span><span class="sxs-lookup"><span data-stu-id="c0829-138">double</span></span>|<span data-ttu-id="c0829-p103">获取或设置区域中所有行的高度。如果行高不统一，则返回 NULL。</span><span class="sxs-lookup"><span data-stu-id="c0829-p103">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="c0829-141">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="c0829-141">verticalAlignment</span></span>|<span data-ttu-id="c0829-142">字符串</span><span class="sxs-lookup"><span data-stu-id="c0829-142">string</span></span>|<span data-ttu-id="c0829-143">代表指定对象的垂直对齐方式。</span><span class="sxs-lookup"><span data-stu-id="c0829-143">Represents the vertical alignment for the specified object. Possible values are: , , , , .</span></span> <span data-ttu-id="c0829-144">可取值为：`Top`、`Center`、`Bottom`、`Justify`、`Distributed`。</span><span class="sxs-lookup"><span data-stu-id="c0829-144">The possible values are `Top`, `Center`, `Bottom`, `Justify`, `Distributed`, , , , , , , or .</span></span>|
|<span data-ttu-id="c0829-145">wrapText</span><span class="sxs-lookup"><span data-stu-id="c0829-145">wrapText</span></span>|<span data-ttu-id="c0829-146">布尔值</span><span class="sxs-lookup"><span data-stu-id="c0829-146">boolean</span></span>|<span data-ttu-id="c0829-p105">指示 Excel 是否将对象中的文本换行。指示整个区域不具有统一换行设置的空值</span><span class="sxs-lookup"><span data-stu-id="c0829-p105">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0829-149">关系</span><span class="sxs-lookup"><span data-stu-id="c0829-149">Relationships</span></span>
| <span data-ttu-id="c0829-150">关系</span><span class="sxs-lookup"><span data-stu-id="c0829-150">Relationship</span></span> | <span data-ttu-id="c0829-151">类型</span><span class="sxs-lookup"><span data-stu-id="c0829-151">Type</span></span>   |<span data-ttu-id="c0829-152">说明</span><span class="sxs-lookup"><span data-stu-id="c0829-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0829-153">边框</span><span class="sxs-lookup"><span data-stu-id="c0829-153">borders</span></span>|<span data-ttu-id="c0829-154">[WorkbookRangeBorder](rangeborder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c0829-154">[WorkbookRangeBorder](rangeborder.md) collection</span></span>|<span data-ttu-id="c0829-155">应用于所选整个区域的边框的对象集合。只读。</span><span class="sxs-lookup"><span data-stu-id="c0829-155">Collection of border objects that apply to the overall range selected Read-only.</span></span>|
|<span data-ttu-id="c0829-156">填充</span><span class="sxs-lookup"><span data-stu-id="c0829-156">fill</span></span>|[<span data-ttu-id="c0829-157">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="c0829-157">WorkbookRangeFill</span></span>](rangefill.md)|<span data-ttu-id="c0829-p106">返回整个区域内定义的填充对象。只读。</span><span class="sxs-lookup"><span data-stu-id="c0829-p106">Returns the fill object defined on the overall range. Read-only.</span></span>|
|<span data-ttu-id="c0829-160">字体</span><span class="sxs-lookup"><span data-stu-id="c0829-160">font</span></span>|[<span data-ttu-id="c0829-161">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="c0829-161">WorkbookRangeFont</span></span>](rangefont.md)|<span data-ttu-id="c0829-162">返回所选整个区域内定义的字体对象。只读。</span><span class="sxs-lookup"><span data-stu-id="c0829-162">Returns the font object defined on the overall range selected Read-only.</span></span>|
|<span data-ttu-id="c0829-163">保护</span><span class="sxs-lookup"><span data-stu-id="c0829-163">protection</span></span>|[<span data-ttu-id="c0829-164">WorkbookFormatProtection</span><span class="sxs-lookup"><span data-stu-id="c0829-164">WorkbookFormatProtection</span></span>](formatprotection.md)|<span data-ttu-id="c0829-p107">返回区域的格式保护对象。只读。</span><span class="sxs-lookup"><span data-stu-id="c0829-p107">Returns the format protection object for a range. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c0829-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c0829-167">JSON representation</span></span>

<span data-ttu-id="c0829-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c0829-168">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookRangeFormat"
}-->

```json
{
  "columnWidth": 1024,
  "horizontalAlignment": "string",
  "rowHeight": 1024,
  "verticalAlignment": "string",
  "wrapText": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->