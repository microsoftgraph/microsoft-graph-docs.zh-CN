---
title: workbookNamedItem 资源类型
description: 表示单元格区域或值的定义名称。名称可以为基元的已命名对象（如以下类型中所示）、range 对象或对区域的引用。此对象可用于获取与名称相关的 range 对象。
localization_priority: Normal
ms.openlocfilehash: 49267379385a13b94e8639e4c129c05192b2ae6f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348607"
---
# <a name="workbooknameditem-resource-type"></a><span data-ttu-id="0f9ca-105">workbookNamedItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="0f9ca-105">workbookNamedItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f9ca-p102">表示单元格区域或值的定义名称。名称可以为基元的已命名对象（如以下类型中所示）、range 对象或对区域的引用。此对象可用于获取与名称相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="0f9ca-p102">Represents a defined name for a range of cells or value. Names can be primitive named objects (as seen in the type below), range object, reference to a range. This object can be used to obtain range object associated with names.</span></span>


## <a name="methods"></a><span data-ttu-id="0f9ca-109">方法</span><span class="sxs-lookup"><span data-stu-id="0f9ca-109">Methods</span></span>

| <span data-ttu-id="0f9ca-110">方法</span><span class="sxs-lookup"><span data-stu-id="0f9ca-110">Method</span></span>           | <span data-ttu-id="0f9ca-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="0f9ca-111">Return Type</span></span>    |<span data-ttu-id="0f9ca-112">说明</span><span class="sxs-lookup"><span data-stu-id="0f9ca-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0f9ca-113">Add</span><span class="sxs-lookup"><span data-stu-id="0f9ca-113">Add</span></span>](../api/nameditem-add.md)|[<span data-ttu-id="0f9ca-114">workbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="0f9ca-114">workbookNamedItem</span></span>](workbooknameditem.md)|<span data-ttu-id="0f9ca-115">将新名称添加到给定范围的集合。</span><span class="sxs-lookup"><span data-stu-id="0f9ca-115">Adds a new name to the collection of the given scope.</span></span>|
|[<span data-ttu-id="0f9ca-116">AddFormulaLocal</span><span class="sxs-lookup"><span data-stu-id="0f9ca-116">AddFormulaLocal</span></span>](../api/nameditem-addformulalocal.md)|[<span data-ttu-id="0f9ca-117">workbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="0f9ca-117">workbookNamedItem</span></span>](workbooknameditem.md)|<span data-ttu-id="0f9ca-118">使用用户的公式区域设置，将新名称添加到给定范围的集合。</span><span class="sxs-lookup"><span data-stu-id="0f9ca-118">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>|
|[<span data-ttu-id="0f9ca-119">获取 NamedItem</span><span class="sxs-lookup"><span data-stu-id="0f9ca-119">Get NamedItem</span></span>](../api/nameditem-get.md) | [<span data-ttu-id="0f9ca-120">workbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="0f9ca-120">workbookNamedItem</span></span>](workbooknameditem.md) |<span data-ttu-id="0f9ca-121">读取 nameditem 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0f9ca-121">Read properties and relationships of namedItem object.</span></span>|
|[<span data-ttu-id="0f9ca-122">更新</span><span class="sxs-lookup"><span data-stu-id="0f9ca-122">Update</span></span>](../api/nameditem-update.md) | [<span data-ttu-id="0f9ca-123">workbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="0f9ca-123">workbookNamedItem</span></span>](workbooknameditem.md)   |<span data-ttu-id="0f9ca-124">更新 NamedItem 对象。</span><span class="sxs-lookup"><span data-stu-id="0f9ca-124">Update NamedItem object.</span></span> |
|[<span data-ttu-id="0f9ca-125">Range</span><span class="sxs-lookup"><span data-stu-id="0f9ca-125">Range</span></span>](../api/nameditem-range.md)|[<span data-ttu-id="0f9ca-126">workbookRange</span><span class="sxs-lookup"><span data-stu-id="0f9ca-126">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="0f9ca-p103">返回与名称相关的 range 对象。如果已命名项目的类型不是区域，将引发异常。</span><span class="sxs-lookup"><span data-stu-id="0f9ca-p103">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>|
|[<span data-ttu-id="0f9ca-129">列出</span><span class="sxs-lookup"><span data-stu-id="0f9ca-129">List</span></span>](../api/nameditem-list.md) | <span data-ttu-id="0f9ca-130">[workbookNamedItem](workbooknameditem.md)集合</span><span class="sxs-lookup"><span data-stu-id="0f9ca-130">[workbookNamedItem](workbooknameditem.md) collection</span></span> |<span data-ttu-id="0f9ca-131">获取 namedItem 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0f9ca-131">Get namedItem object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="0f9ca-132">属性</span><span class="sxs-lookup"><span data-stu-id="0f9ca-132">Properties</span></span>
| <span data-ttu-id="0f9ca-133">属性</span><span class="sxs-lookup"><span data-stu-id="0f9ca-133">Property</span></span>     | <span data-ttu-id="0f9ca-134">类型</span><span class="sxs-lookup"><span data-stu-id="0f9ca-134">Type</span></span>   |<span data-ttu-id="0f9ca-135">说明</span><span class="sxs-lookup"><span data-stu-id="0f9ca-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f9ca-136">name</span><span class="sxs-lookup"><span data-stu-id="0f9ca-136">name</span></span>|<span data-ttu-id="0f9ca-137">string</span><span class="sxs-lookup"><span data-stu-id="0f9ca-137">string</span></span>|<span data-ttu-id="0f9ca-p104">对象的名称。只读。</span><span class="sxs-lookup"><span data-stu-id="0f9ca-p104">The name of the object. Read-only.</span></span>|
|<span data-ttu-id="0f9ca-140">注释</span><span class="sxs-lookup"><span data-stu-id="0f9ca-140">comment</span></span>|<span data-ttu-id="0f9ca-141">string</span><span class="sxs-lookup"><span data-stu-id="0f9ca-141">string</span></span>|<span data-ttu-id="0f9ca-142">表示与此名称相关联的注释。</span><span class="sxs-lookup"><span data-stu-id="0f9ca-142">Represents the comment associated with this name.</span></span>|
|<span data-ttu-id="0f9ca-143">scope</span><span class="sxs-lookup"><span data-stu-id="0f9ca-143">scope</span></span>|<span data-ttu-id="0f9ca-144">string</span><span class="sxs-lookup"><span data-stu-id="0f9ca-144">string</span></span>|<span data-ttu-id="0f9ca-p105">指明是否将 name 限定到工作簿或特定工作表。只读。</span><span class="sxs-lookup"><span data-stu-id="0f9ca-p105">Indicates whether the name is scoped to the workbook or to a specific worksheet. Read-only.</span></span>|
|<span data-ttu-id="0f9ca-147">类型</span><span class="sxs-lookup"><span data-stu-id="0f9ca-147">type</span></span>|<span data-ttu-id="0f9ca-148">字符串</span><span class="sxs-lookup"><span data-stu-id="0f9ca-148">string</span></span>|<span data-ttu-id="0f9ca-p106">指示与名称相关的引用类型。可能的值是：`String`、`Integer`、`Double`、`Boolean`、`Range`。只读。</span><span class="sxs-lookup"><span data-stu-id="0f9ca-p106">Indicates what type of reference is associated with the name. Possible values are: `String`, `Integer`, `Double`, `Boolean`, `Range`. Read-only.</span></span>|
|<span data-ttu-id="0f9ca-152">value</span><span class="sxs-lookup"><span data-stu-id="0f9ca-152">value</span></span>|<span data-ttu-id="0f9ca-153">string</span><span class="sxs-lookup"><span data-stu-id="0f9ca-153">string</span></span>|<span data-ttu-id="0f9ca-p107">表示名称定义为引用的公式。例如 =Sheet14!$B$2:$H$12、=4.75 等。只读。</span><span class="sxs-lookup"><span data-stu-id="0f9ca-p107">Represents the formula that the name is defined to refer to. E.g. =Sheet14!$B$2:$H$12, =4.75, etc. Read-only.</span></span>|
|<span data-ttu-id="0f9ca-157">visible</span><span class="sxs-lookup"><span data-stu-id="0f9ca-157">visible</span></span>|<span data-ttu-id="0f9ca-158">布尔</span><span class="sxs-lookup"><span data-stu-id="0f9ca-158">boolean</span></span>|<span data-ttu-id="0f9ca-159">指定对象是否可见。</span><span class="sxs-lookup"><span data-stu-id="0f9ca-159">Specifies whether the object is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f9ca-160">关系</span><span class="sxs-lookup"><span data-stu-id="0f9ca-160">Relationships</span></span>
| <span data-ttu-id="0f9ca-161">关系</span><span class="sxs-lookup"><span data-stu-id="0f9ca-161">Relationship</span></span>     | <span data-ttu-id="0f9ca-162">类型</span><span class="sxs-lookup"><span data-stu-id="0f9ca-162">Type</span></span>   |<span data-ttu-id="0f9ca-163">说明</span><span class="sxs-lookup"><span data-stu-id="0f9ca-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f9ca-164">worksheet</span><span class="sxs-lookup"><span data-stu-id="0f9ca-164">worksheet</span></span>|[<span data-ttu-id="0f9ca-165">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="0f9ca-165">workbookWorksheet</span></span>](workbookworksheet.md)|<span data-ttu-id="0f9ca-p108">返回已命名项限定到的工作表。仅在该项目的作用域为工作表时才可用。只读。</span><span class="sxs-lookup"><span data-stu-id="0f9ca-p108">Returns the worksheet on which the named item is scoped to. Available only if the item is scoped to the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0f9ca-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0f9ca-169">JSON representation</span></span>

<span data-ttu-id="0f9ca-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f9ca-170">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
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
<!--
{
  "type": "#page.annotation",
  "description": "NamedItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
