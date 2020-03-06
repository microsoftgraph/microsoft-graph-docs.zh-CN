---
title: 工作表资源类型
description: Excel 工作表是由单元格组成的网格。 它可以包含数据、表、图表等。
localization_priority: Priority
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: d9edb4e0ad13f7caf94fd4308f606fccc14861aa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533362"
---
# <a name="worksheet-resource-type"></a><span data-ttu-id="7e2f0-104">工作表资源类型</span><span class="sxs-lookup"><span data-stu-id="7e2f0-104">Worksheet resource type</span></span>

<span data-ttu-id="7e2f0-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e2f0-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7e2f0-106">Excel 工作表是由单元格组成的网格。</span><span class="sxs-lookup"><span data-stu-id="7e2f0-106">An Excel worksheet is a grid of cells.</span></span> <span data-ttu-id="7e2f0-107">它可以包含数据、表、图表等。</span><span class="sxs-lookup"><span data-stu-id="7e2f0-107">It can contain data, tables, charts, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="7e2f0-108">方法</span><span class="sxs-lookup"><span data-stu-id="7e2f0-108">Methods</span></span>

| <span data-ttu-id="7e2f0-109">方法</span><span class="sxs-lookup"><span data-stu-id="7e2f0-109">Method</span></span>           | <span data-ttu-id="7e2f0-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="7e2f0-110">Return Type</span></span>    |<span data-ttu-id="7e2f0-111">说明</span><span class="sxs-lookup"><span data-stu-id="7e2f0-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7e2f0-112">获取工作表</span><span class="sxs-lookup"><span data-stu-id="7e2f0-112">Get Worksheet</span></span>](../api/worksheet-get.md) | [<span data-ttu-id="7e2f0-113">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="7e2f0-113">WorkbookWorksheet</span></span>](worksheet.md) |<span data-ttu-id="7e2f0-114">读取 worksheet 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7e2f0-114">Read properties and relationships of worksheet object.</span></span>|
|[<span data-ttu-id="7e2f0-115">创建图表</span><span class="sxs-lookup"><span data-stu-id="7e2f0-115">Create Chart</span></span>](../api/worksheet-post-charts.md) |[<span data-ttu-id="7e2f0-116">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="7e2f0-116">WorkbookChart</span></span>](chart.md)| <span data-ttu-id="7e2f0-117">通过发布到图表集合创建新的图表。</span><span class="sxs-lookup"><span data-stu-id="7e2f0-117">Create a new Chart by posting to the charts collection.</span></span>|
|[<span data-ttu-id="7e2f0-118">列出名称</span><span class="sxs-lookup"><span data-stu-id="7e2f0-118">List names</span></span>](../api/worksheet-list-names.md) |<span data-ttu-id="7e2f0-119">[WorkbookNamedItem](nameditem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7e2f0-119">[WorkbookNamedItem](nameditem.md) collection</span></span>| <span data-ttu-id="7e2f0-120">获取与工作表关联的命名项的集合。</span><span class="sxs-lookup"><span data-stu-id="7e2f0-120">Get named item collection associated with the worksheet.</span></span>|
|[<span data-ttu-id="7e2f0-121">列出图表</span><span class="sxs-lookup"><span data-stu-id="7e2f0-121">List charts</span></span>](../api/worksheet-list-charts.md) |<span data-ttu-id="7e2f0-122">[WorkbookChart](chart.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7e2f0-122">[WorkbookChart](chart.md) collection</span></span>| <span data-ttu-id="7e2f0-123">获取 Chart 对象集合。</span><span class="sxs-lookup"><span data-stu-id="7e2f0-123">Get a Chart object collection.</span></span>|
|[<span data-ttu-id="7e2f0-124">创建表</span><span class="sxs-lookup"><span data-stu-id="7e2f0-124">Create Table</span></span>](../api/worksheet-post-tables.md) |[<span data-ttu-id="7e2f0-125">WorkbookTable</span><span class="sxs-lookup"><span data-stu-id="7e2f0-125">WorkbookTable</span></span>](table.md)| <span data-ttu-id="7e2f0-126">通过发布到表集合创建新表。</span><span class="sxs-lookup"><span data-stu-id="7e2f0-126">Create a new Table by posting to the tables collection.</span></span>|
|[<span data-ttu-id="7e2f0-127">列出表</span><span class="sxs-lookup"><span data-stu-id="7e2f0-127">List tables</span></span>](../api/worksheet-list-tables.md) |<span data-ttu-id="7e2f0-128">[WorkbookTable](table.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7e2f0-128">[WorkbookTable](table.md) collection</span></span>| <span data-ttu-id="7e2f0-129">获取 Table 对象集合。</span><span class="sxs-lookup"><span data-stu-id="7e2f0-129">Get a Table object collection.</span></span>|
|[<span data-ttu-id="7e2f0-130">更新</span><span class="sxs-lookup"><span data-stu-id="7e2f0-130">Update</span></span>](../api/worksheet-update.md) | [<span data-ttu-id="7e2f0-131">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="7e2f0-131">WorkbookWorksheet</span></span>](worksheet.md)   |<span data-ttu-id="7e2f0-132">更新 Worksheet 对象。</span><span class="sxs-lookup"><span data-stu-id="7e2f0-132">Update Worksheet object.</span></span> |
|[<span data-ttu-id="7e2f0-133">单元格</span><span class="sxs-lookup"><span data-stu-id="7e2f0-133">Cell</span></span>](../api/worksheet-cell.md)|[<span data-ttu-id="7e2f0-134">区域</span><span class="sxs-lookup"><span data-stu-id="7e2f0-134">Range</span></span>](range.md)|<span data-ttu-id="7e2f0-p103">根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。</span><span class="sxs-lookup"><span data-stu-id="7e2f0-p103">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>|
|[<span data-ttu-id="7e2f0-137">区域</span><span class="sxs-lookup"><span data-stu-id="7e2f0-137">Range</span></span>](../api/worksheet-range.md)|[<span data-ttu-id="7e2f0-138">区域</span><span class="sxs-lookup"><span data-stu-id="7e2f0-138">Range</span></span>](range.md)|<span data-ttu-id="7e2f0-139">获取地址或名称指定的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="7e2f0-139">Gets the range object specified by the address or name.</span></span>|
|[<span data-ttu-id="7e2f0-140">Usedrange</span><span class="sxs-lookup"><span data-stu-id="7e2f0-140">Usedrange</span></span>](../api/worksheet-usedrange.md)|[<span data-ttu-id="7e2f0-141">区域</span><span class="sxs-lookup"><span data-stu-id="7e2f0-141">Range</span></span>](range.md)|<span data-ttu-id="7e2f0-p104">使用的区域是包含分配了值或格式化的任何单元格的最小区域。如果工作表为空，此函数将返回左上角的单元格。</span><span class="sxs-lookup"><span data-stu-id="7e2f0-p104">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>|
|[<span data-ttu-id="7e2f0-144">删除</span><span class="sxs-lookup"><span data-stu-id="7e2f0-144">Delete</span></span>](../api/worksheet-delete.md)|<span data-ttu-id="7e2f0-145">无</span><span class="sxs-lookup"><span data-stu-id="7e2f0-145">None</span></span>|<span data-ttu-id="7e2f0-146">从工作簿中删除工作表。</span><span class="sxs-lookup"><span data-stu-id="7e2f0-146">Deletes the worksheet from the workbook.</span></span>|
|[<span data-ttu-id="7e2f0-147">List</span><span class="sxs-lookup"><span data-stu-id="7e2f0-147">List</span></span>](../api/worksheet-list.md) | <span data-ttu-id="7e2f0-148">[WorkbookWorksheet](worksheet.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7e2f0-148">[WorkbookWorksheet](worksheet.md) collection</span></span> |<span data-ttu-id="7e2f0-149">获取 worksheet 对象集合。</span><span class="sxs-lookup"><span data-stu-id="7e2f0-149">Get worksheet object collection.</span></span> |
|[<span data-ttu-id="7e2f0-150">Add</span><span class="sxs-lookup"><span data-stu-id="7e2f0-150">Add</span></span>](../api/worksheetcollection-add.md)|[<span data-ttu-id="7e2f0-151">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="7e2f0-151">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="7e2f0-p105">向工作簿添加新工作表。将工作表添加到现有工作表的末尾。</span><span class="sxs-lookup"><span data-stu-id="7e2f0-p105">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets.</span></span> |
|[<span data-ttu-id="7e2f0-154">List pivotTables</span><span class="sxs-lookup"><span data-stu-id="7e2f0-154">List pivotTables</span></span>](../api/workbookworksheet-list-pivottables.md) |<span data-ttu-id="7e2f0-155">[workbookPivotTable](workbookpivottable.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7e2f0-155">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="7e2f0-156">获取一组 workbookPivotTable 对象。</span><span class="sxs-lookup"><span data-stu-id="7e2f0-156">Get a workbookPivotTable object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="7e2f0-157">属性</span><span class="sxs-lookup"><span data-stu-id="7e2f0-157">Properties</span></span>
| <span data-ttu-id="7e2f0-158">属性</span><span class="sxs-lookup"><span data-stu-id="7e2f0-158">Property</span></span>     | <span data-ttu-id="7e2f0-159">类型</span><span class="sxs-lookup"><span data-stu-id="7e2f0-159">Type</span></span>   |<span data-ttu-id="7e2f0-160">说明</span><span class="sxs-lookup"><span data-stu-id="7e2f0-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e2f0-161">id</span><span class="sxs-lookup"><span data-stu-id="7e2f0-161">id</span></span>|<span data-ttu-id="7e2f0-162">string</span><span class="sxs-lookup"><span data-stu-id="7e2f0-162">string</span></span>|<span data-ttu-id="7e2f0-p106">返回用于唯一标识指定工作簿中工作表的值。即使工作表被重命名或移动，标识符的值仍然相同。只读。</span><span class="sxs-lookup"><span data-stu-id="7e2f0-p106">Returns a value that uniquely identifies the worksheet in a given workbook. The value of the identifier remains the same even when the worksheet is renamed or moved. Read-only.</span></span>|
|<span data-ttu-id="7e2f0-166">name</span><span class="sxs-lookup"><span data-stu-id="7e2f0-166">name</span></span>|<span data-ttu-id="7e2f0-167">string</span><span class="sxs-lookup"><span data-stu-id="7e2f0-167">string</span></span>|<span data-ttu-id="7e2f0-168">工作表的显示名称。</span><span class="sxs-lookup"><span data-stu-id="7e2f0-168">The display name of the worksheet.</span></span>|
|<span data-ttu-id="7e2f0-169">position</span><span class="sxs-lookup"><span data-stu-id="7e2f0-169">position</span></span>|<span data-ttu-id="7e2f0-170">int</span><span class="sxs-lookup"><span data-stu-id="7e2f0-170">int</span></span>|<span data-ttu-id="7e2f0-171">工作表在工作簿中的位置，从零开始。</span><span class="sxs-lookup"><span data-stu-id="7e2f0-171">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="7e2f0-172">visibility</span><span class="sxs-lookup"><span data-stu-id="7e2f0-172">visibility</span></span>|<span data-ttu-id="7e2f0-173">string</span><span class="sxs-lookup"><span data-stu-id="7e2f0-173">string</span></span>|<span data-ttu-id="7e2f0-174">工作表的可见性。</span><span class="sxs-lookup"><span data-stu-id="7e2f0-174">The Visibility of the worksheet.</span></span> <span data-ttu-id="7e2f0-175">可能的值包括 `Visible`、`Hidden`、`VeryHidden`。</span><span class="sxs-lookup"><span data-stu-id="7e2f0-175">The possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e2f0-176">关系</span><span class="sxs-lookup"><span data-stu-id="7e2f0-176">Relationships</span></span>
| <span data-ttu-id="7e2f0-177">关系</span><span class="sxs-lookup"><span data-stu-id="7e2f0-177">Relationship</span></span> | <span data-ttu-id="7e2f0-178">类型</span><span class="sxs-lookup"><span data-stu-id="7e2f0-178">Type</span></span>   |<span data-ttu-id="7e2f0-179">说明</span><span class="sxs-lookup"><span data-stu-id="7e2f0-179">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e2f0-180">图表</span><span class="sxs-lookup"><span data-stu-id="7e2f0-180">charts</span></span>|<span data-ttu-id="7e2f0-181">[WorkbookChart](chart.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7e2f0-181">[WorkbookChart](chart.md) collection</span></span>|<span data-ttu-id="7e2f0-182">返回属于工作表的图表的集合。</span><span class="sxs-lookup"><span data-stu-id="7e2f0-182">Returns collection of charts that are part of the worksheet.</span></span> <span data-ttu-id="7e2f0-183">只读。</span><span class="sxs-lookup"><span data-stu-id="7e2f0-183">Read-only.</span></span>|
|<span data-ttu-id="7e2f0-184">names</span><span class="sxs-lookup"><span data-stu-id="7e2f0-184">names</span></span>|<span data-ttu-id="7e2f0-185">[WorkbookNamedItem](nameditem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7e2f0-185">[WorkbookNamedItem](nameditem.md) collection</span></span>|<span data-ttu-id="7e2f0-186">返回与该工作表关联的名称集合。</span><span class="sxs-lookup"><span data-stu-id="7e2f0-186">Returns collection of names that are associated with the worksheet.</span></span> <span data-ttu-id="7e2f0-187">只读。</span><span class="sxs-lookup"><span data-stu-id="7e2f0-187">Read-only.</span></span>|
|<span data-ttu-id="7e2f0-188">pivotTables</span><span class="sxs-lookup"><span data-stu-id="7e2f0-188">pivotTables</span></span>|<span data-ttu-id="7e2f0-189">[workbookPivotTable](workbookpivottable.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7e2f0-189">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="7e2f0-190">一组属于工作表的数据透视表对象。</span><span class="sxs-lookup"><span data-stu-id="7e2f0-190">Collection of PivotTables that are part of the worksheet.</span></span> |
|<span data-ttu-id="7e2f0-191">保护</span><span class="sxs-lookup"><span data-stu-id="7e2f0-191">protection</span></span>|[<span data-ttu-id="7e2f0-192">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="7e2f0-192">WorkbookWorksheetProtection</span></span>](worksheetprotection.md)|<span data-ttu-id="7e2f0-p110">返回表工作表的工作表保护对象。只读。</span><span class="sxs-lookup"><span data-stu-id="7e2f0-p110">Returns sheet protection object for a worksheet. Read-only.</span></span>|
|<span data-ttu-id="7e2f0-195">表格</span><span class="sxs-lookup"><span data-stu-id="7e2f0-195">tables</span></span>|<span data-ttu-id="7e2f0-196">[WorkbookTable](table.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7e2f0-196">[WorkbookTable](table.md) collection</span></span>|<span data-ttu-id="7e2f0-197">属于工作表的表的集合。</span><span class="sxs-lookup"><span data-stu-id="7e2f0-197">Collection of tables that are part of the worksheet.</span></span> <span data-ttu-id="7e2f0-198">只读。</span><span class="sxs-lookup"><span data-stu-id="7e2f0-198">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7e2f0-199">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7e2f0-199">JSON representation</span></span>

<span data-ttu-id="7e2f0-200">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e2f0-200">Here is a JSON representation of the resource.</span></span>

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
