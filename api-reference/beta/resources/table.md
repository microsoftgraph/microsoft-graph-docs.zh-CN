---
title: 表资源类型
description: 表示一个 Excel 表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7d1f6debdbdab3047d55bebe6fc5ec848adcb832
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956988"
---
# <a name="table-resource-type"></a><span data-ttu-id="cfd05-103">表资源类型</span><span class="sxs-lookup"><span data-stu-id="cfd05-103">Table resource type</span></span>

> <span data-ttu-id="cfd05-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cfd05-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cfd05-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cfd05-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cfd05-106">表示一个 Excel 表。</span><span class="sxs-lookup"><span data-stu-id="cfd05-106">Represents an Excel table.</span></span>

## <a name="methods"></a><span data-ttu-id="cfd05-107">方法</span><span class="sxs-lookup"><span data-stu-id="cfd05-107">Methods</span></span>

| <span data-ttu-id="cfd05-108">方法</span><span class="sxs-lookup"><span data-stu-id="cfd05-108">Method</span></span>           | <span data-ttu-id="cfd05-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="cfd05-109">Return Type</span></span>    |<span data-ttu-id="cfd05-110">说明</span><span class="sxs-lookup"><span data-stu-id="cfd05-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cfd05-111">获取表</span><span class="sxs-lookup"><span data-stu-id="cfd05-111">Get Table</span></span>](../api/table-get.md) | [<span data-ttu-id="cfd05-112">表</span><span class="sxs-lookup"><span data-stu-id="cfd05-112">Table</span></span>](table.md) |<span data-ttu-id="cfd05-113">读取 table 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cfd05-113">Read properties and relationships of table object.</span></span>|
|[<span data-ttu-id="cfd05-114">创建 TableColumn</span><span class="sxs-lookup"><span data-stu-id="cfd05-114">Create TableColumn</span></span>](../api/table-post-columns.md) |[<span data-ttu-id="cfd05-115">TableColumn</span><span class="sxs-lookup"><span data-stu-id="cfd05-115">TableColumn</span></span>](tablecolumn.md)| <span data-ttu-id="cfd05-116">通过发布到列集合创建新的 TableColumn。</span><span class="sxs-lookup"><span data-stu-id="cfd05-116">Create a new TableColumn by posting to the columns collection.</span></span>|
|[<span data-ttu-id="cfd05-117">列出列</span><span class="sxs-lookup"><span data-stu-id="cfd05-117">List columns</span></span>](../api/table-list-columns.md) |<span data-ttu-id="cfd05-118">[TableColumn](tablecolumn.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cfd05-118">[TableColumn](tablecolumn.md) collection</span></span>| <span data-ttu-id="cfd05-119">获取 TableColumn 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="cfd05-119">Get a TableColumn object collection.</span></span>|
|[<span data-ttu-id="cfd05-120">创建 TableRow</span><span class="sxs-lookup"><span data-stu-id="cfd05-120">Create TableRow</span></span>](../api/table-post-rows.md) |[<span data-ttu-id="cfd05-121">TableRow</span><span class="sxs-lookup"><span data-stu-id="cfd05-121">TableRow</span></span>](tablerow.md)| <span data-ttu-id="cfd05-122">通过发布到行集合创建新的 TableRow。</span><span class="sxs-lookup"><span data-stu-id="cfd05-122">Create a new TableRow by posting to the rows collection.</span></span>|
|[<span data-ttu-id="cfd05-123">创建行</span><span class="sxs-lookup"><span data-stu-id="cfd05-123">List rows</span></span>](../api/table-list-rows.md) |<span data-ttu-id="cfd05-124">[TableRow](tablerow.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cfd05-124">[TableRow](tablerow.md) collection</span></span>| <span data-ttu-id="cfd05-125">获取 TableRow 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="cfd05-125">Get a TableRow object collection.</span></span>|
|[<span data-ttu-id="cfd05-126">更新</span><span class="sxs-lookup"><span data-stu-id="cfd05-126">Update</span></span>](../api/table-update.md) | [<span data-ttu-id="cfd05-127">表</span><span class="sxs-lookup"><span data-stu-id="cfd05-127">Table</span></span>](table.md)   |<span data-ttu-id="cfd05-128">更新 Table 对象。</span><span class="sxs-lookup"><span data-stu-id="cfd05-128">Update Table object.</span></span> |
|[<span data-ttu-id="cfd05-129">Databodyrange</span><span class="sxs-lookup"><span data-stu-id="cfd05-129">Databodyrange</span></span>](../api/table-databodyrange.md)|[<span data-ttu-id="cfd05-130">区域</span><span class="sxs-lookup"><span data-stu-id="cfd05-130">Range</span></span>](range.md)|<span data-ttu-id="cfd05-131">获取与表的数据体相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="cfd05-131">Gets the range object associated with the data body of the table.</span></span>|
|[<span data-ttu-id="cfd05-132">Headerrowrange</span><span class="sxs-lookup"><span data-stu-id="cfd05-132">Headerrowrange</span></span>](../api/table-headerrowrange.md)|[<span data-ttu-id="cfd05-133">区域</span><span class="sxs-lookup"><span data-stu-id="cfd05-133">Range</span></span>](range.md)|<span data-ttu-id="cfd05-134">获取与表的标头行相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="cfd05-134">Gets the range object associated with header row of the table.</span></span>|
|[<span data-ttu-id="cfd05-135">区域</span><span class="sxs-lookup"><span data-stu-id="cfd05-135">Range</span></span>](../api/table-range.md)|[<span data-ttu-id="cfd05-136">Range</span><span class="sxs-lookup"><span data-stu-id="cfd05-136">Range</span></span>](range.md)|<span data-ttu-id="cfd05-137">获取与整个表相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="cfd05-137">Gets the range object associated with the entire table.</span></span>|
|[<span data-ttu-id="cfd05-138">Totalrowrange</span><span class="sxs-lookup"><span data-stu-id="cfd05-138">Totalrowrange</span></span>](../api/table-totalrowrange.md)|[<span data-ttu-id="cfd05-139">区域</span><span class="sxs-lookup"><span data-stu-id="cfd05-139">Range</span></span>](range.md)|<span data-ttu-id="cfd05-140">获取与表的总计行相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="cfd05-140">Gets the range object associated with totals row of the table.</span></span>|
|[<span data-ttu-id="cfd05-141">Clearfilters</span><span class="sxs-lookup"><span data-stu-id="cfd05-141">Clearfilters</span></span>](../api/table-clearfilters.md)|<span data-ttu-id="cfd05-142">无</span><span class="sxs-lookup"><span data-stu-id="cfd05-142">None</span></span>|<span data-ttu-id="cfd05-143">清除当前表上应用的所有筛选器。</span><span class="sxs-lookup"><span data-stu-id="cfd05-143">Clears all the filters currently applied on the table.</span></span>|
|[<span data-ttu-id="cfd05-144">Converttorange</span><span class="sxs-lookup"><span data-stu-id="cfd05-144">Converttorange</span></span>](../api/table-converttorange.md)|[<span data-ttu-id="cfd05-145">区域</span><span class="sxs-lookup"><span data-stu-id="cfd05-145">Range</span></span>](range.md)|<span data-ttu-id="cfd05-p102">将表转换为普通单元格区域。保留所有数据。</span><span class="sxs-lookup"><span data-stu-id="cfd05-p102">Converts the table into a normal range of cells. All data is preserved.</span></span>|
|[<span data-ttu-id="cfd05-148">删除</span><span class="sxs-lookup"><span data-stu-id="cfd05-148">Delete</span></span>](../api/table-delete.md)|<span data-ttu-id="cfd05-149">无</span><span class="sxs-lookup"><span data-stu-id="cfd05-149">None</span></span>|<span data-ttu-id="cfd05-150">删除表。</span><span class="sxs-lookup"><span data-stu-id="cfd05-150">Deletes the table.</span></span>|
|[<span data-ttu-id="cfd05-151">Reapplyfilters</span><span class="sxs-lookup"><span data-stu-id="cfd05-151">Reapplyfilters</span></span>](../api/table-reapplyfilters.md)|<span data-ttu-id="cfd05-152">无</span><span class="sxs-lookup"><span data-stu-id="cfd05-152">None</span></span>|<span data-ttu-id="cfd05-153">重新应用当前表上的所有筛选器。</span><span class="sxs-lookup"><span data-stu-id="cfd05-153">Reapplies all the filters currently on the table.</span></span>|
|[<span data-ttu-id="cfd05-154">列出</span><span class="sxs-lookup"><span data-stu-id="cfd05-154">List</span></span>](../api/table-list.md) | <span data-ttu-id="cfd05-155">[表](table.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cfd05-155">[Table](table.md) collection</span></span> |<span data-ttu-id="cfd05-156">获取 table 对象集合。</span><span class="sxs-lookup"><span data-stu-id="cfd05-156">Get table object collection.</span></span> |
|[<span data-ttu-id="cfd05-157">添加</span><span class="sxs-lookup"><span data-stu-id="cfd05-157">Add</span></span>](../api/tablecollection-add.md)|[<span data-ttu-id="cfd05-158">表</span><span class="sxs-lookup"><span data-stu-id="cfd05-158">Table</span></span>](table.md)|<span data-ttu-id="cfd05-p103">创建一个新表。区域源地址确定将在其下添加表的工作表。如果无法添加表（例如，由于地址无效，或者表与另一个表重叠），将抛出错误。</span><span class="sxs-lookup"><span data-stu-id="cfd05-p103">Create a new table. The range source address determines the worksheet under which the table will be added. If the table cannot be added (e.g., because the address is invalid, or the table would overlap with another table), an error will be thrown.</span></span>|

## <a name="properties"></a><span data-ttu-id="cfd05-162">属性</span><span class="sxs-lookup"><span data-stu-id="cfd05-162">Properties</span></span>
| <span data-ttu-id="cfd05-163">属性</span><span class="sxs-lookup"><span data-stu-id="cfd05-163">Property</span></span>     | <span data-ttu-id="cfd05-164">类型</span><span class="sxs-lookup"><span data-stu-id="cfd05-164">Type</span></span>   |<span data-ttu-id="cfd05-165">说明</span><span class="sxs-lookup"><span data-stu-id="cfd05-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cfd05-166">ID</span><span class="sxs-lookup"><span data-stu-id="cfd05-166">id</span></span>|<span data-ttu-id="cfd05-167">string</span><span class="sxs-lookup"><span data-stu-id="cfd05-167">string</span></span>|<span data-ttu-id="cfd05-168">返回用于唯一标识指定工作簿中表的值。</span><span class="sxs-lookup"><span data-stu-id="cfd05-168">Returns a value that uniquely identifies the table in a given workbook.</span></span> <span data-ttu-id="cfd05-169">即使表被重命名，标识符的值仍保持不变。</span><span class="sxs-lookup"><span data-stu-id="cfd05-169">The value of the identifier remains the same even when the table is renamed.</span></span> <span data-ttu-id="cfd05-170">应将此属性解析为不透明的字符串值，不得将它解析为其他任何类型。</span><span class="sxs-lookup"><span data-stu-id="cfd05-170">This property should be interpreted as an opaque string value and should not be parsed to any other type.</span></span> <span data-ttu-id="cfd05-171">只读。</span><span class="sxs-lookup"><span data-stu-id="cfd05-171">Read-only.</span></span>|
|<span data-ttu-id="cfd05-172">name</span><span class="sxs-lookup"><span data-stu-id="cfd05-172">name</span></span>|<span data-ttu-id="cfd05-173">string</span><span class="sxs-lookup"><span data-stu-id="cfd05-173">string</span></span>|<span data-ttu-id="cfd05-174">表的名称。</span><span class="sxs-lookup"><span data-stu-id="cfd05-174">Name of the table.</span></span>|
|<span data-ttu-id="cfd05-175">showHeaders</span><span class="sxs-lookup"><span data-stu-id="cfd05-175">showHeaders</span></span>|<span data-ttu-id="cfd05-176">boolean</span><span class="sxs-lookup"><span data-stu-id="cfd05-176">boolean</span></span>|<span data-ttu-id="cfd05-p105">指示标头行是否可见。该值可以设置为显示或删除标头行。</span><span class="sxs-lookup"><span data-stu-id="cfd05-p105">Indicates whether the header row is visible or not. This value can be set to show or remove the header row.</span></span>|
|<span data-ttu-id="cfd05-179">showTotals</span><span class="sxs-lookup"><span data-stu-id="cfd05-179">showTotals</span></span>|<span data-ttu-id="cfd05-180">boolean</span><span class="sxs-lookup"><span data-stu-id="cfd05-180">boolean</span></span>|<span data-ttu-id="cfd05-p106">指示总计行是否可见。该值可以设置为显示或删除总计行。</span><span class="sxs-lookup"><span data-stu-id="cfd05-p106">Indicates whether the total row is visible or not. This value can be set to show or remove the total row.</span></span>|
|<span data-ttu-id="cfd05-183">style</span><span class="sxs-lookup"><span data-stu-id="cfd05-183">style</span></span>|<span data-ttu-id="cfd05-184">string</span><span class="sxs-lookup"><span data-stu-id="cfd05-184">string</span></span>|<span data-ttu-id="cfd05-p107">表示表格样式的常量值。可能的值是：TableStyleLight1 thru TableStyleLight21、TableStyleMedium1 thru TableStyleMedium28、TableStyleStyleDark1 thru TableStyleStyleDark11。还可以指定工作簿中显示的用户定义的自定义样式。</span><span class="sxs-lookup"><span data-stu-id="cfd05-p107">Constant value that represents the Table style. Possible values are: TableStyleLight1 thru TableStyleLight21, TableStyleMedium1 thru TableStyleMedium28, TableStyleStyleDark1 thru TableStyleStyleDark11. A custom user-defined style present in the workbook can also be specified.</span></span>|
|<span data-ttu-id="cfd05-188">highlightFirstColumn</span><span class="sxs-lookup"><span data-stu-id="cfd05-188">highlightFirstColumn</span></span>|<span data-ttu-id="cfd05-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="cfd05-189">Boolean</span></span>|<span data-ttu-id="cfd05-190">指明第一列是否包含特殊格式。</span><span class="sxs-lookup"><span data-stu-id="cfd05-190">Indicates whether the first column contains special formatting.</span></span>   |
|<span data-ttu-id="cfd05-191">highlightLastColumn</span><span class="sxs-lookup"><span data-stu-id="cfd05-191">highlightLastColumn</span></span>|<span data-ttu-id="cfd05-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="cfd05-192">Boolean</span></span>|<span data-ttu-id="cfd05-193">指明最后一列是否包含特殊格式。</span><span class="sxs-lookup"><span data-stu-id="cfd05-193">Indicates whether the last column contains special formatting.</span></span> |
|<span data-ttu-id="cfd05-194">showBandedColumns</span><span class="sxs-lookup"><span data-stu-id="cfd05-194">showBandedColumns</span></span>|<span data-ttu-id="cfd05-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="cfd05-195">Boolean</span></span>|<span data-ttu-id="cfd05-196">指明列是否采用镶边格式来以不同的方式突出显示奇数列与偶数列，让表更易于阅读。</span><span class="sxs-lookup"><span data-stu-id="cfd05-196">Indicates whether the columns show banded formatting in which odd columns are highlighted differently from even ones to make reading the table easier.</span></span>   |
|<span data-ttu-id="cfd05-197">showBandedRows</span><span class="sxs-lookup"><span data-stu-id="cfd05-197">showBandedRows</span></span>|<span data-ttu-id="cfd05-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="cfd05-198">Boolean</span></span>|<span data-ttu-id="cfd05-199">指明行是否采用镶边格式来以不同的方式突出显示奇数行与偶数行，让表更易于阅读。</span><span class="sxs-lookup"><span data-stu-id="cfd05-199">Indicates whether the rows show banded formatting in which odd rows are highlighted differently from even ones to make reading the table easier.</span></span>    |
|<span data-ttu-id="cfd05-200">showFilterButton</span><span class="sxs-lookup"><span data-stu-id="cfd05-200">showFilterButton</span></span>|<span data-ttu-id="cfd05-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="cfd05-201">Boolean</span></span>|<span data-ttu-id="cfd05-p108">指明是否在每个列标题的顶部显示筛选器按钮。仅当 table 中包含标题行时，才允许设定此设置。</span><span class="sxs-lookup"><span data-stu-id="cfd05-p108">Indicates whether the filter buttons are visible at the top of each column header. Setting this is only allowed if the table contains a header row.</span></span>   |
|<span data-ttu-id="cfd05-204">legacyId</span><span class="sxs-lookup"><span data-stu-id="cfd05-204">legacyId</span></span>|<span data-ttu-id="cfd05-205">String</span><span class="sxs-lookup"><span data-stu-id="cfd05-205">String</span></span>|<span data-ttu-id="cfd05-206">旧版 Excel 客户端中使用的旧 ID。</span><span class="sxs-lookup"><span data-stu-id="cfd05-206">Legacy Id used in older Excle clients.</span></span> <span data-ttu-id="cfd05-207">即使表格已重命名，标识符值也仍保持不变。</span><span class="sxs-lookup"><span data-stu-id="cfd05-207">The value of the identifier remains the same even when the table is renamed.</span></span> <span data-ttu-id="cfd05-208">应将此属性解析为不透明的字符串值，不得将它解析为其他任何类型。</span><span class="sxs-lookup"><span data-stu-id="cfd05-208">This property should be interpreted as an opaque string value and should not be parsed to any other type.</span></span> <span data-ttu-id="cfd05-209">只读。</span><span class="sxs-lookup"><span data-stu-id="cfd05-209">Read-only.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="cfd05-210">Relationships</span><span class="sxs-lookup"><span data-stu-id="cfd05-210">Relationships</span></span>
| <span data-ttu-id="cfd05-211">关系</span><span class="sxs-lookup"><span data-stu-id="cfd05-211">Relationship</span></span> | <span data-ttu-id="cfd05-212">类型</span><span class="sxs-lookup"><span data-stu-id="cfd05-212">Type</span></span>   |<span data-ttu-id="cfd05-213">说明</span><span class="sxs-lookup"><span data-stu-id="cfd05-213">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cfd05-214">columns</span><span class="sxs-lookup"><span data-stu-id="cfd05-214">columns</span></span>|<span data-ttu-id="cfd05-215">[TableColumn](tablecolumn.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cfd05-215">[TableColumn](tablecolumn.md) collection</span></span>|<span data-ttu-id="cfd05-p110">表示表中所有列的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="cfd05-p110">Represents a collection of all the columns in the table. Read-only.</span></span>|
|<span data-ttu-id="cfd05-218">rows</span><span class="sxs-lookup"><span data-stu-id="cfd05-218">rows</span></span>|<span data-ttu-id="cfd05-219">[TableRow](tablerow.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cfd05-219">[TableRow](tablerow.md) collection</span></span>|<span data-ttu-id="cfd05-p111">表示表中所有行的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="cfd05-p111">Represents a collection of all the rows in the table. Read-only.</span></span>|
|<span data-ttu-id="cfd05-222">sort</span><span class="sxs-lookup"><span data-stu-id="cfd05-222">sort</span></span>|[<span data-ttu-id="cfd05-223">TableSort</span><span class="sxs-lookup"><span data-stu-id="cfd05-223">TableSort</span></span>](tablesort.md)|<span data-ttu-id="cfd05-p112">表示表的排序。只读。</span><span class="sxs-lookup"><span data-stu-id="cfd05-p112">Represents the sorting for the table. Read-only.</span></span>|
|<span data-ttu-id="cfd05-226">worksheet</span><span class="sxs-lookup"><span data-stu-id="cfd05-226">worksheet</span></span>|[<span data-ttu-id="cfd05-227">Worksheet</span><span class="sxs-lookup"><span data-stu-id="cfd05-227">Worksheet</span></span>](worksheet.md)|<span data-ttu-id="cfd05-p113">包含当前表的工作表。只读。</span><span class="sxs-lookup"><span data-stu-id="cfd05-p113">The worksheet containing the current table. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cfd05-230">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cfd05-230">JSON representation</span></span>

<span data-ttu-id="cfd05-231">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cfd05-231">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
     "legacyId"
  ],
  "@odata.type": "microsoft.graph.table"
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
