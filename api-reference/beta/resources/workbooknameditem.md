---
title: workbookNamedItem 资源类型
description: 表示单元格区域或值的定义名称。名称可以为基元的已命名对象（如以下类型中所示）、range 对象或对区域的引用。此对象可用于获取与名称相关的 range 对象。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: ''
ms.openlocfilehash: 17b9e7a04a2524febcb949829b626bc6efe6b779
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519209"
---
# <a name="workbooknameditem-resource-type"></a><span data-ttu-id="fdb70-105">workbookNamedItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="fdb70-105">workbookNamedItem resource type</span></span>

<span data-ttu-id="fdb70-106">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="fdb70-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdb70-p102">表示单元格区域或值的定义名称。名称可以为基元的已命名对象（如以下类型中所示）、range 对象或对区域的引用。此对象可用于获取与名称相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="fdb70-p102">Represents a defined name for a range of cells or value. Names can be primitive named objects (as seen in the type below), range object, reference to a range. This object can be used to obtain range object associated with names.</span></span>


## <a name="methods"></a><span data-ttu-id="fdb70-110">方法</span><span class="sxs-lookup"><span data-stu-id="fdb70-110">Methods</span></span>

| <span data-ttu-id="fdb70-111">方法</span><span class="sxs-lookup"><span data-stu-id="fdb70-111">Method</span></span>           | <span data-ttu-id="fdb70-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="fdb70-112">Return Type</span></span>    |<span data-ttu-id="fdb70-113">说明</span><span class="sxs-lookup"><span data-stu-id="fdb70-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fdb70-114">Add</span><span class="sxs-lookup"><span data-stu-id="fdb70-114">Add</span></span>](../api/nameditem-add.md)|[<span data-ttu-id="fdb70-115">workbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="fdb70-115">workbookNamedItem</span></span>](workbooknameditem.md)|<span data-ttu-id="fdb70-116">将新名称添加到给定范围的集合。</span><span class="sxs-lookup"><span data-stu-id="fdb70-116">Adds a new name to the collection of the given scope.</span></span>|
|[<span data-ttu-id="fdb70-117">AddFormulaLocal</span><span class="sxs-lookup"><span data-stu-id="fdb70-117">AddFormulaLocal</span></span>](../api/nameditem-addformulalocal.md)|[<span data-ttu-id="fdb70-118">workbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="fdb70-118">workbookNamedItem</span></span>](workbooknameditem.md)|<span data-ttu-id="fdb70-119">使用用户的公式区域设置，将新名称添加到给定范围的集合。</span><span class="sxs-lookup"><span data-stu-id="fdb70-119">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>|
|[<span data-ttu-id="fdb70-120">获取 NamedItem</span><span class="sxs-lookup"><span data-stu-id="fdb70-120">Get NamedItem</span></span>](../api/nameditem-get.md) | [<span data-ttu-id="fdb70-121">workbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="fdb70-121">workbookNamedItem</span></span>](workbooknameditem.md) |<span data-ttu-id="fdb70-122">读取 nameditem 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fdb70-122">Read properties and relationships of namedItem object.</span></span>|
|[<span data-ttu-id="fdb70-123">更新</span><span class="sxs-lookup"><span data-stu-id="fdb70-123">Update</span></span>](../api/nameditem-update.md) | [<span data-ttu-id="fdb70-124">workbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="fdb70-124">workbookNamedItem</span></span>](workbooknameditem.md)   |<span data-ttu-id="fdb70-125">更新 NamedItem 对象。</span><span class="sxs-lookup"><span data-stu-id="fdb70-125">Update NamedItem object.</span></span> |
|[<span data-ttu-id="fdb70-126">Range</span><span class="sxs-lookup"><span data-stu-id="fdb70-126">Range</span></span>](../api/nameditem-range.md)|[<span data-ttu-id="fdb70-127">workbookRange</span><span class="sxs-lookup"><span data-stu-id="fdb70-127">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="fdb70-p103">返回与名称相关的 range 对象。如果已命名项目的类型不是区域，将引发异常。</span><span class="sxs-lookup"><span data-stu-id="fdb70-p103">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>|
|[<span data-ttu-id="fdb70-130">列出</span><span class="sxs-lookup"><span data-stu-id="fdb70-130">List</span></span>](../api/nameditem-list.md) | <span data-ttu-id="fdb70-131">[workbookNamedItem](workbooknameditem.md)集合</span><span class="sxs-lookup"><span data-stu-id="fdb70-131">[workbookNamedItem](workbooknameditem.md) collection</span></span> |<span data-ttu-id="fdb70-132">获取 namedItem 对象集合。</span><span class="sxs-lookup"><span data-stu-id="fdb70-132">Get namedItem object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="fdb70-133">属性</span><span class="sxs-lookup"><span data-stu-id="fdb70-133">Properties</span></span>
| <span data-ttu-id="fdb70-134">属性</span><span class="sxs-lookup"><span data-stu-id="fdb70-134">Property</span></span>     | <span data-ttu-id="fdb70-135">类型</span><span class="sxs-lookup"><span data-stu-id="fdb70-135">Type</span></span>   |<span data-ttu-id="fdb70-136">说明</span><span class="sxs-lookup"><span data-stu-id="fdb70-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fdb70-137">name</span><span class="sxs-lookup"><span data-stu-id="fdb70-137">name</span></span>|<span data-ttu-id="fdb70-138">string</span><span class="sxs-lookup"><span data-stu-id="fdb70-138">string</span></span>|<span data-ttu-id="fdb70-p104">对象的名称。只读。</span><span class="sxs-lookup"><span data-stu-id="fdb70-p104">The name of the object. Read-only.</span></span>|
|<span data-ttu-id="fdb70-141">comment</span><span class="sxs-lookup"><span data-stu-id="fdb70-141">comment</span></span>|<span data-ttu-id="fdb70-142">string</span><span class="sxs-lookup"><span data-stu-id="fdb70-142">string</span></span>|<span data-ttu-id="fdb70-143">表示与此名称相关联的注释。</span><span class="sxs-lookup"><span data-stu-id="fdb70-143">Represents the comment associated with this name.</span></span>|
|<span data-ttu-id="fdb70-144">scope</span><span class="sxs-lookup"><span data-stu-id="fdb70-144">scope</span></span>|<span data-ttu-id="fdb70-145">string</span><span class="sxs-lookup"><span data-stu-id="fdb70-145">string</span></span>|<span data-ttu-id="fdb70-p105">指明是否将 name 限定到工作簿或特定工作表。只读。</span><span class="sxs-lookup"><span data-stu-id="fdb70-p105">Indicates whether the name is scoped to the workbook or to a specific worksheet. Read-only.</span></span>|
|<span data-ttu-id="fdb70-148">类型</span><span class="sxs-lookup"><span data-stu-id="fdb70-148">type</span></span>|<span data-ttu-id="fdb70-149">字符串</span><span class="sxs-lookup"><span data-stu-id="fdb70-149">string</span></span>|<span data-ttu-id="fdb70-p106">指示与名称相关的引用类型。可能的值是：`String`、`Integer`、`Double`、`Boolean`、`Range`。只读。</span><span class="sxs-lookup"><span data-stu-id="fdb70-p106">Indicates what type of reference is associated with the name. Possible values are: `String`, `Integer`, `Double`, `Boolean`, `Range`. Read-only.</span></span>|
|<span data-ttu-id="fdb70-153">value</span><span class="sxs-lookup"><span data-stu-id="fdb70-153">value</span></span>|<span data-ttu-id="fdb70-154">string</span><span class="sxs-lookup"><span data-stu-id="fdb70-154">string</span></span>|<span data-ttu-id="fdb70-p107">表示名称定义为引用的公式。例如 =Sheet14!$B$2:$H$12、=4.75 等。只读。</span><span class="sxs-lookup"><span data-stu-id="fdb70-p107">Represents the formula that the name is defined to refer to. E.g. =Sheet14!$B$2:$H$12, =4.75, etc. Read-only.</span></span>|
|<span data-ttu-id="fdb70-158">visible</span><span class="sxs-lookup"><span data-stu-id="fdb70-158">visible</span></span>|<span data-ttu-id="fdb70-159">布尔</span><span class="sxs-lookup"><span data-stu-id="fdb70-159">boolean</span></span>|<span data-ttu-id="fdb70-160">指定对象是否可见。</span><span class="sxs-lookup"><span data-stu-id="fdb70-160">Specifies whether the object is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fdb70-161">关系</span><span class="sxs-lookup"><span data-stu-id="fdb70-161">Relationships</span></span>
| <span data-ttu-id="fdb70-162">关系</span><span class="sxs-lookup"><span data-stu-id="fdb70-162">Relationship</span></span>     | <span data-ttu-id="fdb70-163">类型</span><span class="sxs-lookup"><span data-stu-id="fdb70-163">Type</span></span>   |<span data-ttu-id="fdb70-164">说明</span><span class="sxs-lookup"><span data-stu-id="fdb70-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fdb70-165">worksheet</span><span class="sxs-lookup"><span data-stu-id="fdb70-165">worksheet</span></span>|[<span data-ttu-id="fdb70-166">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="fdb70-166">workbookWorksheet</span></span>](workbookworksheet.md)|<span data-ttu-id="fdb70-p108">返回已命名项限定到的工作表。仅在该项目的作用域为工作表时才可用。只读。</span><span class="sxs-lookup"><span data-stu-id="fdb70-p108">Returns the worksheet on which the named item is scoped to. Available only if the item is scoped to the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fdb70-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fdb70-170">JSON representation</span></span>

<span data-ttu-id="fdb70-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fdb70-171">Here is a JSON representation of the resource.</span></span>

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
