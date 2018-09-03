# <a name="rangeborder-resource-type"></a><span data-ttu-id="7c7b8-101">RangeBorder 资源类型</span><span class="sxs-lookup"><span data-stu-id="7c7b8-101">RangeBorder resource type</span></span>

<span data-ttu-id="7c7b8-102">表示对象的边框。</span><span class="sxs-lookup"><span data-stu-id="7c7b8-102">Represents the border of an object.</span></span>


## <a name="methods"></a><span data-ttu-id="7c7b8-103">方法</span><span class="sxs-lookup"><span data-stu-id="7c7b8-103">Methods</span></span>

| <span data-ttu-id="7c7b8-104">方法</span><span class="sxs-lookup"><span data-stu-id="7c7b8-104">Method</span></span>           | <span data-ttu-id="7c7b8-105">返回类型</span><span class="sxs-lookup"><span data-stu-id="7c7b8-105">Return Type</span></span>    |<span data-ttu-id="7c7b8-106">说明</span><span class="sxs-lookup"><span data-stu-id="7c7b8-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7c7b8-107">获取 RangeBorder</span><span class="sxs-lookup"><span data-stu-id="7c7b8-107">Get RangeBorder</span></span>](../api/rangeborder_get.md) | [<span data-ttu-id="7c7b8-108">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="7c7b8-108">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="7c7b8-109">读取 rangeborder 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7c7b8-109">Read properties and relationships of rangeBorder object.</span></span>|
|[<span data-ttu-id="7c7b8-110">更新</span><span class="sxs-lookup"><span data-stu-id="7c7b8-110">Update</span></span>](../api/rangeborder_update.md) | [<span data-ttu-id="7c7b8-111">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="7c7b8-111">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="7c7b8-112">更新 RangeBorder 对象。</span><span class="sxs-lookup"><span data-stu-id="7c7b8-112">Update RangeBorder object.</span></span> |
|[<span data-ttu-id="7c7b8-113">列表</span><span class="sxs-lookup"><span data-stu-id="7c7b8-113">List</span></span>](../api/rangeborder_list.md) | <span data-ttu-id="7c7b8-114">[WorkbookRangeBorder](rangeborder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7c7b8-114">[WorkbookRangeBorder](rangeborder.md) collection</span></span> |<span data-ttu-id="7c7b8-115">获取 rangeBorder 对象集合。</span><span class="sxs-lookup"><span data-stu-id="7c7b8-115">Get rangeBorder object collection.</span></span> |
|[<span data-ttu-id="7c7b8-116">Itemat</span><span class="sxs-lookup"><span data-stu-id="7c7b8-116">Itemat</span></span>](../api/rangebordercollection_itemat.md)|[<span data-ttu-id="7c7b8-117">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="7c7b8-117">WorkbookRangeBorder</span></span>](rangeborder.md)|<span data-ttu-id="7c7b8-118">使用其索引获取 border 对象</span><span class="sxs-lookup"><span data-stu-id="7c7b8-118">Gets a border object using its index</span></span>|

## <a name="properties"></a><span data-ttu-id="7c7b8-119">属性</span><span class="sxs-lookup"><span data-stu-id="7c7b8-119">Properties</span></span>
| <span data-ttu-id="7c7b8-120">属性</span><span class="sxs-lookup"><span data-stu-id="7c7b8-120">Property</span></span>     | <span data-ttu-id="7c7b8-121">类型</span><span class="sxs-lookup"><span data-stu-id="7c7b8-121">Type</span></span>   |<span data-ttu-id="7c7b8-122">说明</span><span class="sxs-lookup"><span data-stu-id="7c7b8-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c7b8-123">color</span><span class="sxs-lookup"><span data-stu-id="7c7b8-123">color</span></span>|<span data-ttu-id="7c7b8-124">string</span><span class="sxs-lookup"><span data-stu-id="7c7b8-124">string</span></span>|<span data-ttu-id="7c7b8-125">表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="7c7b8-125">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="7c7b8-126">id</span><span class="sxs-lookup"><span data-stu-id="7c7b8-126">id</span></span>|<span data-ttu-id="7c7b8-127">string</span><span class="sxs-lookup"><span data-stu-id="7c7b8-127">string</span></span>|<span data-ttu-id="7c7b8-128">代表边框标识符。</span><span class="sxs-lookup"><span data-stu-id="7c7b8-128">Represents border identifier. Possible values are: , , , , , , , . Read-only.</span></span> <span data-ttu-id="7c7b8-129">可取值为：`EdgeTop`、`EdgeBottom`、`EdgeLeft`、`EdgeRight`、`InsideVertical`、`InsideHorizontal`、`DiagonalDown`、`DiagonalUp`。</span><span class="sxs-lookup"><span data-stu-id="7c7b8-129">The possible values are `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`, , , , or .</span></span> <span data-ttu-id="7c7b8-130">只读。</span><span class="sxs-lookup"><span data-stu-id="7c7b8-130">Read-only.</span></span>|
|<span data-ttu-id="7c7b8-131">sideIndex</span><span class="sxs-lookup"><span data-stu-id="7c7b8-131">sideIndex</span></span>|<span data-ttu-id="7c7b8-132">string</span><span class="sxs-lookup"><span data-stu-id="7c7b8-132">string</span></span>|<span data-ttu-id="7c7b8-133">指示边框的特定边的常数值。</span><span class="sxs-lookup"><span data-stu-id="7c7b8-133">Constant value that indicates the specific side of the border. Possible values are: , , , , , , , . Read-only.</span></span> <span data-ttu-id="7c7b8-134">可取值为：`EdgeTop`、`EdgeBottom`、`EdgeLeft`、`EdgeRight`、`InsideVertical`、`InsideHorizontal`、`DiagonalDown`、`DiagonalUp`。</span><span class="sxs-lookup"><span data-stu-id="7c7b8-134">The possible values are `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`, , , , or .</span></span> <span data-ttu-id="7c7b8-135">只读。</span><span class="sxs-lookup"><span data-stu-id="7c7b8-135">Read-only.</span></span>|
|<span data-ttu-id="7c7b8-136">style</span><span class="sxs-lookup"><span data-stu-id="7c7b8-136">style</span></span>|<span data-ttu-id="7c7b8-137">string</span><span class="sxs-lookup"><span data-stu-id="7c7b8-137">string</span></span>|<span data-ttu-id="7c7b8-138">指定边框线型的线型常量之一。</span><span class="sxs-lookup"><span data-stu-id="7c7b8-138">One of the constants of line style specifying the line style for the border. Possible values are: , , , , , , , .</span></span> <span data-ttu-id="7c7b8-139">可取值为：`None`、`Continuous`、`Dash`、`DashDot`、`DashDotDot`、`Dot`、`Double`、`SlantDashDot`。</span><span class="sxs-lookup"><span data-stu-id="7c7b8-139">The possible values are `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`, , , , or .</span></span>|
|<span data-ttu-id="7c7b8-140">weight</span><span class="sxs-lookup"><span data-stu-id="7c7b8-140">weight</span></span>|<span data-ttu-id="7c7b8-141">string</span><span class="sxs-lookup"><span data-stu-id="7c7b8-141">string</span></span>|<span data-ttu-id="7c7b8-142">指定某一区域周围的边框的粗细。</span><span class="sxs-lookup"><span data-stu-id="7c7b8-142">Specifies the weight of the border around a range.</span></span> <span data-ttu-id="7c7b8-143">可取值为：`Hairline`、`Thin`、`Medium`、`Thick`。</span><span class="sxs-lookup"><span data-stu-id="7c7b8-143">The possible values are `Hairline`, `Thin`, `Medium`, `Thick`, , , , , , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="7c7b8-144">关系</span><span class="sxs-lookup"><span data-stu-id="7c7b8-144">Relationships</span></span>
<span data-ttu-id="7c7b8-145">无</span><span class="sxs-lookup"><span data-stu-id="7c7b8-145">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="7c7b8-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7c7b8-146">JSON representation</span></span>

<span data-ttu-id="7c7b8-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7c7b8-147">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeBorder"
}-->

```json
{
  "color": "string",
  "id": "string",
  "sideIndex": "string",
  "style": "string",
  "weight": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->