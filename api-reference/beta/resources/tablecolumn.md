---
title: TableColumn 资源类型
description: 代表表中的一列。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b6f16b078e2d865ec9800f8ebc8668c2a622911d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936583"
---
# <a name="tablecolumn-resource-type"></a><span data-ttu-id="a621a-103">TableColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="a621a-103">TableColumn resource type</span></span>

> <span data-ttu-id="a621a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a621a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a621a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a621a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a621a-106">代表表中的一列。</span><span class="sxs-lookup"><span data-stu-id="a621a-106">Represents a column in a table.</span></span>


## <a name="methods"></a><span data-ttu-id="a621a-107">方法</span><span class="sxs-lookup"><span data-stu-id="a621a-107">Methods</span></span>

| <span data-ttu-id="a621a-108">方法</span><span class="sxs-lookup"><span data-stu-id="a621a-108">Method</span></span>           | <span data-ttu-id="a621a-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a621a-109">Return Type</span></span>    |<span data-ttu-id="a621a-110">说明</span><span class="sxs-lookup"><span data-stu-id="a621a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a621a-111">获取 TableColumn</span><span class="sxs-lookup"><span data-stu-id="a621a-111">Get TableColumn</span></span>](../api/tablecolumn-get.md) | [<span data-ttu-id="a621a-112">TableColumn</span><span class="sxs-lookup"><span data-stu-id="a621a-112">TableColumn</span></span>](tablecolumn.md) |<span data-ttu-id="a621a-113">读取 tablecolumn 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a621a-113">Read properties and relationships of tableColumn object.</span></span>|
|[<span data-ttu-id="a621a-114">更新</span><span class="sxs-lookup"><span data-stu-id="a621a-114">Update</span></span>](../api/tablecolumn-update.md) | [<span data-ttu-id="a621a-115">TableColumn</span><span class="sxs-lookup"><span data-stu-id="a621a-115">TableColumn</span></span>](tablecolumn.md) |<span data-ttu-id="a621a-116">更新 TableColumn 对象</span><span class="sxs-lookup"><span data-stu-id="a621a-116">Update TableColumn object.</span></span> |
|[<span data-ttu-id="a621a-117">Databodyrange</span><span class="sxs-lookup"><span data-stu-id="a621a-117">Databodyrange</span></span>](../api/tablecolumn-databodyrange.md)|[<span data-ttu-id="a621a-118">区域</span><span class="sxs-lookup"><span data-stu-id="a621a-118">Range</span></span>](range.md)|<span data-ttu-id="a621a-119">获取与列的数据体相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="a621a-119">Gets the range object associated with the data body of the column.</span></span>|
|[<span data-ttu-id="a621a-120">Headerrowrange</span><span class="sxs-lookup"><span data-stu-id="a621a-120">Headerrowrange</span></span>](../api/tablecolumn-headerrowrange.md)|[<span data-ttu-id="a621a-121">区域</span><span class="sxs-lookup"><span data-stu-id="a621a-121">Range</span></span>](range.md)|<span data-ttu-id="a621a-122">获取与列的标头行相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="a621a-122">Gets the range object associated with the header row of the column.</span></span>|
|[<span data-ttu-id="a621a-123">区域</span><span class="sxs-lookup"><span data-stu-id="a621a-123">Range</span></span>](../api/tablecolumn-range.md)|[<span data-ttu-id="a621a-124">Range</span><span class="sxs-lookup"><span data-stu-id="a621a-124">Range</span></span>](range.md)|<span data-ttu-id="a621a-125">获取与整个列相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="a621a-125">Gets the range object associated with the entire column.</span></span>|
|[<span data-ttu-id="a621a-126">Totalrowrange</span><span class="sxs-lookup"><span data-stu-id="a621a-126">Totalrowrange</span></span>](../api/tablecolumn-totalrowrange.md)|[<span data-ttu-id="a621a-127">区域</span><span class="sxs-lookup"><span data-stu-id="a621a-127">Range</span></span>](range.md)|<span data-ttu-id="a621a-128">获取与列的总计行相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="a621a-128">Gets the range object associated with the totals row of the column.</span></span>|
|[<span data-ttu-id="a621a-129">删除</span><span class="sxs-lookup"><span data-stu-id="a621a-129">Delete</span></span>](../api/tablecolumn-delete.md)|<span data-ttu-id="a621a-130">无</span><span class="sxs-lookup"><span data-stu-id="a621a-130">None</span></span>|<span data-ttu-id="a621a-131">从表中删除列。</span><span class="sxs-lookup"><span data-stu-id="a621a-131">Deletes the column from the table.</span></span>|
|[<span data-ttu-id="a621a-132">列出</span><span class="sxs-lookup"><span data-stu-id="a621a-132">List</span></span>](../api/tablecolumn-list.md) | <span data-ttu-id="a621a-133">[TableColumn](tablecolumn.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a621a-133">[TableColumn](tablecolumn.md) collection</span></span> |<span data-ttu-id="a621a-134">获取 tableColumn 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="a621a-134">Get tableColumn object collection.</span></span> |
|[<span data-ttu-id="a621a-135">Itemat</span><span class="sxs-lookup"><span data-stu-id="a621a-135">Itemat</span></span>](../api/tablecolumncollection-itemat.md)|[<span data-ttu-id="a621a-136">TableColumn</span><span class="sxs-lookup"><span data-stu-id="a621a-136">TableColumn</span></span>](tablecolumn.md)|<span data-ttu-id="a621a-137">根据其在集合中的位置获取列。</span><span class="sxs-lookup"><span data-stu-id="a621a-137">Gets a column based on its position in the collection.</span></span>|
|[<span data-ttu-id="a621a-138">添加</span><span class="sxs-lookup"><span data-stu-id="a621a-138">Add</span></span>](../api/tablecolumncollection-add.md)|[<span data-ttu-id="a621a-139">TableColumn</span><span class="sxs-lookup"><span data-stu-id="a621a-139">TableColumn</span></span>](tablecolumn.md)|<span data-ttu-id="a621a-140">向表中添加新列。</span><span class="sxs-lookup"><span data-stu-id="a621a-140">Adds a new column to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="a621a-141">属性</span><span class="sxs-lookup"><span data-stu-id="a621a-141">Properties</span></span>
| <span data-ttu-id="a621a-142">属性</span><span class="sxs-lookup"><span data-stu-id="a621a-142">Property</span></span>     | <span data-ttu-id="a621a-143">类型</span><span class="sxs-lookup"><span data-stu-id="a621a-143">Type</span></span>   |<span data-ttu-id="a621a-144">说明</span><span class="sxs-lookup"><span data-stu-id="a621a-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a621a-145">ID</span><span class="sxs-lookup"><span data-stu-id="a621a-145">id</span></span>|<span data-ttu-id="a621a-146">int</span><span class="sxs-lookup"><span data-stu-id="a621a-146">int</span></span>|<span data-ttu-id="a621a-p102">返回标识表内的列的唯一键。只读。</span><span class="sxs-lookup"><span data-stu-id="a621a-p102">Returns a unique key that identifies the column within the table. Read-only.</span></span>|
|<span data-ttu-id="a621a-149">Index</span><span class="sxs-lookup"><span data-stu-id="a621a-149">index</span></span>|<span data-ttu-id="a621a-150">int</span><span class="sxs-lookup"><span data-stu-id="a621a-150">int</span></span>|<span data-ttu-id="a621a-p103">返回表的列集合内列的索引编号。从零开始编制索引。只读。</span><span class="sxs-lookup"><span data-stu-id="a621a-p103">Returns the index number of the column within the columns collection of the table. Zero-indexed. Read-only.</span></span>|
|<span data-ttu-id="a621a-154">name</span><span class="sxs-lookup"><span data-stu-id="a621a-154">name</span></span>|<span data-ttu-id="a621a-155">string</span><span class="sxs-lookup"><span data-stu-id="a621a-155">string</span></span>|<span data-ttu-id="a621a-p104">返回表格列的名称。只读。</span><span class="sxs-lookup"><span data-stu-id="a621a-p104">Returns the name of the table column. Read-only.</span></span>|
|<span data-ttu-id="a621a-158">values</span><span class="sxs-lookup"><span data-stu-id="a621a-158">values</span></span>|<span data-ttu-id="a621a-159">json</span><span class="sxs-lookup"><span data-stu-id="a621a-159">json</span></span>|<span data-ttu-id="a621a-p105">表示指定区域的原始值。返回的数据类型可能是字符串、数字或布尔值。包含一个将返回错误字符串的错误的单元格。</span><span class="sxs-lookup"><span data-stu-id="a621a-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a621a-163">Relationships</span><span class="sxs-lookup"><span data-stu-id="a621a-163">Relationships</span></span>
| <span data-ttu-id="a621a-164">关系</span><span class="sxs-lookup"><span data-stu-id="a621a-164">Relationship</span></span> | <span data-ttu-id="a621a-165">类型</span><span class="sxs-lookup"><span data-stu-id="a621a-165">Type</span></span>   |<span data-ttu-id="a621a-166">说明</span><span class="sxs-lookup"><span data-stu-id="a621a-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a621a-167">筛选器</span><span class="sxs-lookup"><span data-stu-id="a621a-167">filter</span></span>|[<span data-ttu-id="a621a-168">Filter</span><span class="sxs-lookup"><span data-stu-id="a621a-168">Filter</span></span>](filter.md)|<span data-ttu-id="a621a-p106">检索应用于列的筛选器。只读。</span><span class="sxs-lookup"><span data-stu-id="a621a-p106">Retrieve the filter applied to the column. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a621a-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a621a-171">JSON representation</span></span>

<span data-ttu-id="a621a-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a621a-172">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tableColumn"
}-->

```json
{
  "id": 1024,
  "index": 1024,
  "name": "string",
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
