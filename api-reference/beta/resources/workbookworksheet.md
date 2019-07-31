---
title: workbookWorksheet 资源类型
description: Excel 工作表是由单元格组成的网格。 它可以包含数据、表、图表等。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 93386edf60e30069068ceb2fa437fb128b239302
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963855"
---
# <a name="workbookworksheet-resource-type"></a><span data-ttu-id="5cd11-104">workbookWorksheet 资源类型</span><span class="sxs-lookup"><span data-stu-id="5cd11-104">workbookWorksheet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cd11-105">Excel 工作表是由单元格组成的网格。</span><span class="sxs-lookup"><span data-stu-id="5cd11-105">An Excel worksheet is a grid of cells.</span></span> <span data-ttu-id="5cd11-106">它可以包含数据、表、图表等。</span><span class="sxs-lookup"><span data-stu-id="5cd11-106">It can contain data, tables, charts, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="5cd11-107">方法</span><span class="sxs-lookup"><span data-stu-id="5cd11-107">Methods</span></span>

| <span data-ttu-id="5cd11-108">方法</span><span class="sxs-lookup"><span data-stu-id="5cd11-108">Method</span></span>           | <span data-ttu-id="5cd11-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="5cd11-109">Return Type</span></span>    |<span data-ttu-id="5cd11-110">说明</span><span class="sxs-lookup"><span data-stu-id="5cd11-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5cd11-111">获取工作表</span><span class="sxs-lookup"><span data-stu-id="5cd11-111">Get Worksheet</span></span>](../api/worksheet-get.md) | [<span data-ttu-id="5cd11-112">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="5cd11-112">workbookWorksheet</span></span>](workbookworksheet.md) |<span data-ttu-id="5cd11-113">读取 worksheet 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5cd11-113">Read properties and relationships of worksheet object.</span></span>|
|[<span data-ttu-id="5cd11-114">创建图表</span><span class="sxs-lookup"><span data-stu-id="5cd11-114">Create Chart</span></span>](../api/worksheet-post-charts.md) |[<span data-ttu-id="5cd11-115">workbookChart</span><span class="sxs-lookup"><span data-stu-id="5cd11-115">workbookChart</span></span>](workbookchart.md)| <span data-ttu-id="5cd11-116">通过发布到图表集合创建新的图表。</span><span class="sxs-lookup"><span data-stu-id="5cd11-116">Create a new Chart by posting to the charts collection.</span></span>|
|[<span data-ttu-id="5cd11-117">列出名称</span><span class="sxs-lookup"><span data-stu-id="5cd11-117">List names</span></span>](../api/worksheet-list-names.md) |<span data-ttu-id="5cd11-118">[workbookNamedItem](workbooknameditem.md)集合</span><span class="sxs-lookup"><span data-stu-id="5cd11-118">[workbookNamedItem](workbooknameditem.md) collection</span></span>| <span data-ttu-id="5cd11-119">获取与工作表关联的命名项的集合。</span><span class="sxs-lookup"><span data-stu-id="5cd11-119">Get named item collection associated with the worksheet.</span></span>|
|[<span data-ttu-id="5cd11-120">列出图表</span><span class="sxs-lookup"><span data-stu-id="5cd11-120">List charts</span></span>](../api/worksheet-list-charts.md) |<span data-ttu-id="5cd11-121">[workbookChart](workbookchart.md)集合</span><span class="sxs-lookup"><span data-stu-id="5cd11-121">[workbookChart](workbookchart.md) collection</span></span>| <span data-ttu-id="5cd11-122">获取 Chart 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5cd11-122">Get a Chart object collection.</span></span>|
|[<span data-ttu-id="5cd11-123">创建表</span><span class="sxs-lookup"><span data-stu-id="5cd11-123">Create Table</span></span>](../api/worksheet-post-tables.md) |[<span data-ttu-id="5cd11-124">workbookTable</span><span class="sxs-lookup"><span data-stu-id="5cd11-124">workbookTable</span></span>](workbooktable.md)| <span data-ttu-id="5cd11-125">通过发布到表集合创建新表。</span><span class="sxs-lookup"><span data-stu-id="5cd11-125">Create a new Table by posting to the tables collection.</span></span>|
|[<span data-ttu-id="5cd11-126">列出表</span><span class="sxs-lookup"><span data-stu-id="5cd11-126">List tables</span></span>](../api/worksheet-list-tables.md) |<span data-ttu-id="5cd11-127">[workbookTable](workbooktable.md)集合</span><span class="sxs-lookup"><span data-stu-id="5cd11-127">[workbookTable](workbooktable.md) collection</span></span>| <span data-ttu-id="5cd11-128">获取 Table 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5cd11-128">Get a Table object collection.</span></span>|
|[<span data-ttu-id="5cd11-129">更新</span><span class="sxs-lookup"><span data-stu-id="5cd11-129">Update</span></span>](../api/worksheet-update.md) | [<span data-ttu-id="5cd11-130">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="5cd11-130">workbookWorksheet</span></span>](workbookworksheet.md)   |<span data-ttu-id="5cd11-131">更新 Worksheet 对象。</span><span class="sxs-lookup"><span data-stu-id="5cd11-131">Update Worksheet object.</span></span> |
|[<span data-ttu-id="5cd11-132">单元格</span><span class="sxs-lookup"><span data-stu-id="5cd11-132">Cell</span></span>](../api/worksheet-cell.md)|[<span data-ttu-id="5cd11-133">workbookRange</span><span class="sxs-lookup"><span data-stu-id="5cd11-133">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="5cd11-p103">根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。</span><span class="sxs-lookup"><span data-stu-id="5cd11-p103">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>|
|[<span data-ttu-id="5cd11-136">区域</span><span class="sxs-lookup"><span data-stu-id="5cd11-136">Range</span></span>](../api/worksheet-range.md)|[<span data-ttu-id="5cd11-137">workbookRange</span><span class="sxs-lookup"><span data-stu-id="5cd11-137">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="5cd11-138">获取地址或名称指定的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="5cd11-138">Gets the range object specified by the address or name.</span></span>|
|[<span data-ttu-id="5cd11-139">Usedrange</span><span class="sxs-lookup"><span data-stu-id="5cd11-139">Usedrange</span></span>](../api/worksheet-usedrange.md)|[<span data-ttu-id="5cd11-140">workbookRange</span><span class="sxs-lookup"><span data-stu-id="5cd11-140">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="5cd11-p104">使用的区域是包含分配了值或格式化的任何单元格的最小区域。如果工作表为空，此函数将返回左上角的单元格。</span><span class="sxs-lookup"><span data-stu-id="5cd11-p104">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>|
|[<span data-ttu-id="5cd11-143">删除</span><span class="sxs-lookup"><span data-stu-id="5cd11-143">Delete</span></span>](../api/worksheet-delete.md)|<span data-ttu-id="5cd11-144">无</span><span class="sxs-lookup"><span data-stu-id="5cd11-144">None</span></span>|<span data-ttu-id="5cd11-145">从工作簿中删除工作表。</span><span class="sxs-lookup"><span data-stu-id="5cd11-145">Deletes the worksheet from the workbook.</span></span>|
|[<span data-ttu-id="5cd11-146">List</span><span class="sxs-lookup"><span data-stu-id="5cd11-146">List</span></span>](../api/worksheet-list.md) | <span data-ttu-id="5cd11-147">[workbookWorksheet](workbookworksheet.md)集合</span><span class="sxs-lookup"><span data-stu-id="5cd11-147">[workbookWorksheet](workbookworksheet.md) collection</span></span> |<span data-ttu-id="5cd11-148">获取 worksheet 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5cd11-148">Get worksheet object collection.</span></span> |
|[<span data-ttu-id="5cd11-149">Add</span><span class="sxs-lookup"><span data-stu-id="5cd11-149">Add</span></span>](../api/worksheetcollection-add.md)|[<span data-ttu-id="5cd11-150">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="5cd11-150">workbookWorksheet</span></span>](workbookworksheet.md)|<span data-ttu-id="5cd11-p105">向工作簿添加新工作表。将工作表添加到现有工作表的末尾。</span><span class="sxs-lookup"><span data-stu-id="5cd11-p105">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets.</span></span> |
|[<span data-ttu-id="5cd11-153">List pivotTables</span><span class="sxs-lookup"><span data-stu-id="5cd11-153">List pivotTables</span></span>](../api/workbookworksheet-list-pivottables.md) |<span data-ttu-id="5cd11-154">[workbookPivotTable](workbookpivottable.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5cd11-154">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="5cd11-155">获取一组 workbookPivotTable 对象。</span><span class="sxs-lookup"><span data-stu-id="5cd11-155">Get a workbookPivotTable object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="5cd11-156">属性</span><span class="sxs-lookup"><span data-stu-id="5cd11-156">Properties</span></span>
| <span data-ttu-id="5cd11-157">属性</span><span class="sxs-lookup"><span data-stu-id="5cd11-157">Property</span></span>     | <span data-ttu-id="5cd11-158">类型</span><span class="sxs-lookup"><span data-stu-id="5cd11-158">Type</span></span>   |<span data-ttu-id="5cd11-159">说明</span><span class="sxs-lookup"><span data-stu-id="5cd11-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5cd11-160">id</span><span class="sxs-lookup"><span data-stu-id="5cd11-160">id</span></span>|<span data-ttu-id="5cd11-161">string</span><span class="sxs-lookup"><span data-stu-id="5cd11-161">string</span></span>|<span data-ttu-id="5cd11-p106">返回用于唯一标识指定工作簿中工作表的值。即使工作表被重命名或移动，标识符的值仍然相同。只读。</span><span class="sxs-lookup"><span data-stu-id="5cd11-p106">Returns a value that uniquely identifies the worksheet in a given workbook. The value of the identifier remains the same even when the worksheet is renamed or moved. Read-only.</span></span>|
|<span data-ttu-id="5cd11-165">name</span><span class="sxs-lookup"><span data-stu-id="5cd11-165">name</span></span>|<span data-ttu-id="5cd11-166">string</span><span class="sxs-lookup"><span data-stu-id="5cd11-166">string</span></span>|<span data-ttu-id="5cd11-167">工作表的显示名称。</span><span class="sxs-lookup"><span data-stu-id="5cd11-167">The display name of the worksheet.</span></span>|
|<span data-ttu-id="5cd11-168">position</span><span class="sxs-lookup"><span data-stu-id="5cd11-168">position</span></span>|<span data-ttu-id="5cd11-169">int</span><span class="sxs-lookup"><span data-stu-id="5cd11-169">int</span></span>|<span data-ttu-id="5cd11-170">工作表在工作簿中的位置，从零开始。</span><span class="sxs-lookup"><span data-stu-id="5cd11-170">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="5cd11-171">visibility</span><span class="sxs-lookup"><span data-stu-id="5cd11-171">visibility</span></span>|<span data-ttu-id="5cd11-172">string</span><span class="sxs-lookup"><span data-stu-id="5cd11-172">string</span></span>|<span data-ttu-id="5cd11-173">工作表的可见性。</span><span class="sxs-lookup"><span data-stu-id="5cd11-173">The Visibility of the worksheet.</span></span> <span data-ttu-id="5cd11-174">可能的值包括 `Visible`、`Hidden`、`VeryHidden`。</span><span class="sxs-lookup"><span data-stu-id="5cd11-174">The possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5cd11-175">关系</span><span class="sxs-lookup"><span data-stu-id="5cd11-175">Relationships</span></span>
| <span data-ttu-id="5cd11-176">关系</span><span class="sxs-lookup"><span data-stu-id="5cd11-176">Relationship</span></span> | <span data-ttu-id="5cd11-177">类型</span><span class="sxs-lookup"><span data-stu-id="5cd11-177">Type</span></span>   |<span data-ttu-id="5cd11-178">说明</span><span class="sxs-lookup"><span data-stu-id="5cd11-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5cd11-179">图表</span><span class="sxs-lookup"><span data-stu-id="5cd11-179">charts</span></span>|<span data-ttu-id="5cd11-180">[workbookChart](workbookchart.md)集合</span><span class="sxs-lookup"><span data-stu-id="5cd11-180">[workbookChart](workbookchart.md) collection</span></span>|<span data-ttu-id="5cd11-181">返回属于工作表的图表的集合。</span><span class="sxs-lookup"><span data-stu-id="5cd11-181">Returns collection of charts that are part of the worksheet.</span></span> <span data-ttu-id="5cd11-182">只读。</span><span class="sxs-lookup"><span data-stu-id="5cd11-182">Read-only.</span></span>|
|<span data-ttu-id="5cd11-183">names</span><span class="sxs-lookup"><span data-stu-id="5cd11-183">names</span></span>|<span data-ttu-id="5cd11-184">[workbookNamedItem](workbooknameditem.md)集合</span><span class="sxs-lookup"><span data-stu-id="5cd11-184">[workbookNamedItem](workbooknameditem.md) collection</span></span>|<span data-ttu-id="5cd11-185">返回与该工作表关联的名称集合。</span><span class="sxs-lookup"><span data-stu-id="5cd11-185">Returns collection of names that are associated with the worksheet.</span></span> <span data-ttu-id="5cd11-186">只读。</span><span class="sxs-lookup"><span data-stu-id="5cd11-186">Read-only.</span></span>|
|<span data-ttu-id="5cd11-187">pivotTables</span><span class="sxs-lookup"><span data-stu-id="5cd11-187">pivotTables</span></span>|<span data-ttu-id="5cd11-188">[workbookPivotTable](workbookpivottable.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5cd11-188">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="5cd11-189">一组属于工作表的数据透视表对象。</span><span class="sxs-lookup"><span data-stu-id="5cd11-189">Collection of PivotTables that are part of the worksheet.</span></span> |
|<span data-ttu-id="5cd11-190">保护</span><span class="sxs-lookup"><span data-stu-id="5cd11-190">protection</span></span>|[<span data-ttu-id="5cd11-191">workbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="5cd11-191">workbookWorksheetProtection</span></span>](workbookworksheetprotection.md)|<span data-ttu-id="5cd11-p110">返回表工作表的工作表保护对象。只读。</span><span class="sxs-lookup"><span data-stu-id="5cd11-p110">Returns sheet protection object for a worksheet. Read-only.</span></span>|
|<span data-ttu-id="5cd11-194">表格</span><span class="sxs-lookup"><span data-stu-id="5cd11-194">tables</span></span>|<span data-ttu-id="5cd11-195">[workbookTable](workbooktable.md)集合</span><span class="sxs-lookup"><span data-stu-id="5cd11-195">[workbookTable](workbooktable.md) collection</span></span>|<span data-ttu-id="5cd11-196">属于工作表的表的集合。</span><span class="sxs-lookup"><span data-stu-id="5cd11-196">Collection of tables that are part of the worksheet.</span></span> <span data-ttu-id="5cd11-197">只读。</span><span class="sxs-lookup"><span data-stu-id="5cd11-197">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5cd11-198">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5cd11-198">JSON representation</span></span>

<span data-ttu-id="5cd11-199">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5cd11-199">Here is a JSON representation of the resource.</span></span>

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
