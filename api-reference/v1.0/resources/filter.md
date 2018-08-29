# <a name="filter-resource-type"></a><span data-ttu-id="682ab-101">筛选器资源类型</span><span class="sxs-lookup"><span data-stu-id="682ab-101">Filter resource type</span></span>

<span data-ttu-id="682ab-102">管理表格列的筛选。</span><span class="sxs-lookup"><span data-stu-id="682ab-102">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="682ab-103">方法</span><span class="sxs-lookup"><span data-stu-id="682ab-103">Methods</span></span>

| <span data-ttu-id="682ab-104">方法</span><span class="sxs-lookup"><span data-stu-id="682ab-104">Method</span></span>           | <span data-ttu-id="682ab-105">返回类型</span><span class="sxs-lookup"><span data-stu-id="682ab-105">Return Type</span></span>    |<span data-ttu-id="682ab-106">说明</span><span class="sxs-lookup"><span data-stu-id="682ab-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="682ab-107">Apply</span><span class="sxs-lookup"><span data-stu-id="682ab-107">Apply</span></span>](../api/filter_apply.md)|<span data-ttu-id="682ab-108">无</span><span class="sxs-lookup"><span data-stu-id="682ab-108">None</span></span>|<span data-ttu-id="682ab-109">在给定列中应用给定的筛选条件。</span><span class="sxs-lookup"><span data-stu-id="682ab-109">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="682ab-110">Clear</span><span class="sxs-lookup"><span data-stu-id="682ab-110">Clear</span></span>](../api/filter_clear.md)|<span data-ttu-id="682ab-111">无</span><span class="sxs-lookup"><span data-stu-id="682ab-111">None</span></span>|<span data-ttu-id="682ab-112">清除给定列上的筛选器。</span><span class="sxs-lookup"><span data-stu-id="682ab-112">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="682ab-113">属性</span><span class="sxs-lookup"><span data-stu-id="682ab-113">Properties</span></span>

| <span data-ttu-id="682ab-114">名称</span><span class="sxs-lookup"><span data-stu-id="682ab-114">Name</span></span> | <span data-ttu-id="682ab-115">类型</span><span class="sxs-lookup"><span data-stu-id="682ab-115">Type</span></span>   |<span data-ttu-id="682ab-116">说明</span><span class="sxs-lookup"><span data-stu-id="682ab-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="682ab-117">criteria</span><span class="sxs-lookup"><span data-stu-id="682ab-117">criteria</span></span>|[<span data-ttu-id="682ab-118">WorkbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="682ab-118">WorkbookFilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="682ab-p101">给定列上当前应用的筛选器。只读。</span><span class="sxs-lookup"><span data-stu-id="682ab-p101">The currently applied filter on the given column. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="682ab-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="682ab-121">JSON representation</span></span>

<span data-ttu-id="682ab-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="682ab-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilter"
}-->

```json
{
  "criteria": {"@odata.type": "microsoft.graph.workbookFilterCriteria" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->