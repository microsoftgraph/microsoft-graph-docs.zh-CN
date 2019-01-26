---
title: 表资源类型
description: 表示 Excel 表格。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a136d7bac22a127ada69c27c656cbded7f5302b5
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572680"
---
# <a name="table-resource-type"></a><span data-ttu-id="5dfea-103">表资源类型</span><span class="sxs-lookup"><span data-stu-id="5dfea-103">Table resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5dfea-104">表示一个 Excel 表。</span><span class="sxs-lookup"><span data-stu-id="5dfea-104">Represents an Excel table.</span></span>

## <a name="methods"></a><span data-ttu-id="5dfea-105">方法</span><span class="sxs-lookup"><span data-stu-id="5dfea-105">Methods</span></span>

| <span data-ttu-id="5dfea-106">方法</span><span class="sxs-lookup"><span data-stu-id="5dfea-106">Method</span></span>           | <span data-ttu-id="5dfea-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="5dfea-107">Return Type</span></span>    |<span data-ttu-id="5dfea-108">说明</span><span class="sxs-lookup"><span data-stu-id="5dfea-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5dfea-109">Get Table</span><span class="sxs-lookup"><span data-stu-id="5dfea-109">Get Table</span></span>](../api/table-get.md) | [<span data-ttu-id="5dfea-110">表</span><span class="sxs-lookup"><span data-stu-id="5dfea-110">Table</span></span>](table.md) |<span data-ttu-id="5dfea-111">读取 table 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5dfea-111">Read properties and relationships of table object.</span></span>|
|[<span data-ttu-id="5dfea-112">Create TableColumn</span><span class="sxs-lookup"><span data-stu-id="5dfea-112">Create TableColumn</span></span>](../api/table-post-columns.md) |[<span data-ttu-id="5dfea-113">TableColumn</span><span class="sxs-lookup"><span data-stu-id="5dfea-113">TableColumn</span></span>](tablecolumn.md)| <span data-ttu-id="5dfea-114">通过发布到列集合创建新的 TableColumn。</span><span class="sxs-lookup"><span data-stu-id="5dfea-114">Create a new TableColumn by posting to the columns collection.</span></span>|
|[<span data-ttu-id="5dfea-115">List columns</span><span class="sxs-lookup"><span data-stu-id="5dfea-115">List columns</span></span>](../api/table-list-columns.md) |<span data-ttu-id="5dfea-116">[TableColumn](tablecolumn.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5dfea-116">[TableColumn](tablecolumn.md) collection</span></span>| <span data-ttu-id="5dfea-117">获取 TableColumn 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="5dfea-117">Get a TableColumn object collection.</span></span>|
|[<span data-ttu-id="5dfea-118">Create TableRow</span><span class="sxs-lookup"><span data-stu-id="5dfea-118">Create TableRow</span></span>](../api/table-post-rows.md) |[<span data-ttu-id="5dfea-119">TableRow</span><span class="sxs-lookup"><span data-stu-id="5dfea-119">TableRow</span></span>](tablerow.md)| <span data-ttu-id="5dfea-120">通过发布到行集合创建新的 TableRow。</span><span class="sxs-lookup"><span data-stu-id="5dfea-120">Create a new TableRow by posting to the rows collection.</span></span>|
|[<span data-ttu-id="5dfea-121">List rows</span><span class="sxs-lookup"><span data-stu-id="5dfea-121">List rows</span></span>](../api/table-list-rows.md) |<span data-ttu-id="5dfea-122">[TableRow](tablerow.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5dfea-122">[TableRow](tablerow.md) collection</span></span>| <span data-ttu-id="5dfea-123">获取 TableRow 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="5dfea-123">Get a TableRow object collection.</span></span>|
|[<span data-ttu-id="5dfea-124">Update</span><span class="sxs-lookup"><span data-stu-id="5dfea-124">Update</span></span>](../api/table-update.md) | [<span data-ttu-id="5dfea-125">表</span><span class="sxs-lookup"><span data-stu-id="5dfea-125">Table</span></span>](table.md)   |<span data-ttu-id="5dfea-126">更新 Table 对象。</span><span class="sxs-lookup"><span data-stu-id="5dfea-126">Update Table object.</span></span> |
|[<span data-ttu-id="5dfea-127">Databodyrange</span><span class="sxs-lookup"><span data-stu-id="5dfea-127">Databodyrange</span></span>](../api/table-databodyrange.md)|[<span data-ttu-id="5dfea-128">区域</span><span class="sxs-lookup"><span data-stu-id="5dfea-128">Range</span></span>](range.md)|<span data-ttu-id="5dfea-129">获取与表的数据体相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="5dfea-129">Gets the range object associated with the data body of the table.</span></span>|
|[<span data-ttu-id="5dfea-130">Headerrowrange</span><span class="sxs-lookup"><span data-stu-id="5dfea-130">Headerrowrange</span></span>](../api/table-headerrowrange.md)|[<span data-ttu-id="5dfea-131">区域</span><span class="sxs-lookup"><span data-stu-id="5dfea-131">Range</span></span>](range.md)|<span data-ttu-id="5dfea-132">获取与表的标头行相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="5dfea-132">Gets the range object associated with header row of the table.</span></span>|
|[<span data-ttu-id="5dfea-133">区域</span><span class="sxs-lookup"><span data-stu-id="5dfea-133">Range</span></span>](../api/table-range.md)|[<span data-ttu-id="5dfea-134">区域</span><span class="sxs-lookup"><span data-stu-id="5dfea-134">Range</span></span>](range.md)|<span data-ttu-id="5dfea-135">获取与整个表相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="5dfea-135">Gets the range object associated with the entire table.</span></span>|
|[<span data-ttu-id="5dfea-136">Totalrowrange</span><span class="sxs-lookup"><span data-stu-id="5dfea-136">Totalrowrange</span></span>](../api/table-totalrowrange.md)|[<span data-ttu-id="5dfea-137">区域</span><span class="sxs-lookup"><span data-stu-id="5dfea-137">Range</span></span>](range.md)|<span data-ttu-id="5dfea-138">获取与表的总计行相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="5dfea-138">Gets the range object associated with totals row of the table.</span></span>|
|[<span data-ttu-id="5dfea-139">Clearfilters</span><span class="sxs-lookup"><span data-stu-id="5dfea-139">Clearfilters</span></span>](../api/table-clearfilters.md)|<span data-ttu-id="5dfea-140">无</span><span class="sxs-lookup"><span data-stu-id="5dfea-140">None</span></span>|<span data-ttu-id="5dfea-141">清除当前表上应用的所有筛选器。</span><span class="sxs-lookup"><span data-stu-id="5dfea-141">Clears all the filters currently applied on the table.</span></span>|
|[<span data-ttu-id="5dfea-142">Converttorange</span><span class="sxs-lookup"><span data-stu-id="5dfea-142">Converttorange</span></span>](../api/table-converttorange.md)|[<span data-ttu-id="5dfea-143">区域</span><span class="sxs-lookup"><span data-stu-id="5dfea-143">Range</span></span>](range.md)|<span data-ttu-id="5dfea-p101">将表转换为普通单元格区域。保留所有数据。</span><span class="sxs-lookup"><span data-stu-id="5dfea-p101">Converts the table into a normal range of cells. All data is preserved.</span></span>|
|[<span data-ttu-id="5dfea-146">删除</span><span class="sxs-lookup"><span data-stu-id="5dfea-146">Delete</span></span>](../api/table-delete.md)|<span data-ttu-id="5dfea-147">无</span><span class="sxs-lookup"><span data-stu-id="5dfea-147">None</span></span>|<span data-ttu-id="5dfea-148">删除表。</span><span class="sxs-lookup"><span data-stu-id="5dfea-148">Deletes the table.</span></span>|
|[<span data-ttu-id="5dfea-149">Reapplyfilters</span><span class="sxs-lookup"><span data-stu-id="5dfea-149">Reapplyfilters</span></span>](../api/table-reapplyfilters.md)|<span data-ttu-id="5dfea-150">无</span><span class="sxs-lookup"><span data-stu-id="5dfea-150">None</span></span>|<span data-ttu-id="5dfea-151">重新应用当前表上的所有筛选器。</span><span class="sxs-lookup"><span data-stu-id="5dfea-151">Reapplies all the filters currently on the table.</span></span>|
|[<span data-ttu-id="5dfea-152">List</span><span class="sxs-lookup"><span data-stu-id="5dfea-152">List</span></span>](../api/table-list.md) | <span data-ttu-id="5dfea-153">[表](table.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5dfea-153">[Table](table.md) collection</span></span> |<span data-ttu-id="5dfea-154">获取 table 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="5dfea-154">Get table object collection.</span></span> |
|[<span data-ttu-id="5dfea-155">Add</span><span class="sxs-lookup"><span data-stu-id="5dfea-155">Add</span></span>](../api/tablecollection-add.md)|[<span data-ttu-id="5dfea-156">表</span><span class="sxs-lookup"><span data-stu-id="5dfea-156">Table</span></span>](table.md)|<span data-ttu-id="5dfea-p102">创建一个新表。区域源地址确定将在其下添加表的工作表。如果无法添加表（例如，由于地址无效，或者表与另一个表重叠），将抛出错误。</span><span class="sxs-lookup"><span data-stu-id="5dfea-p102">Create a new table. The range source address determines the worksheet under which the table will be added. If the table cannot be added (e.g., because the address is invalid, or the table would overlap with another table), an error will be thrown.</span></span>|

## <a name="properties"></a><span data-ttu-id="5dfea-160">属性</span><span class="sxs-lookup"><span data-stu-id="5dfea-160">Properties</span></span>
| <span data-ttu-id="5dfea-161">属性</span><span class="sxs-lookup"><span data-stu-id="5dfea-161">Property</span></span>     | <span data-ttu-id="5dfea-162">类型</span><span class="sxs-lookup"><span data-stu-id="5dfea-162">Type</span></span>   |<span data-ttu-id="5dfea-163">说明</span><span class="sxs-lookup"><span data-stu-id="5dfea-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5dfea-164">id</span><span class="sxs-lookup"><span data-stu-id="5dfea-164">id</span></span>|<span data-ttu-id="5dfea-165">string</span><span class="sxs-lookup"><span data-stu-id="5dfea-165">string</span></span>|<span data-ttu-id="5dfea-166">返回用于唯一标识指定工作簿中表的值。</span><span class="sxs-lookup"><span data-stu-id="5dfea-166">Returns a value that uniquely identifies the table in a given workbook.</span></span> <span data-ttu-id="5dfea-167">即使表被重命名，标识符的值仍保持不变。</span><span class="sxs-lookup"><span data-stu-id="5dfea-167">The value of the identifier remains the same even when the table is renamed.</span></span> <span data-ttu-id="5dfea-168">应将此属性解析为不透明的字符串值，不得将它解析为其他任何类型。</span><span class="sxs-lookup"><span data-stu-id="5dfea-168">This property should be interpreted as an opaque string value and should not be parsed to any other type.</span></span> <span data-ttu-id="5dfea-169">只读。</span><span class="sxs-lookup"><span data-stu-id="5dfea-169">Read-only.</span></span>|
|<span data-ttu-id="5dfea-170">name</span><span class="sxs-lookup"><span data-stu-id="5dfea-170">name</span></span>|<span data-ttu-id="5dfea-171">string</span><span class="sxs-lookup"><span data-stu-id="5dfea-171">string</span></span>|<span data-ttu-id="5dfea-172">表的名称。</span><span class="sxs-lookup"><span data-stu-id="5dfea-172">Name of the table.</span></span>|
|<span data-ttu-id="5dfea-173">showHeaders</span><span class="sxs-lookup"><span data-stu-id="5dfea-173">showHeaders</span></span>|<span data-ttu-id="5dfea-174">boolean</span><span class="sxs-lookup"><span data-stu-id="5dfea-174">boolean</span></span>|<span data-ttu-id="5dfea-p104">指示标头行是否可见。该值可以设置为显示或删除标头行。</span><span class="sxs-lookup"><span data-stu-id="5dfea-p104">Indicates whether the header row is visible or not. This value can be set to show or remove the header row.</span></span>|
|<span data-ttu-id="5dfea-177">showTotals</span><span class="sxs-lookup"><span data-stu-id="5dfea-177">showTotals</span></span>|<span data-ttu-id="5dfea-178">boolean</span><span class="sxs-lookup"><span data-stu-id="5dfea-178">boolean</span></span>|<span data-ttu-id="5dfea-p105">指示总计行是否可见。该值可以设置为显示或删除总计行。</span><span class="sxs-lookup"><span data-stu-id="5dfea-p105">Indicates whether the total row is visible or not. This value can be set to show or remove the total row.</span></span>|
|<span data-ttu-id="5dfea-181">style</span><span class="sxs-lookup"><span data-stu-id="5dfea-181">style</span></span>|<span data-ttu-id="5dfea-182">string</span><span class="sxs-lookup"><span data-stu-id="5dfea-182">string</span></span>|<span data-ttu-id="5dfea-p106">表示表格样式的常量值。可能的值是：TableStyleLight1 thru TableStyleLight21、TableStyleMedium1 thru TableStyleMedium28、TableStyleStyleDark1 thru TableStyleStyleDark11。还可以指定工作簿中显示的用户定义的自定义样式。</span><span class="sxs-lookup"><span data-stu-id="5dfea-p106">Constant value that represents the Table style. Possible values are: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11. A custom user-defined style present in the workbook can also be specified.</span></span>|
|<span data-ttu-id="5dfea-186">highlightFirstColumn</span><span class="sxs-lookup"><span data-stu-id="5dfea-186">highlightFirstColumn</span></span>|<span data-ttu-id="5dfea-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="5dfea-187">Boolean</span></span>|<span data-ttu-id="5dfea-188">指明第一列是否包含特殊格式。</span><span class="sxs-lookup"><span data-stu-id="5dfea-188">Indicates whether the first column contains special formatting.</span></span>   |
|<span data-ttu-id="5dfea-189">highlightLastColumn</span><span class="sxs-lookup"><span data-stu-id="5dfea-189">highlightLastColumn</span></span>|<span data-ttu-id="5dfea-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="5dfea-190">Boolean</span></span>|<span data-ttu-id="5dfea-191">指明最后一列是否包含特殊格式。</span><span class="sxs-lookup"><span data-stu-id="5dfea-191">Indicates whether the last column contains special formatting.</span></span> |
|<span data-ttu-id="5dfea-192">showBandedColumns</span><span class="sxs-lookup"><span data-stu-id="5dfea-192">showBandedColumns</span></span>|<span data-ttu-id="5dfea-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="5dfea-193">Boolean</span></span>|<span data-ttu-id="5dfea-194">指明列是否采用镶边格式来以不同的方式突出显示奇数列与偶数列，让表更易于阅读。</span><span class="sxs-lookup"><span data-stu-id="5dfea-194">Indicates whether the columns show banded formatting in which odd columns are highlighted differently from even ones to make reading the table easier.</span></span>   |
|<span data-ttu-id="5dfea-195">showBandedRows</span><span class="sxs-lookup"><span data-stu-id="5dfea-195">showBandedRows</span></span>|<span data-ttu-id="5dfea-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="5dfea-196">Boolean</span></span>|<span data-ttu-id="5dfea-197">指明行是否采用镶边格式来以不同的方式突出显示奇数行与偶数行，让表更易于阅读。</span><span class="sxs-lookup"><span data-stu-id="5dfea-197">Indicates whether the rows show banded formatting in which odd rows are highlighted differently from even ones to make reading the table easier.</span></span>    |
|<span data-ttu-id="5dfea-198">showFilterButton</span><span class="sxs-lookup"><span data-stu-id="5dfea-198">showFilterButton</span></span>|<span data-ttu-id="5dfea-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="5dfea-199">Boolean</span></span>|<span data-ttu-id="5dfea-p107">指明是否在每个列标题的顶部显示筛选器按钮。仅当 table 中包含标题行时，才允许设定此设置。</span><span class="sxs-lookup"><span data-stu-id="5dfea-p107">Indicates whether the filter buttons are visible at the top of each column header. Setting this is only allowed if the table contains a header row.</span></span>   |
|<span data-ttu-id="5dfea-202">legacyId</span><span class="sxs-lookup"><span data-stu-id="5dfea-202">legacyId</span></span>|<span data-ttu-id="5dfea-203">String</span><span class="sxs-lookup"><span data-stu-id="5dfea-203">String</span></span>|<span data-ttu-id="5dfea-204">旧版 Excel 客户端中使用的旧 ID。</span><span class="sxs-lookup"><span data-stu-id="5dfea-204">Legacy Id used in older Excle clients.</span></span> <span data-ttu-id="5dfea-205">即使表格已重命名，标识符值也仍保持不变。</span><span class="sxs-lookup"><span data-stu-id="5dfea-205">The value of the identifier remains the same even when the table is renamed.</span></span> <span data-ttu-id="5dfea-206">应将此属性解析为不透明的字符串值，不得将它解析为其他任何类型。</span><span class="sxs-lookup"><span data-stu-id="5dfea-206">This property should be interpreted as an opaque string value and should not be parsed to any other type.</span></span> <span data-ttu-id="5dfea-207">只读。</span><span class="sxs-lookup"><span data-stu-id="5dfea-207">Read-only.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="5dfea-208">关系</span><span class="sxs-lookup"><span data-stu-id="5dfea-208">Relationships</span></span>
| <span data-ttu-id="5dfea-209">关系</span><span class="sxs-lookup"><span data-stu-id="5dfea-209">Relationship</span></span> | <span data-ttu-id="5dfea-210">类型</span><span class="sxs-lookup"><span data-stu-id="5dfea-210">Type</span></span>   |<span data-ttu-id="5dfea-211">说明</span><span class="sxs-lookup"><span data-stu-id="5dfea-211">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5dfea-212">columns</span><span class="sxs-lookup"><span data-stu-id="5dfea-212">columns</span></span>|<span data-ttu-id="5dfea-213">[tableColumn](tablecolumn.md)集合</span><span class="sxs-lookup"><span data-stu-id="5dfea-213">[tableColumn](tablecolumn.md) collection</span></span>|<span data-ttu-id="5dfea-p109">表示表中所有列的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="5dfea-p109">Represents a collection of all the columns in the table. Read-only.</span></span>|
|<span data-ttu-id="5dfea-216">rows</span><span class="sxs-lookup"><span data-stu-id="5dfea-216">rows</span></span>|<span data-ttu-id="5dfea-217">[tableRow](tablerow.md)集合</span><span class="sxs-lookup"><span data-stu-id="5dfea-217">[tableRow](tablerow.md) collection</span></span>|<span data-ttu-id="5dfea-p110">表示表中所有行的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="5dfea-p110">Represents a collection of all the rows in the table. Read-only.</span></span>|
|<span data-ttu-id="5dfea-220">sort</span><span class="sxs-lookup"><span data-stu-id="5dfea-220">sort</span></span>|[<span data-ttu-id="5dfea-221">tableSort</span><span class="sxs-lookup"><span data-stu-id="5dfea-221">tableSort</span></span>](tablesort.md)|<span data-ttu-id="5dfea-p111">表示表的排序。只读。</span><span class="sxs-lookup"><span data-stu-id="5dfea-p111">Represents the sorting for the table. Read-only.</span></span>|
|<span data-ttu-id="5dfea-224">worksheet</span><span class="sxs-lookup"><span data-stu-id="5dfea-224">worksheet</span></span>|[<span data-ttu-id="5dfea-225">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="5dfea-225">workbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="5dfea-p112">包含当前表的工作表。只读。</span><span class="sxs-lookup"><span data-stu-id="5dfea-p112">The worksheet containing the current table. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5dfea-228">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5dfea-228">JSON representation</span></span>

<span data-ttu-id="5dfea-229">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5dfea-229">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
     "legacyId"
  ],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/table.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
