---
title: workbookTableRow 资源类型
description: 表示表中的行。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ba7b481f4b20033e1a4ffcd42ac92421bc3536a4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519118"
---
# <a name="workbooktablerow-resource-type"></a><span data-ttu-id="033d9-103">workbookTableRow 资源类型</span><span class="sxs-lookup"><span data-stu-id="033d9-103">workbookTableRow resource type</span></span>

<span data-ttu-id="033d9-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="033d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="033d9-105">表示表中的行。</span><span class="sxs-lookup"><span data-stu-id="033d9-105">Represents a row in a table.</span></span>


## <a name="methods"></a><span data-ttu-id="033d9-106">方法</span><span class="sxs-lookup"><span data-stu-id="033d9-106">Methods</span></span>

| <span data-ttu-id="033d9-107">方法</span><span class="sxs-lookup"><span data-stu-id="033d9-107">Method</span></span>           | <span data-ttu-id="033d9-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="033d9-108">Return Type</span></span>    |<span data-ttu-id="033d9-109">说明</span><span class="sxs-lookup"><span data-stu-id="033d9-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="033d9-110">获取 TableRow</span><span class="sxs-lookup"><span data-stu-id="033d9-110">Get TableRow</span></span>](../api/tablerow-get.md) | [<span data-ttu-id="033d9-111">workbookTableRow</span><span class="sxs-lookup"><span data-stu-id="033d9-111">workbookTableRow</span></span>](workbooktablerow.md) |<span data-ttu-id="033d9-112">读取 tableRow 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="033d9-112">Read properties and relationships of tableRow object.</span></span>|
|[<span data-ttu-id="033d9-113">更新</span><span class="sxs-lookup"><span data-stu-id="033d9-113">Update</span></span>](../api/tablerow-update.md) | [<span data-ttu-id="033d9-114">workbookTableRow</span><span class="sxs-lookup"><span data-stu-id="033d9-114">workbookTableRow</span></span>](workbooktablerow.md)  |<span data-ttu-id="033d9-115">更新 TableRow 对象。</span><span class="sxs-lookup"><span data-stu-id="033d9-115">Update TableRow object.</span></span> |
|[<span data-ttu-id="033d9-116">Range</span><span class="sxs-lookup"><span data-stu-id="033d9-116">Range</span></span>](../api/tablerow-range.md)|[<span data-ttu-id="033d9-117">workbookRange</span><span class="sxs-lookup"><span data-stu-id="033d9-117">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="033d9-118">返回与整个行相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="033d9-118">Returns the range object associated with the entire row.</span></span>|
|[<span data-ttu-id="033d9-119">删除</span><span class="sxs-lookup"><span data-stu-id="033d9-119">Delete</span></span>](../api/tablerow-delete.md)|<span data-ttu-id="033d9-120">无</span><span class="sxs-lookup"><span data-stu-id="033d9-120">None</span></span>|<span data-ttu-id="033d9-121">从表中删除行。</span><span class="sxs-lookup"><span data-stu-id="033d9-121">Deletes the row from the table.</span></span>|
|[<span data-ttu-id="033d9-122">列出</span><span class="sxs-lookup"><span data-stu-id="033d9-122">List</span></span>](../api/tablerow-list.md) | <span data-ttu-id="033d9-123">[workbookTableRow](workbooktablerow.md)集合</span><span class="sxs-lookup"><span data-stu-id="033d9-123">[workbookTableRow](workbooktablerow.md) collection</span></span> |<span data-ttu-id="033d9-124">获取 tableRow 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="033d9-124">Get tableRow object collection.</span></span> |
|[<span data-ttu-id="033d9-125">Itemat</span><span class="sxs-lookup"><span data-stu-id="033d9-125">Itemat</span></span>](../api/tablerowcollection-itemat.md)|[<span data-ttu-id="033d9-126">workbookTableRow</span><span class="sxs-lookup"><span data-stu-id="033d9-126">workbookTableRow</span></span>](workbooktablerow.md)|<span data-ttu-id="033d9-127">根据其在集合中的位置获取行。</span><span class="sxs-lookup"><span data-stu-id="033d9-127">Gets a row based on its position in the collection.</span></span>|
|[<span data-ttu-id="033d9-128">添加</span><span class="sxs-lookup"><span data-stu-id="033d9-128">Add</span></span>](../api/tablerowcollection-add.md)|[<span data-ttu-id="033d9-129">workbookTableRow</span><span class="sxs-lookup"><span data-stu-id="033d9-129">workbookTableRow</span></span>](workbooktablerow.md)|<span data-ttu-id="033d9-130">向表中添加新行。</span><span class="sxs-lookup"><span data-stu-id="033d9-130">Adds a new row to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="033d9-131">属性</span><span class="sxs-lookup"><span data-stu-id="033d9-131">Properties</span></span>
| <span data-ttu-id="033d9-132">属性</span><span class="sxs-lookup"><span data-stu-id="033d9-132">Property</span></span>     | <span data-ttu-id="033d9-133">类型</span><span class="sxs-lookup"><span data-stu-id="033d9-133">Type</span></span>   |<span data-ttu-id="033d9-134">说明</span><span class="sxs-lookup"><span data-stu-id="033d9-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="033d9-135">index</span><span class="sxs-lookup"><span data-stu-id="033d9-135">index</span></span>|<span data-ttu-id="033d9-136">int</span><span class="sxs-lookup"><span data-stu-id="033d9-136">int</span></span>|<span data-ttu-id="033d9-p101">返回表的行集合内行的索引编号。从零开始编制索引。只读。</span><span class="sxs-lookup"><span data-stu-id="033d9-p101">Returns the index number of the row within the rows collection of the table. Zero-indexed. Read-only.</span></span>|
|<span data-ttu-id="033d9-140">values</span><span class="sxs-lookup"><span data-stu-id="033d9-140">values</span></span>|<span data-ttu-id="033d9-141">Json</span><span class="sxs-lookup"><span data-stu-id="033d9-141">Json</span></span>|<span data-ttu-id="033d9-p102">表示指定区域的原始值。返回的数据类型可能是字符串、数字或布尔值。包含一个将返回错误字符串的错误的单元格。</span><span class="sxs-lookup"><span data-stu-id="033d9-p102">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="relationships"></a><span data-ttu-id="033d9-145">关系</span><span class="sxs-lookup"><span data-stu-id="033d9-145">Relationships</span></span>
<span data-ttu-id="033d9-146">无</span><span class="sxs-lookup"><span data-stu-id="033d9-146">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="033d9-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="033d9-147">JSON representation</span></span>

<span data-ttu-id="033d9-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="033d9-148">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "TableRow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
