---
title: TableColumn 资源类型
description: 代表表中的一列。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9f70b5363ccc7552975db8f2396af705d8bf1557
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565609"
---
# <a name="tablecolumn-resource-type"></a><span data-ttu-id="db3e4-103">TableColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="db3e4-103">TableColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db3e4-104">代表表中的一列。</span><span class="sxs-lookup"><span data-stu-id="db3e4-104">Represents a column in a table.</span></span>


## <a name="methods"></a><span data-ttu-id="db3e4-105">方法</span><span class="sxs-lookup"><span data-stu-id="db3e4-105">Methods</span></span>

| <span data-ttu-id="db3e4-106">方法</span><span class="sxs-lookup"><span data-stu-id="db3e4-106">Method</span></span>           | <span data-ttu-id="db3e4-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="db3e4-107">Return Type</span></span>    |<span data-ttu-id="db3e4-108">说明</span><span class="sxs-lookup"><span data-stu-id="db3e4-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="db3e4-109">获取 TableColumn</span><span class="sxs-lookup"><span data-stu-id="db3e4-109">Get TableColumn</span></span>](../api/tablecolumn-get.md) | [<span data-ttu-id="db3e4-110">TableColumn</span><span class="sxs-lookup"><span data-stu-id="db3e4-110">TableColumn</span></span>](tablecolumn.md) |<span data-ttu-id="db3e4-111">读取 tablecolumn 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="db3e4-111">Read properties and relationships of tableColumn object.</span></span>|
|[<span data-ttu-id="db3e4-112">更新</span><span class="sxs-lookup"><span data-stu-id="db3e4-112">Update</span></span>](../api/tablecolumn-update.md) | [<span data-ttu-id="db3e4-113">TableColumn</span><span class="sxs-lookup"><span data-stu-id="db3e4-113">TableColumn</span></span>](tablecolumn.md) |<span data-ttu-id="db3e4-114">更新 TableColumn 对象</span><span class="sxs-lookup"><span data-stu-id="db3e4-114">Update TableColumn object.</span></span> |
|[<span data-ttu-id="db3e4-115">Databodyrange</span><span class="sxs-lookup"><span data-stu-id="db3e4-115">Databodyrange</span></span>](../api/tablecolumn-databodyrange.md)|[<span data-ttu-id="db3e4-116">Range</span><span class="sxs-lookup"><span data-stu-id="db3e4-116">Range</span></span>](range.md)|<span data-ttu-id="db3e4-117">获取与列的数据体相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="db3e4-117">Gets the range object associated with the data body of the column.</span></span>|
|[<span data-ttu-id="db3e4-118">Headerrowrange</span><span class="sxs-lookup"><span data-stu-id="db3e4-118">Headerrowrange</span></span>](../api/tablecolumn-headerrowrange.md)|[<span data-ttu-id="db3e4-119">Range</span><span class="sxs-lookup"><span data-stu-id="db3e4-119">Range</span></span>](range.md)|<span data-ttu-id="db3e4-120">获取与列的标头行相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="db3e4-120">Gets the range object associated with the header row of the column.</span></span>|
|[<span data-ttu-id="db3e4-121">区域</span><span class="sxs-lookup"><span data-stu-id="db3e4-121">Range</span></span>](../api/tablecolumn-range.md)|[<span data-ttu-id="db3e4-122">Range</span><span class="sxs-lookup"><span data-stu-id="db3e4-122">Range</span></span>](range.md)|<span data-ttu-id="db3e4-123">获取与整个列相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="db3e4-123">Gets the range object associated with the entire column.</span></span>|
|[<span data-ttu-id="db3e4-124">Totalrowrange</span><span class="sxs-lookup"><span data-stu-id="db3e4-124">Totalrowrange</span></span>](../api/tablecolumn-totalrowrange.md)|[<span data-ttu-id="db3e4-125">Range</span><span class="sxs-lookup"><span data-stu-id="db3e4-125">Range</span></span>](range.md)|<span data-ttu-id="db3e4-126">获取与列的总计行相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="db3e4-126">Gets the range object associated with the totals row of the column.</span></span>|
|[<span data-ttu-id="db3e4-127">删除</span><span class="sxs-lookup"><span data-stu-id="db3e4-127">Delete</span></span>](../api/tablecolumn-delete.md)|<span data-ttu-id="db3e4-128">无</span><span class="sxs-lookup"><span data-stu-id="db3e4-128">None</span></span>|<span data-ttu-id="db3e4-129">从表中删除列。</span><span class="sxs-lookup"><span data-stu-id="db3e4-129">Deletes the column from the table.</span></span>|
|[<span data-ttu-id="db3e4-130">列出</span><span class="sxs-lookup"><span data-stu-id="db3e4-130">List</span></span>](../api/tablecolumn-list.md) | <span data-ttu-id="db3e4-131">[TableColumn](tablecolumn.md) 集合</span><span class="sxs-lookup"><span data-stu-id="db3e4-131">[TableColumn](tablecolumn.md) collection</span></span> |<span data-ttu-id="db3e4-132">获取 tableColumn 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="db3e4-132">Get tableColumn object collection.</span></span> |
|[<span data-ttu-id="db3e4-133">Itemat</span><span class="sxs-lookup"><span data-stu-id="db3e4-133">Itemat</span></span>](../api/tablecolumncollection-itemat.md)|[<span data-ttu-id="db3e4-134">TableColumn</span><span class="sxs-lookup"><span data-stu-id="db3e4-134">TableColumn</span></span>](tablecolumn.md)|<span data-ttu-id="db3e4-135">根据其在集合中的位置获取列。</span><span class="sxs-lookup"><span data-stu-id="db3e4-135">Gets a column based on its position in the collection.</span></span>|
|[<span data-ttu-id="db3e4-136">添加</span><span class="sxs-lookup"><span data-stu-id="db3e4-136">Add</span></span>](../api/tablecolumncollection-add.md)|[<span data-ttu-id="db3e4-137">TableColumn</span><span class="sxs-lookup"><span data-stu-id="db3e4-137">TableColumn</span></span>](tablecolumn.md)|<span data-ttu-id="db3e4-138">向表中添加新列。</span><span class="sxs-lookup"><span data-stu-id="db3e4-138">Adds a new column to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="db3e4-139">属性</span><span class="sxs-lookup"><span data-stu-id="db3e4-139">Properties</span></span>
| <span data-ttu-id="db3e4-140">属性</span><span class="sxs-lookup"><span data-stu-id="db3e4-140">Property</span></span>     | <span data-ttu-id="db3e4-141">类型</span><span class="sxs-lookup"><span data-stu-id="db3e4-141">Type</span></span>   |<span data-ttu-id="db3e4-142">说明</span><span class="sxs-lookup"><span data-stu-id="db3e4-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db3e4-143">id</span><span class="sxs-lookup"><span data-stu-id="db3e4-143">id</span></span>|<span data-ttu-id="db3e4-144">int</span><span class="sxs-lookup"><span data-stu-id="db3e4-144">int</span></span>|<span data-ttu-id="db3e4-p101">返回标识表内的列的唯一键。只读。</span><span class="sxs-lookup"><span data-stu-id="db3e4-p101">Returns a unique key that identifies the column within the table. Read-only.</span></span>|
|<span data-ttu-id="db3e4-147">Index</span><span class="sxs-lookup"><span data-stu-id="db3e4-147">index</span></span>|<span data-ttu-id="db3e4-148">INT</span><span class="sxs-lookup"><span data-stu-id="db3e4-148">int</span></span>|<span data-ttu-id="db3e4-p102">返回表的列集合内列的索引编号。从零开始编制索引。只读。</span><span class="sxs-lookup"><span data-stu-id="db3e4-p102">Returns the index number of the column within the columns collection of the table. Zero-indexed. Read-only.</span></span>|
|<span data-ttu-id="db3e4-152">name</span><span class="sxs-lookup"><span data-stu-id="db3e4-152">name</span></span>|<span data-ttu-id="db3e4-153">string</span><span class="sxs-lookup"><span data-stu-id="db3e4-153">string</span></span>|<span data-ttu-id="db3e4-p103">返回表格列的名称。只读。</span><span class="sxs-lookup"><span data-stu-id="db3e4-p103">Returns the name of the table column. Read-only.</span></span>|
|<span data-ttu-id="db3e4-156">值</span><span class="sxs-lookup"><span data-stu-id="db3e4-156">values</span></span>|<span data-ttu-id="db3e4-157">json</span><span class="sxs-lookup"><span data-stu-id="db3e4-157">json</span></span>|<span data-ttu-id="db3e4-p104">表示指定区域的原始值。返回的数据类型可能是字符串、数字或布尔值。包含一个将返回错误字符串的错误的单元格。</span><span class="sxs-lookup"><span data-stu-id="db3e4-p104">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="relationships"></a><span data-ttu-id="db3e4-161">关系</span><span class="sxs-lookup"><span data-stu-id="db3e4-161">Relationships</span></span>
| <span data-ttu-id="db3e4-162">关系</span><span class="sxs-lookup"><span data-stu-id="db3e4-162">Relationship</span></span> | <span data-ttu-id="db3e4-163">类型</span><span class="sxs-lookup"><span data-stu-id="db3e4-163">Type</span></span>   |<span data-ttu-id="db3e4-164">说明</span><span class="sxs-lookup"><span data-stu-id="db3e4-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db3e4-165">筛选器</span><span class="sxs-lookup"><span data-stu-id="db3e4-165">filter</span></span>|[<span data-ttu-id="db3e4-166">筛选</span><span class="sxs-lookup"><span data-stu-id="db3e4-166">Filter</span></span>](filter.md)|<span data-ttu-id="db3e4-p105">检索应用于列的筛选器。只读。</span><span class="sxs-lookup"><span data-stu-id="db3e4-p105">Retrieve the filter applied to the column. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="db3e4-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="db3e4-169">JSON representation</span></span>

<span data-ttu-id="db3e4-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db3e4-170">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "TableColumn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/tablecolumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
