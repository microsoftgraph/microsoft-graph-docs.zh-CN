---
title: TableColumn 资源类型
description: 代表表中的一列。
author: lumine2008
ms.openlocfilehash: d2d83859c15a24624d8711a7ef86e3b0c89448e1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315125"
---
# <a name="tablecolumn-resource-type"></a><span data-ttu-id="d8916-103">TableColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="d8916-103">TableColumn resource type</span></span>

<span data-ttu-id="d8916-104">代表表中的一列。</span><span class="sxs-lookup"><span data-stu-id="d8916-104">Represents a column in a table.</span></span>


## <a name="methods"></a><span data-ttu-id="d8916-105">方法</span><span class="sxs-lookup"><span data-stu-id="d8916-105">Methods</span></span>

| <span data-ttu-id="d8916-106">方法</span><span class="sxs-lookup"><span data-stu-id="d8916-106">Method</span></span>           | <span data-ttu-id="d8916-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="d8916-107">Return Type</span></span>    |<span data-ttu-id="d8916-108">说明</span><span class="sxs-lookup"><span data-stu-id="d8916-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d8916-109">获取 TableColumn</span><span class="sxs-lookup"><span data-stu-id="d8916-109">Get TableColumn</span></span>](../api/tablecolumn-get.md) | [<span data-ttu-id="d8916-110">WorkbookTableColumn</span><span class="sxs-lookup"><span data-stu-id="d8916-110">WorkbookTableColumn</span></span>](tablecolumn.md) |<span data-ttu-id="d8916-111">读取 tablecolumn 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d8916-111">Read properties and relationships of tableColumn object.</span></span>|
|[<span data-ttu-id="d8916-112">更新</span><span class="sxs-lookup"><span data-stu-id="d8916-112">Update</span></span>](../api/tablecolumn-update.md) | [<span data-ttu-id="d8916-113">WorkbookTableColumn</span><span class="sxs-lookup"><span data-stu-id="d8916-113">WorkbookTableColumn</span></span>](tablecolumn.md) |<span data-ttu-id="d8916-114">更新 TableColumn 对象</span><span class="sxs-lookup"><span data-stu-id="d8916-114">Update TableColumn object.</span></span> |
|[<span data-ttu-id="d8916-115">Databodyrange</span><span class="sxs-lookup"><span data-stu-id="d8916-115">Databodyrange</span></span>](../api/tablecolumn-databodyrange.md)|[<span data-ttu-id="d8916-116">区域</span><span class="sxs-lookup"><span data-stu-id="d8916-116">Range</span></span>](range.md)|<span data-ttu-id="d8916-117">获取与列的数据体相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="d8916-117">Gets the range object associated with the data body of the column.</span></span>|
|[<span data-ttu-id="d8916-118">Headerrowrange</span><span class="sxs-lookup"><span data-stu-id="d8916-118">Headerrowrange</span></span>](../api/tablecolumn-headerrowrange.md)|[<span data-ttu-id="d8916-119">区域</span><span class="sxs-lookup"><span data-stu-id="d8916-119">Range</span></span>](range.md)|<span data-ttu-id="d8916-120">获取与列的标头行相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="d8916-120">Gets the range object associated with the header row of the column.</span></span>|
|[<span data-ttu-id="d8916-121">区域</span><span class="sxs-lookup"><span data-stu-id="d8916-121">Range</span></span>](../api/tablecolumn-range.md)|[<span data-ttu-id="d8916-122">Range</span><span class="sxs-lookup"><span data-stu-id="d8916-122">Range</span></span>](range.md)|<span data-ttu-id="d8916-123">获取与整个列相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="d8916-123">Gets the range object associated with the entire column.</span></span>|
|[<span data-ttu-id="d8916-124">Totalrowrange</span><span class="sxs-lookup"><span data-stu-id="d8916-124">Totalrowrange</span></span>](../api/tablecolumn-totalrowrange.md)|[<span data-ttu-id="d8916-125">区域</span><span class="sxs-lookup"><span data-stu-id="d8916-125">Range</span></span>](range.md)|<span data-ttu-id="d8916-126">获取与列的总计行相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="d8916-126">Gets the range object associated with the totals row of the column.</span></span>|
|[<span data-ttu-id="d8916-127">删除</span><span class="sxs-lookup"><span data-stu-id="d8916-127">Delete</span></span>](../api/tablecolumn-delete.md)|<span data-ttu-id="d8916-128">无</span><span class="sxs-lookup"><span data-stu-id="d8916-128">None</span></span>|<span data-ttu-id="d8916-129">从表中删除列。</span><span class="sxs-lookup"><span data-stu-id="d8916-129">Deletes the column from the table.</span></span>|
|[<span data-ttu-id="d8916-130">列出</span><span class="sxs-lookup"><span data-stu-id="d8916-130">List</span></span>](../api/tablecolumn-list.md) | <span data-ttu-id="d8916-131">[WorkbookTableColumn](tablecolumn.md)集合</span><span class="sxs-lookup"><span data-stu-id="d8916-131">[WorkbookTableColumn](tablecolumn.md) collection</span></span> |<span data-ttu-id="d8916-132">获取 tableColumn 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="d8916-132">Get tableColumn object collection.</span></span> |
|[<span data-ttu-id="d8916-133">Itemat</span><span class="sxs-lookup"><span data-stu-id="d8916-133">Itemat</span></span>](../api/tablecolumncollection-itemat.md)|[<span data-ttu-id="d8916-134">WorkbookTableColumn</span><span class="sxs-lookup"><span data-stu-id="d8916-134">WorkbookTableColumn</span></span>](tablecolumn.md)|<span data-ttu-id="d8916-135">根据其在集合中的位置获取列。</span><span class="sxs-lookup"><span data-stu-id="d8916-135">Gets a column based on its position in the collection.</span></span>|
|[<span data-ttu-id="d8916-136">添加</span><span class="sxs-lookup"><span data-stu-id="d8916-136">Add</span></span>](../api/tablecolumncollection-add.md)|[<span data-ttu-id="d8916-137">WorkbookTableColumn</span><span class="sxs-lookup"><span data-stu-id="d8916-137">WorkbookTableColumn</span></span>](tablecolumn.md)|<span data-ttu-id="d8916-138">向表中添加新列。</span><span class="sxs-lookup"><span data-stu-id="d8916-138">Adds a new column to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="d8916-139">属性</span><span class="sxs-lookup"><span data-stu-id="d8916-139">Properties</span></span>
| <span data-ttu-id="d8916-140">属性</span><span class="sxs-lookup"><span data-stu-id="d8916-140">Property</span></span>     | <span data-ttu-id="d8916-141">类型</span><span class="sxs-lookup"><span data-stu-id="d8916-141">Type</span></span>   |<span data-ttu-id="d8916-142">说明</span><span class="sxs-lookup"><span data-stu-id="d8916-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8916-143">ID</span><span class="sxs-lookup"><span data-stu-id="d8916-143">id</span></span>|<span data-ttu-id="d8916-144">string</span><span class="sxs-lookup"><span data-stu-id="d8916-144">string</span></span>|<span data-ttu-id="d8916-145">返回用于标识表中列的唯一键。</span><span class="sxs-lookup"><span data-stu-id="d8916-145">Returns a unique key that identifies the column within the table.</span></span> <span data-ttu-id="d8916-146">应将此属性解析为不透明的字符串值，不得将它解析为其他任何类型。</span><span class="sxs-lookup"><span data-stu-id="d8916-146">This property should be interpreted as an opaque string value and should not be parsed to any other type.</span></span> <span data-ttu-id="d8916-147">只读。</span><span class="sxs-lookup"><span data-stu-id="d8916-147">Read-only.</span></span>|
|<span data-ttu-id="d8916-148">Index</span><span class="sxs-lookup"><span data-stu-id="d8916-148">index</span></span>|<span data-ttu-id="d8916-149">整数</span><span class="sxs-lookup"><span data-stu-id="d8916-149">int</span></span>|<span data-ttu-id="d8916-p102">返回表的列集合内列的索引编号。从零开始编制索引。只读。</span><span class="sxs-lookup"><span data-stu-id="d8916-p102">Returns the index number of the column within the columns collection of the table. Zero-indexed. Read-only.</span></span>|
|<span data-ttu-id="d8916-153">name</span><span class="sxs-lookup"><span data-stu-id="d8916-153">name</span></span>|<span data-ttu-id="d8916-154">string</span><span class="sxs-lookup"><span data-stu-id="d8916-154">string</span></span>|<span data-ttu-id="d8916-p103">返回表格列的名称。只读。</span><span class="sxs-lookup"><span data-stu-id="d8916-p103">Returns the name of the table column. Read-only.</span></span>|
|<span data-ttu-id="d8916-157">values</span><span class="sxs-lookup"><span data-stu-id="d8916-157">values</span></span>|<span data-ttu-id="d8916-158">Json</span><span class="sxs-lookup"><span data-stu-id="d8916-158">Json</span></span>|<span data-ttu-id="d8916-p104">表示指定区域的原始值。返回的数据类型可能是字符串、数字或布尔值。包含一个将返回错误字符串的错误的单元格。</span><span class="sxs-lookup"><span data-stu-id="d8916-p104">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8916-162">Relationships</span><span class="sxs-lookup"><span data-stu-id="d8916-162">Relationships</span></span>
| <span data-ttu-id="d8916-163">关系</span><span class="sxs-lookup"><span data-stu-id="d8916-163">Relationship</span></span> | <span data-ttu-id="d8916-164">类型</span><span class="sxs-lookup"><span data-stu-id="d8916-164">Type</span></span>   |<span data-ttu-id="d8916-165">说明</span><span class="sxs-lookup"><span data-stu-id="d8916-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8916-166">筛选器</span><span class="sxs-lookup"><span data-stu-id="d8916-166">filter</span></span>|[<span data-ttu-id="d8916-167">WorkbookFilter</span><span class="sxs-lookup"><span data-stu-id="d8916-167">WorkbookFilter</span></span>](filter.md)|<span data-ttu-id="d8916-p105">检索应用于列的筛选器。只读。</span><span class="sxs-lookup"><span data-stu-id="d8916-p105">Retrieve the filter applied to the column. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d8916-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d8916-170">JSON representation</span></span>

<span data-ttu-id="d8916-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8916-171">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableColumn"
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
