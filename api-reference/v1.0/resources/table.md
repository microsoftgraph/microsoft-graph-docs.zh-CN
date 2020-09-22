---
title: 表资源类型
description: 表示 Excel 表格。
author: lumine2008
localization_priority: Priority
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: dc01389c119ff145ec976056327b2a56a2256a0d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094097"
---
# <a name="table-resource-type"></a><span data-ttu-id="cd95b-103">表资源类型</span><span class="sxs-lookup"><span data-stu-id="cd95b-103">Table resource type</span></span>

<span data-ttu-id="cd95b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd95b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cd95b-105">表示 Excel 表格。</span><span class="sxs-lookup"><span data-stu-id="cd95b-105">Represents an Excel table.</span></span>


## <a name="methods"></a><span data-ttu-id="cd95b-106">方法</span><span class="sxs-lookup"><span data-stu-id="cd95b-106">Methods</span></span>

| <span data-ttu-id="cd95b-107">方法</span><span class="sxs-lookup"><span data-stu-id="cd95b-107">Method</span></span>           | <span data-ttu-id="cd95b-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="cd95b-108">Return Type</span></span>    |<span data-ttu-id="cd95b-109">说明</span><span class="sxs-lookup"><span data-stu-id="cd95b-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cd95b-110">Get Table</span><span class="sxs-lookup"><span data-stu-id="cd95b-110">Get Table</span></span>](../api/table-get.md) | [<span data-ttu-id="cd95b-111">WorkbookTable</span><span class="sxs-lookup"><span data-stu-id="cd95b-111">WorkbookTable</span></span>](table.md) |<span data-ttu-id="cd95b-112">读取 table 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cd95b-112">Read properties and relationships of table object.</span></span>|
|[<span data-ttu-id="cd95b-113">Create TableColumn</span><span class="sxs-lookup"><span data-stu-id="cd95b-113">Create TableColumn</span></span>](../api/table-post-columns.md) |[<span data-ttu-id="cd95b-114">WorkbookTableColumn</span><span class="sxs-lookup"><span data-stu-id="cd95b-114">WorkbookTableColumn</span></span>](workbooktablecolumn.md)| <span data-ttu-id="cd95b-115">通过发布到列集合创建新的 TableColumn。</span><span class="sxs-lookup"><span data-stu-id="cd95b-115">Create a new TableColumn by posting to the columns collection.</span></span>|
|[<span data-ttu-id="cd95b-116">List columns</span><span class="sxs-lookup"><span data-stu-id="cd95b-116">List columns</span></span>](../api/table-list-columns.md) |<span data-ttu-id="cd95b-117">[WorkbookTableColumn](workbooktablecolumn.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cd95b-117">[WorkbookTableColumn](workbooktablecolumn.md) collection</span></span>| <span data-ttu-id="cd95b-118">获取 TableColumn 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="cd95b-118">Get a TableColumn object collection.</span></span>|
|[<span data-ttu-id="cd95b-119">Create TableRow</span><span class="sxs-lookup"><span data-stu-id="cd95b-119">Create TableRow</span></span>](../api/table-post-rows.md) |[<span data-ttu-id="cd95b-120">WorkbookTableRow</span><span class="sxs-lookup"><span data-stu-id="cd95b-120">WorkbookTableRow</span></span>](tablerow.md)| <span data-ttu-id="cd95b-121">通过发布到行集合创建新的 TableRow。</span><span class="sxs-lookup"><span data-stu-id="cd95b-121">Create a new TableRow by posting to the rows collection.</span></span>|
|[<span data-ttu-id="cd95b-122">List rows</span><span class="sxs-lookup"><span data-stu-id="cd95b-122">List rows</span></span>](../api/table-list-rows.md) |<span data-ttu-id="cd95b-123">[WorkbookTableRow](tablerow.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cd95b-123">[WorkbookTableRow](tablerow.md) collection</span></span>| <span data-ttu-id="cd95b-124">获取 TableRow 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="cd95b-124">Get a TableRow object collection.</span></span>|
|[<span data-ttu-id="cd95b-125">Update</span><span class="sxs-lookup"><span data-stu-id="cd95b-125">Update</span></span>](../api/table-update.md) | [<span data-ttu-id="cd95b-126">WorkbookTable</span><span class="sxs-lookup"><span data-stu-id="cd95b-126">WorkbookTable</span></span>](table.md)   |<span data-ttu-id="cd95b-127">更新 Table 对象。</span><span class="sxs-lookup"><span data-stu-id="cd95b-127">Update Table object.</span></span> |
|[<span data-ttu-id="cd95b-128">Databodyrange</span><span class="sxs-lookup"><span data-stu-id="cd95b-128">Databodyrange</span></span>](../api/table-databodyrange.md)|[<span data-ttu-id="cd95b-129">区域</span><span class="sxs-lookup"><span data-stu-id="cd95b-129">Range</span></span>](range.md)|<span data-ttu-id="cd95b-130">获取与表的数据体相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="cd95b-130">Gets the range object associated with the data body of the table.</span></span>|
|[<span data-ttu-id="cd95b-131">Headerrowrange</span><span class="sxs-lookup"><span data-stu-id="cd95b-131">Headerrowrange</span></span>](../api/table-headerrowrange.md)|[<span data-ttu-id="cd95b-132">区域</span><span class="sxs-lookup"><span data-stu-id="cd95b-132">Range</span></span>](range.md)|<span data-ttu-id="cd95b-133">获取与表的标头行相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="cd95b-133">Gets the range object associated with header row of the table.</span></span>|
|[<span data-ttu-id="cd95b-134">区域</span><span class="sxs-lookup"><span data-stu-id="cd95b-134">Range</span></span>](../api/table-range.md)|[<span data-ttu-id="cd95b-135">区域</span><span class="sxs-lookup"><span data-stu-id="cd95b-135">Range</span></span>](range.md)|<span data-ttu-id="cd95b-136">获取与整个表相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="cd95b-136">Gets the range object associated with the entire table.</span></span>|
|[<span data-ttu-id="cd95b-137">Totalrowrange</span><span class="sxs-lookup"><span data-stu-id="cd95b-137">Totalrowrange</span></span>](../api/table-totalrowrange.md)|[<span data-ttu-id="cd95b-138">区域</span><span class="sxs-lookup"><span data-stu-id="cd95b-138">Range</span></span>](range.md)|<span data-ttu-id="cd95b-139">获取与表的总计行相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="cd95b-139">Gets the range object associated with totals row of the table.</span></span>|
|[<span data-ttu-id="cd95b-140">Clearfilters</span><span class="sxs-lookup"><span data-stu-id="cd95b-140">Clearfilters</span></span>](../api/table-clearfilters.md)|<span data-ttu-id="cd95b-141">无</span><span class="sxs-lookup"><span data-stu-id="cd95b-141">None</span></span>|<span data-ttu-id="cd95b-142">清除当前表上应用的所有筛选器。</span><span class="sxs-lookup"><span data-stu-id="cd95b-142">Clears all the filters currently applied on the table.</span></span>|
|[<span data-ttu-id="cd95b-143">Converttorange</span><span class="sxs-lookup"><span data-stu-id="cd95b-143">Converttorange</span></span>](../api/table-converttorange.md)|[<span data-ttu-id="cd95b-144">区域</span><span class="sxs-lookup"><span data-stu-id="cd95b-144">Range</span></span>](range.md)|<span data-ttu-id="cd95b-p101">将表转换为普通单元格区域。保留所有数据。</span><span class="sxs-lookup"><span data-stu-id="cd95b-p101">Converts the table into a normal range of cells. All data is preserved.</span></span>|
|[<span data-ttu-id="cd95b-147">删除</span><span class="sxs-lookup"><span data-stu-id="cd95b-147">Delete</span></span>](../api/table-delete.md)|<span data-ttu-id="cd95b-148">无</span><span class="sxs-lookup"><span data-stu-id="cd95b-148">None</span></span>|<span data-ttu-id="cd95b-149">删除表。</span><span class="sxs-lookup"><span data-stu-id="cd95b-149">Deletes the table.</span></span>|
|[<span data-ttu-id="cd95b-150">Reapplyfilters</span><span class="sxs-lookup"><span data-stu-id="cd95b-150">Reapplyfilters</span></span>](../api/table-reapplyfilters.md)|<span data-ttu-id="cd95b-151">无</span><span class="sxs-lookup"><span data-stu-id="cd95b-151">None</span></span>|<span data-ttu-id="cd95b-152">重新应用当前表上的所有筛选器。</span><span class="sxs-lookup"><span data-stu-id="cd95b-152">Reapplies all the filters currently on the table.</span></span>|
|[<span data-ttu-id="cd95b-153">List</span><span class="sxs-lookup"><span data-stu-id="cd95b-153">List</span></span>](../api/table-list.md) | <span data-ttu-id="cd95b-154">[WorkbookTable](table.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cd95b-154">[WorkbookTable](table.md) collection</span></span> |<span data-ttu-id="cd95b-155">获取 table 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="cd95b-155">Get table object collection.</span></span> |
|[<span data-ttu-id="cd95b-156">Add</span><span class="sxs-lookup"><span data-stu-id="cd95b-156">Add</span></span>](../api/tablecollection-add.md)|[<span data-ttu-id="cd95b-157">WorkbookTable</span><span class="sxs-lookup"><span data-stu-id="cd95b-157">WorkbookTable</span></span>](table.md)|<span data-ttu-id="cd95b-p102">创建一个新表。区域源地址确定将在其下添加表的工作表。如果无法添加表（例如，由于地址无效，或者表与另一个表重叠），将抛出错误。</span><span class="sxs-lookup"><span data-stu-id="cd95b-p102">Create a new table. The range source address determines the worksheet under which the table will be added. If the table cannot be added (e.g., because the address is invalid, or the table would overlap with another table), an error will be thrown.</span></span>|

## <a name="properties"></a><span data-ttu-id="cd95b-161">属性</span><span class="sxs-lookup"><span data-stu-id="cd95b-161">Properties</span></span>
| <span data-ttu-id="cd95b-162">属性</span><span class="sxs-lookup"><span data-stu-id="cd95b-162">Property</span></span>     | <span data-ttu-id="cd95b-163">类型</span><span class="sxs-lookup"><span data-stu-id="cd95b-163">Type</span></span>   |<span data-ttu-id="cd95b-164">说明</span><span class="sxs-lookup"><span data-stu-id="cd95b-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd95b-165">id</span><span class="sxs-lookup"><span data-stu-id="cd95b-165">id</span></span>|<span data-ttu-id="cd95b-166">string</span><span class="sxs-lookup"><span data-stu-id="cd95b-166">string</span></span>|<span data-ttu-id="cd95b-167">返回用于唯一标识指定工作簿中表的值。</span><span class="sxs-lookup"><span data-stu-id="cd95b-167">Returns a value that uniquely identifies the table in a given workbook.</span></span> <span data-ttu-id="cd95b-168">即使表被重命名，标识符的值仍保持不变。</span><span class="sxs-lookup"><span data-stu-id="cd95b-168">The value of the identifier remains the same even when the table is renamed.</span></span> <span data-ttu-id="cd95b-169">应将此属性解析为不透明的字符串值，不得将它解析为其他任何类型。</span><span class="sxs-lookup"><span data-stu-id="cd95b-169">This property should be interpreted as an opaque string value and should not be parsed to any other type.</span></span> <span data-ttu-id="cd95b-170">只读。</span><span class="sxs-lookup"><span data-stu-id="cd95b-170">Read-only.</span></span>|
|<span data-ttu-id="cd95b-171">name</span><span class="sxs-lookup"><span data-stu-id="cd95b-171">name</span></span>|<span data-ttu-id="cd95b-172">string</span><span class="sxs-lookup"><span data-stu-id="cd95b-172">string</span></span>|<span data-ttu-id="cd95b-173">表的名称。</span><span class="sxs-lookup"><span data-stu-id="cd95b-173">Name of the table.</span></span>|
|<span data-ttu-id="cd95b-174">showHeaders</span><span class="sxs-lookup"><span data-stu-id="cd95b-174">showHeaders</span></span>|<span data-ttu-id="cd95b-175">boolean</span><span class="sxs-lookup"><span data-stu-id="cd95b-175">boolean</span></span>|<span data-ttu-id="cd95b-p104">指示标头行是否可见。该值可以设置为显示或删除标头行。</span><span class="sxs-lookup"><span data-stu-id="cd95b-p104">Indicates whether the header row is visible or not. This value can be set to show or remove the header row.</span></span>|
|<span data-ttu-id="cd95b-178">showTotals</span><span class="sxs-lookup"><span data-stu-id="cd95b-178">showTotals</span></span>|<span data-ttu-id="cd95b-179">boolean</span><span class="sxs-lookup"><span data-stu-id="cd95b-179">boolean</span></span>|<span data-ttu-id="cd95b-p105">指示总计行是否可见。该值可以设置为显示或删除总计行。</span><span class="sxs-lookup"><span data-stu-id="cd95b-p105">Indicates whether the total row is visible or not. This value can be set to show or remove the total row.</span></span>|
|<span data-ttu-id="cd95b-182">style</span><span class="sxs-lookup"><span data-stu-id="cd95b-182">style</span></span>|<span data-ttu-id="cd95b-183">string</span><span class="sxs-lookup"><span data-stu-id="cd95b-183">string</span></span>|<span data-ttu-id="cd95b-184">表示表格样式的常量值。</span><span class="sxs-lookup"><span data-stu-id="cd95b-184">Constant value that represents the Table style.</span></span> <span data-ttu-id="cd95b-185">可取值为：TableStyleLight1 到 TableStyleLight21、TableStyleMedium1 到 TableStyleMedium28、TableStyleStyleDark1 到 TableStyleStyleDark11。</span><span class="sxs-lookup"><span data-stu-id="cd95b-185">The possible values are: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11.</span></span> <span data-ttu-id="cd95b-186">还可以指定工作簿中显示的用户定义的自定义样式。</span><span class="sxs-lookup"><span data-stu-id="cd95b-186">A custom user-defined style present in the workbook can also be specified.</span></span>|
|<span data-ttu-id="cd95b-187">highlightFirstColumn</span><span class="sxs-lookup"><span data-stu-id="cd95b-187">highlightFirstColumn</span></span>|<span data-ttu-id="cd95b-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd95b-188">Boolean</span></span>|<span data-ttu-id="cd95b-189">指明第一列是否包含特殊格式。</span><span class="sxs-lookup"><span data-stu-id="cd95b-189">Indicates whether the first column contains special formatting.</span></span>   |
|<span data-ttu-id="cd95b-190">highlightLastColumn</span><span class="sxs-lookup"><span data-stu-id="cd95b-190">highlightLastColumn</span></span>|<span data-ttu-id="cd95b-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd95b-191">Boolean</span></span>|<span data-ttu-id="cd95b-192">指明最后一列是否包含特殊格式。</span><span class="sxs-lookup"><span data-stu-id="cd95b-192">Indicates whether the last column contains special formatting.</span></span> |
|<span data-ttu-id="cd95b-193">showBandedColumns</span><span class="sxs-lookup"><span data-stu-id="cd95b-193">showBandedColumns</span></span>|<span data-ttu-id="cd95b-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd95b-194">Boolean</span></span>|<span data-ttu-id="cd95b-195">指明列是否采用镶边格式来以不同的方式突出显示奇数列与偶数列，让表更易于阅读。</span><span class="sxs-lookup"><span data-stu-id="cd95b-195">Indicates whether the columns show banded formatting in which odd columns are highlighted differently from even ones to make reading the table easier.</span></span>   |
|<span data-ttu-id="cd95b-196">showBandedRows</span><span class="sxs-lookup"><span data-stu-id="cd95b-196">showBandedRows</span></span>|<span data-ttu-id="cd95b-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd95b-197">Boolean</span></span>|<span data-ttu-id="cd95b-198">指明行是否采用镶边格式来以不同的方式突出显示奇数行与偶数行，让表更易于阅读。</span><span class="sxs-lookup"><span data-stu-id="cd95b-198">Indicates whether the rows show banded formatting in which odd rows are highlighted differently from even ones to make reading the table easier.</span></span>    |
|<span data-ttu-id="cd95b-199">showFilterButton</span><span class="sxs-lookup"><span data-stu-id="cd95b-199">showFilterButton</span></span>|<span data-ttu-id="cd95b-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd95b-200">Boolean</span></span>|<span data-ttu-id="cd95b-p107">指明是否在每个列标题的顶部显示筛选器按钮。仅当 table 中包含标题行时，才允许设定此设置。</span><span class="sxs-lookup"><span data-stu-id="cd95b-p107">Indicates whether the filter buttons are visible at the top of each column header. Setting this is only allowed if the table contains a header row.</span></span>   |
|<span data-ttu-id="cd95b-203">legacyId</span><span class="sxs-lookup"><span data-stu-id="cd95b-203">legacyId</span></span>|<span data-ttu-id="cd95b-204">String</span><span class="sxs-lookup"><span data-stu-id="cd95b-204">String</span></span>|<span data-ttu-id="cd95b-205">旧版 Excel 客户端中使用的旧 ID。</span><span class="sxs-lookup"><span data-stu-id="cd95b-205">Legacy Id used in older Excle clients.</span></span> <span data-ttu-id="cd95b-206">即使表格已重命名，标识符值也仍保持不变。</span><span class="sxs-lookup"><span data-stu-id="cd95b-206">The value of the identifier remains the same even when the table is renamed.</span></span> <span data-ttu-id="cd95b-207">应将此属性解析为不透明的字符串值，不得将它解析为其他任何类型。</span><span class="sxs-lookup"><span data-stu-id="cd95b-207">This property should be interpreted as an opaque string value and should not be parsed to any other type.</span></span> <span data-ttu-id="cd95b-208">只读。</span><span class="sxs-lookup"><span data-stu-id="cd95b-208">Read-only.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="cd95b-209">关系</span><span class="sxs-lookup"><span data-stu-id="cd95b-209">Relationships</span></span>
| <span data-ttu-id="cd95b-210">关系</span><span class="sxs-lookup"><span data-stu-id="cd95b-210">Relationship</span></span> | <span data-ttu-id="cd95b-211">类型</span><span class="sxs-lookup"><span data-stu-id="cd95b-211">Type</span></span>   |<span data-ttu-id="cd95b-212">说明</span><span class="sxs-lookup"><span data-stu-id="cd95b-212">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd95b-213">columns</span><span class="sxs-lookup"><span data-stu-id="cd95b-213">columns</span></span>|<span data-ttu-id="cd95b-214">[WorkbookTableColumn](workbooktablecolumn.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cd95b-214">[WorkbookTableColumn](workbooktablecolumn.md) collection</span></span>|<span data-ttu-id="cd95b-p109">表示表中所有列的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="cd95b-p109">Represents a collection of all the columns in the table. Read-only.</span></span>|
|<span data-ttu-id="cd95b-217">rows</span><span class="sxs-lookup"><span data-stu-id="cd95b-217">rows</span></span>|<span data-ttu-id="cd95b-218">[WorkbookTableRow](tablerow.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cd95b-218">[WorkbookTableRow](tablerow.md) collection</span></span>|<span data-ttu-id="cd95b-p110">表示表中所有行的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="cd95b-p110">Represents a collection of all the rows in the table. Read-only.</span></span>|
|<span data-ttu-id="cd95b-221">sort</span><span class="sxs-lookup"><span data-stu-id="cd95b-221">sort</span></span>|[<span data-ttu-id="cd95b-222">WorkbookTableSort</span><span class="sxs-lookup"><span data-stu-id="cd95b-222">WorkbookTableSort</span></span>](tablesort.md)|<span data-ttu-id="cd95b-p111">表示表的排序。只读。</span><span class="sxs-lookup"><span data-stu-id="cd95b-p111">Represents the sorting for the table. Read-only.</span></span>|
|<span data-ttu-id="cd95b-225">worksheet</span><span class="sxs-lookup"><span data-stu-id="cd95b-225">worksheet</span></span>|[<span data-ttu-id="cd95b-226">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="cd95b-226">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="cd95b-p112">包含当前表的工作表。只读。</span><span class="sxs-lookup"><span data-stu-id="cd95b-p112">The worksheet containing the current table. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cd95b-229">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cd95b-229">JSON representation</span></span>

<span data-ttu-id="cd95b-230">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd95b-230">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
     "legacyId"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTable"
}-->

```json
{
  "highlightFirstColumn": true,
  "highlightLastColumn": true,
  "id": "String (identifier)",
  "name": "String",
  "showBandedColumns": true,
  "showBandedRows": true,
  "showFilterButton": true,
  "showHeaders": true,
  "showTotals": true,
  "style": "String",
  "legacyId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Table resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

