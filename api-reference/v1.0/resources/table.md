---
title: 表资源类型
description: 表示 Excel 表格。
author: lumine2008
localization_priority: Priority
ms.prod: excel
ms.openlocfilehash: 97755052a1f0e5cf91fb45987870b498832ee735
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555925"
---
# <a name="table-resource-type"></a><span data-ttu-id="88faf-103">表资源类型</span><span class="sxs-lookup"><span data-stu-id="88faf-103">Table resource type</span></span>

<span data-ttu-id="88faf-104">表示一个 Excel 表。</span><span class="sxs-lookup"><span data-stu-id="88faf-104">Represents an Excel table.</span></span>


## <a name="methods"></a><span data-ttu-id="88faf-105">方法</span><span class="sxs-lookup"><span data-stu-id="88faf-105">Methods</span></span>

| <span data-ttu-id="88faf-106">方法</span><span class="sxs-lookup"><span data-stu-id="88faf-106">Method</span></span>           | <span data-ttu-id="88faf-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="88faf-107">Return Type</span></span>    |<span data-ttu-id="88faf-108">说明</span><span class="sxs-lookup"><span data-stu-id="88faf-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="88faf-109">Get Table</span><span class="sxs-lookup"><span data-stu-id="88faf-109">Get Table</span></span>](../api/table-get.md) | [<span data-ttu-id="88faf-110">WorkbookTable</span><span class="sxs-lookup"><span data-stu-id="88faf-110">WorkbookTable</span></span>](table.md) |<span data-ttu-id="88faf-111">读取 table 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="88faf-111">Read properties and relationships of table object.</span></span>|
|[<span data-ttu-id="88faf-112">Create TableColumn</span><span class="sxs-lookup"><span data-stu-id="88faf-112">Create TableColumn</span></span>](../api/table-post-columns.md) |[<span data-ttu-id="88faf-113">WorkbookTableColumn</span><span class="sxs-lookup"><span data-stu-id="88faf-113">WorkbookTableColumn</span></span>](tablecolumn.md)| <span data-ttu-id="88faf-114">通过发布到列集合创建新的 TableColumn。</span><span class="sxs-lookup"><span data-stu-id="88faf-114">Create a new TableColumn by posting to the columns collection.</span></span>|
|[<span data-ttu-id="88faf-115">List columns</span><span class="sxs-lookup"><span data-stu-id="88faf-115">List columns</span></span>](../api/table-list-columns.md) |<span data-ttu-id="88faf-116">[WorkbookTableColumn](tablecolumn.md) 集合</span><span class="sxs-lookup"><span data-stu-id="88faf-116">[WorkbookTableColumn](tablecolumn.md) collection</span></span>| <span data-ttu-id="88faf-117">获取 TableColumn 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="88faf-117">Get a TableColumn object collection.</span></span>|
|[<span data-ttu-id="88faf-118">Create TableRow</span><span class="sxs-lookup"><span data-stu-id="88faf-118">Create TableRow</span></span>](../api/table-post-rows.md) |[<span data-ttu-id="88faf-119">WorkbookTableRow</span><span class="sxs-lookup"><span data-stu-id="88faf-119">WorkbookTableRow</span></span>](tablerow.md)| <span data-ttu-id="88faf-120">通过发布到行集合创建新的 TableRow。</span><span class="sxs-lookup"><span data-stu-id="88faf-120">Create a new TableRow by posting to the rows collection.</span></span>|
|[<span data-ttu-id="88faf-121">List rows</span><span class="sxs-lookup"><span data-stu-id="88faf-121">List rows</span></span>](../api/table-list-rows.md) |<span data-ttu-id="88faf-122">[WorkbookTableRow](tablerow.md) 集合</span><span class="sxs-lookup"><span data-stu-id="88faf-122">[WorkbookTableRow](tablerow.md) collection</span></span>| <span data-ttu-id="88faf-123">获取 TableRow 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="88faf-123">Get a TableRow object collection.</span></span>|
|[<span data-ttu-id="88faf-124">Update</span><span class="sxs-lookup"><span data-stu-id="88faf-124">Update</span></span>](../api/table-update.md) | [<span data-ttu-id="88faf-125">WorkbookTable</span><span class="sxs-lookup"><span data-stu-id="88faf-125">WorkbookTable</span></span>](table.md)   |<span data-ttu-id="88faf-126">更新 Table 对象。</span><span class="sxs-lookup"><span data-stu-id="88faf-126">Update Table object.</span></span> |
|[<span data-ttu-id="88faf-127">Databodyrange</span><span class="sxs-lookup"><span data-stu-id="88faf-127">Databodyrange</span></span>](../api/table-databodyrange.md)|[<span data-ttu-id="88faf-128">区域</span><span class="sxs-lookup"><span data-stu-id="88faf-128">Range</span></span>](range.md)|<span data-ttu-id="88faf-129">获取与表的数据体相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="88faf-129">Gets the range object associated with the data body of the table.</span></span>|
|[<span data-ttu-id="88faf-130">Headerrowrange</span><span class="sxs-lookup"><span data-stu-id="88faf-130">Headerrowrange</span></span>](../api/table-headerrowrange.md)|[<span data-ttu-id="88faf-131">区域</span><span class="sxs-lookup"><span data-stu-id="88faf-131">Range</span></span>](range.md)|<span data-ttu-id="88faf-132">获取与表的标头行相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="88faf-132">Gets the range object associated with header row of the table.</span></span>|
|[<span data-ttu-id="88faf-133">区域</span><span class="sxs-lookup"><span data-stu-id="88faf-133">Range</span></span>](../api/table-range.md)|[<span data-ttu-id="88faf-134">区域</span><span class="sxs-lookup"><span data-stu-id="88faf-134">Range</span></span>](range.md)|<span data-ttu-id="88faf-135">获取与整个表相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="88faf-135">Gets the range object associated with the entire table.</span></span>|
|[<span data-ttu-id="88faf-136">Totalrowrange</span><span class="sxs-lookup"><span data-stu-id="88faf-136">Totalrowrange</span></span>](../api/table-totalrowrange.md)|[<span data-ttu-id="88faf-137">区域</span><span class="sxs-lookup"><span data-stu-id="88faf-137">Range</span></span>](range.md)|<span data-ttu-id="88faf-138">获取与表的总计行相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="88faf-138">Gets the range object associated with totals row of the table.</span></span>|
|[<span data-ttu-id="88faf-139">Clearfilters</span><span class="sxs-lookup"><span data-stu-id="88faf-139">Clearfilters</span></span>](../api/table-clearfilters.md)|<span data-ttu-id="88faf-140">无</span><span class="sxs-lookup"><span data-stu-id="88faf-140">None</span></span>|<span data-ttu-id="88faf-141">清除当前表上应用的所有筛选器。</span><span class="sxs-lookup"><span data-stu-id="88faf-141">Clears all the filters currently applied on the table.</span></span>|
|[<span data-ttu-id="88faf-142">Converttorange</span><span class="sxs-lookup"><span data-stu-id="88faf-142">Converttorange</span></span>](../api/table-converttorange.md)|[<span data-ttu-id="88faf-143">区域</span><span class="sxs-lookup"><span data-stu-id="88faf-143">Range</span></span>](range.md)|<span data-ttu-id="88faf-p101">将表转换为普通单元格区域。保留所有数据。</span><span class="sxs-lookup"><span data-stu-id="88faf-p101">Converts the table into a normal range of cells. All data is preserved.</span></span>|
|[<span data-ttu-id="88faf-146">删除</span><span class="sxs-lookup"><span data-stu-id="88faf-146">Delete</span></span>](../api/table-delete.md)|<span data-ttu-id="88faf-147">无</span><span class="sxs-lookup"><span data-stu-id="88faf-147">None</span></span>|<span data-ttu-id="88faf-148">删除表。</span><span class="sxs-lookup"><span data-stu-id="88faf-148">Deletes the table.</span></span>|
|[<span data-ttu-id="88faf-149">Reapplyfilters</span><span class="sxs-lookup"><span data-stu-id="88faf-149">Reapplyfilters</span></span>](../api/table-reapplyfilters.md)|<span data-ttu-id="88faf-150">无</span><span class="sxs-lookup"><span data-stu-id="88faf-150">None</span></span>|<span data-ttu-id="88faf-151">重新应用当前表上的所有筛选器。</span><span class="sxs-lookup"><span data-stu-id="88faf-151">Reapplies all the filters currently on the table.</span></span>|
|[<span data-ttu-id="88faf-152">List</span><span class="sxs-lookup"><span data-stu-id="88faf-152">List</span></span>](../api/table-list.md) | <span data-ttu-id="88faf-153">[WorkbookTable](table.md) 集合</span><span class="sxs-lookup"><span data-stu-id="88faf-153">[WorkbookTable](table.md) collection</span></span> |<span data-ttu-id="88faf-154">获取 table 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="88faf-154">Get table object collection.</span></span> |
|[<span data-ttu-id="88faf-155">Add</span><span class="sxs-lookup"><span data-stu-id="88faf-155">Add</span></span>](../api/tablecollection-add.md)|[<span data-ttu-id="88faf-156">WorkbookTable</span><span class="sxs-lookup"><span data-stu-id="88faf-156">WorkbookTable</span></span>](table.md)|<span data-ttu-id="88faf-p102">创建一个新表。区域源地址确定将在其下添加表的工作表。如果无法添加表（例如，由于地址无效，或者表与另一个表重叠），将抛出错误。</span><span class="sxs-lookup"><span data-stu-id="88faf-p102">Create a new table. The range source address determines the worksheet under which the table will be added. If the table cannot be added (e.g., because the address is invalid, or the table would overlap with another table), an error will be thrown.</span></span>|

## <a name="properties"></a><span data-ttu-id="88faf-160">属性</span><span class="sxs-lookup"><span data-stu-id="88faf-160">Properties</span></span>
| <span data-ttu-id="88faf-161">属性</span><span class="sxs-lookup"><span data-stu-id="88faf-161">Property</span></span>     | <span data-ttu-id="88faf-162">类型</span><span class="sxs-lookup"><span data-stu-id="88faf-162">Type</span></span>   |<span data-ttu-id="88faf-163">说明</span><span class="sxs-lookup"><span data-stu-id="88faf-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88faf-164">id</span><span class="sxs-lookup"><span data-stu-id="88faf-164">id</span></span>|<span data-ttu-id="88faf-165">string</span><span class="sxs-lookup"><span data-stu-id="88faf-165">string</span></span>|<span data-ttu-id="88faf-166">返回用于唯一标识指定工作簿中表的值。</span><span class="sxs-lookup"><span data-stu-id="88faf-166">Returns a value that uniquely identifies the table in a given workbook.</span></span> <span data-ttu-id="88faf-167">即使表被重命名，标识符的值仍保持不变。</span><span class="sxs-lookup"><span data-stu-id="88faf-167">The value of the identifier remains the same even when the table is renamed.</span></span> <span data-ttu-id="88faf-168">应将此属性解析为不透明的字符串值，不得将它解析为其他任何类型。</span><span class="sxs-lookup"><span data-stu-id="88faf-168">This property should be interpreted as an opaque string value and should not be parsed to any other type.</span></span> <span data-ttu-id="88faf-169">只读。</span><span class="sxs-lookup"><span data-stu-id="88faf-169">Read-only.</span></span>|
|<span data-ttu-id="88faf-170">name</span><span class="sxs-lookup"><span data-stu-id="88faf-170">name</span></span>|<span data-ttu-id="88faf-171">string</span><span class="sxs-lookup"><span data-stu-id="88faf-171">string</span></span>|<span data-ttu-id="88faf-172">表的名称。</span><span class="sxs-lookup"><span data-stu-id="88faf-172">Name of the table.</span></span>|
|<span data-ttu-id="88faf-173">showHeaders</span><span class="sxs-lookup"><span data-stu-id="88faf-173">showHeaders</span></span>|<span data-ttu-id="88faf-174">boolean</span><span class="sxs-lookup"><span data-stu-id="88faf-174">boolean</span></span>|<span data-ttu-id="88faf-p104">指示标头行是否可见。该值可以设置为显示或删除标头行。</span><span class="sxs-lookup"><span data-stu-id="88faf-p104">Indicates whether the header row is visible or not. This value can be set to show or remove the header row.</span></span>|
|<span data-ttu-id="88faf-177">showTotals</span><span class="sxs-lookup"><span data-stu-id="88faf-177">showTotals</span></span>|<span data-ttu-id="88faf-178">boolean</span><span class="sxs-lookup"><span data-stu-id="88faf-178">boolean</span></span>|<span data-ttu-id="88faf-p105">指示总计行是否可见。该值可以设置为显示或删除总计行。</span><span class="sxs-lookup"><span data-stu-id="88faf-p105">Indicates whether the total row is visible or not. This value can be set to show or remove the total row.</span></span>|
|<span data-ttu-id="88faf-181">style</span><span class="sxs-lookup"><span data-stu-id="88faf-181">style</span></span>|<span data-ttu-id="88faf-182">string</span><span class="sxs-lookup"><span data-stu-id="88faf-182">string</span></span>|<span data-ttu-id="88faf-183">表示表格样式的常量值。</span><span class="sxs-lookup"><span data-stu-id="88faf-183">Constant value that represents the Table style.</span></span> <span data-ttu-id="88faf-184">可取值为：TableStyleLight1 到 TableStyleLight21、TableStyleMedium1 到 TableStyleMedium28、TableStyleStyleDark1 到 TableStyleStyleDark11。</span><span class="sxs-lookup"><span data-stu-id="88faf-184">The possible values are: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11.</span></span> <span data-ttu-id="88faf-185">还可以指定工作簿中显示的用户定义的自定义样式。</span><span class="sxs-lookup"><span data-stu-id="88faf-185">A custom user-defined style present in the workbook can also be specified.</span></span>|
|<span data-ttu-id="88faf-186">highlightFirstColumn</span><span class="sxs-lookup"><span data-stu-id="88faf-186">highlightFirstColumn</span></span>|<span data-ttu-id="88faf-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="88faf-187">Boolean</span></span>|<span data-ttu-id="88faf-188">指明第一列是否包含特殊格式。</span><span class="sxs-lookup"><span data-stu-id="88faf-188">Indicates whether the first column contains special formatting.</span></span>   |
|<span data-ttu-id="88faf-189">highlightLastColumn</span><span class="sxs-lookup"><span data-stu-id="88faf-189">highlightLastColumn</span></span>|<span data-ttu-id="88faf-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="88faf-190">Boolean</span></span>|<span data-ttu-id="88faf-191">指明最后一列是否包含特殊格式。</span><span class="sxs-lookup"><span data-stu-id="88faf-191">Indicates whether the last column contains special formatting.</span></span> |
|<span data-ttu-id="88faf-192">showBandedColumns</span><span class="sxs-lookup"><span data-stu-id="88faf-192">showBandedColumns</span></span>|<span data-ttu-id="88faf-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="88faf-193">Boolean</span></span>|<span data-ttu-id="88faf-194">指明列是否采用镶边格式来以不同的方式突出显示奇数列与偶数列，让表更易于阅读。</span><span class="sxs-lookup"><span data-stu-id="88faf-194">Indicates whether the columns show banded formatting in which odd columns are highlighted differently from even ones to make reading the table easier.</span></span>   |
|<span data-ttu-id="88faf-195">showBandedRows</span><span class="sxs-lookup"><span data-stu-id="88faf-195">showBandedRows</span></span>|<span data-ttu-id="88faf-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="88faf-196">Boolean</span></span>|<span data-ttu-id="88faf-197">指明行是否采用镶边格式来以不同的方式突出显示奇数行与偶数行，让表更易于阅读。</span><span class="sxs-lookup"><span data-stu-id="88faf-197">Indicates whether the rows show banded formatting in which odd rows are highlighted differently from even ones to make reading the table easier.</span></span>    |
|<span data-ttu-id="88faf-198">showFilterButton</span><span class="sxs-lookup"><span data-stu-id="88faf-198">showFilterButton</span></span>|<span data-ttu-id="88faf-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="88faf-199">Boolean</span></span>|<span data-ttu-id="88faf-p107">指明是否在每个列标题的顶部显示筛选器按钮。仅当 table 中包含标题行时，才允许设定此设置。</span><span class="sxs-lookup"><span data-stu-id="88faf-p107">Indicates whether the filter buttons are visible at the top of each column header. Setting this is only allowed if the table contains a header row.</span></span>   |
|<span data-ttu-id="88faf-202">legacyId</span><span class="sxs-lookup"><span data-stu-id="88faf-202">legacyId</span></span>|<span data-ttu-id="88faf-203">String</span><span class="sxs-lookup"><span data-stu-id="88faf-203">String</span></span>|<span data-ttu-id="88faf-204">旧版 Excel 客户端中使用的旧 ID。</span><span class="sxs-lookup"><span data-stu-id="88faf-204">Legacy Id used in older Excle clients.</span></span> <span data-ttu-id="88faf-205">即使表格已重命名，标识符值也仍保持不变。</span><span class="sxs-lookup"><span data-stu-id="88faf-205">The value of the identifier remains the same even when the table is renamed.</span></span> <span data-ttu-id="88faf-206">应将此属性解析为不透明的字符串值，不得将它解析为其他任何类型。</span><span class="sxs-lookup"><span data-stu-id="88faf-206">This property should be interpreted as an opaque string value and should not be parsed to any other type.</span></span> <span data-ttu-id="88faf-207">只读。</span><span class="sxs-lookup"><span data-stu-id="88faf-207">Read-only.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="88faf-208">关系</span><span class="sxs-lookup"><span data-stu-id="88faf-208">Relationships</span></span>
| <span data-ttu-id="88faf-209">关系</span><span class="sxs-lookup"><span data-stu-id="88faf-209">Relationship</span></span> | <span data-ttu-id="88faf-210">类型</span><span class="sxs-lookup"><span data-stu-id="88faf-210">Type</span></span>   |<span data-ttu-id="88faf-211">说明</span><span class="sxs-lookup"><span data-stu-id="88faf-211">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88faf-212">columns</span><span class="sxs-lookup"><span data-stu-id="88faf-212">columns</span></span>|<span data-ttu-id="88faf-213">[WorkbookTableColumn](tablecolumn.md) 集合</span><span class="sxs-lookup"><span data-stu-id="88faf-213">[WorkbookTableColumn](tablecolumn.md) collection</span></span>|<span data-ttu-id="88faf-p109">表示表中所有列的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="88faf-p109">Represents a collection of all the columns in the table. Read-only.</span></span>|
|<span data-ttu-id="88faf-216">rows</span><span class="sxs-lookup"><span data-stu-id="88faf-216">rows</span></span>|<span data-ttu-id="88faf-217">[WorkbookTableRow](tablerow.md) 集合</span><span class="sxs-lookup"><span data-stu-id="88faf-217">[WorkbookTableRow](tablerow.md) collection</span></span>|<span data-ttu-id="88faf-p110">表示表中所有行的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="88faf-p110">Represents a collection of all the rows in the table. Read-only.</span></span>|
|<span data-ttu-id="88faf-220">sort</span><span class="sxs-lookup"><span data-stu-id="88faf-220">sort</span></span>|[<span data-ttu-id="88faf-221">WorkbookTableSort</span><span class="sxs-lookup"><span data-stu-id="88faf-221">WorkbookTableSort</span></span>](tablesort.md)|<span data-ttu-id="88faf-p111">表示表的排序。只读。</span><span class="sxs-lookup"><span data-stu-id="88faf-p111">Represents the sorting for the table. Read-only.</span></span>|
|<span data-ttu-id="88faf-224">worksheet</span><span class="sxs-lookup"><span data-stu-id="88faf-224">worksheet</span></span>|[<span data-ttu-id="88faf-225">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="88faf-225">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="88faf-p112">包含当前表的工作表。只读。</span><span class="sxs-lookup"><span data-stu-id="88faf-p112">The worksheet containing the current table. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="88faf-228">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="88faf-228">JSON representation</span></span>

<span data-ttu-id="88faf-229">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88faf-229">Here is a JSON representation of the resource.</span></span>

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
