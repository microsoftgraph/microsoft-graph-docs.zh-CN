# <a name="nameditem-resource-type"></a><span data-ttu-id="21989-101">NamedItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="21989-101">NamedItem resource type</span></span>

<span data-ttu-id="21989-p101">表示单元格区域或值的定义名称。名称可以为基元的已命名对象（如以下类型中所示）、range 对象或对区域的引用。此对象可用于获取与名称相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="21989-p101">Represents a defined name for a range of cells or value. Names can be primitive named objects (as seen in the type below), range object, reference to a range. This object can be used to obtain range object associated with names.</span></span>


## <a name="methods"></a><span data-ttu-id="21989-105">方法</span><span class="sxs-lookup"><span data-stu-id="21989-105">Methods</span></span>

| <span data-ttu-id="21989-106">方法</span><span class="sxs-lookup"><span data-stu-id="21989-106">Method</span></span>           | <span data-ttu-id="21989-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="21989-107">Return Type</span></span>    |<span data-ttu-id="21989-108">说明</span><span class="sxs-lookup"><span data-stu-id="21989-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="21989-109">Add</span><span class="sxs-lookup"><span data-stu-id="21989-109">Add</span></span>](../api/nameditem_add.md)|[<span data-ttu-id="21989-110">WorkbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="21989-110">WorkbookNamedItem</span></span>](nameditem.md)|<span data-ttu-id="21989-111">将新名称添加到给定范围的集合。</span><span class="sxs-lookup"><span data-stu-id="21989-111">Adds a new name to the collection of the given scope.</span></span>|
|[<span data-ttu-id="21989-112">AddFormulaLocal</span><span class="sxs-lookup"><span data-stu-id="21989-112">AddFormulaLocal</span></span>](../api/nameditem_addformulalocal.md)|[<span data-ttu-id="21989-113">WorkbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="21989-113">WorkbookNamedItem</span></span>](nameditem.md)|<span data-ttu-id="21989-114">使用用户的公式区域设置，将新名称添加到给定范围的集合。</span><span class="sxs-lookup"><span data-stu-id="21989-114">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>|
|[<span data-ttu-id="21989-115">获取 NamedItem</span><span class="sxs-lookup"><span data-stu-id="21989-115">Get NamedItem</span></span>](../api/nameditem_get.md) | [<span data-ttu-id="21989-116">WorkbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="21989-116">WorkbookNamedItem</span></span>](nameditem.md) |<span data-ttu-id="21989-117">读取 nameditem 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="21989-117">Read properties and relationships of namedItem object.</span></span>|
|[<span data-ttu-id="21989-118">更新</span><span class="sxs-lookup"><span data-stu-id="21989-118">Update</span></span>](../api/nameditem_update.md) | [<span data-ttu-id="21989-119">WorkbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="21989-119">WorkbookNamedItem</span></span>](nameditem.md)   |<span data-ttu-id="21989-120">更新 NamedItem 对象。</span><span class="sxs-lookup"><span data-stu-id="21989-120">Update NamedItem object.</span></span> |
|[<span data-ttu-id="21989-121">区域</span><span class="sxs-lookup"><span data-stu-id="21989-121">Range</span></span>](../api/nameditem_range.md)|[<span data-ttu-id="21989-122">区域</span><span class="sxs-lookup"><span data-stu-id="21989-122">Range</span></span>](range.md)|<span data-ttu-id="21989-p102">返回与名称相关的 range 对象。如果已命名项目的类型不是区域，将引发异常。</span><span class="sxs-lookup"><span data-stu-id="21989-p102">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>|
|[<span data-ttu-id="21989-125">列表</span><span class="sxs-lookup"><span data-stu-id="21989-125">List</span></span>](../api/nameditem_list.md) | <span data-ttu-id="21989-126">[WorkbookNamedItem](nameditem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="21989-126">[WorkbookNamedItem](nameditem.md) collection</span></span> |<span data-ttu-id="21989-127">获取 namedItem 对象集合。</span><span class="sxs-lookup"><span data-stu-id="21989-127">Get namedItem object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="21989-128">属性</span><span class="sxs-lookup"><span data-stu-id="21989-128">Properties</span></span>
| <span data-ttu-id="21989-129">属性</span><span class="sxs-lookup"><span data-stu-id="21989-129">Property</span></span>     | <span data-ttu-id="21989-130">类型</span><span class="sxs-lookup"><span data-stu-id="21989-130">Type</span></span>   |<span data-ttu-id="21989-131">说明</span><span class="sxs-lookup"><span data-stu-id="21989-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21989-132">name</span><span class="sxs-lookup"><span data-stu-id="21989-132">name</span></span>|<span data-ttu-id="21989-133">string</span><span class="sxs-lookup"><span data-stu-id="21989-133">string</span></span>|<span data-ttu-id="21989-p103">对象的名称。只读。</span><span class="sxs-lookup"><span data-stu-id="21989-p103">The name of the object. Read-only.</span></span>|
|<span data-ttu-id="21989-136">注释</span><span class="sxs-lookup"><span data-stu-id="21989-136">comment</span></span>|<span data-ttu-id="21989-137">string</span><span class="sxs-lookup"><span data-stu-id="21989-137">string</span></span>|<span data-ttu-id="21989-138">表示与此名称相关联的注释。</span><span class="sxs-lookup"><span data-stu-id="21989-138">Represents the comment associated with this name.</span></span>|
|<span data-ttu-id="21989-139">scope</span><span class="sxs-lookup"><span data-stu-id="21989-139">scope</span></span>|<span data-ttu-id="21989-140">string</span><span class="sxs-lookup"><span data-stu-id="21989-140">string</span></span>|<span data-ttu-id="21989-p104">指明是否将 name 限定到工作簿或特定工作表。只读。</span><span class="sxs-lookup"><span data-stu-id="21989-p104">Indicates whether the name is scoped to the workbook or to a specific worksheet. Read-only.</span></span>|
|<span data-ttu-id="21989-143">类型</span><span class="sxs-lookup"><span data-stu-id="21989-143">type</span></span>|<span data-ttu-id="21989-144">string</span><span class="sxs-lookup"><span data-stu-id="21989-144">string</span></span>|<span data-ttu-id="21989-145">指示与名称相关的引用类型。</span><span class="sxs-lookup"><span data-stu-id="21989-145">Indicates what type of reference is associated with the name. Possible values are: , , , , . Read-only.</span></span> <span data-ttu-id="21989-146">可取值为：`String`、`Integer`、`Double`、`Boolean`、`Range`。</span><span class="sxs-lookup"><span data-stu-id="21989-146">The possible values are `String`, `Integer`, `Double`, `Boolean`, `Range`, , , , , , , or .</span></span> <span data-ttu-id="21989-147">只读。</span><span class="sxs-lookup"><span data-stu-id="21989-147">Read-only.</span></span>|
|<span data-ttu-id="21989-148">值</span><span class="sxs-lookup"><span data-stu-id="21989-148">value</span></span>|<span data-ttu-id="21989-149">Json</span><span class="sxs-lookup"><span data-stu-id="21989-149">Json</span></span>|<span data-ttu-id="21989-p106">表示名称定义为引用的公式。例如 =Sheet14!$B$2:$H$12、=4.75 等。只读。</span><span class="sxs-lookup"><span data-stu-id="21989-p106">Represents the formula that the name is defined to refer to. E.g. =Sheet14!$B$2:$H$12, =4.75, etc. Read-only.</span></span>|
|<span data-ttu-id="21989-153">visible</span><span class="sxs-lookup"><span data-stu-id="21989-153">visible</span></span>|<span data-ttu-id="21989-154">boolean</span><span class="sxs-lookup"><span data-stu-id="21989-154">boolean</span></span>|<span data-ttu-id="21989-155">指定对象是否可见。</span><span class="sxs-lookup"><span data-stu-id="21989-155">Specifies whether the object is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21989-156">关系</span><span class="sxs-lookup"><span data-stu-id="21989-156">Relationships</span></span>
| <span data-ttu-id="21989-157">关系</span><span class="sxs-lookup"><span data-stu-id="21989-157">Relationship</span></span>     | <span data-ttu-id="21989-158">类型</span><span class="sxs-lookup"><span data-stu-id="21989-158">Type</span></span>   |<span data-ttu-id="21989-159">说明</span><span class="sxs-lookup"><span data-stu-id="21989-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21989-160">worksheet</span><span class="sxs-lookup"><span data-stu-id="21989-160">worksheet</span></span>|[<span data-ttu-id="21989-161">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="21989-161">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="21989-p107">返回已命名项限定到的工作表。仅在该项目的作用域为工作表时才可用。只读。</span><span class="sxs-lookup"><span data-stu-id="21989-p107">Returns the worksheet on which the named item is scoped to. Available only if the item is scoped to the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="21989-165">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="21989-165">JSON representation</span></span>

<span data-ttu-id="21989-166">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="21989-166">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookNamedItem"
}-->

```json
{
  "name": "string",
  "comment": "string",
  "scope": "string",
  "type": "string",
  "value": {"@odata.type": "microsoft.graph.Json"},
  "visible": true
  
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
