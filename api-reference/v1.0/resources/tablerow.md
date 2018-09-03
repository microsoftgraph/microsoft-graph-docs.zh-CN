# <a name="tablerow-resource-type"></a><span data-ttu-id="81099-101">TableRow 资源类型</span><span class="sxs-lookup"><span data-stu-id="81099-101">TableRow resource type</span></span>

<span data-ttu-id="81099-102">表示表中的行。</span><span class="sxs-lookup"><span data-stu-id="81099-102">Represents a row in a table.</span></span>


## <a name="methods"></a><span data-ttu-id="81099-103">方法</span><span class="sxs-lookup"><span data-stu-id="81099-103">Methods</span></span>

| <span data-ttu-id="81099-104">方法</span><span class="sxs-lookup"><span data-stu-id="81099-104">Method</span></span>           | <span data-ttu-id="81099-105">返回类型</span><span class="sxs-lookup"><span data-stu-id="81099-105">Return Type</span></span>    |<span data-ttu-id="81099-106">说明</span><span class="sxs-lookup"><span data-stu-id="81099-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="81099-107">获取 TableRow</span><span class="sxs-lookup"><span data-stu-id="81099-107">Get TableRow</span></span>](../api/tablerow_get.md) | [<span data-ttu-id="81099-108">WorkbookTableRow</span><span class="sxs-lookup"><span data-stu-id="81099-108">WorkbookTableRow</span></span>](tablerow.md) |<span data-ttu-id="81099-109">读取 tableRow 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="81099-109">Read properties and relationships of tableRow object.</span></span>|
|[<span data-ttu-id="81099-110">更新</span><span class="sxs-lookup"><span data-stu-id="81099-110">Update</span></span>](../api/tablerow_update.md) | [<span data-ttu-id="81099-111">WorkbookTableRow</span><span class="sxs-lookup"><span data-stu-id="81099-111">WorkbookTableRow</span></span>](tablerow.md)  |<span data-ttu-id="81099-112">更新 TableRow 对象。</span><span class="sxs-lookup"><span data-stu-id="81099-112">Update TableRow object.</span></span> |
|[<span data-ttu-id="81099-113">区域</span><span class="sxs-lookup"><span data-stu-id="81099-113">Range</span></span>](../api/tablerow_range.md)|[<span data-ttu-id="81099-114">区域</span><span class="sxs-lookup"><span data-stu-id="81099-114">Range</span></span>](range.md)|<span data-ttu-id="81099-115">返回与整行相关联的范围对象。</span><span class="sxs-lookup"><span data-stu-id="81099-115">Returns the range object associated with the entire row.</span></span>|
|[<span data-ttu-id="81099-116">删除</span><span class="sxs-lookup"><span data-stu-id="81099-116">Delete</span></span>](../api/tablerow_delete.md)|<span data-ttu-id="81099-117">无</span><span class="sxs-lookup"><span data-stu-id="81099-117">None</span></span>|<span data-ttu-id="81099-118">从表中删除行。</span><span class="sxs-lookup"><span data-stu-id="81099-118">Deletes the row from the table.</span></span>|
|[<span data-ttu-id="81099-119">列表</span><span class="sxs-lookup"><span data-stu-id="81099-119">List</span></span>](../api/tablerow_list.md) | <span data-ttu-id="81099-120">[WorkbookTableRow](tablerow.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81099-120">[WorkbookTableRow](tablerow.md) collection</span></span> |<span data-ttu-id="81099-121">获取 tableRow 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="81099-121">Get tableRow object collection.</span></span> |
|[<span data-ttu-id="81099-122">Itemat</span><span class="sxs-lookup"><span data-stu-id="81099-122">Itemat</span></span>](../api/tablerowcollection_itemat.md)|[<span data-ttu-id="81099-123">WorkbookTableRow</span><span class="sxs-lookup"><span data-stu-id="81099-123">WorkbookTableRow</span></span>](tablerow.md)|<span data-ttu-id="81099-124">根据其在集合中的位置获取行。</span><span class="sxs-lookup"><span data-stu-id="81099-124">Gets a row based on its position in the collection.</span></span>|
|[<span data-ttu-id="81099-125">添加</span><span class="sxs-lookup"><span data-stu-id="81099-125">Add</span></span>](../api/tablerowcollection_add.md)|[<span data-ttu-id="81099-126">WorkbookTableRow</span><span class="sxs-lookup"><span data-stu-id="81099-126">WorkbookTableRow</span></span>](tablerow.md)|<span data-ttu-id="81099-127">向表中添加新行。</span><span class="sxs-lookup"><span data-stu-id="81099-127">Adds a new row to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="81099-128">属性</span><span class="sxs-lookup"><span data-stu-id="81099-128">Properties</span></span>
| <span data-ttu-id="81099-129">属性</span><span class="sxs-lookup"><span data-stu-id="81099-129">Property</span></span>     | <span data-ttu-id="81099-130">类型</span><span class="sxs-lookup"><span data-stu-id="81099-130">Type</span></span>   |<span data-ttu-id="81099-131">说明</span><span class="sxs-lookup"><span data-stu-id="81099-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81099-132">索引</span><span class="sxs-lookup"><span data-stu-id="81099-132">index</span></span>|<span data-ttu-id="81099-133">int</span><span class="sxs-lookup"><span data-stu-id="81099-133">int</span></span>|<span data-ttu-id="81099-p101">返回表的行集合内行的索引编号。从零开始编制索引。只读。</span><span class="sxs-lookup"><span data-stu-id="81099-p101">Returns the index number of the row within the rows collection of the table. Zero-indexed. Read-only.</span></span>|
|<span data-ttu-id="81099-137">值</span><span class="sxs-lookup"><span data-stu-id="81099-137">values</span></span>|<span data-ttu-id="81099-138">Json</span><span class="sxs-lookup"><span data-stu-id="81099-138">Json</span></span>|<span data-ttu-id="81099-p102">表示指定区域的原始值。返回的数据类型可能是字符串、数字或布尔值。包含一个将返回错误字符串的错误的单元格。</span><span class="sxs-lookup"><span data-stu-id="81099-p102">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81099-142">关系</span><span class="sxs-lookup"><span data-stu-id="81099-142">Relationships</span></span>
<span data-ttu-id="81099-143">无</span><span class="sxs-lookup"><span data-stu-id="81099-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="81099-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81099-144">JSON representation</span></span>

<span data-ttu-id="81099-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81099-145">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableRow"
}-->

```json
{
  "index": 1024,
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->