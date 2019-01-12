---
title: TableRow 资源类型
description: 表示表中的行。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c266476715da36bcdc0b621538722ba6320eba85
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937507"
---
# <a name="tablerow-resource-type"></a><span data-ttu-id="30e95-103">TableRow 资源类型</span><span class="sxs-lookup"><span data-stu-id="30e95-103">TableRow resource type</span></span>

<span data-ttu-id="30e95-104">表示表中的行。</span><span class="sxs-lookup"><span data-stu-id="30e95-104">Represents a row in a table.</span></span>


## <a name="methods"></a><span data-ttu-id="30e95-105">方法</span><span class="sxs-lookup"><span data-stu-id="30e95-105">Methods</span></span>

| <span data-ttu-id="30e95-106">方法</span><span class="sxs-lookup"><span data-stu-id="30e95-106">Method</span></span>           | <span data-ttu-id="30e95-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="30e95-107">Return Type</span></span>    |<span data-ttu-id="30e95-108">说明</span><span class="sxs-lookup"><span data-stu-id="30e95-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="30e95-109">获取 TableRow</span><span class="sxs-lookup"><span data-stu-id="30e95-109">Get TableRow</span></span>](../api/tablerow-get.md) | [<span data-ttu-id="30e95-110">WorkbookTableRow</span><span class="sxs-lookup"><span data-stu-id="30e95-110">WorkbookTableRow</span></span>](tablerow.md) |<span data-ttu-id="30e95-111">读取 tableRow 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="30e95-111">Read properties and relationships of tableRow object.</span></span>|
|[<span data-ttu-id="30e95-112">Update</span><span class="sxs-lookup"><span data-stu-id="30e95-112">Update</span></span>](../api/tablerow-update.md) | [<span data-ttu-id="30e95-113">WorkbookTableRow</span><span class="sxs-lookup"><span data-stu-id="30e95-113">WorkbookTableRow</span></span>](tablerow.md)  |<span data-ttu-id="30e95-114">更新 TableRow 对象。</span><span class="sxs-lookup"><span data-stu-id="30e95-114">Update TableRow object.</span></span> |
|[<span data-ttu-id="30e95-115">区域</span><span class="sxs-lookup"><span data-stu-id="30e95-115">Range</span></span>](../api/tablerow-range.md)|[<span data-ttu-id="30e95-116">Range</span><span class="sxs-lookup"><span data-stu-id="30e95-116">Range</span></span>](range.md)|<span data-ttu-id="30e95-117">返回与整个行相关联的范围对象。</span><span class="sxs-lookup"><span data-stu-id="30e95-117">Returns the range object associated with the entire row.</span></span>|
|[<span data-ttu-id="30e95-118">删除</span><span class="sxs-lookup"><span data-stu-id="30e95-118">Delete</span></span>](../api/tablerow-delete.md)|<span data-ttu-id="30e95-119">无</span><span class="sxs-lookup"><span data-stu-id="30e95-119">None</span></span>|<span data-ttu-id="30e95-120">从表中删除行。</span><span class="sxs-lookup"><span data-stu-id="30e95-120">Deletes the row from the table.</span></span>|
|[<span data-ttu-id="30e95-121">List</span><span class="sxs-lookup"><span data-stu-id="30e95-121">List</span></span>](../api/tablerow-list.md) | <span data-ttu-id="30e95-122">[WorkbookTableRow](tablerow.md)集合</span><span class="sxs-lookup"><span data-stu-id="30e95-122">[WorkbookTableRow](tablerow.md) collection</span></span> |<span data-ttu-id="30e95-123">获取 tableRow 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="30e95-123">Get tableRow object collection.</span></span> |
|[<span data-ttu-id="30e95-124">Itemat</span><span class="sxs-lookup"><span data-stu-id="30e95-124">Itemat</span></span>](../api/tablerowcollection-itemat.md)|[<span data-ttu-id="30e95-125">WorkbookTableRow</span><span class="sxs-lookup"><span data-stu-id="30e95-125">WorkbookTableRow</span></span>](tablerow.md)|<span data-ttu-id="30e95-126">根据其在集合中的位置获取行。</span><span class="sxs-lookup"><span data-stu-id="30e95-126">Gets a row based on its position in the collection.</span></span>|
|[<span data-ttu-id="30e95-127">Add</span><span class="sxs-lookup"><span data-stu-id="30e95-127">Add</span></span>](../api/tablerowcollection-add.md)|[<span data-ttu-id="30e95-128">WorkbookTableRow</span><span class="sxs-lookup"><span data-stu-id="30e95-128">WorkbookTableRow</span></span>](tablerow.md)|<span data-ttu-id="30e95-129">向表中添加新行。</span><span class="sxs-lookup"><span data-stu-id="30e95-129">Adds a new row to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="30e95-130">属性</span><span class="sxs-lookup"><span data-stu-id="30e95-130">Properties</span></span>
| <span data-ttu-id="30e95-131">属性</span><span class="sxs-lookup"><span data-stu-id="30e95-131">Property</span></span>     | <span data-ttu-id="30e95-132">类型</span><span class="sxs-lookup"><span data-stu-id="30e95-132">Type</span></span>   |<span data-ttu-id="30e95-133">说明</span><span class="sxs-lookup"><span data-stu-id="30e95-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30e95-134">index</span><span class="sxs-lookup"><span data-stu-id="30e95-134">index</span></span>|<span data-ttu-id="30e95-135">int</span><span class="sxs-lookup"><span data-stu-id="30e95-135">int</span></span>|<span data-ttu-id="30e95-p101">返回表的行集合内行的索引编号。从零开始编制索引。只读。</span><span class="sxs-lookup"><span data-stu-id="30e95-p101">Returns the index number of the row within the rows collection of the table. Zero-indexed. Read-only.</span></span>|
|<span data-ttu-id="30e95-139">values</span><span class="sxs-lookup"><span data-stu-id="30e95-139">values</span></span>|<span data-ttu-id="30e95-140">Json</span><span class="sxs-lookup"><span data-stu-id="30e95-140">Json</span></span>|<span data-ttu-id="30e95-p102">表示指定区域的原始值。返回的数据类型可能是字符串、数字或布尔值。包含一个将返回错误字符串的错误的单元格。</span><span class="sxs-lookup"><span data-stu-id="30e95-p102">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="relationships"></a><span data-ttu-id="30e95-144">Relationships</span><span class="sxs-lookup"><span data-stu-id="30e95-144">Relationships</span></span>
<span data-ttu-id="30e95-145">无</span><span class="sxs-lookup"><span data-stu-id="30e95-145">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="30e95-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="30e95-146">JSON representation</span></span>

<span data-ttu-id="30e95-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="30e95-147">Here is a JSON representation of the resource.</span></span>

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
