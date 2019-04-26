---
title: TableRow 资源类型
description: 表示表中的行。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c266476715da36bcdc0b621538722ba6320eba85
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563754"
---
# <a name="tablerow-resource-type"></a><span data-ttu-id="3ec2c-103">TableRow 资源类型</span><span class="sxs-lookup"><span data-stu-id="3ec2c-103">TableRow resource type</span></span>

<span data-ttu-id="3ec2c-104">表示表中的行。</span><span class="sxs-lookup"><span data-stu-id="3ec2c-104">Represents a row in a table.</span></span>


## <a name="methods"></a><span data-ttu-id="3ec2c-105">方法</span><span class="sxs-lookup"><span data-stu-id="3ec2c-105">Methods</span></span>

| <span data-ttu-id="3ec2c-106">方法</span><span class="sxs-lookup"><span data-stu-id="3ec2c-106">Method</span></span>           | <span data-ttu-id="3ec2c-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="3ec2c-107">Return Type</span></span>    |<span data-ttu-id="3ec2c-108">说明</span><span class="sxs-lookup"><span data-stu-id="3ec2c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3ec2c-109">获取 TableRow</span><span class="sxs-lookup"><span data-stu-id="3ec2c-109">Get TableRow</span></span>](../api/tablerow-get.md) | [<span data-ttu-id="3ec2c-110">WorkbookTableRow</span><span class="sxs-lookup"><span data-stu-id="3ec2c-110">WorkbookTableRow</span></span>](tablerow.md) |<span data-ttu-id="3ec2c-111">读取 tableRow 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3ec2c-111">Read properties and relationships of tableRow object.</span></span>|
|[<span data-ttu-id="3ec2c-112">更新</span><span class="sxs-lookup"><span data-stu-id="3ec2c-112">Update</span></span>](../api/tablerow-update.md) | [<span data-ttu-id="3ec2c-113">WorkbookTableRow</span><span class="sxs-lookup"><span data-stu-id="3ec2c-113">WorkbookTableRow</span></span>](tablerow.md)  |<span data-ttu-id="3ec2c-114">更新 TableRow 对象。</span><span class="sxs-lookup"><span data-stu-id="3ec2c-114">Update TableRow object.</span></span> |
|[<span data-ttu-id="3ec2c-115">区域</span><span class="sxs-lookup"><span data-stu-id="3ec2c-115">Range</span></span>](../api/tablerow-range.md)|[<span data-ttu-id="3ec2c-116">Range</span><span class="sxs-lookup"><span data-stu-id="3ec2c-116">Range</span></span>](range.md)|<span data-ttu-id="3ec2c-117">返回与整个行相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="3ec2c-117">Returns the range object associated with the entire row.</span></span>|
|[<span data-ttu-id="3ec2c-118">删除</span><span class="sxs-lookup"><span data-stu-id="3ec2c-118">Delete</span></span>](../api/tablerow-delete.md)|<span data-ttu-id="3ec2c-119">无</span><span class="sxs-lookup"><span data-stu-id="3ec2c-119">None</span></span>|<span data-ttu-id="3ec2c-120">从表中删除行。</span><span class="sxs-lookup"><span data-stu-id="3ec2c-120">Deletes the row from the table.</span></span>|
|[<span data-ttu-id="3ec2c-121">列出</span><span class="sxs-lookup"><span data-stu-id="3ec2c-121">List</span></span>](../api/tablerow-list.md) | <span data-ttu-id="3ec2c-122">[WorkbookTableRow](tablerow.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3ec2c-122">[WorkbookTableRow](tablerow.md) collection</span></span> |<span data-ttu-id="3ec2c-123">获取 tableRow 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="3ec2c-123">Get tableRow object collection.</span></span> |
|[<span data-ttu-id="3ec2c-124">Itemat</span><span class="sxs-lookup"><span data-stu-id="3ec2c-124">Itemat</span></span>](../api/tablerowcollection-itemat.md)|[<span data-ttu-id="3ec2c-125">WorkbookTableRow</span><span class="sxs-lookup"><span data-stu-id="3ec2c-125">WorkbookTableRow</span></span>](tablerow.md)|<span data-ttu-id="3ec2c-126">根据其在集合中的位置获取行。</span><span class="sxs-lookup"><span data-stu-id="3ec2c-126">Gets a row based on its position in the collection.</span></span>|
|[<span data-ttu-id="3ec2c-127">添加</span><span class="sxs-lookup"><span data-stu-id="3ec2c-127">Add</span></span>](../api/tablerowcollection-add.md)|[<span data-ttu-id="3ec2c-128">WorkbookTableRow</span><span class="sxs-lookup"><span data-stu-id="3ec2c-128">WorkbookTableRow</span></span>](tablerow.md)|<span data-ttu-id="3ec2c-129">向表中添加新行。</span><span class="sxs-lookup"><span data-stu-id="3ec2c-129">Adds a new row to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="3ec2c-130">属性</span><span class="sxs-lookup"><span data-stu-id="3ec2c-130">Properties</span></span>
| <span data-ttu-id="3ec2c-131">属性</span><span class="sxs-lookup"><span data-stu-id="3ec2c-131">Property</span></span>     | <span data-ttu-id="3ec2c-132">类型</span><span class="sxs-lookup"><span data-stu-id="3ec2c-132">Type</span></span>   |<span data-ttu-id="3ec2c-133">说明</span><span class="sxs-lookup"><span data-stu-id="3ec2c-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3ec2c-134">index</span><span class="sxs-lookup"><span data-stu-id="3ec2c-134">index</span></span>|<span data-ttu-id="3ec2c-135">int</span><span class="sxs-lookup"><span data-stu-id="3ec2c-135">int</span></span>|<span data-ttu-id="3ec2c-p101">返回表的行集合内行的索引编号。从零开始编制索引。只读。</span><span class="sxs-lookup"><span data-stu-id="3ec2c-p101">Returns the index number of the row within the rows collection of the table. Zero-indexed. Read-only.</span></span>|
|<span data-ttu-id="3ec2c-139">values</span><span class="sxs-lookup"><span data-stu-id="3ec2c-139">values</span></span>|<span data-ttu-id="3ec2c-140">Json</span><span class="sxs-lookup"><span data-stu-id="3ec2c-140">Json</span></span>|<span data-ttu-id="3ec2c-p102">表示指定区域的原始值。返回的数据类型可能是字符串、数字或布尔值。包含一个将返回错误字符串的错误的单元格。</span><span class="sxs-lookup"><span data-stu-id="3ec2c-p102">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ec2c-144">关系</span><span class="sxs-lookup"><span data-stu-id="3ec2c-144">Relationships</span></span>
<span data-ttu-id="3ec2c-145">无</span><span class="sxs-lookup"><span data-stu-id="3ec2c-145">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3ec2c-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3ec2c-146">JSON representation</span></span>

<span data-ttu-id="3ec2c-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3ec2c-147">Here is a JSON representation of the resource.</span></span>

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
