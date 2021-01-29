---
title: workbookTableColumn 资源类型
description: 代表表格中的一列。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 85a8c4b53eb39ae440946872718447f272ef841b
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2021
ms.locfileid: "50033909"
---
# <a name="workbooktablecolumn-resource-type"></a><span data-ttu-id="5df84-103">workbookTableColumn 资源类型</span><span class="sxs-lookup"><span data-stu-id="5df84-103">workbookTableColumn resource type</span></span>

<span data-ttu-id="5df84-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5df84-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5df84-105">代表表格中的一列。</span><span class="sxs-lookup"><span data-stu-id="5df84-105">Represents a column in a table.</span></span>


## <a name="methods"></a><span data-ttu-id="5df84-106">方法</span><span class="sxs-lookup"><span data-stu-id="5df84-106">Methods</span></span>

| <span data-ttu-id="5df84-107">方法</span><span class="sxs-lookup"><span data-stu-id="5df84-107">Method</span></span>           | <span data-ttu-id="5df84-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="5df84-108">Return Type</span></span>    |<span data-ttu-id="5df84-109">说明</span><span class="sxs-lookup"><span data-stu-id="5df84-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5df84-110">获取 TableColumn</span><span class="sxs-lookup"><span data-stu-id="5df84-110">Get TableColumn</span></span>](../api/tablecolumn-get.md) | [<span data-ttu-id="5df84-111">WorkbookTableColumn</span><span class="sxs-lookup"><span data-stu-id="5df84-111">WorkbookTableColumn</span></span>](workbooktablecolumn.md) |<span data-ttu-id="5df84-112">读取 tablecolumn 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5df84-112">Read properties and relationships of tableColumn object.</span></span>|
|[<span data-ttu-id="5df84-113">更新</span><span class="sxs-lookup"><span data-stu-id="5df84-113">Update</span></span>](../api/tablecolumn-update.md) | [<span data-ttu-id="5df84-114">WorkbookTableColumn</span><span class="sxs-lookup"><span data-stu-id="5df84-114">WorkbookTableColumn</span></span>](workbooktablecolumn.md) |<span data-ttu-id="5df84-115">更新 TableColumn 对象</span><span class="sxs-lookup"><span data-stu-id="5df84-115">Update TableColumn object.</span></span> |
|[<span data-ttu-id="5df84-116">Databodyrange</span><span class="sxs-lookup"><span data-stu-id="5df84-116">Databodyrange</span></span>](../api/tablecolumn-databodyrange.md)|[<span data-ttu-id="5df84-117">区域</span><span class="sxs-lookup"><span data-stu-id="5df84-117">Range</span></span>](range.md)|<span data-ttu-id="5df84-118">获取与列的数据体相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="5df84-118">Gets the range object associated with the data body of the column.</span></span>|
|[<span data-ttu-id="5df84-119">Headerrowrange</span><span class="sxs-lookup"><span data-stu-id="5df84-119">Headerrowrange</span></span>](../api/tablecolumn-headerrowrange.md)|[<span data-ttu-id="5df84-120">区域</span><span class="sxs-lookup"><span data-stu-id="5df84-120">Range</span></span>](range.md)|<span data-ttu-id="5df84-121">获取与列的标头行相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="5df84-121">Gets the range object associated with the header row of the column.</span></span>|
|[<span data-ttu-id="5df84-122">区域</span><span class="sxs-lookup"><span data-stu-id="5df84-122">Range</span></span>](../api/tablecolumn-range.md)|[<span data-ttu-id="5df84-123">区域</span><span class="sxs-lookup"><span data-stu-id="5df84-123">Range</span></span>](range.md)|<span data-ttu-id="5df84-124">获取与整个列相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="5df84-124">Gets the range object associated with the entire column.</span></span>|
|[<span data-ttu-id="5df84-125">Totalrowrange</span><span class="sxs-lookup"><span data-stu-id="5df84-125">Totalrowrange</span></span>](../api/tablecolumn-totalrowrange.md)|[<span data-ttu-id="5df84-126">区域</span><span class="sxs-lookup"><span data-stu-id="5df84-126">Range</span></span>](range.md)|<span data-ttu-id="5df84-127">获取与列的总计行相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="5df84-127">Gets the range object associated with the totals row of the column.</span></span>|
|[<span data-ttu-id="5df84-128">删除</span><span class="sxs-lookup"><span data-stu-id="5df84-128">Delete</span></span>](../api/tablecolumn-delete.md)|<span data-ttu-id="5df84-129">无</span><span class="sxs-lookup"><span data-stu-id="5df84-129">None</span></span>|<span data-ttu-id="5df84-130">从表中删除列。</span><span class="sxs-lookup"><span data-stu-id="5df84-130">Deletes the column from the table.</span></span>|
|[<span data-ttu-id="5df84-131">列出</span><span class="sxs-lookup"><span data-stu-id="5df84-131">List</span></span>](../api/tablecolumn-list.md) | <span data-ttu-id="5df84-132">[WorkbookTableColumn](workbooktablecolumn.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5df84-132">[WorkbookTableColumn](workbooktablecolumn.md) collection</span></span> |<span data-ttu-id="5df84-133">获取 tableColumn 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="5df84-133">Get tableColumn object collection.</span></span> |
|[<span data-ttu-id="5df84-134">Itemat</span><span class="sxs-lookup"><span data-stu-id="5df84-134">Itemat</span></span>](../api/tablecolumncollection-itemat.md)|[<span data-ttu-id="5df84-135">WorkbookTableColumn</span><span class="sxs-lookup"><span data-stu-id="5df84-135">WorkbookTableColumn</span></span>](workbooktablecolumn.md)|<span data-ttu-id="5df84-136">根据其在集合中的位置获取列。</span><span class="sxs-lookup"><span data-stu-id="5df84-136">Gets a column based on its position in the collection.</span></span>|
|[<span data-ttu-id="5df84-137">添加</span><span class="sxs-lookup"><span data-stu-id="5df84-137">Add</span></span>](../api/tablecolumncollection-add.md)|[<span data-ttu-id="5df84-138">WorkbookTableColumn</span><span class="sxs-lookup"><span data-stu-id="5df84-138">WorkbookTableColumn</span></span>](workbooktablecolumn.md)|<span data-ttu-id="5df84-139">向表中添加新列。</span><span class="sxs-lookup"><span data-stu-id="5df84-139">Adds a new column to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="5df84-140">属性</span><span class="sxs-lookup"><span data-stu-id="5df84-140">Properties</span></span>
| <span data-ttu-id="5df84-141">属性</span><span class="sxs-lookup"><span data-stu-id="5df84-141">Property</span></span>     | <span data-ttu-id="5df84-142">类型</span><span class="sxs-lookup"><span data-stu-id="5df84-142">Type</span></span>   |<span data-ttu-id="5df84-143">说明</span><span class="sxs-lookup"><span data-stu-id="5df84-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5df84-144">id</span><span class="sxs-lookup"><span data-stu-id="5df84-144">id</span></span>|<span data-ttu-id="5df84-145">string</span><span class="sxs-lookup"><span data-stu-id="5df84-145">string</span></span>|<span data-ttu-id="5df84-146">返回用于标识表中列的唯一键。</span><span class="sxs-lookup"><span data-stu-id="5df84-146">Returns a unique key that identifies the column within the table.</span></span> <span data-ttu-id="5df84-147">应将此属性解析为不透明的字符串值，不得将它解析为其他任何类型。</span><span class="sxs-lookup"><span data-stu-id="5df84-147">This property should be interpreted as an opaque string value and should not be parsed to any other type.</span></span> <span data-ttu-id="5df84-148">只读。</span><span class="sxs-lookup"><span data-stu-id="5df84-148">Read-only.</span></span>|
|<span data-ttu-id="5df84-149">index</span><span class="sxs-lookup"><span data-stu-id="5df84-149">index</span></span>|<span data-ttu-id="5df84-150">int</span><span class="sxs-lookup"><span data-stu-id="5df84-150">int</span></span>|<span data-ttu-id="5df84-p102">返回表的列集合内列的索引编号。从零开始编制索引。只读。</span><span class="sxs-lookup"><span data-stu-id="5df84-p102">Returns the index number of the column within the columns collection of the table. Zero-indexed. Read-only.</span></span>|
|<span data-ttu-id="5df84-154">name</span><span class="sxs-lookup"><span data-stu-id="5df84-154">name</span></span>|<span data-ttu-id="5df84-155">string</span><span class="sxs-lookup"><span data-stu-id="5df84-155">string</span></span>|<span data-ttu-id="5df84-156">返回表格列的名称。</span><span class="sxs-lookup"><span data-stu-id="5df84-156">Returns the name of the table column.</span></span>|
|<span data-ttu-id="5df84-157">values</span><span class="sxs-lookup"><span data-stu-id="5df84-157">values</span></span>|<span data-ttu-id="5df84-158">Json</span><span class="sxs-lookup"><span data-stu-id="5df84-158">Json</span></span>|<span data-ttu-id="5df84-p103">表示指定区域的原始值。返回的数据类型可能是字符串、数字或布尔值。包含一个将返回错误字符串的错误的单元格。</span><span class="sxs-lookup"><span data-stu-id="5df84-p103">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5df84-162">关系</span><span class="sxs-lookup"><span data-stu-id="5df84-162">Relationships</span></span>
| <span data-ttu-id="5df84-163">关系</span><span class="sxs-lookup"><span data-stu-id="5df84-163">Relationship</span></span> | <span data-ttu-id="5df84-164">类型</span><span class="sxs-lookup"><span data-stu-id="5df84-164">Type</span></span>   |<span data-ttu-id="5df84-165">说明</span><span class="sxs-lookup"><span data-stu-id="5df84-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5df84-166">筛选器</span><span class="sxs-lookup"><span data-stu-id="5df84-166">filter</span></span>|[<span data-ttu-id="5df84-167">WorkbookFilter</span><span class="sxs-lookup"><span data-stu-id="5df84-167">WorkbookFilter</span></span>](filter.md)|<span data-ttu-id="5df84-p104">检索应用于列的筛选器。只读。</span><span class="sxs-lookup"><span data-stu-id="5df84-p104">Retrieve the filter applied to the column. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5df84-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5df84-170">JSON representation</span></span>

<span data-ttu-id="5df84-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5df84-171">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableColumn"
}-->

```json
{
  "id": "1024",
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

