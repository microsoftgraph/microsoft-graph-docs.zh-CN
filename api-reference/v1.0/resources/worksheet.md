---
title: 工作表资源类型
description: Excel 工作表是由单元格组成的网格。它可以包含数据、表、图表等。
localization_priority: Priority
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 60e31738329943d96e1a4f3ea8293851e759eaff
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983868"
---
# <a name="worksheet-resource-type"></a><span data-ttu-id="dbbe1-104">工作表资源类型</span><span class="sxs-lookup"><span data-stu-id="dbbe1-104">Worksheet resource type</span></span>

<span data-ttu-id="dbbe1-p102">Excel 工作表是由单元格组成的网格。它可以包含数据、表、图表等。</span><span class="sxs-lookup"><span data-stu-id="dbbe1-p102">An Excel worksheet is a grid of cells. It can contain data, tables, charts, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="dbbe1-107">方法</span><span class="sxs-lookup"><span data-stu-id="dbbe1-107">Methods</span></span>

| <span data-ttu-id="dbbe1-108">方法</span><span class="sxs-lookup"><span data-stu-id="dbbe1-108">Method</span></span>           | <span data-ttu-id="dbbe1-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="dbbe1-109">Return Type</span></span>    |<span data-ttu-id="dbbe1-110">说明</span><span class="sxs-lookup"><span data-stu-id="dbbe1-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dbbe1-111">获取工作表</span><span class="sxs-lookup"><span data-stu-id="dbbe1-111">Get Worksheet</span></span>](../api/worksheet-get.md) | [<span data-ttu-id="dbbe1-112">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="dbbe1-112">WorkbookWorksheet</span></span>](worksheet.md) |<span data-ttu-id="dbbe1-113">读取 worksheet 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dbbe1-113">Read properties and relationships of worksheet object.</span></span>|
|[<span data-ttu-id="dbbe1-114">创建图表</span><span class="sxs-lookup"><span data-stu-id="dbbe1-114">Create Chart</span></span>](../api/worksheet-post-charts.md) |[<span data-ttu-id="dbbe1-115">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="dbbe1-115">WorkbookChart</span></span>](chart.md)| <span data-ttu-id="dbbe1-116">通过发布到图表集合创建新的图表。</span><span class="sxs-lookup"><span data-stu-id="dbbe1-116">Create a new Chart by posting to the charts collection.</span></span>|
|[<span data-ttu-id="dbbe1-117">列出名称</span><span class="sxs-lookup"><span data-stu-id="dbbe1-117">List names</span></span>](../api/worksheet-list-names.md) |<span data-ttu-id="dbbe1-118">[WorkbookNamedItem](nameditem.md)集合</span><span class="sxs-lookup"><span data-stu-id="dbbe1-118">[WorkbookNamedItem](nameditem.md) collection</span></span>| <span data-ttu-id="dbbe1-119">获取与工作表关联的命名项的集合。</span><span class="sxs-lookup"><span data-stu-id="dbbe1-119">Get named item collection associated with the worksheet.</span></span>|
|[<span data-ttu-id="dbbe1-120">列出图表</span><span class="sxs-lookup"><span data-stu-id="dbbe1-120">List charts</span></span>](../api/worksheet-list-charts.md) |<span data-ttu-id="dbbe1-121">[WorkbookChart](chart.md)集合</span><span class="sxs-lookup"><span data-stu-id="dbbe1-121">[WorkbookChart](chart.md) collection</span></span>| <span data-ttu-id="dbbe1-122">获取 Chart 对象集合。</span><span class="sxs-lookup"><span data-stu-id="dbbe1-122">Get a Chart object collection.</span></span>|
|[<span data-ttu-id="dbbe1-123">创建表</span><span class="sxs-lookup"><span data-stu-id="dbbe1-123">Create Table</span></span>](../api/worksheet-post-tables.md) |[<span data-ttu-id="dbbe1-124">WorkbookTable</span><span class="sxs-lookup"><span data-stu-id="dbbe1-124">WorkbookTable</span></span>](table.md)| <span data-ttu-id="dbbe1-125">通过发布到表集合创建新表。</span><span class="sxs-lookup"><span data-stu-id="dbbe1-125">Create a new Table by posting to the tables collection.</span></span>|
|[<span data-ttu-id="dbbe1-126">列出表</span><span class="sxs-lookup"><span data-stu-id="dbbe1-126">List tables</span></span>](../api/worksheet-list-tables.md) |<span data-ttu-id="dbbe1-127">[WorkbookTable](table.md)集合</span><span class="sxs-lookup"><span data-stu-id="dbbe1-127">[WorkbookTable](table.md) collection</span></span>| <span data-ttu-id="dbbe1-128">获取 Table 对象集合。</span><span class="sxs-lookup"><span data-stu-id="dbbe1-128">Get a Table object collection.</span></span>|
|[<span data-ttu-id="dbbe1-129">更新</span><span class="sxs-lookup"><span data-stu-id="dbbe1-129">Update</span></span>](../api/worksheet-update.md) | [<span data-ttu-id="dbbe1-130">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="dbbe1-130">WorkbookWorksheet</span></span>](worksheet.md)   |<span data-ttu-id="dbbe1-131">更新 Worksheet 对象。</span><span class="sxs-lookup"><span data-stu-id="dbbe1-131">Update Worksheet object.</span></span> |
|[<span data-ttu-id="dbbe1-132">Cell</span><span class="sxs-lookup"><span data-stu-id="dbbe1-132">Cell</span></span>](../api/worksheet-cell.md)|[<span data-ttu-id="dbbe1-133">Range</span><span class="sxs-lookup"><span data-stu-id="dbbe1-133">Range</span></span>](range.md)|<span data-ttu-id="dbbe1-p103">根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。</span><span class="sxs-lookup"><span data-stu-id="dbbe1-p103">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>|
|[<span data-ttu-id="dbbe1-136">区域</span><span class="sxs-lookup"><span data-stu-id="dbbe1-136">Range</span></span>](../api/worksheet-range.md)|[<span data-ttu-id="dbbe1-137">Range</span><span class="sxs-lookup"><span data-stu-id="dbbe1-137">Range</span></span>](range.md)|<span data-ttu-id="dbbe1-138">获取地址或名称指定的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="dbbe1-138">Gets the range object specified by the address or name.</span></span>|
|[<span data-ttu-id="dbbe1-139">Usedrange</span><span class="sxs-lookup"><span data-stu-id="dbbe1-139">Usedrange</span></span>](../api/worksheet-usedrange.md)|[<span data-ttu-id="dbbe1-140">Range</span><span class="sxs-lookup"><span data-stu-id="dbbe1-140">Range</span></span>](range.md)|<span data-ttu-id="dbbe1-p104">使用的区域是包含分配了值或格式化的任何单元格的最小区域。如果工作表为空，此函数将返回左上角的单元格。</span><span class="sxs-lookup"><span data-stu-id="dbbe1-p104">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>|
|[<span data-ttu-id="dbbe1-143">删除</span><span class="sxs-lookup"><span data-stu-id="dbbe1-143">Delete</span></span>](../api/worksheet-delete.md)|<span data-ttu-id="dbbe1-144">无</span><span class="sxs-lookup"><span data-stu-id="dbbe1-144">None</span></span>|<span data-ttu-id="dbbe1-145">从工作簿中删除工作表。</span><span class="sxs-lookup"><span data-stu-id="dbbe1-145">Deletes the worksheet from the workbook.</span></span>|
|[<span data-ttu-id="dbbe1-146">列出</span><span class="sxs-lookup"><span data-stu-id="dbbe1-146">List</span></span>](../api/worksheet-list.md) | <span data-ttu-id="dbbe1-147">[WorkbookWorksheet](worksheet.md)集合</span><span class="sxs-lookup"><span data-stu-id="dbbe1-147">[WorkbookWorksheet](worksheet.md) collection</span></span> |<span data-ttu-id="dbbe1-148">获取 worksheet 对象集合。</span><span class="sxs-lookup"><span data-stu-id="dbbe1-148">Get worksheet object collection.</span></span> |
|[<span data-ttu-id="dbbe1-149">Add</span><span class="sxs-lookup"><span data-stu-id="dbbe1-149">Add</span></span>](../api/worksheetcollection-add.md)|[<span data-ttu-id="dbbe1-150">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="dbbe1-150">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="dbbe1-p105">向工作簿添加新工作表。将工作表添加到现有工作表的末尾。</span><span class="sxs-lookup"><span data-stu-id="dbbe1-p105">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets.</span></span> |
|[<span data-ttu-id="dbbe1-153">List pivotTables</span><span class="sxs-lookup"><span data-stu-id="dbbe1-153">List pivotTables</span></span>](../api/workbookworksheet-list-pivottables.md) |<span data-ttu-id="dbbe1-154">[workbookPivotTable](workbookpivottable.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dbbe1-154">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="dbbe1-155">获取一组 workbookPivotTable 对象。</span><span class="sxs-lookup"><span data-stu-id="dbbe1-155">Get a workbookPivotTable object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="dbbe1-156">属性</span><span class="sxs-lookup"><span data-stu-id="dbbe1-156">Properties</span></span>
| <span data-ttu-id="dbbe1-157">属性</span><span class="sxs-lookup"><span data-stu-id="dbbe1-157">Property</span></span>     | <span data-ttu-id="dbbe1-158">类型</span><span class="sxs-lookup"><span data-stu-id="dbbe1-158">Type</span></span>   |<span data-ttu-id="dbbe1-159">说明</span><span class="sxs-lookup"><span data-stu-id="dbbe1-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dbbe1-160">ID</span><span class="sxs-lookup"><span data-stu-id="dbbe1-160">id</span></span>|<span data-ttu-id="dbbe1-161">string</span><span class="sxs-lookup"><span data-stu-id="dbbe1-161">string</span></span>|<span data-ttu-id="dbbe1-p106">返回用于唯一标识指定工作簿中工作表的值。即使工作表被重命名或移动，标识符的值仍然相同。只读。</span><span class="sxs-lookup"><span data-stu-id="dbbe1-p106">Returns a value that uniquely identifies the worksheet in a given workbook. The value of the identifier remains the same even when the worksheet is renamed or moved. Read-only.</span></span>|
|<span data-ttu-id="dbbe1-165">name</span><span class="sxs-lookup"><span data-stu-id="dbbe1-165">name</span></span>|<span data-ttu-id="dbbe1-166">string</span><span class="sxs-lookup"><span data-stu-id="dbbe1-166">string</span></span>|<span data-ttu-id="dbbe1-167">工作表的显示名称。</span><span class="sxs-lookup"><span data-stu-id="dbbe1-167">The display name of the worksheet.</span></span>|
|<span data-ttu-id="dbbe1-168">position</span><span class="sxs-lookup"><span data-stu-id="dbbe1-168">position</span></span>|<span data-ttu-id="dbbe1-169">int</span><span class="sxs-lookup"><span data-stu-id="dbbe1-169">int</span></span>|<span data-ttu-id="dbbe1-170">工作表在工作簿中的位置，从零开始。</span><span class="sxs-lookup"><span data-stu-id="dbbe1-170">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="dbbe1-171">visibility</span><span class="sxs-lookup"><span data-stu-id="dbbe1-171">visibility</span></span>|<span data-ttu-id="dbbe1-172">string</span><span class="sxs-lookup"><span data-stu-id="dbbe1-172">string</span></span>|<span data-ttu-id="dbbe1-173">在工作表的可见性。</span><span class="sxs-lookup"><span data-stu-id="dbbe1-173">The Visibility of the worksheet.</span></span> <span data-ttu-id="dbbe1-174">可能的值为： `Visible`， `Hidden`， `VeryHidden`。</span><span class="sxs-lookup"><span data-stu-id="dbbe1-174">The possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dbbe1-175">Relationships</span><span class="sxs-lookup"><span data-stu-id="dbbe1-175">Relationships</span></span>
| <span data-ttu-id="dbbe1-176">关系</span><span class="sxs-lookup"><span data-stu-id="dbbe1-176">Relationship</span></span> | <span data-ttu-id="dbbe1-177">类型</span><span class="sxs-lookup"><span data-stu-id="dbbe1-177">Type</span></span>   |<span data-ttu-id="dbbe1-178">说明</span><span class="sxs-lookup"><span data-stu-id="dbbe1-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dbbe1-179">图表</span><span class="sxs-lookup"><span data-stu-id="dbbe1-179">charts</span></span>|<span data-ttu-id="dbbe1-180">[WorkbookChart](chart.md)集合</span><span class="sxs-lookup"><span data-stu-id="dbbe1-180">[WorkbookChart](chart.md) collection</span></span>|<span data-ttu-id="dbbe1-p108">返回属于工作表的图表的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="dbbe1-p108">Returns collection of charts that are part of the worksheet. Read-only.</span></span>|
|<span data-ttu-id="dbbe1-183">names</span><span class="sxs-lookup"><span data-stu-id="dbbe1-183">names</span></span>|<span data-ttu-id="dbbe1-184">[WorkbookNamedItem](nameditem.md)集合</span><span class="sxs-lookup"><span data-stu-id="dbbe1-184">[WorkbookNamedItem](nameditem.md) collection</span></span>|<span data-ttu-id="dbbe1-p109">返回与该工作表关联的名称集合。只读。</span><span class="sxs-lookup"><span data-stu-id="dbbe1-p109">Returns collection of names that are associated with the worksheet. Read-only.</span></span>|
|<span data-ttu-id="dbbe1-187">pivotTables</span><span class="sxs-lookup"><span data-stu-id="dbbe1-187">pivotTables</span></span>|<span data-ttu-id="dbbe1-188">[workbookPivotTable](workbookpivottable.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dbbe1-188">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="dbbe1-189">一组属于工作表的数据透视表对象。</span><span class="sxs-lookup"><span data-stu-id="dbbe1-189">Collection of PivotTables that are part of the worksheet.</span></span> |
|<span data-ttu-id="dbbe1-190">protection</span><span class="sxs-lookup"><span data-stu-id="dbbe1-190">protection</span></span>|[<span data-ttu-id="dbbe1-191">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="dbbe1-191">WorkbookWorksheetProtection</span></span>](worksheetprotection.md)|<span data-ttu-id="dbbe1-p110">返回表工作表的工作表保护对象。只读。</span><span class="sxs-lookup"><span data-stu-id="dbbe1-p110">Returns sheet protection object for a worksheet. Read-only.</span></span>|
|<span data-ttu-id="dbbe1-194">表格</span><span class="sxs-lookup"><span data-stu-id="dbbe1-194">tables</span></span>|<span data-ttu-id="dbbe1-195">[WorkbookTable](table.md)集合</span><span class="sxs-lookup"><span data-stu-id="dbbe1-195">[WorkbookTable](table.md) collection</span></span>|<span data-ttu-id="dbbe1-p111">属于工作表的表的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="dbbe1-p111">Collection of tables that are part of the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dbbe1-198">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dbbe1-198">JSON representation</span></span>

<span data-ttu-id="dbbe1-199">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dbbe1-199">Here is a JSON representation of the resource.</span></span>

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
