# <a name="tablesort-resource-type"></a><span data-ttu-id="fd359-101">TableSort 资源类型</span><span class="sxs-lookup"><span data-stu-id="fd359-101">TableSort resource type</span></span>

<span data-ttu-id="fd359-102">管理对 Table 对象的排序操作。</span><span class="sxs-lookup"><span data-stu-id="fd359-102">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="fd359-103">方法</span><span class="sxs-lookup"><span data-stu-id="fd359-103">Methods</span></span>

| <span data-ttu-id="fd359-104">方法</span><span class="sxs-lookup"><span data-stu-id="fd359-104">Method</span></span>           | <span data-ttu-id="fd359-105">返回类型</span><span class="sxs-lookup"><span data-stu-id="fd359-105">Return Type</span></span>    |<span data-ttu-id="fd359-106">说明</span><span class="sxs-lookup"><span data-stu-id="fd359-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fd359-107">获取 TableSort</span><span class="sxs-lookup"><span data-stu-id="fd359-107">Get TableSort</span></span>](../api/tablesort_get.md) | [<span data-ttu-id="fd359-108">WorkbookTableSort</span><span class="sxs-lookup"><span data-stu-id="fd359-108">WorkbookTableSort</span></span>](tablesort.md) |<span data-ttu-id="fd359-109">读取 tableSort 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fd359-109">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="fd359-110">应用</span><span class="sxs-lookup"><span data-stu-id="fd359-110">Apply</span></span>](../api/tablesort_apply.md)|<span data-ttu-id="fd359-111">无</span><span class="sxs-lookup"><span data-stu-id="fd359-111">None</span></span>|<span data-ttu-id="fd359-112">执行排序操作。</span><span class="sxs-lookup"><span data-stu-id="fd359-112">Perform a sort operation.</span></span>|
|[<span data-ttu-id="fd359-113">清除</span><span class="sxs-lookup"><span data-stu-id="fd359-113">Clear</span></span>](../api/tablesort_clear.md)|<span data-ttu-id="fd359-114">无</span><span class="sxs-lookup"><span data-stu-id="fd359-114">None</span></span>|<span data-ttu-id="fd359-p101">清除表上的当前排序。尽管这不能修改表的排序，但它会清除标题按钮的状态。</span><span class="sxs-lookup"><span data-stu-id="fd359-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="fd359-117">重新应用</span><span class="sxs-lookup"><span data-stu-id="fd359-117">Reapply</span></span>](../api/tablesort_reapply.md)|<span data-ttu-id="fd359-118">无</span><span class="sxs-lookup"><span data-stu-id="fd359-118">None</span></span>|<span data-ttu-id="fd359-119">对表重新应用当前的排序参数。</span><span class="sxs-lookup"><span data-stu-id="fd359-119">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="fd359-120">属性</span><span class="sxs-lookup"><span data-stu-id="fd359-120">Properties</span></span>
| <span data-ttu-id="fd359-121">属性</span><span class="sxs-lookup"><span data-stu-id="fd359-121">Property</span></span>     | <span data-ttu-id="fd359-122">类型</span><span class="sxs-lookup"><span data-stu-id="fd359-122">Type</span></span>   |<span data-ttu-id="fd359-123">说明</span><span class="sxs-lookup"><span data-stu-id="fd359-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd359-124">字段</span><span class="sxs-lookup"><span data-stu-id="fd359-124">fields</span></span>|<span data-ttu-id="fd359-125">[WorkbookSortField](sortfield.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fd359-125">[WorkbookSortField](sortfield.md) collection</span></span>|<span data-ttu-id="fd359-p102">表示最后一次对表排序所使用的当前条件。只读。</span><span class="sxs-lookup"><span data-stu-id="fd359-p102">Represents the current conditions used to last sort the table. Read-only.</span></span>|
|<span data-ttu-id="fd359-128">matchCase</span><span class="sxs-lookup"><span data-stu-id="fd359-128">matchCase</span></span>|<span data-ttu-id="fd359-129">布尔值</span><span class="sxs-lookup"><span data-stu-id="fd359-129">boolean</span></span>|<span data-ttu-id="fd359-p103">表示最后一次对表进行排序时大小写是否有影响。只读。</span><span class="sxs-lookup"><span data-stu-id="fd359-p103">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="fd359-132">方法</span><span class="sxs-lookup"><span data-stu-id="fd359-132">method</span></span>|<span data-ttu-id="fd359-133">字符串</span><span class="sxs-lookup"><span data-stu-id="fd359-133">string</span></span>|<span data-ttu-id="fd359-134">代表上次表排序使用的中文排序方法。</span><span class="sxs-lookup"><span data-stu-id="fd359-134">Represents Chinese character ordering method last used to sort the table. Possible values are: , . Read-only.</span></span> <span data-ttu-id="fd359-135">可取值为：`PinYin`、`StrokeCount`。</span><span class="sxs-lookup"><span data-stu-id="fd359-135">The possible values are:</span></span> <span data-ttu-id="fd359-136">只读。</span><span class="sxs-lookup"><span data-stu-id="fd359-136">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fd359-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fd359-137">JSON representation</span></span>

<span data-ttu-id="fd359-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd359-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableSort"
}-->

```json
{
  "matchCase": true,
  "method": "string",
  "fields": [{ "@odata.type": "microsoft.graph.workbookSortField" }]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->