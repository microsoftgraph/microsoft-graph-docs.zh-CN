---
title: NamedItem 资源类型
description: 表示单元格区域或值的定义名称。名称可以为基元的已命名对象（如以下类型中所示）、range 对象或对区域的引用。此对象可用于获取与名称相关的 range 对象。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0aece739f4a65db35271e4fe6f2c87db3a2c56a5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534208"
---
# <a name="nameditem-resource-type"></a><span data-ttu-id="e4ac1-105">NamedItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="e4ac1-105">NamedItem resource type</span></span>

<span data-ttu-id="e4ac1-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4ac1-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e4ac1-p102">表示单元格区域或值的定义名称。名称可以为基元的已命名对象（如以下类型中所示）、range 对象或对区域的引用。此对象可用于获取与名称相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="e4ac1-p102">Represents a defined name for a range of cells or value. Names can be primitive named objects (as seen in the type below), range object, reference to a range. This object can be used to obtain range object associated with names.</span></span>


## <a name="methods"></a><span data-ttu-id="e4ac1-110">Methods</span><span class="sxs-lookup"><span data-stu-id="e4ac1-110">Methods</span></span>

| <span data-ttu-id="e4ac1-111">方法</span><span class="sxs-lookup"><span data-stu-id="e4ac1-111">Method</span></span>           | <span data-ttu-id="e4ac1-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="e4ac1-112">Return Type</span></span>    |<span data-ttu-id="e4ac1-113">说明</span><span class="sxs-lookup"><span data-stu-id="e4ac1-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e4ac1-114">Add</span><span class="sxs-lookup"><span data-stu-id="e4ac1-114">Add</span></span>](../api/nameditem-add.md)|[<span data-ttu-id="e4ac1-115">WorkbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="e4ac1-115">WorkbookNamedItem</span></span>](nameditem.md)|<span data-ttu-id="e4ac1-116">将新名称添加到给定范围的集合。</span><span class="sxs-lookup"><span data-stu-id="e4ac1-116">Adds a new name to the collection of the given scope.</span></span>|
|[<span data-ttu-id="e4ac1-117">AddFormulaLocal</span><span class="sxs-lookup"><span data-stu-id="e4ac1-117">AddFormulaLocal</span></span>](../api/nameditem-addformulalocal.md)|[<span data-ttu-id="e4ac1-118">WorkbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="e4ac1-118">WorkbookNamedItem</span></span>](nameditem.md)|<span data-ttu-id="e4ac1-119">使用用户的公式区域设置，将新名称添加到给定范围的集合。</span><span class="sxs-lookup"><span data-stu-id="e4ac1-119">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>|
|[<span data-ttu-id="e4ac1-120">获取 NamedItem</span><span class="sxs-lookup"><span data-stu-id="e4ac1-120">Get NamedItem</span></span>](../api/nameditem-get.md) | [<span data-ttu-id="e4ac1-121">WorkbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="e4ac1-121">WorkbookNamedItem</span></span>](nameditem.md) |<span data-ttu-id="e4ac1-122">读取 nameditem 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e4ac1-122">Read properties and relationships of namedItem object.</span></span>|
|[<span data-ttu-id="e4ac1-123">更新</span><span class="sxs-lookup"><span data-stu-id="e4ac1-123">Update</span></span>](../api/nameditem-update.md) | [<span data-ttu-id="e4ac1-124">WorkbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="e4ac1-124">WorkbookNamedItem</span></span>](nameditem.md)   |<span data-ttu-id="e4ac1-125">更新 NamedItem 对象。</span><span class="sxs-lookup"><span data-stu-id="e4ac1-125">Update NamedItem object.</span></span> |
|[<span data-ttu-id="e4ac1-126">区域</span><span class="sxs-lookup"><span data-stu-id="e4ac1-126">Range</span></span>](../api/nameditem-range.md)|[<span data-ttu-id="e4ac1-127">区域</span><span class="sxs-lookup"><span data-stu-id="e4ac1-127">Range</span></span>](range.md)|<span data-ttu-id="e4ac1-p103">返回与名称相关的 range 对象。如果已命名项目的类型不是区域，将引发异常。</span><span class="sxs-lookup"><span data-stu-id="e4ac1-p103">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>|
|[<span data-ttu-id="e4ac1-130">列出</span><span class="sxs-lookup"><span data-stu-id="e4ac1-130">List</span></span>](../api/nameditem-list.md) | <span data-ttu-id="e4ac1-131">[WorkbookNamedItem](nameditem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e4ac1-131">[WorkbookNamedItem](nameditem.md) collection</span></span> |<span data-ttu-id="e4ac1-132">获取 namedItem 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e4ac1-132">Get namedItem object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="e4ac1-133">属性</span><span class="sxs-lookup"><span data-stu-id="e4ac1-133">Properties</span></span>
| <span data-ttu-id="e4ac1-134">属性</span><span class="sxs-lookup"><span data-stu-id="e4ac1-134">Property</span></span>     | <span data-ttu-id="e4ac1-135">类型</span><span class="sxs-lookup"><span data-stu-id="e4ac1-135">Type</span></span>   |<span data-ttu-id="e4ac1-136">说明</span><span class="sxs-lookup"><span data-stu-id="e4ac1-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4ac1-137">name</span><span class="sxs-lookup"><span data-stu-id="e4ac1-137">name</span></span>|<span data-ttu-id="e4ac1-138">字符串</span><span class="sxs-lookup"><span data-stu-id="e4ac1-138">string</span></span>|<span data-ttu-id="e4ac1-p104">对象的名称。只读。</span><span class="sxs-lookup"><span data-stu-id="e4ac1-p104">The name of the object. Read-only.</span></span>|
|<span data-ttu-id="e4ac1-141">comment</span><span class="sxs-lookup"><span data-stu-id="e4ac1-141">comment</span></span>|<span data-ttu-id="e4ac1-142">string</span><span class="sxs-lookup"><span data-stu-id="e4ac1-142">string</span></span>|<span data-ttu-id="e4ac1-143">表示与此名称相关联的注释。</span><span class="sxs-lookup"><span data-stu-id="e4ac1-143">Represents the comment associated with this name.</span></span>|
|<span data-ttu-id="e4ac1-144">scope</span><span class="sxs-lookup"><span data-stu-id="e4ac1-144">scope</span></span>|<span data-ttu-id="e4ac1-145">string</span><span class="sxs-lookup"><span data-stu-id="e4ac1-145">string</span></span>|<span data-ttu-id="e4ac1-p105">指明是否将 name 限定到工作簿或特定工作表。只读。</span><span class="sxs-lookup"><span data-stu-id="e4ac1-p105">Indicates whether the name is scoped to the workbook or to a specific worksheet. Read-only.</span></span>|
|<span data-ttu-id="e4ac1-148">类型</span><span class="sxs-lookup"><span data-stu-id="e4ac1-148">type</span></span>|<span data-ttu-id="e4ac1-149">字符串</span><span class="sxs-lookup"><span data-stu-id="e4ac1-149">string</span></span>|<span data-ttu-id="e4ac1-150">指示与名称相关的引用类型。</span><span class="sxs-lookup"><span data-stu-id="e4ac1-150">Indicates what type of reference is associated with the name.</span></span> <span data-ttu-id="e4ac1-151">可能的值包括 `String`、`Integer`、`Double`、`Boolean`、`Range`。</span><span class="sxs-lookup"><span data-stu-id="e4ac1-151">The possible values are: `String`, `Integer`, `Double`, `Boolean`, `Range`.</span></span> <span data-ttu-id="e4ac1-152">只读。</span><span class="sxs-lookup"><span data-stu-id="e4ac1-152">Read-only.</span></span>|
|<span data-ttu-id="e4ac1-153">value</span><span class="sxs-lookup"><span data-stu-id="e4ac1-153">value</span></span>|<span data-ttu-id="e4ac1-154">Json</span><span class="sxs-lookup"><span data-stu-id="e4ac1-154">Json</span></span>|<span data-ttu-id="e4ac1-p107">表示名称定义为引用的公式。例如 =Sheet14!$B$2:$H$12、=4.75 等。只读。</span><span class="sxs-lookup"><span data-stu-id="e4ac1-p107">Represents the formula that the name is defined to refer to. E.g. =Sheet14!$B$2:$H$12, =4.75, etc. Read-only.</span></span>|
|<span data-ttu-id="e4ac1-158">visible</span><span class="sxs-lookup"><span data-stu-id="e4ac1-158">visible</span></span>|<span data-ttu-id="e4ac1-159">布尔</span><span class="sxs-lookup"><span data-stu-id="e4ac1-159">boolean</span></span>|<span data-ttu-id="e4ac1-160">指定对象是否可见。</span><span class="sxs-lookup"><span data-stu-id="e4ac1-160">Specifies whether the object is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4ac1-161">关系</span><span class="sxs-lookup"><span data-stu-id="e4ac1-161">Relationships</span></span>
| <span data-ttu-id="e4ac1-162">关系</span><span class="sxs-lookup"><span data-stu-id="e4ac1-162">Relationship</span></span>     | <span data-ttu-id="e4ac1-163">类型</span><span class="sxs-lookup"><span data-stu-id="e4ac1-163">Type</span></span>   |<span data-ttu-id="e4ac1-164">说明</span><span class="sxs-lookup"><span data-stu-id="e4ac1-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4ac1-165">worksheet</span><span class="sxs-lookup"><span data-stu-id="e4ac1-165">worksheet</span></span>|[<span data-ttu-id="e4ac1-166">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="e4ac1-166">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="e4ac1-p108">返回已命名项限定到的工作表。仅在该项目的作用域为工作表时才可用。只读。</span><span class="sxs-lookup"><span data-stu-id="e4ac1-p108">Returns the worksheet on which the named item is scoped to. Available only if the item is scoped to the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e4ac1-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e4ac1-170">JSON representation</span></span>

<span data-ttu-id="e4ac1-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4ac1-171">Here is a JSON representation of the resource.</span></span>

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
