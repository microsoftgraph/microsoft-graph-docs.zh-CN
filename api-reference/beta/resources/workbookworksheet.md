---
title: workbookWorksheet 资源类型
description: Excel 工作表是由单元格组成的网格。 它可以包含数据、表、图表等。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 1700c61ed84b1ac218163e2cff3ac812f59cc8ed
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348575"
---
# <a name="workbookworksheet-resource-type"></a><span data-ttu-id="b58ae-104">workbookWorksheet 资源类型</span><span class="sxs-lookup"><span data-stu-id="b58ae-104">workbookWorksheet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b58ae-105">Excel 工作表是由单元格组成的网格。</span><span class="sxs-lookup"><span data-stu-id="b58ae-105">An Excel worksheet is a grid of cells.</span></span> <span data-ttu-id="b58ae-106">它可以包含数据、表、图表等。</span><span class="sxs-lookup"><span data-stu-id="b58ae-106">It can contain data, tables, charts, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="b58ae-107">方法</span><span class="sxs-lookup"><span data-stu-id="b58ae-107">Methods</span></span>

| <span data-ttu-id="b58ae-108">方法</span><span class="sxs-lookup"><span data-stu-id="b58ae-108">Method</span></span>           | <span data-ttu-id="b58ae-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="b58ae-109">Return Type</span></span>    |<span data-ttu-id="b58ae-110">说明</span><span class="sxs-lookup"><span data-stu-id="b58ae-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b58ae-111">获取工作表</span><span class="sxs-lookup"><span data-stu-id="b58ae-111">Get Worksheet</span></span>](../api/worksheet-get.md) | [<span data-ttu-id="b58ae-112">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="b58ae-112">workbookWorksheet</span></span>](workbookworksheet.md) |<span data-ttu-id="b58ae-113">读取 worksheet 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b58ae-113">Read properties and relationships of worksheet object.</span></span>|
|[<span data-ttu-id="b58ae-114">创建图表</span><span class="sxs-lookup"><span data-stu-id="b58ae-114">Create Chart</span></span>](../api/worksheet-post-charts.md) |[<span data-ttu-id="b58ae-115">workbookChart</span><span class="sxs-lookup"><span data-stu-id="b58ae-115">workbookChart</span></span>](workbookchart.md)| <span data-ttu-id="b58ae-116">通过发布到图表集合创建新的图表。</span><span class="sxs-lookup"><span data-stu-id="b58ae-116">Create a new Chart by posting to the charts collection.</span></span>|
|[<span data-ttu-id="b58ae-117">列出名称</span><span class="sxs-lookup"><span data-stu-id="b58ae-117">List names</span></span>](../api/worksheet-list-names.md) |<span data-ttu-id="b58ae-118">[workbookNamedItem](workbooknameditem.md)集合</span><span class="sxs-lookup"><span data-stu-id="b58ae-118">[workbookNamedItem](workbooknameditem.md) collection</span></span>| <span data-ttu-id="b58ae-119">获取与工作表关联的命名项的集合。</span><span class="sxs-lookup"><span data-stu-id="b58ae-119">Get named item collection associated with the worksheet.</span></span>|
|[<span data-ttu-id="b58ae-120">列出图表</span><span class="sxs-lookup"><span data-stu-id="b58ae-120">List charts</span></span>](../api/worksheet-list-charts.md) |<span data-ttu-id="b58ae-121">[workbookChart](workbookchart.md)集合</span><span class="sxs-lookup"><span data-stu-id="b58ae-121">[workbookChart](workbookchart.md) collection</span></span>| <span data-ttu-id="b58ae-122">获取 Chart 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b58ae-122">Get a Chart object collection.</span></span>|
|[<span data-ttu-id="b58ae-123">创建表</span><span class="sxs-lookup"><span data-stu-id="b58ae-123">Create Table</span></span>](../api/worksheet-post-tables.md) |[<span data-ttu-id="b58ae-124">workbookTable</span><span class="sxs-lookup"><span data-stu-id="b58ae-124">workbookTable</span></span>](workbooktable.md)| <span data-ttu-id="b58ae-125">通过发布到表集合创建新表。</span><span class="sxs-lookup"><span data-stu-id="b58ae-125">Create a new Table by posting to the tables collection.</span></span>|
|[<span data-ttu-id="b58ae-126">列出表</span><span class="sxs-lookup"><span data-stu-id="b58ae-126">List tables</span></span>](../api/worksheet-list-tables.md) |<span data-ttu-id="b58ae-127">[workbookTable](workbooktable.md)集合</span><span class="sxs-lookup"><span data-stu-id="b58ae-127">[workbookTable](workbooktable.md) collection</span></span>| <span data-ttu-id="b58ae-128">获取 Table 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b58ae-128">Get a Table object collection.</span></span>|
|[<span data-ttu-id="b58ae-129">更新</span><span class="sxs-lookup"><span data-stu-id="b58ae-129">Update</span></span>](../api/worksheet-update.md) | [<span data-ttu-id="b58ae-130">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="b58ae-130">workbookWorksheet</span></span>](workbookworksheet.md)   |<span data-ttu-id="b58ae-131">更新 Worksheet 对象。</span><span class="sxs-lookup"><span data-stu-id="b58ae-131">Update Worksheet object.</span></span> |
|[<span data-ttu-id="b58ae-132">单元格</span><span class="sxs-lookup"><span data-stu-id="b58ae-132">Cell</span></span>](../api/worksheet-cell.md)|[<span data-ttu-id="b58ae-133">workbookRange</span><span class="sxs-lookup"><span data-stu-id="b58ae-133">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="b58ae-p103">根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。</span><span class="sxs-lookup"><span data-stu-id="b58ae-p103">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>|
|[<span data-ttu-id="b58ae-136">区域</span><span class="sxs-lookup"><span data-stu-id="b58ae-136">Range</span></span>](../api/worksheet-range.md)|[<span data-ttu-id="b58ae-137">workbookRange</span><span class="sxs-lookup"><span data-stu-id="b58ae-137">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="b58ae-138">获取地址或名称指定的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="b58ae-138">Gets the range object specified by the address or name.</span></span>|
|[<span data-ttu-id="b58ae-139">Usedrange</span><span class="sxs-lookup"><span data-stu-id="b58ae-139">Usedrange</span></span>](../api/worksheet-usedrange.md)|[<span data-ttu-id="b58ae-140">workbookRange</span><span class="sxs-lookup"><span data-stu-id="b58ae-140">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="b58ae-p104">使用的区域是包含分配了值或格式化的任何单元格的最小区域。如果工作表为空，此函数将返回左上角的单元格。</span><span class="sxs-lookup"><span data-stu-id="b58ae-p104">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>|
|[<span data-ttu-id="b58ae-143">删除</span><span class="sxs-lookup"><span data-stu-id="b58ae-143">Delete</span></span>](../api/worksheet-delete.md)|<span data-ttu-id="b58ae-144">无</span><span class="sxs-lookup"><span data-stu-id="b58ae-144">None</span></span>|<span data-ttu-id="b58ae-145">从工作簿中删除工作表。</span><span class="sxs-lookup"><span data-stu-id="b58ae-145">Deletes the worksheet from the workbook.</span></span>|
|[<span data-ttu-id="b58ae-146">List</span><span class="sxs-lookup"><span data-stu-id="b58ae-146">List</span></span>](../api/worksheet-list.md) | <span data-ttu-id="b58ae-147">[workbookWorksheet](workbookworksheet.md)集合</span><span class="sxs-lookup"><span data-stu-id="b58ae-147">[workbookWorksheet](workbookworksheet.md) collection</span></span> |<span data-ttu-id="b58ae-148">获取 worksheet 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b58ae-148">Get worksheet object collection.</span></span> |
|[<span data-ttu-id="b58ae-149">Add</span><span class="sxs-lookup"><span data-stu-id="b58ae-149">Add</span></span>](../api/worksheetcollection-add.md)|[<span data-ttu-id="b58ae-150">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="b58ae-150">workbookWorksheet</span></span>](workbookworksheet.md)|<span data-ttu-id="b58ae-p105">向工作簿添加新工作表。将工作表添加到现有工作表的末尾。</span><span class="sxs-lookup"><span data-stu-id="b58ae-p105">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets.</span></span> |
|[<span data-ttu-id="b58ae-153">List pivotTables</span><span class="sxs-lookup"><span data-stu-id="b58ae-153">List pivotTables</span></span>](../api/workbookworksheet-list-pivottables.md) |<span data-ttu-id="b58ae-154">[workbookPivotTable](workbookpivottable.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b58ae-154">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="b58ae-155">获取一组 workbookPivotTable 对象。</span><span class="sxs-lookup"><span data-stu-id="b58ae-155">Get a workbookPivotTable object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="b58ae-156">属性</span><span class="sxs-lookup"><span data-stu-id="b58ae-156">Properties</span></span>
| <span data-ttu-id="b58ae-157">属性</span><span class="sxs-lookup"><span data-stu-id="b58ae-157">Property</span></span>     | <span data-ttu-id="b58ae-158">类型</span><span class="sxs-lookup"><span data-stu-id="b58ae-158">Type</span></span>   |<span data-ttu-id="b58ae-159">说明</span><span class="sxs-lookup"><span data-stu-id="b58ae-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b58ae-160">id</span><span class="sxs-lookup"><span data-stu-id="b58ae-160">id</span></span>|<span data-ttu-id="b58ae-161">string</span><span class="sxs-lookup"><span data-stu-id="b58ae-161">string</span></span>|<span data-ttu-id="b58ae-p106">返回用于唯一标识指定工作簿中工作表的值。即使工作表被重命名或移动，标识符的值仍然相同。只读。</span><span class="sxs-lookup"><span data-stu-id="b58ae-p106">Returns a value that uniquely identifies the worksheet in a given workbook. The value of the identifier remains the same even when the worksheet is renamed or moved. Read-only.</span></span>|
|<span data-ttu-id="b58ae-165">name</span><span class="sxs-lookup"><span data-stu-id="b58ae-165">name</span></span>|<span data-ttu-id="b58ae-166">string</span><span class="sxs-lookup"><span data-stu-id="b58ae-166">string</span></span>|<span data-ttu-id="b58ae-167">工作表的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b58ae-167">The display name of the worksheet.</span></span>|
|<span data-ttu-id="b58ae-168">position</span><span class="sxs-lookup"><span data-stu-id="b58ae-168">position</span></span>|<span data-ttu-id="b58ae-169">int</span><span class="sxs-lookup"><span data-stu-id="b58ae-169">int</span></span>|<span data-ttu-id="b58ae-170">工作表在工作簿中的位置，从零开始。</span><span class="sxs-lookup"><span data-stu-id="b58ae-170">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="b58ae-171">visibility</span><span class="sxs-lookup"><span data-stu-id="b58ae-171">visibility</span></span>|<span data-ttu-id="b58ae-172">string</span><span class="sxs-lookup"><span data-stu-id="b58ae-172">string</span></span>|<span data-ttu-id="b58ae-173">工作表的可见性。</span><span class="sxs-lookup"><span data-stu-id="b58ae-173">The Visibility of the worksheet.</span></span> <span data-ttu-id="b58ae-174">可能的值包括 `Visible`、`Hidden`、`VeryHidden`。</span><span class="sxs-lookup"><span data-stu-id="b58ae-174">The possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b58ae-175">关系</span><span class="sxs-lookup"><span data-stu-id="b58ae-175">Relationships</span></span>
| <span data-ttu-id="b58ae-176">关系</span><span class="sxs-lookup"><span data-stu-id="b58ae-176">Relationship</span></span> | <span data-ttu-id="b58ae-177">类型</span><span class="sxs-lookup"><span data-stu-id="b58ae-177">Type</span></span>   |<span data-ttu-id="b58ae-178">说明</span><span class="sxs-lookup"><span data-stu-id="b58ae-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b58ae-179">图表</span><span class="sxs-lookup"><span data-stu-id="b58ae-179">charts</span></span>|<span data-ttu-id="b58ae-180">[workbookChart](workbookchart.md)集合</span><span class="sxs-lookup"><span data-stu-id="b58ae-180">[workbookChart](workbookchart.md) collection</span></span>|<span data-ttu-id="b58ae-181">返回属于工作表的图表的集合。</span><span class="sxs-lookup"><span data-stu-id="b58ae-181">Returns collection of charts that are part of the worksheet.</span></span> <span data-ttu-id="b58ae-182">只读。</span><span class="sxs-lookup"><span data-stu-id="b58ae-182">Read-only.</span></span>|
|<span data-ttu-id="b58ae-183">names</span><span class="sxs-lookup"><span data-stu-id="b58ae-183">names</span></span>|<span data-ttu-id="b58ae-184">[workbookNamedItem](workbooknameditem.md)集合</span><span class="sxs-lookup"><span data-stu-id="b58ae-184">[workbookNamedItem](workbooknameditem.md) collection</span></span>|<span data-ttu-id="b58ae-185">返回与该工作表关联的名称集合。</span><span class="sxs-lookup"><span data-stu-id="b58ae-185">Returns collection of names that are associated with the worksheet.</span></span> <span data-ttu-id="b58ae-186">只读。</span><span class="sxs-lookup"><span data-stu-id="b58ae-186">Read-only.</span></span>|
|<span data-ttu-id="b58ae-187">pivotTables</span><span class="sxs-lookup"><span data-stu-id="b58ae-187">pivotTables</span></span>|<span data-ttu-id="b58ae-188">[workbookPivotTable](workbookpivottable.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b58ae-188">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="b58ae-189">一组属于工作表的数据透视表对象。</span><span class="sxs-lookup"><span data-stu-id="b58ae-189">Collection of PivotTables that are part of the worksheet.</span></span> |
|<span data-ttu-id="b58ae-190">保护</span><span class="sxs-lookup"><span data-stu-id="b58ae-190">protection</span></span>|[<span data-ttu-id="b58ae-191">workbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="b58ae-191">workbookWorksheetProtection</span></span>](workbookworksheetprotection.md)|<span data-ttu-id="b58ae-p110">返回表工作表的工作表保护对象。只读。</span><span class="sxs-lookup"><span data-stu-id="b58ae-p110">Returns sheet protection object for a worksheet. Read-only.</span></span>|
|<span data-ttu-id="b58ae-194">表格</span><span class="sxs-lookup"><span data-stu-id="b58ae-194">tables</span></span>|<span data-ttu-id="b58ae-195">[workbookTable](workbooktable.md)集合</span><span class="sxs-lookup"><span data-stu-id="b58ae-195">[workbookTable](workbooktable.md) collection</span></span>|<span data-ttu-id="b58ae-196">属于工作表的表的集合。</span><span class="sxs-lookup"><span data-stu-id="b58ae-196">Collection of tables that are part of the worksheet.</span></span> <span data-ttu-id="b58ae-197">只读。</span><span class="sxs-lookup"><span data-stu-id="b58ae-197">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b58ae-198">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b58ae-198">JSON representation</span></span>

<span data-ttu-id="b58ae-199">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b58ae-199">Here is a JSON representation of the resource.</span></span>

<!-- {
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
<!--
{
  "type": "#page.annotation",
  "description": "Worksheet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
