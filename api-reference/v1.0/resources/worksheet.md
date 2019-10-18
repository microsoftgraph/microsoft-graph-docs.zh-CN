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
# <a name="worksheet-resource-type"></a><span data-ttu-id="d78fe-104">工作表资源类型</span><span class="sxs-lookup"><span data-stu-id="d78fe-104">Worksheet resource type</span></span>

<span data-ttu-id="d78fe-105">Excel 工作表是由单元格组成的网格。</span><span class="sxs-lookup"><span data-stu-id="d78fe-105">An Excel worksheet is a grid of cells.</span></span> <span data-ttu-id="d78fe-106">它可以包含数据、表、图表等。</span><span class="sxs-lookup"><span data-stu-id="d78fe-106">It can contain data, tables, charts, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="d78fe-107">方法</span><span class="sxs-lookup"><span data-stu-id="d78fe-107">Methods</span></span>

| <span data-ttu-id="d78fe-108">方法</span><span class="sxs-lookup"><span data-stu-id="d78fe-108">Method</span></span>           | <span data-ttu-id="d78fe-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d78fe-109">Return Type</span></span>    |<span data-ttu-id="d78fe-110">说明</span><span class="sxs-lookup"><span data-stu-id="d78fe-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d78fe-111">获取工作表</span><span class="sxs-lookup"><span data-stu-id="d78fe-111">Get Worksheet</span></span>](../api/worksheet-get.md) | [<span data-ttu-id="d78fe-112">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="d78fe-112">WorkbookWorksheet</span></span>](worksheet.md) |<span data-ttu-id="d78fe-113">读取 worksheet 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d78fe-113">Read properties and relationships of worksheet object.</span></span>|
|[<span data-ttu-id="d78fe-114">创建图表</span><span class="sxs-lookup"><span data-stu-id="d78fe-114">Create Chart</span></span>](../api/worksheet-post-charts.md) |[<span data-ttu-id="d78fe-115">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="d78fe-115">WorkbookChart</span></span>](chart.md)| <span data-ttu-id="d78fe-116">通过发布到图表集合创建新的图表。</span><span class="sxs-lookup"><span data-stu-id="d78fe-116">Create a new Chart by posting to the charts collection.</span></span>|
|[<span data-ttu-id="d78fe-117">列出名称</span><span class="sxs-lookup"><span data-stu-id="d78fe-117">List names</span></span>](../api/worksheet-list-names.md) |<span data-ttu-id="d78fe-118">[WorkbookNamedItem](nameditem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d78fe-118">[WorkbookNamedItem](nameditem.md) collection</span></span>| <span data-ttu-id="d78fe-119">获取与工作表关联的命名项的集合。</span><span class="sxs-lookup"><span data-stu-id="d78fe-119">Get named item collection associated with the worksheet.</span></span>|
|[<span data-ttu-id="d78fe-120">列出图表</span><span class="sxs-lookup"><span data-stu-id="d78fe-120">List charts</span></span>](../api/worksheet-list-charts.md) |<span data-ttu-id="d78fe-121">[WorkbookChart](chart.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d78fe-121">[WorkbookChart](chart.md) collection</span></span>| <span data-ttu-id="d78fe-122">获取 Chart 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d78fe-122">Get a Chart object collection.</span></span>|
|[<span data-ttu-id="d78fe-123">创建表</span><span class="sxs-lookup"><span data-stu-id="d78fe-123">Create Table</span></span>](../api/worksheet-post-tables.md) |[<span data-ttu-id="d78fe-124">WorkbookTable</span><span class="sxs-lookup"><span data-stu-id="d78fe-124">WorkbookTable</span></span>](table.md)| <span data-ttu-id="d78fe-125">通过发布到表集合创建新表。</span><span class="sxs-lookup"><span data-stu-id="d78fe-125">Create a new Table by posting to the tables collection.</span></span>|
|[<span data-ttu-id="d78fe-126">列出表</span><span class="sxs-lookup"><span data-stu-id="d78fe-126">List tables</span></span>](../api/worksheet-list-tables.md) |<span data-ttu-id="d78fe-127">[WorkbookTable](table.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d78fe-127">[WorkbookTable](table.md) collection</span></span>| <span data-ttu-id="d78fe-128">获取 Table 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d78fe-128">Get a Table object collection.</span></span>|
|[<span data-ttu-id="d78fe-129">更新</span><span class="sxs-lookup"><span data-stu-id="d78fe-129">Update</span></span>](../api/worksheet-update.md) | [<span data-ttu-id="d78fe-130">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="d78fe-130">WorkbookWorksheet</span></span>](worksheet.md)   |<span data-ttu-id="d78fe-131">更新 Worksheet 对象。</span><span class="sxs-lookup"><span data-stu-id="d78fe-131">Update Worksheet object.</span></span> |
|[<span data-ttu-id="d78fe-132">单元格</span><span class="sxs-lookup"><span data-stu-id="d78fe-132">Cell</span></span>](../api/worksheet-cell.md)|[<span data-ttu-id="d78fe-133">区域</span><span class="sxs-lookup"><span data-stu-id="d78fe-133">Range</span></span>](range.md)|<span data-ttu-id="d78fe-p103">根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。</span><span class="sxs-lookup"><span data-stu-id="d78fe-p103">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>|
|[<span data-ttu-id="d78fe-136">区域</span><span class="sxs-lookup"><span data-stu-id="d78fe-136">Range</span></span>](../api/worksheet-range.md)|[<span data-ttu-id="d78fe-137">区域</span><span class="sxs-lookup"><span data-stu-id="d78fe-137">Range</span></span>](range.md)|<span data-ttu-id="d78fe-138">获取地址或名称指定的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="d78fe-138">Gets the range object specified by the address or name.</span></span>|
|[<span data-ttu-id="d78fe-139">Usedrange</span><span class="sxs-lookup"><span data-stu-id="d78fe-139">Usedrange</span></span>](../api/worksheet-usedrange.md)|[<span data-ttu-id="d78fe-140">区域</span><span class="sxs-lookup"><span data-stu-id="d78fe-140">Range</span></span>](range.md)|<span data-ttu-id="d78fe-p104">使用的区域是包含分配了值或格式化的任何单元格的最小区域。如果工作表为空，此函数将返回左上角的单元格。</span><span class="sxs-lookup"><span data-stu-id="d78fe-p104">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>|
|[<span data-ttu-id="d78fe-143">删除</span><span class="sxs-lookup"><span data-stu-id="d78fe-143">Delete</span></span>](../api/worksheet-delete.md)|<span data-ttu-id="d78fe-144">无</span><span class="sxs-lookup"><span data-stu-id="d78fe-144">None</span></span>|<span data-ttu-id="d78fe-145">从工作簿中删除工作表。</span><span class="sxs-lookup"><span data-stu-id="d78fe-145">Deletes the worksheet from the workbook.</span></span>|
|[<span data-ttu-id="d78fe-146">List</span><span class="sxs-lookup"><span data-stu-id="d78fe-146">List</span></span>](../api/worksheet-list.md) | <span data-ttu-id="d78fe-147">[WorkbookWorksheet](worksheet.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d78fe-147">[WorkbookWorksheet](worksheet.md) collection</span></span> |<span data-ttu-id="d78fe-148">获取 worksheet 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d78fe-148">Get worksheet object collection.</span></span> |
|[<span data-ttu-id="d78fe-149">Add</span><span class="sxs-lookup"><span data-stu-id="d78fe-149">Add</span></span>](../api/worksheetcollection-add.md)|[<span data-ttu-id="d78fe-150">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="d78fe-150">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="d78fe-p105">向工作簿添加新工作表。将工作表添加到现有工作表的末尾。</span><span class="sxs-lookup"><span data-stu-id="d78fe-p105">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets.</span></span> |
|[<span data-ttu-id="d78fe-153">List pivotTables</span><span class="sxs-lookup"><span data-stu-id="d78fe-153">List pivotTables</span></span>](../api/workbookworksheet-list-pivottables.md) |<span data-ttu-id="d78fe-154">[workbookPivotTable](workbookpivottable.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d78fe-154">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="d78fe-155">获取一组 workbookPivotTable 对象。</span><span class="sxs-lookup"><span data-stu-id="d78fe-155">Get a workbookPivotTable object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="d78fe-156">属性</span><span class="sxs-lookup"><span data-stu-id="d78fe-156">Properties</span></span>
| <span data-ttu-id="d78fe-157">属性</span><span class="sxs-lookup"><span data-stu-id="d78fe-157">Property</span></span>     | <span data-ttu-id="d78fe-158">类型</span><span class="sxs-lookup"><span data-stu-id="d78fe-158">Type</span></span>   |<span data-ttu-id="d78fe-159">说明</span><span class="sxs-lookup"><span data-stu-id="d78fe-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d78fe-160">id</span><span class="sxs-lookup"><span data-stu-id="d78fe-160">id</span></span>|<span data-ttu-id="d78fe-161">string</span><span class="sxs-lookup"><span data-stu-id="d78fe-161">string</span></span>|<span data-ttu-id="d78fe-p106">返回用于唯一标识指定工作簿中工作表的值。即使工作表被重命名或移动，标识符的值仍然相同。只读。</span><span class="sxs-lookup"><span data-stu-id="d78fe-p106">Returns a value that uniquely identifies the worksheet in a given workbook. The value of the identifier remains the same even when the worksheet is renamed or moved. Read-only.</span></span>|
|<span data-ttu-id="d78fe-165">name</span><span class="sxs-lookup"><span data-stu-id="d78fe-165">name</span></span>|<span data-ttu-id="d78fe-166">string</span><span class="sxs-lookup"><span data-stu-id="d78fe-166">string</span></span>|<span data-ttu-id="d78fe-167">工作表的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d78fe-167">The display name of the worksheet.</span></span>|
|<span data-ttu-id="d78fe-168">position</span><span class="sxs-lookup"><span data-stu-id="d78fe-168">position</span></span>|<span data-ttu-id="d78fe-169">int</span><span class="sxs-lookup"><span data-stu-id="d78fe-169">int</span></span>|<span data-ttu-id="d78fe-170">工作表在工作簿中的位置，从零开始。</span><span class="sxs-lookup"><span data-stu-id="d78fe-170">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="d78fe-171">visibility</span><span class="sxs-lookup"><span data-stu-id="d78fe-171">visibility</span></span>|<span data-ttu-id="d78fe-172">string</span><span class="sxs-lookup"><span data-stu-id="d78fe-172">string</span></span>|<span data-ttu-id="d78fe-173">工作表的可见性。</span><span class="sxs-lookup"><span data-stu-id="d78fe-173">The Visibility of the worksheet.</span></span> <span data-ttu-id="d78fe-174">可能的值包括 `Visible`、`Hidden`、`VeryHidden`。</span><span class="sxs-lookup"><span data-stu-id="d78fe-174">The possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d78fe-175">关系</span><span class="sxs-lookup"><span data-stu-id="d78fe-175">Relationships</span></span>
| <span data-ttu-id="d78fe-176">关系</span><span class="sxs-lookup"><span data-stu-id="d78fe-176">Relationship</span></span> | <span data-ttu-id="d78fe-177">类型</span><span class="sxs-lookup"><span data-stu-id="d78fe-177">Type</span></span>   |<span data-ttu-id="d78fe-178">说明</span><span class="sxs-lookup"><span data-stu-id="d78fe-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d78fe-179">图表</span><span class="sxs-lookup"><span data-stu-id="d78fe-179">charts</span></span>|<span data-ttu-id="d78fe-180">[WorkbookChart](chart.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d78fe-180">[WorkbookChart](chart.md) collection</span></span>|<span data-ttu-id="d78fe-181">返回属于工作表的图表的集合。</span><span class="sxs-lookup"><span data-stu-id="d78fe-181">Returns collection of charts that are part of the worksheet.</span></span> <span data-ttu-id="d78fe-182">只读。</span><span class="sxs-lookup"><span data-stu-id="d78fe-182">Read-only.</span></span>|
|<span data-ttu-id="d78fe-183">names</span><span class="sxs-lookup"><span data-stu-id="d78fe-183">names</span></span>|<span data-ttu-id="d78fe-184">[WorkbookNamedItem](nameditem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d78fe-184">[WorkbookNamedItem](nameditem.md) collection</span></span>|<span data-ttu-id="d78fe-185">返回与该工作表关联的名称集合。</span><span class="sxs-lookup"><span data-stu-id="d78fe-185">Returns collection of names that are associated with the worksheet.</span></span> <span data-ttu-id="d78fe-186">只读。</span><span class="sxs-lookup"><span data-stu-id="d78fe-186">Read-only.</span></span>|
|<span data-ttu-id="d78fe-187">pivotTables</span><span class="sxs-lookup"><span data-stu-id="d78fe-187">pivotTables</span></span>|<span data-ttu-id="d78fe-188">[workbookPivotTable](workbookpivottable.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d78fe-188">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="d78fe-189">一组属于工作表的数据透视表对象。</span><span class="sxs-lookup"><span data-stu-id="d78fe-189">Collection of PivotTables that are part of the worksheet.</span></span> |
|<span data-ttu-id="d78fe-190">保护</span><span class="sxs-lookup"><span data-stu-id="d78fe-190">protection</span></span>|[<span data-ttu-id="d78fe-191">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="d78fe-191">WorkbookWorksheetProtection</span></span>](worksheetprotection.md)|<span data-ttu-id="d78fe-p110">返回表工作表的工作表保护对象。只读。</span><span class="sxs-lookup"><span data-stu-id="d78fe-p110">Returns sheet protection object for a worksheet. Read-only.</span></span>|
|<span data-ttu-id="d78fe-194">表格</span><span class="sxs-lookup"><span data-stu-id="d78fe-194">tables</span></span>|<span data-ttu-id="d78fe-195">[WorkbookTable](table.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d78fe-195">[WorkbookTable](table.md) collection</span></span>|<span data-ttu-id="d78fe-196">属于工作表的表的集合。</span><span class="sxs-lookup"><span data-stu-id="d78fe-196">Collection of tables that are part of the worksheet.</span></span> <span data-ttu-id="d78fe-197">只读。</span><span class="sxs-lookup"><span data-stu-id="d78fe-197">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d78fe-198">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d78fe-198">JSON representation</span></span>

<span data-ttu-id="d78fe-199">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d78fe-199">Here is a JSON representation of the resource.</span></span>

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
