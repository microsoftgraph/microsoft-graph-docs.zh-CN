# <a name="icon-resource-type"></a><span data-ttu-id="1cfdf-101">图标资源类型</span><span class="sxs-lookup"><span data-stu-id="1cfdf-101">Icon resource type</span></span>

<span data-ttu-id="1cfdf-102">表示单元格图标。</span><span class="sxs-lookup"><span data-stu-id="1cfdf-102">Represents a cell icon.</span></span>


## <a name="methods"></a><span data-ttu-id="1cfdf-103">方法</span><span class="sxs-lookup"><span data-stu-id="1cfdf-103">Methods</span></span>

| <span data-ttu-id="1cfdf-104">方法</span><span class="sxs-lookup"><span data-stu-id="1cfdf-104">Method</span></span>           | <span data-ttu-id="1cfdf-105">返回类型</span><span class="sxs-lookup"><span data-stu-id="1cfdf-105">Return Type</span></span>    |<span data-ttu-id="1cfdf-106">说明</span><span class="sxs-lookup"><span data-stu-id="1cfdf-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1cfdf-107">Get Icon</span><span class="sxs-lookup"><span data-stu-id="1cfdf-107">Get Icon</span></span>](../api/icon_get.md) | [<span data-ttu-id="1cfdf-108">Icon</span><span class="sxs-lookup"><span data-stu-id="1cfdf-108">Icon</span></span>](icon.md) |<span data-ttu-id="1cfdf-109">读取 icon 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1cfdf-109">Read properties and relationships of icon object.</span></span>|
|[<span data-ttu-id="1cfdf-110">Update</span><span class="sxs-lookup"><span data-stu-id="1cfdf-110">Update</span></span>](../api/icon_update.md) | [<span data-ttu-id="1cfdf-111">Icon</span><span class="sxs-lookup"><span data-stu-id="1cfdf-111">Icon</span></span>](icon.md)  |<span data-ttu-id="1cfdf-112">更新 icon 对象。</span><span class="sxs-lookup"><span data-stu-id="1cfdf-112">Update Icon object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1cfdf-113">属性</span><span class="sxs-lookup"><span data-stu-id="1cfdf-113">Properties</span></span>
| <span data-ttu-id="1cfdf-114">属性</span><span class="sxs-lookup"><span data-stu-id="1cfdf-114">Property</span></span>     | <span data-ttu-id="1cfdf-115">类型</span><span class="sxs-lookup"><span data-stu-id="1cfdf-115">Type</span></span>   |<span data-ttu-id="1cfdf-116">说明</span><span class="sxs-lookup"><span data-stu-id="1cfdf-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1cfdf-117">index</span><span class="sxs-lookup"><span data-stu-id="1cfdf-117">index</span></span>|<span data-ttu-id="1cfdf-118">int</span><span class="sxs-lookup"><span data-stu-id="1cfdf-118">int</span></span>|<span data-ttu-id="1cfdf-119">表示给定集合中图标的索引。</span><span class="sxs-lookup"><span data-stu-id="1cfdf-119">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="1cfdf-120">set</span><span class="sxs-lookup"><span data-stu-id="1cfdf-120">set</span></span>|<span data-ttu-id="1cfdf-121">string</span><span class="sxs-lookup"><span data-stu-id="1cfdf-121">string</span></span>|<span data-ttu-id="1cfdf-122">表示图标所属的集合。</span><span class="sxs-lookup"><span data-stu-id="1cfdf-122">Represents the set that the icon is part of. Possible values are: , , , , , , , , , , , , , , , , , , , , .</span></span> <span data-ttu-id="1cfdf-123">可能的值为：`Invalid`、`ThreeArrows`、`ThreeArrowsGray`、`ThreeFlags`、`ThreeTrafficLights1`、`ThreeTrafficLights2`、`ThreeSigns`、`ThreeSymbols`、`ThreeSymbols2`、`FourArrows`、`FourArrowsGray`、`FourRedToBlack`、`FourRating`、`FourTrafficLights`、`FiveArrows`、`FiveArrowsGray`、`FiveRating`、`FiveQuarters`、`ThreeStars`、`ThreeTriangles`、`FiveBoxes`。</span><span class="sxs-lookup"><span data-stu-id="1cfdf-123">The possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1cfdf-124">关系</span><span class="sxs-lookup"><span data-stu-id="1cfdf-124">Relationships</span></span>
<span data-ttu-id="1cfdf-125">无</span><span class="sxs-lookup"><span data-stu-id="1cfdf-125">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1cfdf-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1cfdf-126">JSON representation</span></span>

<span data-ttu-id="1cfdf-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1cfdf-127">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookIcon"
}-->

```json
{
  "index": 1024,
  "set": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Icon resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->