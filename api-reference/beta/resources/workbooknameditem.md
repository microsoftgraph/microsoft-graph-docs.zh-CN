---
title: WorkbookNamedItem 资源类型
description: 表示单元格区域或值的定义名称。名称可以为基元的已命名对象（如以下类型中所示）、range 对象或对区域的引用。此对象可用于获取与名称相关的 range 对象。
localization_priority: Normal
ms.openlocfilehash: 79ed5211c60555d2cfc55e01c49565ebecd58a8b
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29579847"
---
# <a name="nameditem-resource-type"></a><span data-ttu-id="88dd2-105">NamedItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="88dd2-105">NamedItem resource type</span></span>

<span data-ttu-id="88dd2-p102">表示单元格区域或值的定义名称。名称可以为基元的已命名对象（如以下类型中所示）、range 对象或对区域的引用。此对象可用于获取与名称相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="88dd2-p102">Represents a defined name for a range of cells or value. Names can be primitive named objects (as seen in the type below), range object, reference to a range. This object can be used to obtain range object associated with names.</span></span>


## <a name="methods"></a><span data-ttu-id="88dd2-109">方法</span><span class="sxs-lookup"><span data-stu-id="88dd2-109">Methods</span></span>

| <span data-ttu-id="88dd2-110">方法</span><span class="sxs-lookup"><span data-stu-id="88dd2-110">Method</span></span>           | <span data-ttu-id="88dd2-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="88dd2-111">Return Type</span></span>    |<span data-ttu-id="88dd2-112">说明</span><span class="sxs-lookup"><span data-stu-id="88dd2-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="88dd2-113">Add</span><span class="sxs-lookup"><span data-stu-id="88dd2-113">Add</span></span>](../api/nameditem-add.md)|[<span data-ttu-id="88dd2-114">workbookNameditem</span><span class="sxs-lookup"><span data-stu-id="88dd2-114">workbookNameditem</span></span>](workbooknameditem.md)|<span data-ttu-id="88dd2-115">将新名称添加到给定范围的集合。</span><span class="sxs-lookup"><span data-stu-id="88dd2-115">Adds a new name to the collection of the given scope.</span></span>|
|[<span data-ttu-id="88dd2-116">AddFormulaLocal</span><span class="sxs-lookup"><span data-stu-id="88dd2-116">AddFormulaLocal</span></span>](../api/nameditem-addformulalocal.md)|[<span data-ttu-id="88dd2-117">workbookNameditem</span><span class="sxs-lookup"><span data-stu-id="88dd2-117">workbookNameditem</span></span>](workbooknameditem.md)|<span data-ttu-id="88dd2-118">使用用户的公式区域设置，将新名称添加到给定范围的集合。</span><span class="sxs-lookup"><span data-stu-id="88dd2-118">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>|
|[<span data-ttu-id="88dd2-119">获取 NamedItem</span><span class="sxs-lookup"><span data-stu-id="88dd2-119">Get NamedItem</span></span>](../api/nameditem-get.md) | [<span data-ttu-id="88dd2-120">workbookNameditem</span><span class="sxs-lookup"><span data-stu-id="88dd2-120">workbookNameditem</span></span>](workbooknameditem.md) |<span data-ttu-id="88dd2-121">读取 nameditem 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="88dd2-121">Read properties and relationships of namedItem object.</span></span>|
|[<span data-ttu-id="88dd2-122">更新</span><span class="sxs-lookup"><span data-stu-id="88dd2-122">Update</span></span>](../api/nameditem-update.md) | [<span data-ttu-id="88dd2-123">workbookNameditem</span><span class="sxs-lookup"><span data-stu-id="88dd2-123">workbookNameditem</span></span>](workbooknameditem.md)   |<span data-ttu-id="88dd2-124">更新 NamedItem 对象。</span><span class="sxs-lookup"><span data-stu-id="88dd2-124">Update NamedItem object.</span></span> |
|[<span data-ttu-id="88dd2-125">区域</span><span class="sxs-lookup"><span data-stu-id="88dd2-125">Range</span></span>](../api/nameditem-range.md)|[<span data-ttu-id="88dd2-126">range</span><span class="sxs-lookup"><span data-stu-id="88dd2-126">range</span></span>](range.md)|<span data-ttu-id="88dd2-p103">返回与名称相关的 range 对象。如果已命名项目的类型不是区域，将引发异常。</span><span class="sxs-lookup"><span data-stu-id="88dd2-p103">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>|
|[<span data-ttu-id="88dd2-129">列出</span><span class="sxs-lookup"><span data-stu-id="88dd2-129">List</span></span>](../api/nameditem-list.md) | <span data-ttu-id="88dd2-130">[workbookNameditem](workbooknameditem.md)集合</span><span class="sxs-lookup"><span data-stu-id="88dd2-130">[workbookNameditem](workbooknameditem.md) collection</span></span> |<span data-ttu-id="88dd2-131">获取 namedItem 对象集合。</span><span class="sxs-lookup"><span data-stu-id="88dd2-131">Get namedItem object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="88dd2-132">属性</span><span class="sxs-lookup"><span data-stu-id="88dd2-132">Properties</span></span>
| <span data-ttu-id="88dd2-133">属性</span><span class="sxs-lookup"><span data-stu-id="88dd2-133">Property</span></span>     | <span data-ttu-id="88dd2-134">类型</span><span class="sxs-lookup"><span data-stu-id="88dd2-134">Type</span></span>   |<span data-ttu-id="88dd2-135">说明</span><span class="sxs-lookup"><span data-stu-id="88dd2-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88dd2-136">name</span><span class="sxs-lookup"><span data-stu-id="88dd2-136">name</span></span>|<span data-ttu-id="88dd2-137">string</span><span class="sxs-lookup"><span data-stu-id="88dd2-137">string</span></span>|<span data-ttu-id="88dd2-p104">对象的名称。只读。</span><span class="sxs-lookup"><span data-stu-id="88dd2-p104">The name of the object. Read-only.</span></span>|
|<span data-ttu-id="88dd2-140">注释</span><span class="sxs-lookup"><span data-stu-id="88dd2-140">comment</span></span>|<span data-ttu-id="88dd2-141">string</span><span class="sxs-lookup"><span data-stu-id="88dd2-141">string</span></span>|<span data-ttu-id="88dd2-142">表示与此名称相关联的注释。</span><span class="sxs-lookup"><span data-stu-id="88dd2-142">Represents the comment associated with this name.</span></span>|
|<span data-ttu-id="88dd2-143">scope</span><span class="sxs-lookup"><span data-stu-id="88dd2-143">scope</span></span>|<span data-ttu-id="88dd2-144">string</span><span class="sxs-lookup"><span data-stu-id="88dd2-144">string</span></span>|<span data-ttu-id="88dd2-p105">指明是否将 name 限定到工作簿或特定工作表。只读。</span><span class="sxs-lookup"><span data-stu-id="88dd2-p105">Indicates whether the name is scoped to the workbook or to a specific worksheet. Read-only.</span></span>|
|<span data-ttu-id="88dd2-147">type</span><span class="sxs-lookup"><span data-stu-id="88dd2-147">type</span></span>|<span data-ttu-id="88dd2-148">string</span><span class="sxs-lookup"><span data-stu-id="88dd2-148">string</span></span>|<span data-ttu-id="88dd2-p106">指示与名称相关的引用类型。可能的值是：`String`、`Integer`、`Double`、`Boolean`、`Range`。只读。</span><span class="sxs-lookup"><span data-stu-id="88dd2-p106">Indicates what type of reference is associated with the name. Possible values are: `String`, `Integer`, `Double`, `Boolean`, `Range`. Read-only.</span></span>|
|<span data-ttu-id="88dd2-152">值</span><span class="sxs-lookup"><span data-stu-id="88dd2-152">value</span></span>|<span data-ttu-id="88dd2-153">string</span><span class="sxs-lookup"><span data-stu-id="88dd2-153">string</span></span>|<span data-ttu-id="88dd2-p107">表示名称定义为引用的公式。例如 =Sheet14!$B$2:$H$12、=4.75 等。只读。</span><span class="sxs-lookup"><span data-stu-id="88dd2-p107">Represents the formula that the name is defined to refer to. E.g. =Sheet14!$B$2:$H$12, =4.75, etc. Read-only.</span></span>|
|<span data-ttu-id="88dd2-157">visible</span><span class="sxs-lookup"><span data-stu-id="88dd2-157">visible</span></span>|<span data-ttu-id="88dd2-158">布尔</span><span class="sxs-lookup"><span data-stu-id="88dd2-158">boolean</span></span>|<span data-ttu-id="88dd2-159">指定对象是否可见。</span><span class="sxs-lookup"><span data-stu-id="88dd2-159">Specifies whether the object is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88dd2-160">关系</span><span class="sxs-lookup"><span data-stu-id="88dd2-160">Relationships</span></span>
| <span data-ttu-id="88dd2-161">关系</span><span class="sxs-lookup"><span data-stu-id="88dd2-161">Relationship</span></span>     | <span data-ttu-id="88dd2-162">类型</span><span class="sxs-lookup"><span data-stu-id="88dd2-162">Type</span></span>   |<span data-ttu-id="88dd2-163">说明</span><span class="sxs-lookup"><span data-stu-id="88dd2-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88dd2-164">worksheet</span><span class="sxs-lookup"><span data-stu-id="88dd2-164">worksheet</span></span>|[<span data-ttu-id="88dd2-165">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="88dd2-165">workbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="88dd2-p108">返回已命名项限定到的工作表。仅在该项目的作用域为工作表时才可用。只读。</span><span class="sxs-lookup"><span data-stu-id="88dd2-p108">Returns the worksheet on which the named item is scoped to. Available only if the item is scoped to the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="88dd2-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="88dd2-169">JSON representation</span></span>

<span data-ttu-id="88dd2-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88dd2-170">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookNamedItem"
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
