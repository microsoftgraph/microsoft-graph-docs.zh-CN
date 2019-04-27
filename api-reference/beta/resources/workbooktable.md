---
title: workbookTable 资源类型
description: 表示一个 Excel 表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 330b11869576dc3251b51c7239b9c0aacdc51e70
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348605"
---
# <a name="workbooktable-resource-type"></a><span data-ttu-id="53670-103">workbookTable 资源类型</span><span class="sxs-lookup"><span data-stu-id="53670-103">workbookTable resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53670-104">表示一个 Excel 表。</span><span class="sxs-lookup"><span data-stu-id="53670-104">Represents an Excel table.</span></span>

## <a name="methods"></a><span data-ttu-id="53670-105">方法</span><span class="sxs-lookup"><span data-stu-id="53670-105">Methods</span></span>

| <span data-ttu-id="53670-106">方法</span><span class="sxs-lookup"><span data-stu-id="53670-106">Method</span></span>           | <span data-ttu-id="53670-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="53670-107">Return Type</span></span>    |<span data-ttu-id="53670-108">说明</span><span class="sxs-lookup"><span data-stu-id="53670-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="53670-109">获取 workbookTable</span><span class="sxs-lookup"><span data-stu-id="53670-109">Get workbookTable</span></span>](../api/table-get.md) | [<span data-ttu-id="53670-110">workbookTable</span><span class="sxs-lookup"><span data-stu-id="53670-110">workbookTable</span></span>](workbooktable.md) |<span data-ttu-id="53670-111">读取 table 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="53670-111">Read properties and relationships of table object.</span></span>|
|[<span data-ttu-id="53670-112">创建 workbookTableColumn</span><span class="sxs-lookup"><span data-stu-id="53670-112">Create workbookTableColumn</span></span>](../api/table-post-columns.md) |[<span data-ttu-id="53670-113">workbookTableColumn</span><span class="sxs-lookup"><span data-stu-id="53670-113">workbookTableColumn</span></span>](workbooktablecolumn.md)| <span data-ttu-id="53670-114">通过发布到列集合创建新的 TableColumn。</span><span class="sxs-lookup"><span data-stu-id="53670-114">Create a new TableColumn by posting to the columns collection.</span></span>|
|[<span data-ttu-id="53670-115">List columns</span><span class="sxs-lookup"><span data-stu-id="53670-115">List columns</span></span>](../api/table-list-columns.md) |<span data-ttu-id="53670-116">[workbookTableColumn](workbooktablecolumn.md)集合</span><span class="sxs-lookup"><span data-stu-id="53670-116">[workbookTableColumn](workbooktablecolumn.md) collection</span></span>| <span data-ttu-id="53670-117">获取 TableColumn 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="53670-117">Get a TableColumn object collection.</span></span>|
|[<span data-ttu-id="53670-118">创建 workbookTableRow</span><span class="sxs-lookup"><span data-stu-id="53670-118">Create workbookTableRow</span></span>](../api/table-post-rows.md) |[<span data-ttu-id="53670-119">workbookTableRow</span><span class="sxs-lookup"><span data-stu-id="53670-119">workbookTableRow</span></span>](workbooktablerow.md)| <span data-ttu-id="53670-120">通过发布到行集合创建新的 TableRow。</span><span class="sxs-lookup"><span data-stu-id="53670-120">Create a new TableRow by posting to the rows collection.</span></span>|
|[<span data-ttu-id="53670-121">List rows</span><span class="sxs-lookup"><span data-stu-id="53670-121">List rows</span></span>](../api/table-list-rows.md) |<span data-ttu-id="53670-122">[workbookTableRow](workbooktablerow.md)集合</span><span class="sxs-lookup"><span data-stu-id="53670-122">[workbookTableRow](workbooktablerow.md) collection</span></span>| <span data-ttu-id="53670-123">获取 TableRow 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="53670-123">Get a TableRow object collection.</span></span>|
|[<span data-ttu-id="53670-124">Update</span><span class="sxs-lookup"><span data-stu-id="53670-124">Update</span></span>](../api/table-update.md) | [<span data-ttu-id="53670-125">workbookTable</span><span class="sxs-lookup"><span data-stu-id="53670-125">workbookTable</span></span>](workbooktable.md)   |<span data-ttu-id="53670-126">更新 Table 对象。</span><span class="sxs-lookup"><span data-stu-id="53670-126">Update Table object.</span></span> |
|[<span data-ttu-id="53670-127">Databodyrange</span><span class="sxs-lookup"><span data-stu-id="53670-127">Databodyrange</span></span>](../api/table-databodyrange.md)|[<span data-ttu-id="53670-128">workbookRange</span><span class="sxs-lookup"><span data-stu-id="53670-128">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="53670-129">获取与表的数据体相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="53670-129">Gets the range object associated with the data body of the table.</span></span>|
|[<span data-ttu-id="53670-130">Headerrowrange</span><span class="sxs-lookup"><span data-stu-id="53670-130">Headerrowrange</span></span>](../api/table-headerrowrange.md)|[<span data-ttu-id="53670-131">workbookRange</span><span class="sxs-lookup"><span data-stu-id="53670-131">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="53670-132">获取与表的标头行相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="53670-132">Gets the range object associated with header row of the table.</span></span>|
|[<span data-ttu-id="53670-133">区域</span><span class="sxs-lookup"><span data-stu-id="53670-133">Range</span></span>](../api/table-range.md)|[<span data-ttu-id="53670-134">workbookRange</span><span class="sxs-lookup"><span data-stu-id="53670-134">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="53670-135">获取与整个表相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="53670-135">Gets the range object associated with the entire table.</span></span>|
|[<span data-ttu-id="53670-136">Totalrowrange</span><span class="sxs-lookup"><span data-stu-id="53670-136">Totalrowrange</span></span>](../api/table-totalrowrange.md)|[<span data-ttu-id="53670-137">workbookRange</span><span class="sxs-lookup"><span data-stu-id="53670-137">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="53670-138">获取与表的总计行相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="53670-138">Gets the range object associated with totals row of the table.</span></span>|
|[<span data-ttu-id="53670-139">Clearfilters</span><span class="sxs-lookup"><span data-stu-id="53670-139">Clearfilters</span></span>](../api/table-clearfilters.md)|<span data-ttu-id="53670-140">无</span><span class="sxs-lookup"><span data-stu-id="53670-140">None</span></span>|<span data-ttu-id="53670-141">清除当前表上应用的所有筛选器。</span><span class="sxs-lookup"><span data-stu-id="53670-141">Clears all the filters currently applied on the table.</span></span>|
|[<span data-ttu-id="53670-142">Converttorange</span><span class="sxs-lookup"><span data-stu-id="53670-142">Converttorange</span></span>](../api/table-converttorange.md)|[<span data-ttu-id="53670-143">workbookRange</span><span class="sxs-lookup"><span data-stu-id="53670-143">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="53670-p101">将表转换为普通单元格区域。保留所有数据。</span><span class="sxs-lookup"><span data-stu-id="53670-p101">Converts the table into a normal range of cells. All data is preserved.</span></span>|
|[<span data-ttu-id="53670-146">删除</span><span class="sxs-lookup"><span data-stu-id="53670-146">Delete</span></span>](../api/table-delete.md)|<span data-ttu-id="53670-147">None</span><span class="sxs-lookup"><span data-stu-id="53670-147">None</span></span>|<span data-ttu-id="53670-148">删除表。</span><span class="sxs-lookup"><span data-stu-id="53670-148">Deletes the table.</span></span>|
|[<span data-ttu-id="53670-149">Reapplyfilters</span><span class="sxs-lookup"><span data-stu-id="53670-149">Reapplyfilters</span></span>](../api/table-reapplyfilters.md)|<span data-ttu-id="53670-150">无</span><span class="sxs-lookup"><span data-stu-id="53670-150">None</span></span>|<span data-ttu-id="53670-151">重新应用当前表上的所有筛选器。</span><span class="sxs-lookup"><span data-stu-id="53670-151">Reapplies all the filters currently on the table.</span></span>|
|[<span data-ttu-id="53670-152">List</span><span class="sxs-lookup"><span data-stu-id="53670-152">List</span></span>](../api/table-list.md) | <span data-ttu-id="53670-153">[workbookTable](workbooktable.md)集合</span><span class="sxs-lookup"><span data-stu-id="53670-153">[workbookTable](workbooktable.md) collection</span></span> |<span data-ttu-id="53670-154">获取 table 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="53670-154">Get table object collection.</span></span> |
|[<span data-ttu-id="53670-155">Add</span><span class="sxs-lookup"><span data-stu-id="53670-155">Add</span></span>](../api/tablecollection-add.md)|[<span data-ttu-id="53670-156">workbookTable</span><span class="sxs-lookup"><span data-stu-id="53670-156">workbookTable</span></span>](workbooktable.md)|<span data-ttu-id="53670-p102">创建一个新表。区域源地址确定将在其下添加表的工作表。如果无法添加表（例如，由于地址无效，或者表与另一个表重叠），将抛出错误。</span><span class="sxs-lookup"><span data-stu-id="53670-p102">Create a new table. The range source address determines the worksheet under which the table will be added. If the table cannot be added (e.g., because the address is invalid, or the table would overlap with another table), an error will be thrown.</span></span>|

## <a name="properties"></a><span data-ttu-id="53670-160">属性</span><span class="sxs-lookup"><span data-stu-id="53670-160">Properties</span></span>
| <span data-ttu-id="53670-161">属性</span><span class="sxs-lookup"><span data-stu-id="53670-161">Property</span></span>     | <span data-ttu-id="53670-162">类型</span><span class="sxs-lookup"><span data-stu-id="53670-162">Type</span></span>   |<span data-ttu-id="53670-163">说明</span><span class="sxs-lookup"><span data-stu-id="53670-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53670-164">id</span><span class="sxs-lookup"><span data-stu-id="53670-164">id</span></span>|<span data-ttu-id="53670-165">string</span><span class="sxs-lookup"><span data-stu-id="53670-165">string</span></span>|<span data-ttu-id="53670-166">返回用于唯一标识指定工作簿中表的值。</span><span class="sxs-lookup"><span data-stu-id="53670-166">Returns a value that uniquely identifies the table in a given workbook.</span></span> <span data-ttu-id="53670-167">即使表被重命名，标识符的值仍保持不变。</span><span class="sxs-lookup"><span data-stu-id="53670-167">The value of the identifier remains the same even when the table is renamed.</span></span> <span data-ttu-id="53670-168">应将此属性解析为不透明的字符串值，不得将它解析为其他任何类型。</span><span class="sxs-lookup"><span data-stu-id="53670-168">This property should be interpreted as an opaque string value and should not be parsed to any other type.</span></span> <span data-ttu-id="53670-169">只读。</span><span class="sxs-lookup"><span data-stu-id="53670-169">Read-only.</span></span>|
|<span data-ttu-id="53670-170">name</span><span class="sxs-lookup"><span data-stu-id="53670-170">name</span></span>|<span data-ttu-id="53670-171">string</span><span class="sxs-lookup"><span data-stu-id="53670-171">string</span></span>|<span data-ttu-id="53670-172">表的名称。</span><span class="sxs-lookup"><span data-stu-id="53670-172">Name of the table.</span></span>|
|<span data-ttu-id="53670-173">showHeaders</span><span class="sxs-lookup"><span data-stu-id="53670-173">showHeaders</span></span>|<span data-ttu-id="53670-174">布尔</span><span class="sxs-lookup"><span data-stu-id="53670-174">boolean</span></span>|<span data-ttu-id="53670-p104">指示标头行是否可见。该值可以设置为显示或删除标头行。</span><span class="sxs-lookup"><span data-stu-id="53670-p104">Indicates whether the header row is visible or not. This value can be set to show or remove the header row.</span></span>|
|<span data-ttu-id="53670-177">showTotals</span><span class="sxs-lookup"><span data-stu-id="53670-177">showTotals</span></span>|<span data-ttu-id="53670-178">boolean</span><span class="sxs-lookup"><span data-stu-id="53670-178">boolean</span></span>|<span data-ttu-id="53670-p105">指示总计行是否可见。该值可以设置为显示或删除总计行。</span><span class="sxs-lookup"><span data-stu-id="53670-p105">Indicates whether the total row is visible or not. This value can be set to show or remove the total row.</span></span>|
|<span data-ttu-id="53670-181">style</span><span class="sxs-lookup"><span data-stu-id="53670-181">style</span></span>|<span data-ttu-id="53670-182">string</span><span class="sxs-lookup"><span data-stu-id="53670-182">string</span></span>|<span data-ttu-id="53670-p106">表示表格样式的常量值。可能的值是：TableStyleLight1 thru TableStyleLight21、TableStyleMedium1 thru TableStyleMedium28、TableStyleStyleDark1 thru TableStyleStyleDark11。还可以指定工作簿中显示的用户定义的自定义样式。</span><span class="sxs-lookup"><span data-stu-id="53670-p106">Constant value that represents the Table style. Possible values are: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11. A custom user-defined style present in the workbook can also be specified.</span></span>|
|<span data-ttu-id="53670-186">highlightFirstColumn</span><span class="sxs-lookup"><span data-stu-id="53670-186">highlightFirstColumn</span></span>|<span data-ttu-id="53670-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="53670-187">Boolean</span></span>|<span data-ttu-id="53670-188">指明第一列是否包含特殊格式。</span><span class="sxs-lookup"><span data-stu-id="53670-188">Indicates whether the first column contains special formatting.</span></span>   |
|<span data-ttu-id="53670-189">highlightLastColumn</span><span class="sxs-lookup"><span data-stu-id="53670-189">highlightLastColumn</span></span>|<span data-ttu-id="53670-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="53670-190">Boolean</span></span>|<span data-ttu-id="53670-191">指明最后一列是否包含特殊格式。</span><span class="sxs-lookup"><span data-stu-id="53670-191">Indicates whether the last column contains special formatting.</span></span> |
|<span data-ttu-id="53670-192">showBandedColumns</span><span class="sxs-lookup"><span data-stu-id="53670-192">showBandedColumns</span></span>|<span data-ttu-id="53670-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="53670-193">Boolean</span></span>|<span data-ttu-id="53670-194">指明列是否采用镶边格式来以不同的方式突出显示奇数列与偶数列，让表更易于阅读。</span><span class="sxs-lookup"><span data-stu-id="53670-194">Indicates whether the columns show banded formatting in which odd columns are highlighted differently from even ones to make reading the table easier.</span></span>   |
|<span data-ttu-id="53670-195">showBandedRows</span><span class="sxs-lookup"><span data-stu-id="53670-195">showBandedRows</span></span>|<span data-ttu-id="53670-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="53670-196">Boolean</span></span>|<span data-ttu-id="53670-197">指明行是否采用镶边格式来以不同的方式突出显示奇数行与偶数行，让表更易于阅读。</span><span class="sxs-lookup"><span data-stu-id="53670-197">Indicates whether the rows show banded formatting in which odd rows are highlighted differently from even ones to make reading the table easier.</span></span>    |
|<span data-ttu-id="53670-198">showFilterButton</span><span class="sxs-lookup"><span data-stu-id="53670-198">showFilterButton</span></span>|<span data-ttu-id="53670-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="53670-199">Boolean</span></span>|<span data-ttu-id="53670-p107">指明是否在每个列标题的顶部显示筛选器按钮。仅当 table 中包含标题行时，才允许设定此设置。</span><span class="sxs-lookup"><span data-stu-id="53670-p107">Indicates whether the filter buttons are visible at the top of each column header. Setting this is only allowed if the table contains a header row.</span></span>   |
|<span data-ttu-id="53670-202">legacyId</span><span class="sxs-lookup"><span data-stu-id="53670-202">legacyId</span></span>|<span data-ttu-id="53670-203">String</span><span class="sxs-lookup"><span data-stu-id="53670-203">String</span></span>|<span data-ttu-id="53670-204">旧版 Excel 客户端中使用的旧 ID。</span><span class="sxs-lookup"><span data-stu-id="53670-204">Legacy Id used in older Excle clients.</span></span> <span data-ttu-id="53670-205">即使表格已重命名，标识符值也仍保持不变。</span><span class="sxs-lookup"><span data-stu-id="53670-205">The value of the identifier remains the same even when the table is renamed.</span></span> <span data-ttu-id="53670-206">应将此属性解析为不透明的字符串值，不得将它解析为其他任何类型。</span><span class="sxs-lookup"><span data-stu-id="53670-206">This property should be interpreted as an opaque string value and should not be parsed to any other type.</span></span> <span data-ttu-id="53670-207">只读。</span><span class="sxs-lookup"><span data-stu-id="53670-207">Read-only.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="53670-208">关系</span><span class="sxs-lookup"><span data-stu-id="53670-208">Relationships</span></span>
| <span data-ttu-id="53670-209">关系</span><span class="sxs-lookup"><span data-stu-id="53670-209">Relationship</span></span> | <span data-ttu-id="53670-210">类型</span><span class="sxs-lookup"><span data-stu-id="53670-210">Type</span></span>   |<span data-ttu-id="53670-211">说明</span><span class="sxs-lookup"><span data-stu-id="53670-211">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53670-212">columns</span><span class="sxs-lookup"><span data-stu-id="53670-212">columns</span></span>|<span data-ttu-id="53670-213">[workbookTableColumn](workbooktablecolumn.md)集合</span><span class="sxs-lookup"><span data-stu-id="53670-213">[workbookTableColumn](workbooktablecolumn.md) collection</span></span>|<span data-ttu-id="53670-p109">表示表中所有列的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="53670-p109">Represents a collection of all the columns in the table. Read-only.</span></span>|
|<span data-ttu-id="53670-216">rows</span><span class="sxs-lookup"><span data-stu-id="53670-216">rows</span></span>|<span data-ttu-id="53670-217">[workbookTableRow](workbooktablerow.md)集合</span><span class="sxs-lookup"><span data-stu-id="53670-217">[workbookTableRow](workbooktablerow.md) collection</span></span>|<span data-ttu-id="53670-p110">表示表中所有行的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="53670-p110">Represents a collection of all the rows in the table. Read-only.</span></span>|
|<span data-ttu-id="53670-220">sort</span><span class="sxs-lookup"><span data-stu-id="53670-220">sort</span></span>|[<span data-ttu-id="53670-221">workbookTableSort</span><span class="sxs-lookup"><span data-stu-id="53670-221">workbookTableSort</span></span>](workbooktablesort.md)|<span data-ttu-id="53670-p111">表示表的排序。只读。</span><span class="sxs-lookup"><span data-stu-id="53670-p111">Represents the sorting for the table. Read-only.</span></span>|
|<span data-ttu-id="53670-224">worksheet</span><span class="sxs-lookup"><span data-stu-id="53670-224">worksheet</span></span>|[<span data-ttu-id="53670-225">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="53670-225">workbookWorksheet</span></span>](workbookworksheet.md)|<span data-ttu-id="53670-p112">包含当前表的工作表。只读。</span><span class="sxs-lookup"><span data-stu-id="53670-p112">The worksheet containing the current table. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="53670-228">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="53670-228">JSON representation</span></span>

<span data-ttu-id="53670-229">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53670-229">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
     "legacyId"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
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
<!--
{
  "type": "#page.annotation",
  "description": "Table resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
