# <a name="sortfield-resource-type"></a><span data-ttu-id="88631-101">SortField 资源类型</span><span class="sxs-lookup"><span data-stu-id="88631-101">SortField resource type</span></span>

<span data-ttu-id="88631-102">表示排序操作中的条件。</span><span class="sxs-lookup"><span data-stu-id="88631-102">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="88631-103">属性</span><span class="sxs-lookup"><span data-stu-id="88631-103">Properties</span></span>
| <span data-ttu-id="88631-104">属性</span><span class="sxs-lookup"><span data-stu-id="88631-104">Property</span></span>     | <span data-ttu-id="88631-105">类型</span><span class="sxs-lookup"><span data-stu-id="88631-105">Type</span></span>   |<span data-ttu-id="88631-106">说明</span><span class="sxs-lookup"><span data-stu-id="88631-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88631-107">ascending</span><span class="sxs-lookup"><span data-stu-id="88631-107">ascending</span></span>|<span data-ttu-id="88631-108">布尔值</span><span class="sxs-lookup"><span data-stu-id="88631-108">boolean</span></span>|<span data-ttu-id="88631-109">表示是否以升序方式进行排序。</span><span class="sxs-lookup"><span data-stu-id="88631-109">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="88631-110">color</span><span class="sxs-lookup"><span data-stu-id="88631-110">color</span></span>|<span data-ttu-id="88631-111">string</span><span class="sxs-lookup"><span data-stu-id="88631-111">string</span></span>|<span data-ttu-id="88631-112">表示按字体或单元格颜色进行排序时，条件的目标颜色。</span><span class="sxs-lookup"><span data-stu-id="88631-112">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="88631-113">dataOption</span><span class="sxs-lookup"><span data-stu-id="88631-113">dataOption</span></span>|<span data-ttu-id="88631-114">string</span><span class="sxs-lookup"><span data-stu-id="88631-114">string</span></span>|<span data-ttu-id="88631-115">代表用于此字段的其他排序选项。</span><span class="sxs-lookup"><span data-stu-id="88631-115">Represents additional sorting options for this field. Possible values are: , .</span></span> <span data-ttu-id="88631-116">可取值为：`Normal`、`TextAsNumber`。</span><span class="sxs-lookup"><span data-stu-id="88631-116">The possible values are:</span></span>|
|<span data-ttu-id="88631-117">Key</span><span class="sxs-lookup"><span data-stu-id="88631-117">key</span></span>|<span data-ttu-id="88631-118">int</span><span class="sxs-lookup"><span data-stu-id="88631-118">int</span></span>|<span data-ttu-id="88631-p102">表示条件所在的列（或行，具体取决于排序方向）。表示与第一列（或行）的偏移量。</span><span class="sxs-lookup"><span data-stu-id="88631-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="88631-121">sortOn</span><span class="sxs-lookup"><span data-stu-id="88631-121">sortOn</span></span>|<span data-ttu-id="88631-122">string</span><span class="sxs-lookup"><span data-stu-id="88631-122">string</span></span>|<span data-ttu-id="88631-123">表示此条件的排序类型。</span><span class="sxs-lookup"><span data-stu-id="88631-123">Represents the type of sorting of this condition. Possible values are: , , , .</span></span> <span data-ttu-id="88631-124">可取值为：`Value`、`CellColor`、`FontColor`、`Icon`。</span><span class="sxs-lookup"><span data-stu-id="88631-124">The possible values are `Value`, `CellColor`, `FontColor`, `Icon`, , , , , , , , or .</span></span>|
|<span data-ttu-id="88631-125">icon</span><span class="sxs-lookup"><span data-stu-id="88631-125">icon</span></span>|[<span data-ttu-id="88631-126">WorkbookIcon</span><span class="sxs-lookup"><span data-stu-id="88631-126">WorkbookIcon</span></span>](icon.md)|<span data-ttu-id="88631-127">表示对单元格图标进行排序时，条件的目标图标。</span><span class="sxs-lookup"><span data-stu-id="88631-127">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="88631-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="88631-128">JSON representation</span></span>

<span data-ttu-id="88631-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88631-129">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookSortField"
}-->

```json
{
  "ascending": true,
  "color": "string",
  "dataOption": "string",
  "key": 1024,
  "sortOn": "string",
  "icon": { "@odata.type": "microsoft.graph.workbookIcon" }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "SortField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->