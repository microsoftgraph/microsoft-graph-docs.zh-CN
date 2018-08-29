# <a name="rangefill-resource-type"></a><span data-ttu-id="c22db-101">RangeFill 资源类型</span><span class="sxs-lookup"><span data-stu-id="c22db-101">RangeFill resource type</span></span>

<span data-ttu-id="c22db-102">表示 range 对象的背景。</span><span class="sxs-lookup"><span data-stu-id="c22db-102">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="c22db-103">方法</span><span class="sxs-lookup"><span data-stu-id="c22db-103">Methods</span></span>

| <span data-ttu-id="c22db-104">方法</span><span class="sxs-lookup"><span data-stu-id="c22db-104">Method</span></span>           | <span data-ttu-id="c22db-105">返回类型</span><span class="sxs-lookup"><span data-stu-id="c22db-105">Return Type</span></span>    |<span data-ttu-id="c22db-106">说明</span><span class="sxs-lookup"><span data-stu-id="c22db-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c22db-107">获取 RangeFill</span><span class="sxs-lookup"><span data-stu-id="c22db-107">Get RangeFill</span></span>](../api/rangefill_get.md) | [<span data-ttu-id="c22db-108">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="c22db-108">WorkbookRangeFill</span></span>](rangefill.md) |<span data-ttu-id="c22db-109">读取 rangeFill 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c22db-109">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="c22db-110">Update</span><span class="sxs-lookup"><span data-stu-id="c22db-110">Update</span></span>](../api/rangefill_update.md) | [<span data-ttu-id="c22db-111">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="c22db-111">WorkbookRangeFill</span></span>](rangefill.md)   |<span data-ttu-id="c22db-112">更新 RangeFill 对象。</span><span class="sxs-lookup"><span data-stu-id="c22db-112">Update RangeFill object.</span></span> |
|[<span data-ttu-id="c22db-113">清除</span><span class="sxs-lookup"><span data-stu-id="c22db-113">Clear</span></span>](../api/rangefill_clear.md)|<span data-ttu-id="c22db-114">无</span><span class="sxs-lookup"><span data-stu-id="c22db-114">None</span></span>|<span data-ttu-id="c22db-115">重置区域背景。</span><span class="sxs-lookup"><span data-stu-id="c22db-115">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="c22db-116">属性</span><span class="sxs-lookup"><span data-stu-id="c22db-116">Properties</span></span>
| <span data-ttu-id="c22db-117">属性</span><span class="sxs-lookup"><span data-stu-id="c22db-117">Property</span></span>     | <span data-ttu-id="c22db-118">类型</span><span class="sxs-lookup"><span data-stu-id="c22db-118">Type</span></span>   |<span data-ttu-id="c22db-119">说明</span><span class="sxs-lookup"><span data-stu-id="c22db-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c22db-120">颜色</span><span class="sxs-lookup"><span data-stu-id="c22db-120">color</span></span>|<span data-ttu-id="c22db-121">字符串</span><span class="sxs-lookup"><span data-stu-id="c22db-121">string</span></span>|<span data-ttu-id="c22db-122">表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="c22db-122">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="c22db-123">关系</span><span class="sxs-lookup"><span data-stu-id="c22db-123">Relationships</span></span>
<span data-ttu-id="c22db-124">无</span><span class="sxs-lookup"><span data-stu-id="c22db-124">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c22db-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c22db-125">JSON representation</span></span>

<span data-ttu-id="c22db-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c22db-126">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeFill"
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
  "description": "RangeFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->