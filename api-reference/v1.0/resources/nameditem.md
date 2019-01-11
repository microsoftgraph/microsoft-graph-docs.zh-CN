---
title: NamedItem 资源类型
description: 表示单元格区域或值的定义名称。名称可以为基元的已命名对象（如以下类型中所示）、range 对象或对区域的引用。此对象可用于获取与名称相关的 range 对象。
localization_priority: Normal
ms.openlocfilehash: e413361cc42a0f8f65e23e12d36b49d2c7bcebb3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883823"
---
# <a name="nameditem-resource-type"></a><span data-ttu-id="c0ff8-105">NamedItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="c0ff8-105">NamedItem resource type</span></span>

<span data-ttu-id="c0ff8-p102">表示单元格区域或值的定义名称。名称可以为基元的已命名对象（如以下类型中所示）、range 对象或对区域的引用。此对象可用于获取与名称相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="c0ff8-p102">Represents a defined name for a range of cells or value. Names can be primitive named objects (as seen in the type below), range object, reference to a range. This object can be used to obtain range object associated with names.</span></span>


## <a name="methods"></a><span data-ttu-id="c0ff8-109">方法</span><span class="sxs-lookup"><span data-stu-id="c0ff8-109">Methods</span></span>

| <span data-ttu-id="c0ff8-110">方法</span><span class="sxs-lookup"><span data-stu-id="c0ff8-110">Method</span></span>           | <span data-ttu-id="c0ff8-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="c0ff8-111">Return Type</span></span>    |<span data-ttu-id="c0ff8-112">说明</span><span class="sxs-lookup"><span data-stu-id="c0ff8-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c0ff8-113">Add</span><span class="sxs-lookup"><span data-stu-id="c0ff8-113">Add</span></span>](../api/nameditem-add.md)|[<span data-ttu-id="c0ff8-114">WorkbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="c0ff8-114">WorkbookNamedItem</span></span>](nameditem.md)|<span data-ttu-id="c0ff8-115">将新名称添加到给定范围的集合。</span><span class="sxs-lookup"><span data-stu-id="c0ff8-115">Adds a new name to the collection of the given scope.</span></span>|
|[<span data-ttu-id="c0ff8-116">AddFormulaLocal</span><span class="sxs-lookup"><span data-stu-id="c0ff8-116">AddFormulaLocal</span></span>](../api/nameditem-addformulalocal.md)|[<span data-ttu-id="c0ff8-117">WorkbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="c0ff8-117">WorkbookNamedItem</span></span>](nameditem.md)|<span data-ttu-id="c0ff8-118">使用用户的公式区域设置，将新名称添加到给定范围的集合。</span><span class="sxs-lookup"><span data-stu-id="c0ff8-118">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>|
|[<span data-ttu-id="c0ff8-119">获取 NamedItem</span><span class="sxs-lookup"><span data-stu-id="c0ff8-119">Get NamedItem</span></span>](../api/nameditem-get.md) | [<span data-ttu-id="c0ff8-120">WorkbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="c0ff8-120">WorkbookNamedItem</span></span>](nameditem.md) |<span data-ttu-id="c0ff8-121">读取 nameditem 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c0ff8-121">Read properties and relationships of namedItem object.</span></span>|
|[<span data-ttu-id="c0ff8-122">更新</span><span class="sxs-lookup"><span data-stu-id="c0ff8-122">Update</span></span>](../api/nameditem-update.md) | [<span data-ttu-id="c0ff8-123">WorkbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="c0ff8-123">WorkbookNamedItem</span></span>](nameditem.md)   |<span data-ttu-id="c0ff8-124">更新 NamedItem 对象。</span><span class="sxs-lookup"><span data-stu-id="c0ff8-124">Update NamedItem object.</span></span> |
|[<span data-ttu-id="c0ff8-125">区域</span><span class="sxs-lookup"><span data-stu-id="c0ff8-125">Range</span></span>](../api/nameditem-range.md)|[<span data-ttu-id="c0ff8-126">Range</span><span class="sxs-lookup"><span data-stu-id="c0ff8-126">Range</span></span>](range.md)|<span data-ttu-id="c0ff8-p103">返回与名称相关的 range 对象。如果已命名项目的类型不是区域，将引发异常。</span><span class="sxs-lookup"><span data-stu-id="c0ff8-p103">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>|
|[<span data-ttu-id="c0ff8-129">列出</span><span class="sxs-lookup"><span data-stu-id="c0ff8-129">List</span></span>](../api/nameditem-list.md) | <span data-ttu-id="c0ff8-130">[WorkbookNamedItem](nameditem.md)集合</span><span class="sxs-lookup"><span data-stu-id="c0ff8-130">[WorkbookNamedItem](nameditem.md) collection</span></span> |<span data-ttu-id="c0ff8-131">获取 namedItem 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c0ff8-131">Get namedItem object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="c0ff8-132">属性</span><span class="sxs-lookup"><span data-stu-id="c0ff8-132">Properties</span></span>
| <span data-ttu-id="c0ff8-133">属性</span><span class="sxs-lookup"><span data-stu-id="c0ff8-133">Property</span></span>     | <span data-ttu-id="c0ff8-134">类型</span><span class="sxs-lookup"><span data-stu-id="c0ff8-134">Type</span></span>   |<span data-ttu-id="c0ff8-135">说明</span><span class="sxs-lookup"><span data-stu-id="c0ff8-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0ff8-136">name</span><span class="sxs-lookup"><span data-stu-id="c0ff8-136">name</span></span>|<span data-ttu-id="c0ff8-137">string</span><span class="sxs-lookup"><span data-stu-id="c0ff8-137">string</span></span>|<span data-ttu-id="c0ff8-p104">对象的名称。只读。</span><span class="sxs-lookup"><span data-stu-id="c0ff8-p104">The name of the object. Read-only.</span></span>|
|<span data-ttu-id="c0ff8-140">注释</span><span class="sxs-lookup"><span data-stu-id="c0ff8-140">comment</span></span>|<span data-ttu-id="c0ff8-141">string</span><span class="sxs-lookup"><span data-stu-id="c0ff8-141">string</span></span>|<span data-ttu-id="c0ff8-142">表示与此名称相关联的注释。</span><span class="sxs-lookup"><span data-stu-id="c0ff8-142">Represents the comment associated with this name.</span></span>|
|<span data-ttu-id="c0ff8-143">scope</span><span class="sxs-lookup"><span data-stu-id="c0ff8-143">scope</span></span>|<span data-ttu-id="c0ff8-144">string</span><span class="sxs-lookup"><span data-stu-id="c0ff8-144">string</span></span>|<span data-ttu-id="c0ff8-p105">指明是否将 name 限定到工作簿或特定工作表。只读。</span><span class="sxs-lookup"><span data-stu-id="c0ff8-p105">Indicates whether the name is scoped to the workbook or to a specific worksheet. Read-only.</span></span>|
|<span data-ttu-id="c0ff8-147">type</span><span class="sxs-lookup"><span data-stu-id="c0ff8-147">type</span></span>|<span data-ttu-id="c0ff8-148">string</span><span class="sxs-lookup"><span data-stu-id="c0ff8-148">string</span></span>|<span data-ttu-id="c0ff8-149">指示与名称引用的内容类型相关联。</span><span class="sxs-lookup"><span data-stu-id="c0ff8-149">Indicates what type of reference is associated with the name.</span></span> <span data-ttu-id="c0ff8-150">可能的值为： `String`， `Integer`， `Double`， `Boolean`， `Range`。</span><span class="sxs-lookup"><span data-stu-id="c0ff8-150">The possible values are: `String`, `Integer`, `Double`, `Boolean`, `Range`.</span></span> <span data-ttu-id="c0ff8-151">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="c0ff8-151">Read-only.</span></span>|
|<span data-ttu-id="c0ff8-152">值</span><span class="sxs-lookup"><span data-stu-id="c0ff8-152">value</span></span>|<span data-ttu-id="c0ff8-153">Json</span><span class="sxs-lookup"><span data-stu-id="c0ff8-153">Json</span></span>|<span data-ttu-id="c0ff8-p107">表示名称定义为引用的公式。例如 =Sheet14!$B$2:$H$12、=4.75 等。只读。</span><span class="sxs-lookup"><span data-stu-id="c0ff8-p107">Represents the formula that the name is defined to refer to. E.g. =Sheet14!$B$2:$H$12, =4.75, etc. Read-only.</span></span>|
|<span data-ttu-id="c0ff8-157">visible</span><span class="sxs-lookup"><span data-stu-id="c0ff8-157">visible</span></span>|<span data-ttu-id="c0ff8-158">boolean</span><span class="sxs-lookup"><span data-stu-id="c0ff8-158">boolean</span></span>|<span data-ttu-id="c0ff8-159">指定对象是否可见。</span><span class="sxs-lookup"><span data-stu-id="c0ff8-159">Specifies whether the object is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0ff8-160">Relationships</span><span class="sxs-lookup"><span data-stu-id="c0ff8-160">Relationships</span></span>
| <span data-ttu-id="c0ff8-161">关系</span><span class="sxs-lookup"><span data-stu-id="c0ff8-161">Relationship</span></span>     | <span data-ttu-id="c0ff8-162">类型</span><span class="sxs-lookup"><span data-stu-id="c0ff8-162">Type</span></span>   |<span data-ttu-id="c0ff8-163">说明</span><span class="sxs-lookup"><span data-stu-id="c0ff8-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0ff8-164">worksheet</span><span class="sxs-lookup"><span data-stu-id="c0ff8-164">worksheet</span></span>|[<span data-ttu-id="c0ff8-165">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="c0ff8-165">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="c0ff8-p108">返回已命名项限定到的工作表。仅在该项目的作用域为工作表时才可用。只读。</span><span class="sxs-lookup"><span data-stu-id="c0ff8-p108">Returns the worksheet on which the named item is scoped to. Available only if the item is scoped to the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c0ff8-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c0ff8-169">JSON representation</span></span>

<span data-ttu-id="c0ff8-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c0ff8-170">Here is a JSON representation of the resource.</span></span>

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
