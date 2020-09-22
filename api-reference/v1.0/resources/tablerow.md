---
title: TableRow 资源类型
description: 表示表中的行。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 3eca83aeea75300ed9165ac822b15212c866f152
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094090"
---
# <a name="tablerow-resource-type"></a><span data-ttu-id="82217-103">TableRow 资源类型</span><span class="sxs-lookup"><span data-stu-id="82217-103">TableRow resource type</span></span>

<span data-ttu-id="82217-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82217-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="82217-105">表示表中的行。</span><span class="sxs-lookup"><span data-stu-id="82217-105">Represents a row in a table.</span></span>


## <a name="methods"></a><span data-ttu-id="82217-106">方法</span><span class="sxs-lookup"><span data-stu-id="82217-106">Methods</span></span>

| <span data-ttu-id="82217-107">方法</span><span class="sxs-lookup"><span data-stu-id="82217-107">Method</span></span>           | <span data-ttu-id="82217-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="82217-108">Return Type</span></span>    |<span data-ttu-id="82217-109">说明</span><span class="sxs-lookup"><span data-stu-id="82217-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="82217-110">获取 TableRow</span><span class="sxs-lookup"><span data-stu-id="82217-110">Get TableRow</span></span>](../api/tablerow-get.md) | [<span data-ttu-id="82217-111">WorkbookTableRow</span><span class="sxs-lookup"><span data-stu-id="82217-111">WorkbookTableRow</span></span>](tablerow.md) |<span data-ttu-id="82217-112">读取 tableRow 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="82217-112">Read properties and relationships of tableRow object.</span></span>|
|[<span data-ttu-id="82217-113">更新</span><span class="sxs-lookup"><span data-stu-id="82217-113">Update</span></span>](../api/tablerow-update.md) | [<span data-ttu-id="82217-114">WorkbookTableRow</span><span class="sxs-lookup"><span data-stu-id="82217-114">WorkbookTableRow</span></span>](tablerow.md)  |<span data-ttu-id="82217-115">更新 TableRow 对象。</span><span class="sxs-lookup"><span data-stu-id="82217-115">Update TableRow object.</span></span> |
|[<span data-ttu-id="82217-116">区域</span><span class="sxs-lookup"><span data-stu-id="82217-116">Range</span></span>](../api/tablerow-range.md)|[<span data-ttu-id="82217-117">区域</span><span class="sxs-lookup"><span data-stu-id="82217-117">Range</span></span>](range.md)|<span data-ttu-id="82217-118">返回与整个行相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="82217-118">Returns the range object associated with the entire row.</span></span>|
|[<span data-ttu-id="82217-119">删除</span><span class="sxs-lookup"><span data-stu-id="82217-119">Delete</span></span>](../api/tablerow-delete.md)|<span data-ttu-id="82217-120">无</span><span class="sxs-lookup"><span data-stu-id="82217-120">None</span></span>|<span data-ttu-id="82217-121">从表中删除行。</span><span class="sxs-lookup"><span data-stu-id="82217-121">Deletes the row from the table.</span></span>|
|[<span data-ttu-id="82217-122">列出</span><span class="sxs-lookup"><span data-stu-id="82217-122">List</span></span>](../api/tablerow-list.md) | <span data-ttu-id="82217-123">[WorkbookTableRow](tablerow.md) 集合</span><span class="sxs-lookup"><span data-stu-id="82217-123">[WorkbookTableRow](tablerow.md) collection</span></span> |<span data-ttu-id="82217-124">获取 tableRow 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="82217-124">Get tableRow object collection.</span></span> |
|[<span data-ttu-id="82217-125">Itemat</span><span class="sxs-lookup"><span data-stu-id="82217-125">Itemat</span></span>](../api/tablerowcollection-itemat.md)|[<span data-ttu-id="82217-126">WorkbookTableRow</span><span class="sxs-lookup"><span data-stu-id="82217-126">WorkbookTableRow</span></span>](tablerow.md)|<span data-ttu-id="82217-127">根据其在集合中的位置获取行。</span><span class="sxs-lookup"><span data-stu-id="82217-127">Gets a row based on its position in the collection.</span></span>|
|[<span data-ttu-id="82217-128">添加</span><span class="sxs-lookup"><span data-stu-id="82217-128">Add</span></span>](../api/tablerowcollection-add.md)|[<span data-ttu-id="82217-129">WorkbookTableRow</span><span class="sxs-lookup"><span data-stu-id="82217-129">WorkbookTableRow</span></span>](tablerow.md)|<span data-ttu-id="82217-130">向表中添加新行。</span><span class="sxs-lookup"><span data-stu-id="82217-130">Adds a new row to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="82217-131">属性</span><span class="sxs-lookup"><span data-stu-id="82217-131">Properties</span></span>
| <span data-ttu-id="82217-132">属性</span><span class="sxs-lookup"><span data-stu-id="82217-132">Property</span></span>     | <span data-ttu-id="82217-133">类型</span><span class="sxs-lookup"><span data-stu-id="82217-133">Type</span></span>   |<span data-ttu-id="82217-134">说明</span><span class="sxs-lookup"><span data-stu-id="82217-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82217-135">index</span><span class="sxs-lookup"><span data-stu-id="82217-135">index</span></span>|<span data-ttu-id="82217-136">int</span><span class="sxs-lookup"><span data-stu-id="82217-136">int</span></span>|<span data-ttu-id="82217-p101">返回表的行集合内行的索引编号。从零开始编制索引。只读。</span><span class="sxs-lookup"><span data-stu-id="82217-p101">Returns the index number of the row within the rows collection of the table. Zero-indexed. Read-only.</span></span>|
|<span data-ttu-id="82217-140">values</span><span class="sxs-lookup"><span data-stu-id="82217-140">values</span></span>|<span data-ttu-id="82217-141">Json</span><span class="sxs-lookup"><span data-stu-id="82217-141">Json</span></span>|<span data-ttu-id="82217-p102">表示指定区域的原始值。返回的数据类型可能是字符串、数字或布尔值。包含一个将返回错误字符串的错误的单元格。</span><span class="sxs-lookup"><span data-stu-id="82217-p102">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="relationships"></a><span data-ttu-id="82217-145">关系</span><span class="sxs-lookup"><span data-stu-id="82217-145">Relationships</span></span>
<span data-ttu-id="82217-146">无</span><span class="sxs-lookup"><span data-stu-id="82217-146">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="82217-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="82217-147">JSON representation</span></span>

<span data-ttu-id="82217-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82217-148">Here is a JSON representation of the resource.</span></span>

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

