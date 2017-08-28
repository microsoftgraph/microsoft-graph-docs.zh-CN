# <a name="rangeview-resource-type"></a><span data-ttu-id="a1e1d-101">rangeView 资源类型</span><span class="sxs-lookup"><span data-stu-id="a1e1d-101">rangeView resource type</span></span>
<span data-ttu-id="a1e1d-102">RangeView 表示父范围的一组可见单元格。</span><span class="sxs-lookup"><span data-stu-id="a1e1d-102">RangeView represents a set of visible cells of the parent range.</span></span>

## <a name="methods"></a><span data-ttu-id="a1e1d-103">方法</span><span class="sxs-lookup"><span data-stu-id="a1e1d-103">Methods</span></span>

| <span data-ttu-id="a1e1d-104">方法</span><span class="sxs-lookup"><span data-stu-id="a1e1d-104">Method</span></span>           | <span data-ttu-id="a1e1d-105">返回类型</span><span class="sxs-lookup"><span data-stu-id="a1e1d-105">Return Type</span></span>    |<span data-ttu-id="a1e1d-106">说明</span><span class="sxs-lookup"><span data-stu-id="a1e1d-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a1e1d-107">List rows</span><span class="sxs-lookup"><span data-stu-id="a1e1d-107">List rows</span></span>](../api/workbookrangeview_list_rows.md) |<span data-ttu-id="a1e1d-108">[workbookRangeView](workbookrangeview.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a1e1d-108">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="a1e1d-109">获取一组 workbookRangeView 对象。</span><span class="sxs-lookup"><span data-stu-id="a1e1d-109">Get a workbookRangeView object collection.</span></span>|
|[<span data-ttu-id="a1e1d-110">Itemat</span><span class="sxs-lookup"><span data-stu-id="a1e1d-110">Itemat</span></span>](../api/workbookrangeview_itemat.md)|[<span data-ttu-id="a1e1d-111">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="a1e1d-111">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="a1e1d-112">按索引获取范围视图项。</span><span class="sxs-lookup"><span data-stu-id="a1e1d-112">Get a range view item based in index.</span></span>|
|[<span data-ttu-id="a1e1d-113">Range</span><span class="sxs-lookup"><span data-stu-id="a1e1d-113">Range</span></span>](../api/workbookrangeview_range.md)|[<span data-ttu-id="a1e1d-114">workbookRange</span><span class="sxs-lookup"><span data-stu-id="a1e1d-114">workbookRange</span></span>](range.md)|<span data-ttu-id="a1e1d-115">返回与范围视图相关联的范围对象</span><span class="sxs-lookup"><span data-stu-id="a1e1d-115">Return the range object associated with the range view</span></span>|

## <a name="properties"></a><span data-ttu-id="a1e1d-116">属性</span><span class="sxs-lookup"><span data-stu-id="a1e1d-116">Properties</span></span>
| <span data-ttu-id="a1e1d-117">属性</span><span class="sxs-lookup"><span data-stu-id="a1e1d-117">Property</span></span>     | <span data-ttu-id="a1e1d-118">类型</span><span class="sxs-lookup"><span data-stu-id="a1e1d-118">Type</span></span>   |<span data-ttu-id="a1e1d-119">说明</span><span class="sxs-lookup"><span data-stu-id="a1e1d-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1e1d-120">columnCount</span><span class="sxs-lookup"><span data-stu-id="a1e1d-120">columnCount</span></span>|<span data-ttu-id="a1e1d-121">Int32</span><span class="sxs-lookup"><span data-stu-id="a1e1d-121">Int32</span></span>|<span data-ttu-id="a1e1d-p101">返回可见列数。只读。</span><span class="sxs-lookup"><span data-stu-id="a1e1d-p101">Returns the number of visible columns. Read-only.</span></span>|
|<span data-ttu-id="a1e1d-124">formulas</span><span class="sxs-lookup"><span data-stu-id="a1e1d-124">formulas</span></span>|<span data-ttu-id="a1e1d-125">Json</span><span class="sxs-lookup"><span data-stu-id="a1e1d-125">Json</span></span>|<span data-ttu-id="a1e1d-126">表示采用 A1 表示法的公式。</span><span class="sxs-lookup"><span data-stu-id="a1e1d-126">Represents the formula in A1-style notation.</span></span> |
|<span data-ttu-id="a1e1d-127">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="a1e1d-127">formulasLocal</span></span>|<span data-ttu-id="a1e1d-128">Json</span><span class="sxs-lookup"><span data-stu-id="a1e1d-128">Json</span></span>|<span data-ttu-id="a1e1d-p102">表示采用 A1 表示法的公式，使用用户语言和数字格式区域设置。例如，英语中的公式 "=SUM(A1, 1.5)" 在德语中变为 "=SUMME(A1; 1,5)"。</span><span class="sxs-lookup"><span data-stu-id="a1e1d-p102">Represents the formula in A1-style notation, in the user's language and number-formatting locale. For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>    |
|<span data-ttu-id="a1e1d-131">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="a1e1d-131">formulasR1C1</span></span>|<span data-ttu-id="a1e1d-132">Json</span><span class="sxs-lookup"><span data-stu-id="a1e1d-132">Json</span></span>|<span data-ttu-id="a1e1d-133">表示采用 R1C1 表示法的公式。</span><span class="sxs-lookup"><span data-stu-id="a1e1d-133">Represents the formula in R1C1-style notation.</span></span>   |
|<span data-ttu-id="a1e1d-134">index</span><span class="sxs-lookup"><span data-stu-id="a1e1d-134">index</span></span>|<span data-ttu-id="a1e1d-135">Int32</span><span class="sxs-lookup"><span data-stu-id="a1e1d-135">Int32</span></span>|<span data-ttu-id="a1e1d-136">范围的索引。</span><span class="sxs-lookup"><span data-stu-id="a1e1d-136">Index of the range.</span></span>|
|<span data-ttu-id="a1e1d-137">numberFormat</span><span class="sxs-lookup"><span data-stu-id="a1e1d-137">numberFormat</span></span>|<span data-ttu-id="a1e1d-138">Json</span><span class="sxs-lookup"><span data-stu-id="a1e1d-138">Json</span></span>|<span data-ttu-id="a1e1d-p103">表示 Excel 中指定单元格的数字格式代码。只读。</span><span class="sxs-lookup"><span data-stu-id="a1e1d-p103">Represents Excel's number format code for the given cell. Read-only.</span></span> |
|<span data-ttu-id="a1e1d-141">rowCount</span><span class="sxs-lookup"><span data-stu-id="a1e1d-141">rowCount</span></span>|<span data-ttu-id="a1e1d-142">Int32</span><span class="sxs-lookup"><span data-stu-id="a1e1d-142">Int32</span></span>|<span data-ttu-id="a1e1d-p104">返回可见行数。只读。</span><span class="sxs-lookup"><span data-stu-id="a1e1d-p104">Returns the number of visible rows. Read-only.</span></span>  |
|<span data-ttu-id="a1e1d-145">text</span><span class="sxs-lookup"><span data-stu-id="a1e1d-145">text</span></span>|<span data-ttu-id="a1e1d-146">Json</span><span class="sxs-lookup"><span data-stu-id="a1e1d-146">Json</span></span>|<span data-ttu-id="a1e1d-p105">指定区域的文本值。文本值与单元格宽度无关。在 Excel UI 中替代 # 符号不会影响 API 返回的文本值。只读。</span><span class="sxs-lookup"><span data-stu-id="a1e1d-p105">Text values of the specified range. The Text value will not depend on the cell width. The # sign substitution that happens in Excel UI will not affect the text value returned by the API. Read-only.</span></span>    |
|<span data-ttu-id="a1e1d-151">valueTypes</span><span class="sxs-lookup"><span data-stu-id="a1e1d-151">valueTypes</span></span>|<span data-ttu-id="a1e1d-152">Json</span><span class="sxs-lookup"><span data-stu-id="a1e1d-152">Json</span></span>|<span data-ttu-id="a1e1d-p106">表示每个单元格的数据类型。只读。可能的值是：Unknown、Empty、String、Integer、Double、Boolean、Error。</span><span class="sxs-lookup"><span data-stu-id="a1e1d-p106">Represents the type of data of each cell. Read-only. Possible values are: Unknown, Empty, String, Integer, Double, Boolean, Error.</span></span> |
|<span data-ttu-id="a1e1d-156">values</span><span class="sxs-lookup"><span data-stu-id="a1e1d-156">values</span></span>|<span data-ttu-id="a1e1d-157">Json</span><span class="sxs-lookup"><span data-stu-id="a1e1d-157">Json</span></span>|<span data-ttu-id="a1e1d-p107">表示指定的 RangeView 的原始值。返回的数据可能是字符串、数字，也可能是布尔值。包含错误的单元格将返回错误字符串。</span><span class="sxs-lookup"><span data-stu-id="a1e1d-p107">Represents the raw values of the specified range view. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="a1e1d-161">关系</span><span class="sxs-lookup"><span data-stu-id="a1e1d-161">Relationships</span></span>
| <span data-ttu-id="a1e1d-162">关系</span><span class="sxs-lookup"><span data-stu-id="a1e1d-162">Relationship</span></span> | <span data-ttu-id="a1e1d-163">类型</span><span class="sxs-lookup"><span data-stu-id="a1e1d-163">Type</span></span>   |<span data-ttu-id="a1e1d-164">说明</span><span class="sxs-lookup"><span data-stu-id="a1e1d-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1e1d-165">rows</span><span class="sxs-lookup"><span data-stu-id="a1e1d-165">rows</span></span>|<span data-ttu-id="a1e1d-166">[workbookRangeView](workbookrangeview.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a1e1d-166">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="a1e1d-p108">表示一组与范围相关联的范围视图。只读。  只读。</span><span class="sxs-lookup"><span data-stu-id="a1e1d-p108">Represents a collection of range views associated with the range. Read-only.    Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a1e1d-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a1e1d-170">JSON representation</span></span>
<span data-ttu-id="a1e1d-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1e1d-171">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.workbookRangeView"
}-->
```json
{
  "cellAddresses": "Json",
  "columnCount": 1024,
  "formulas": "Json",
  "formulasLocal": "Json",
  "formulasR1C1": "Json",
  "id": "String (identifier)",
  "index": 1024,
  "numberFormat": "Json",
  "rowCount": 1024,
  "text": "Json",
  "valueTypes": "Json",
  "values": "Json"
}
```
