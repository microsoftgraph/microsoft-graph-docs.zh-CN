---
title: 工作表资源类型
description: Excel 工作表是由单元格组成的网格。 它可以包含数据、表、图表等。
localization_priority: Priority
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ded792f69573b4434e4157d7c665471683273169
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033318"
---
# <a name="worksheet-resource-type"></a><span data-ttu-id="cd6a7-104">工作表资源类型</span><span class="sxs-lookup"><span data-stu-id="cd6a7-104">Worksheet resource type</span></span>

<span data-ttu-id="cd6a7-105">Excel 工作表是由单元格组成的网格。</span><span class="sxs-lookup"><span data-stu-id="cd6a7-105">An Excel worksheet is a grid of cells.</span></span> <span data-ttu-id="cd6a7-106">它可以包含数据、表、图表等。</span><span class="sxs-lookup"><span data-stu-id="cd6a7-106">It can contain data, tables, charts, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="cd6a7-107">方法</span><span class="sxs-lookup"><span data-stu-id="cd6a7-107">Methods</span></span>

| <span data-ttu-id="cd6a7-108">方法</span><span class="sxs-lookup"><span data-stu-id="cd6a7-108">Method</span></span>           | <span data-ttu-id="cd6a7-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="cd6a7-109">Return Type</span></span>    |<span data-ttu-id="cd6a7-110">说明</span><span class="sxs-lookup"><span data-stu-id="cd6a7-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cd6a7-111">获取工作表</span><span class="sxs-lookup"><span data-stu-id="cd6a7-111">Get Worksheet</span></span>](../api/worksheet-get.md) | [<span data-ttu-id="cd6a7-112">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="cd6a7-112">WorkbookWorksheet</span></span>](worksheet.md) |<span data-ttu-id="cd6a7-113">读取 worksheet 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cd6a7-113">Read properties and relationships of worksheet object.</span></span>|
|[<span data-ttu-id="cd6a7-114">创建图表</span><span class="sxs-lookup"><span data-stu-id="cd6a7-114">Create Chart</span></span>](../api/worksheet-post-charts.md) |[<span data-ttu-id="cd6a7-115">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="cd6a7-115">WorkbookChart</span></span>](chart.md)| <span data-ttu-id="cd6a7-116">通过发布到图表集合创建新的图表。</span><span class="sxs-lookup"><span data-stu-id="cd6a7-116">Create a new Chart by posting to the charts collection.</span></span>|
|[<span data-ttu-id="cd6a7-117">列出名称</span><span class="sxs-lookup"><span data-stu-id="cd6a7-117">List names</span></span>](../api/worksheet-list-names.md) |<span data-ttu-id="cd6a7-118">[WorkbookNamedItem](nameditem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cd6a7-118">[WorkbookNamedItem](nameditem.md) collection</span></span>| <span data-ttu-id="cd6a7-119">获取与工作表关联的命名项的集合。</span><span class="sxs-lookup"><span data-stu-id="cd6a7-119">Get named item collection associated with the worksheet.</span></span>|
|[<span data-ttu-id="cd6a7-120">列出图表</span><span class="sxs-lookup"><span data-stu-id="cd6a7-120">List charts</span></span>](../api/worksheet-list-charts.md) |<span data-ttu-id="cd6a7-121">[WorkbookChart](chart.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cd6a7-121">[WorkbookChart](chart.md) collection</span></span>| <span data-ttu-id="cd6a7-122">获取 Chart 对象集合。</span><span class="sxs-lookup"><span data-stu-id="cd6a7-122">Get a Chart object collection.</span></span>|
|[<span data-ttu-id="cd6a7-123">创建表</span><span class="sxs-lookup"><span data-stu-id="cd6a7-123">Create Table</span></span>](../api/worksheet-post-tables.md) |[<span data-ttu-id="cd6a7-124">WorkbookTable</span><span class="sxs-lookup"><span data-stu-id="cd6a7-124">WorkbookTable</span></span>](table.md)| <span data-ttu-id="cd6a7-125">通过发布到表集合创建新表。</span><span class="sxs-lookup"><span data-stu-id="cd6a7-125">Create a new Table by posting to the tables collection.</span></span>|
|[<span data-ttu-id="cd6a7-126">列出表</span><span class="sxs-lookup"><span data-stu-id="cd6a7-126">List tables</span></span>](../api/worksheet-list-tables.md) |<span data-ttu-id="cd6a7-127">[WorkbookTable](table.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cd6a7-127">[WorkbookTable](table.md) collection</span></span>| <span data-ttu-id="cd6a7-128">获取 Table 对象集合。</span><span class="sxs-lookup"><span data-stu-id="cd6a7-128">Get a Table object collection.</span></span>|
|[<span data-ttu-id="cd6a7-129">更新</span><span class="sxs-lookup"><span data-stu-id="cd6a7-129">Update</span></span>](../api/worksheet-update.md) | [<span data-ttu-id="cd6a7-130">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="cd6a7-130">WorkbookWorksheet</span></span>](worksheet.md)   |<span data-ttu-id="cd6a7-131">更新 Worksheet 对象。</span><span class="sxs-lookup"><span data-stu-id="cd6a7-131">Update Worksheet object.</span></span> |
|[<span data-ttu-id="cd6a7-132">单元格</span><span class="sxs-lookup"><span data-stu-id="cd6a7-132">Cell</span></span>](../api/worksheet-cell.md)|[<span data-ttu-id="cd6a7-133">区域</span><span class="sxs-lookup"><span data-stu-id="cd6a7-133">Range</span></span>](range.md)|<span data-ttu-id="cd6a7-p103">根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。</span><span class="sxs-lookup"><span data-stu-id="cd6a7-p103">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>|
|[<span data-ttu-id="cd6a7-136">区域</span><span class="sxs-lookup"><span data-stu-id="cd6a7-136">Range</span></span>](../api/worksheet-range.md)|[<span data-ttu-id="cd6a7-137">区域</span><span class="sxs-lookup"><span data-stu-id="cd6a7-137">Range</span></span>](range.md)|<span data-ttu-id="cd6a7-138">获取地址或名称指定的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="cd6a7-138">Gets the range object specified by the address or name.</span></span>|
|[<span data-ttu-id="cd6a7-139">Usedrange</span><span class="sxs-lookup"><span data-stu-id="cd6a7-139">Usedrange</span></span>](../api/worksheet-usedrange.md)|[<span data-ttu-id="cd6a7-140">区域</span><span class="sxs-lookup"><span data-stu-id="cd6a7-140">Range</span></span>](range.md)|<span data-ttu-id="cd6a7-p104">使用的区域是包含分配了值或格式化的任何单元格的最小区域。如果工作表为空，此函数将返回左上角的单元格。</span><span class="sxs-lookup"><span data-stu-id="cd6a7-p104">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>|
|[<span data-ttu-id="cd6a7-143">删除</span><span class="sxs-lookup"><span data-stu-id="cd6a7-143">Delete</span></span>](../api/worksheet-delete.md)|<span data-ttu-id="cd6a7-144">无</span><span class="sxs-lookup"><span data-stu-id="cd6a7-144">None</span></span>|<span data-ttu-id="cd6a7-145">从工作簿中删除工作表。</span><span class="sxs-lookup"><span data-stu-id="cd6a7-145">Deletes the worksheet from the workbook.</span></span>|
|[<span data-ttu-id="cd6a7-146">List</span><span class="sxs-lookup"><span data-stu-id="cd6a7-146">List</span></span>](../api/worksheet-list.md) | <span data-ttu-id="cd6a7-147">[WorkbookWorksheet](worksheet.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cd6a7-147">[WorkbookWorksheet](worksheet.md) collection</span></span> |<span data-ttu-id="cd6a7-148">获取 worksheet 对象集合。</span><span class="sxs-lookup"><span data-stu-id="cd6a7-148">Get worksheet object collection.</span></span> |
|[<span data-ttu-id="cd6a7-149">Add</span><span class="sxs-lookup"><span data-stu-id="cd6a7-149">Add</span></span>](../api/worksheetcollection-add.md)|[<span data-ttu-id="cd6a7-150">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="cd6a7-150">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="cd6a7-p105">向工作簿添加新工作表。将工作表添加到现有工作表的末尾。</span><span class="sxs-lookup"><span data-stu-id="cd6a7-p105">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets.</span></span> |
|[<span data-ttu-id="cd6a7-153">List pivotTables</span><span class="sxs-lookup"><span data-stu-id="cd6a7-153">List pivotTables</span></span>](../api/workbookworksheet-list-pivottables.md) |<span data-ttu-id="cd6a7-154">[workbookPivotTable](workbookpivottable.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cd6a7-154">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="cd6a7-155">获取一组 workbookPivotTable 对象。</span><span class="sxs-lookup"><span data-stu-id="cd6a7-155">Get a workbookPivotTable object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="cd6a7-156">属性</span><span class="sxs-lookup"><span data-stu-id="cd6a7-156">Properties</span></span>
| <span data-ttu-id="cd6a7-157">属性</span><span class="sxs-lookup"><span data-stu-id="cd6a7-157">Property</span></span>     | <span data-ttu-id="cd6a7-158">类型</span><span class="sxs-lookup"><span data-stu-id="cd6a7-158">Type</span></span>   |<span data-ttu-id="cd6a7-159">说明</span><span class="sxs-lookup"><span data-stu-id="cd6a7-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd6a7-160">id</span><span class="sxs-lookup"><span data-stu-id="cd6a7-160">id</span></span>|<span data-ttu-id="cd6a7-161">string</span><span class="sxs-lookup"><span data-stu-id="cd6a7-161">string</span></span>|<span data-ttu-id="cd6a7-p106">返回用于唯一标识指定工作簿中工作表的值。即使工作表被重命名或移动，标识符的值仍然相同。只读。</span><span class="sxs-lookup"><span data-stu-id="cd6a7-p106">Returns a value that uniquely identifies the worksheet in a given workbook. The value of the identifier remains the same even when the worksheet is renamed or moved. Read-only.</span></span>|
|<span data-ttu-id="cd6a7-165">name</span><span class="sxs-lookup"><span data-stu-id="cd6a7-165">name</span></span>|<span data-ttu-id="cd6a7-166">string</span><span class="sxs-lookup"><span data-stu-id="cd6a7-166">string</span></span>|<span data-ttu-id="cd6a7-167">工作表的显示名称。</span><span class="sxs-lookup"><span data-stu-id="cd6a7-167">The display name of the worksheet.</span></span>|
|<span data-ttu-id="cd6a7-168">position</span><span class="sxs-lookup"><span data-stu-id="cd6a7-168">position</span></span>|<span data-ttu-id="cd6a7-169">int</span><span class="sxs-lookup"><span data-stu-id="cd6a7-169">int</span></span>|<span data-ttu-id="cd6a7-170">工作表在工作簿中的位置，从零开始。</span><span class="sxs-lookup"><span data-stu-id="cd6a7-170">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="cd6a7-171">visibility</span><span class="sxs-lookup"><span data-stu-id="cd6a7-171">visibility</span></span>|<span data-ttu-id="cd6a7-172">string</span><span class="sxs-lookup"><span data-stu-id="cd6a7-172">string</span></span>|<span data-ttu-id="cd6a7-173">工作表的可见性。</span><span class="sxs-lookup"><span data-stu-id="cd6a7-173">The Visibility of the worksheet.</span></span> <span data-ttu-id="cd6a7-174">可能的值包括 `Visible`、`Hidden`、`VeryHidden`。</span><span class="sxs-lookup"><span data-stu-id="cd6a7-174">The possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd6a7-175">关系</span><span class="sxs-lookup"><span data-stu-id="cd6a7-175">Relationships</span></span>
| <span data-ttu-id="cd6a7-176">关系</span><span class="sxs-lookup"><span data-stu-id="cd6a7-176">Relationship</span></span> | <span data-ttu-id="cd6a7-177">类型</span><span class="sxs-lookup"><span data-stu-id="cd6a7-177">Type</span></span>   |<span data-ttu-id="cd6a7-178">说明</span><span class="sxs-lookup"><span data-stu-id="cd6a7-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd6a7-179">图表</span><span class="sxs-lookup"><span data-stu-id="cd6a7-179">charts</span></span>|<span data-ttu-id="cd6a7-180">[WorkbookChart](chart.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cd6a7-180">[WorkbookChart](chart.md) collection</span></span>|<span data-ttu-id="cd6a7-181">返回属于工作表的图表的集合。</span><span class="sxs-lookup"><span data-stu-id="cd6a7-181">Returns collection of charts that are part of the worksheet.</span></span> <span data-ttu-id="cd6a7-182">只读。</span><span class="sxs-lookup"><span data-stu-id="cd6a7-182">Read-only.</span></span>|
|<span data-ttu-id="cd6a7-183">names</span><span class="sxs-lookup"><span data-stu-id="cd6a7-183">names</span></span>|<span data-ttu-id="cd6a7-184">[WorkbookNamedItem](nameditem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cd6a7-184">[WorkbookNamedItem](nameditem.md) collection</span></span>|<span data-ttu-id="cd6a7-185">返回与该工作表关联的名称集合。</span><span class="sxs-lookup"><span data-stu-id="cd6a7-185">Returns collection of names that are associated with the worksheet.</span></span> <span data-ttu-id="cd6a7-186">只读。</span><span class="sxs-lookup"><span data-stu-id="cd6a7-186">Read-only.</span></span>|
|<span data-ttu-id="cd6a7-187">pivotTables</span><span class="sxs-lookup"><span data-stu-id="cd6a7-187">pivotTables</span></span>|<span data-ttu-id="cd6a7-188">[workbookPivotTable](workbookpivottable.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cd6a7-188">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="cd6a7-189">一组属于工作表的数据透视表对象。</span><span class="sxs-lookup"><span data-stu-id="cd6a7-189">Collection of PivotTables that are part of the worksheet.</span></span> |
|<span data-ttu-id="cd6a7-190">保护</span><span class="sxs-lookup"><span data-stu-id="cd6a7-190">protection</span></span>|[<span data-ttu-id="cd6a7-191">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="cd6a7-191">WorkbookWorksheetProtection</span></span>](worksheetprotection.md)|<span data-ttu-id="cd6a7-p110">返回表工作表的工作表保护对象。只读。</span><span class="sxs-lookup"><span data-stu-id="cd6a7-p110">Returns sheet protection object for a worksheet. Read-only.</span></span>|
|<span data-ttu-id="cd6a7-194">表格</span><span class="sxs-lookup"><span data-stu-id="cd6a7-194">tables</span></span>|<span data-ttu-id="cd6a7-195">[WorkbookTable](table.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cd6a7-195">[WorkbookTable](table.md) collection</span></span>|<span data-ttu-id="cd6a7-196">属于工作表的表的集合。</span><span class="sxs-lookup"><span data-stu-id="cd6a7-196">Collection of tables that are part of the worksheet.</span></span> <span data-ttu-id="cd6a7-197">只读。</span><span class="sxs-lookup"><span data-stu-id="cd6a7-197">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cd6a7-198">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cd6a7-198">JSON representation</span></span>

<span data-ttu-id="cd6a7-199">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd6a7-199">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookWorksheet"
}-->

```json
{
  "id": "string",
  "name": "string",
  "position": 1024,
  "visibility": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
