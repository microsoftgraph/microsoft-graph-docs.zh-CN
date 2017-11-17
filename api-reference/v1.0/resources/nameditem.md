# <a name="nameditem-resource-type"></a><span data-ttu-id="bef0e-101">NamedItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="bef0e-101">NamedItem resource type</span></span>

<span data-ttu-id="bef0e-p101">表示单元格区域或值的定义名称。名称可以为基元的已命名对象（如以下类型中所示）、range 对象或对区域的引用。此对象可用于获取与名称相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="bef0e-p101">Represents a defined name for a range of cells or value. Names can be primitive named objects (as seen in the type below), range object, reference to a range. This object can be used to obtain range object associated with names.</span></span>


## <a name="methods"></a><span data-ttu-id="bef0e-105">方法</span><span class="sxs-lookup"><span data-stu-id="bef0e-105">Methods</span></span>

| <span data-ttu-id="bef0e-106">方法</span><span class="sxs-lookup"><span data-stu-id="bef0e-106">Method</span></span>           | <span data-ttu-id="bef0e-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="bef0e-107">Return Type</span></span>    |<span data-ttu-id="bef0e-108">说明</span><span class="sxs-lookup"><span data-stu-id="bef0e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bef0e-109">Add</span><span class="sxs-lookup"><span data-stu-id="bef0e-109">Add</span></span>](../api/nameditem_add.md)|[<span data-ttu-id="bef0e-110">NamedItem</span><span class="sxs-lookup"><span data-stu-id="bef0e-110">NamedItem</span></span>](nameditem.md)|<span data-ttu-id="bef0e-111">将新名称添加到给定范围的集合。</span><span class="sxs-lookup"><span data-stu-id="bef0e-111">Adds a new name to the collection of the given scope.</span></span>|
|[<span data-ttu-id="bef0e-112">AddFormulaLocal</span><span class="sxs-lookup"><span data-stu-id="bef0e-112">AddFormulaLocal</span></span>](../api/nameditem_addformulalocal.md)|[<span data-ttu-id="bef0e-113">NamedItem</span><span class="sxs-lookup"><span data-stu-id="bef0e-113">NamedItem</span></span>](nameditem.md)|<span data-ttu-id="bef0e-114">使用用户的公式区域设置，将新名称添加到给定范围的集合。</span><span class="sxs-lookup"><span data-stu-id="bef0e-114">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>|
|[<span data-ttu-id="bef0e-115">获取 NamedItem</span><span class="sxs-lookup"><span data-stu-id="bef0e-115">Get NamedItem</span></span>](../api/nameditem_get.md) | [<span data-ttu-id="bef0e-116">NamedItem</span><span class="sxs-lookup"><span data-stu-id="bef0e-116">NamedItem</span></span>](nameditem.md) |<span data-ttu-id="bef0e-117">读取 nameditem 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bef0e-117">Read properties and relationships of namedItem object.</span></span>|
|[<span data-ttu-id="bef0e-118">更新</span><span class="sxs-lookup"><span data-stu-id="bef0e-118">Update</span></span>](../api/nameditem_update.md) | [<span data-ttu-id="bef0e-119">NamedItem</span><span class="sxs-lookup"><span data-stu-id="bef0e-119">NamedItem</span></span>](nameditem.md)   |<span data-ttu-id="bef0e-120">更新 NamedItem 对象。</span><span class="sxs-lookup"><span data-stu-id="bef0e-120">Update NamedItem object.</span></span> |
|[<span data-ttu-id="bef0e-121">区域</span><span class="sxs-lookup"><span data-stu-id="bef0e-121">Range</span></span>](../api/nameditem_range.md)|[<span data-ttu-id="bef0e-122">Range</span><span class="sxs-lookup"><span data-stu-id="bef0e-122">Range</span></span>](range.md)|<span data-ttu-id="bef0e-p102">返回与名称相关的 range 对象。如果已命名项目的类型不是区域，将引发异常。</span><span class="sxs-lookup"><span data-stu-id="bef0e-p102">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>|
|[<span data-ttu-id="bef0e-125">列出</span><span class="sxs-lookup"><span data-stu-id="bef0e-125">List</span></span>](../api/nameditem_list.md) | <span data-ttu-id="bef0e-126">[NamedItem](nameditem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bef0e-126">[NamedItem](nameditem.md) collection</span></span> |<span data-ttu-id="bef0e-127">获取 namedItem 对象集合。</span><span class="sxs-lookup"><span data-stu-id="bef0e-127">Get namedItem object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="bef0e-128">属性</span><span class="sxs-lookup"><span data-stu-id="bef0e-128">Properties</span></span>
| <span data-ttu-id="bef0e-129">属性</span><span class="sxs-lookup"><span data-stu-id="bef0e-129">Property</span></span>     | <span data-ttu-id="bef0e-130">类型</span><span class="sxs-lookup"><span data-stu-id="bef0e-130">Type</span></span>   |<span data-ttu-id="bef0e-131">说明</span><span class="sxs-lookup"><span data-stu-id="bef0e-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bef0e-132">name</span><span class="sxs-lookup"><span data-stu-id="bef0e-132">name</span></span>|<span data-ttu-id="bef0e-133">string</span><span class="sxs-lookup"><span data-stu-id="bef0e-133">string</span></span>|<span data-ttu-id="bef0e-p103">对象的名称。只读。</span><span class="sxs-lookup"><span data-stu-id="bef0e-p103">The name of the object. Read-only.</span></span>|
|<span data-ttu-id="bef0e-136">注释</span><span class="sxs-lookup"><span data-stu-id="bef0e-136">comment</span></span>|<span data-ttu-id="bef0e-137">string</span><span class="sxs-lookup"><span data-stu-id="bef0e-137">string</span></span>|<span data-ttu-id="bef0e-138">表示与此名称相关联的注释。</span><span class="sxs-lookup"><span data-stu-id="bef0e-138">Represents the comment associated with this name.</span></span>|
|<span data-ttu-id="bef0e-139">scope</span><span class="sxs-lookup"><span data-stu-id="bef0e-139">scope</span></span>|<span data-ttu-id="bef0e-140">string</span><span class="sxs-lookup"><span data-stu-id="bef0e-140">string</span></span>|<span data-ttu-id="bef0e-p104">指明是否将 name 限定到工作簿或特定工作表。只读。</span><span class="sxs-lookup"><span data-stu-id="bef0e-p104">Indicates whether the name is scoped to the workbook or to a specific worksheet. Read-only.</span></span>|
|<span data-ttu-id="bef0e-143">类型</span><span class="sxs-lookup"><span data-stu-id="bef0e-143">type</span></span>|<span data-ttu-id="bef0e-144">string</span><span class="sxs-lookup"><span data-stu-id="bef0e-144">string</span></span>|<span data-ttu-id="bef0e-p105">指示与名称相关的引用类型。可能的值是：`String`、`Integer`、`Double`、`Boolean`、`Range`。只读。</span><span class="sxs-lookup"><span data-stu-id="bef0e-p105">Indicates what type of reference is associated with the name. Possible values are: `String`, `Integer`, `Double`, `Boolean`, `Range`. Read-only.</span></span>|
|<span data-ttu-id="bef0e-148">值</span><span class="sxs-lookup"><span data-stu-id="bef0e-148">value</span></span>|<span data-ttu-id="bef0e-149">string</span><span class="sxs-lookup"><span data-stu-id="bef0e-149">string</span></span>|<span data-ttu-id="bef0e-p106">表示名称定义为引用的公式。例如 =Sheet14!$B$2:$H$12、=4.75 等。只读。</span><span class="sxs-lookup"><span data-stu-id="bef0e-p106">Represents the formula that the name is defined to refer to. E.g. =Sheet14!$B$2:$H$12, =4.75, etc. Read-only.</span></span>|
|<span data-ttu-id="bef0e-153">visible</span><span class="sxs-lookup"><span data-stu-id="bef0e-153">visible</span></span>|<span data-ttu-id="bef0e-154">boolean</span><span class="sxs-lookup"><span data-stu-id="bef0e-154">boolean</span></span>|<span data-ttu-id="bef0e-155">指定对象是否可见。</span><span class="sxs-lookup"><span data-stu-id="bef0e-155">Specifies whether the object is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bef0e-156">关系</span><span class="sxs-lookup"><span data-stu-id="bef0e-156">Relationships</span></span>
| <span data-ttu-id="bef0e-157">关系</span><span class="sxs-lookup"><span data-stu-id="bef0e-157">Relationship</span></span>     | <span data-ttu-id="bef0e-158">类型</span><span class="sxs-lookup"><span data-stu-id="bef0e-158">Type</span></span>   |<span data-ttu-id="bef0e-159">说明</span><span class="sxs-lookup"><span data-stu-id="bef0e-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bef0e-160">worksheet</span><span class="sxs-lookup"><span data-stu-id="bef0e-160">worksheet</span></span>|[<span data-ttu-id="bef0e-161">worksheet</span><span class="sxs-lookup"><span data-stu-id="bef0e-161">worksheet</span></span>](worksheet.md)|<span data-ttu-id="bef0e-p107">返回已命名项限定到的工作表。仅在该项目的作用域为工作表时才可用。只读。</span><span class="sxs-lookup"><span data-stu-id="bef0e-p107">Returns the worksheet on which the named item is scoped to. Available only if the item is scoped to the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bef0e-165">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bef0e-165">JSON representation</span></span>

<span data-ttu-id="bef0e-166">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bef0e-166">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.namedItem"
}-->

```json
{
  "name": "string",
  "comment": "string",
  "scope": "string",
  "type": "string",
  "value": "string",
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
