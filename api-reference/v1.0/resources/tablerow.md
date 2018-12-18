---
title: TableRow 资源类型
description: 表示表中的行。
author: lumine2008
ms.openlocfilehash: f34190aa4ac565d09ec8b07e96b2923f785b8d7c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341333"
---
# <a name="tablerow-resource-type"></a><span data-ttu-id="785a6-103">TableRow 资源类型</span><span class="sxs-lookup"><span data-stu-id="785a6-103">TableRow resource type</span></span>

<span data-ttu-id="785a6-104">表示表中的行。</span><span class="sxs-lookup"><span data-stu-id="785a6-104">Represents a row in a table.</span></span>


## <a name="methods"></a><span data-ttu-id="785a6-105">方法</span><span class="sxs-lookup"><span data-stu-id="785a6-105">Methods</span></span>

| <span data-ttu-id="785a6-106">方法</span><span class="sxs-lookup"><span data-stu-id="785a6-106">Method</span></span>           | <span data-ttu-id="785a6-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="785a6-107">Return Type</span></span>    |<span data-ttu-id="785a6-108">说明</span><span class="sxs-lookup"><span data-stu-id="785a6-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="785a6-109">获取 TableRow</span><span class="sxs-lookup"><span data-stu-id="785a6-109">Get TableRow</span></span>](../api/tablerow-get.md) | [<span data-ttu-id="785a6-110">WorkbookTableRow</span><span class="sxs-lookup"><span data-stu-id="785a6-110">WorkbookTableRow</span></span>](tablerow.md) |<span data-ttu-id="785a6-111">读取 tableRow 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="785a6-111">Read properties and relationships of tableRow object.</span></span>|
|[<span data-ttu-id="785a6-112">Update</span><span class="sxs-lookup"><span data-stu-id="785a6-112">Update</span></span>](../api/tablerow-update.md) | [<span data-ttu-id="785a6-113">WorkbookTableRow</span><span class="sxs-lookup"><span data-stu-id="785a6-113">WorkbookTableRow</span></span>](tablerow.md)  |<span data-ttu-id="785a6-114">更新 TableRow 对象。</span><span class="sxs-lookup"><span data-stu-id="785a6-114">Update TableRow object.</span></span> |
|[<span data-ttu-id="785a6-115">区域</span><span class="sxs-lookup"><span data-stu-id="785a6-115">Range</span></span>](../api/tablerow-range.md)|[<span data-ttu-id="785a6-116">Range</span><span class="sxs-lookup"><span data-stu-id="785a6-116">Range</span></span>](range.md)|<span data-ttu-id="785a6-117">返回与整个行相关联的范围对象。</span><span class="sxs-lookup"><span data-stu-id="785a6-117">Returns the range object associated with the entire row.</span></span>|
|[<span data-ttu-id="785a6-118">删除</span><span class="sxs-lookup"><span data-stu-id="785a6-118">Delete</span></span>](../api/tablerow-delete.md)|<span data-ttu-id="785a6-119">无</span><span class="sxs-lookup"><span data-stu-id="785a6-119">None</span></span>|<span data-ttu-id="785a6-120">从表中删除行。</span><span class="sxs-lookup"><span data-stu-id="785a6-120">Deletes the row from the table.</span></span>|
|[<span data-ttu-id="785a6-121">List</span><span class="sxs-lookup"><span data-stu-id="785a6-121">List</span></span>](../api/tablerow-list.md) | <span data-ttu-id="785a6-122">[WorkbookTableRow](tablerow.md)集合</span><span class="sxs-lookup"><span data-stu-id="785a6-122">[WorkbookTableRow](tablerow.md) collection</span></span> |<span data-ttu-id="785a6-123">获取 tableRow 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="785a6-123">Get tableRow object collection.</span></span> |
|[<span data-ttu-id="785a6-124">Itemat</span><span class="sxs-lookup"><span data-stu-id="785a6-124">Itemat</span></span>](../api/tablerowcollection-itemat.md)|[<span data-ttu-id="785a6-125">WorkbookTableRow</span><span class="sxs-lookup"><span data-stu-id="785a6-125">WorkbookTableRow</span></span>](tablerow.md)|<span data-ttu-id="785a6-126">根据其在集合中的位置获取行。</span><span class="sxs-lookup"><span data-stu-id="785a6-126">Gets a row based on its position in the collection.</span></span>|
|[<span data-ttu-id="785a6-127">Add</span><span class="sxs-lookup"><span data-stu-id="785a6-127">Add</span></span>](../api/tablerowcollection-add.md)|[<span data-ttu-id="785a6-128">WorkbookTableRow</span><span class="sxs-lookup"><span data-stu-id="785a6-128">WorkbookTableRow</span></span>](tablerow.md)|<span data-ttu-id="785a6-129">向表中添加新行。</span><span class="sxs-lookup"><span data-stu-id="785a6-129">Adds a new row to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="785a6-130">属性</span><span class="sxs-lookup"><span data-stu-id="785a6-130">Properties</span></span>
| <span data-ttu-id="785a6-131">属性</span><span class="sxs-lookup"><span data-stu-id="785a6-131">Property</span></span>     | <span data-ttu-id="785a6-132">类型</span><span class="sxs-lookup"><span data-stu-id="785a6-132">Type</span></span>   |<span data-ttu-id="785a6-133">说明</span><span class="sxs-lookup"><span data-stu-id="785a6-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="785a6-134">index</span><span class="sxs-lookup"><span data-stu-id="785a6-134">index</span></span>|<span data-ttu-id="785a6-135">整数</span><span class="sxs-lookup"><span data-stu-id="785a6-135">int</span></span>|<span data-ttu-id="785a6-p101">返回表的行集合内行的索引编号。从零开始编制索引。只读。</span><span class="sxs-lookup"><span data-stu-id="785a6-p101">Returns the index number of the row within the rows collection of the table. Zero-indexed. Read-only.</span></span>|
|<span data-ttu-id="785a6-139">values</span><span class="sxs-lookup"><span data-stu-id="785a6-139">values</span></span>|<span data-ttu-id="785a6-140">Json</span><span class="sxs-lookup"><span data-stu-id="785a6-140">Json</span></span>|<span data-ttu-id="785a6-p102">表示指定区域的原始值。返回的数据类型可能是字符串、数字或布尔值。包含一个将返回错误字符串的错误的单元格。</span><span class="sxs-lookup"><span data-stu-id="785a6-p102">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="relationships"></a><span data-ttu-id="785a6-144">Relationships</span><span class="sxs-lookup"><span data-stu-id="785a6-144">Relationships</span></span>
<span data-ttu-id="785a6-145">无</span><span class="sxs-lookup"><span data-stu-id="785a6-145">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="785a6-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="785a6-146">JSON representation</span></span>

<span data-ttu-id="785a6-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="785a6-147">Here is a JSON representation of the resource.</span></span>

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