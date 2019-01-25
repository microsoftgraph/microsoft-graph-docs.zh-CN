---
title: 工作表资源类型
description: Excel 工作表是由单元格组成的网格。它可以包含数据、表、图表等。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: beffb9747045d0d3792d994237710e886ff0b3d8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509145"
---
# <a name="worksheet-resource-type"></a><span data-ttu-id="26976-104">工作表资源类型</span><span class="sxs-lookup"><span data-stu-id="26976-104">Worksheet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26976-p102">Excel 工作表是由单元格组成的网格。它可以包含数据、表、图表等。</span><span class="sxs-lookup"><span data-stu-id="26976-p102">An Excel worksheet is a grid of cells. It can contain data, tables, charts, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="26976-107">方法</span><span class="sxs-lookup"><span data-stu-id="26976-107">Methods</span></span>

| <span data-ttu-id="26976-108">方法</span><span class="sxs-lookup"><span data-stu-id="26976-108">Method</span></span>           | <span data-ttu-id="26976-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="26976-109">Return Type</span></span>    |<span data-ttu-id="26976-110">说明</span><span class="sxs-lookup"><span data-stu-id="26976-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26976-111">获取工作表</span><span class="sxs-lookup"><span data-stu-id="26976-111">[Get Worksheet](../api/worksheet-get.md)</span></span> | [<span data-ttu-id="26976-112">Worksheet</span><span class="sxs-lookup"><span data-stu-id="26976-112">Worksheet</span></span>](worksheet.md) |<span data-ttu-id="26976-113">读取 worksheet 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="26976-113">Read properties and relationships of worksheet object.</span></span>|
|<span data-ttu-id="26976-114">创建图表</span><span class="sxs-lookup"><span data-stu-id="26976-114">[Create Chart](../api/worksheet-post-charts.md)</span></span> |[<span data-ttu-id="26976-115">Chart</span><span class="sxs-lookup"><span data-stu-id="26976-115">Chart</span></span>](chart.md)| <span data-ttu-id="26976-116">通过发布到图表集合创建新的图表。</span><span class="sxs-lookup"><span data-stu-id="26976-116">Create a new Chart by posting to the charts collection.</span></span>|
|<span data-ttu-id="26976-117">列出名称</span><span class="sxs-lookup"><span data-stu-id="26976-117">[List names](../api/worksheet-list-names.md)</span></span> |<span data-ttu-id="26976-118">[NamedItem](nameditem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="26976-118">[NamedItem](nameditem.md) collection</span></span>| <span data-ttu-id="26976-119">获取与工作表关联的命名项的集合。</span><span class="sxs-lookup"><span data-stu-id="26976-119">Get named item collection associated with the worksheet.</span></span>|
|<span data-ttu-id="26976-120">列出图表</span><span class="sxs-lookup"><span data-stu-id="26976-120">[List charts](../api/worksheet-list-charts.md)</span></span> |<span data-ttu-id="26976-121">图表 集合</span><span class="sxs-lookup"><span data-stu-id="26976-121">[Chart](chart.md) collection</span></span>| <span data-ttu-id="26976-122">获取 Chart 对象集合。</span><span class="sxs-lookup"><span data-stu-id="26976-122">Get a Chart object collection.</span></span>|
|<span data-ttu-id="26976-123">创建表</span><span class="sxs-lookup"><span data-stu-id="26976-123">[Create Table](../api/worksheet-post-tables.md)</span></span> |[<span data-ttu-id="26976-124">Table</span><span class="sxs-lookup"><span data-stu-id="26976-124">Table</span></span>](table.md)| <span data-ttu-id="26976-125">通过发布到表集合创建新表。</span><span class="sxs-lookup"><span data-stu-id="26976-125">Create a new Table by posting to the tables collection.</span></span>|
|<span data-ttu-id="26976-126">列出表</span><span class="sxs-lookup"><span data-stu-id="26976-126">[List tables](../api/worksheet-list-tables.md)</span></span> |<span data-ttu-id="26976-127">[表](table.md) 集合</span><span class="sxs-lookup"><span data-stu-id="26976-127">[Table](table.md) collection</span></span>| <span data-ttu-id="26976-128">获取 Table 对象集合。</span><span class="sxs-lookup"><span data-stu-id="26976-128">Get a Table object collection.</span></span>|
|[<span data-ttu-id="26976-129">Update</span><span class="sxs-lookup"><span data-stu-id="26976-129">Update</span></span>](../api/worksheet-update.md) | [<span data-ttu-id="26976-130">Worksheet</span><span class="sxs-lookup"><span data-stu-id="26976-130">Worksheet</span></span>](worksheet.md)   |<span data-ttu-id="26976-131">更新 Worksheet 对象。</span><span class="sxs-lookup"><span data-stu-id="26976-131">Update Worksheet object.</span></span> |
|[<span data-ttu-id="26976-132">单元格</span><span class="sxs-lookup"><span data-stu-id="26976-132">Cell</span></span>](../api/worksheet-cell.md)|[<span data-ttu-id="26976-133">Range</span><span class="sxs-lookup"><span data-stu-id="26976-133">Range</span></span>](range.md)|<span data-ttu-id="26976-p103">根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。</span><span class="sxs-lookup"><span data-stu-id="26976-p103">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>|
|[<span data-ttu-id="26976-136">区域</span><span class="sxs-lookup"><span data-stu-id="26976-136">Range</span></span>](../api/worksheet-range.md)|[<span data-ttu-id="26976-137">Range</span><span class="sxs-lookup"><span data-stu-id="26976-137">Range</span></span>](range.md)|<span data-ttu-id="26976-138">获取地址或名称指定的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="26976-138">Gets the range object specified by the address or name.</span></span>|
|[<span data-ttu-id="26976-139">Usedrange</span><span class="sxs-lookup"><span data-stu-id="26976-139">Usedrange</span></span>](../api/worksheet-usedrange.md)|[<span data-ttu-id="26976-140">区域</span><span class="sxs-lookup"><span data-stu-id="26976-140">Range</span></span>](range.md)|<span data-ttu-id="26976-p104">使用的区域是包含分配了值或格式化的任何单元格的最小区域。如果工作表为空，此函数将返回左上角的单元格。</span><span class="sxs-lookup"><span data-stu-id="26976-p104">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>|
|[<span data-ttu-id="26976-143">删除</span><span class="sxs-lookup"><span data-stu-id="26976-143">Delete</span></span>](../api/worksheet-delete.md)|<span data-ttu-id="26976-144">无</span><span class="sxs-lookup"><span data-stu-id="26976-144">None</span></span>|<span data-ttu-id="26976-145">从工作簿中删除工作表。</span><span class="sxs-lookup"><span data-stu-id="26976-145">Deletes the worksheet from the workbook.</span></span>|
|[<span data-ttu-id="26976-146">List</span><span class="sxs-lookup"><span data-stu-id="26976-146">List</span></span>](../api/worksheet-list.md) | <span data-ttu-id="26976-147">[Worksheet](worksheet.md) 集合</span><span class="sxs-lookup"><span data-stu-id="26976-147">[Worksheet](worksheet.md) collection</span></span> |<span data-ttu-id="26976-148">获取 worksheet 对象集合。</span><span class="sxs-lookup"><span data-stu-id="26976-148">Get worksheet object collection.</span></span> |
|[<span data-ttu-id="26976-149">Add</span><span class="sxs-lookup"><span data-stu-id="26976-149">Add</span></span>](../api/worksheetcollection-add.md)|[<span data-ttu-id="26976-150">Worksheet</span><span class="sxs-lookup"><span data-stu-id="26976-150">Worksheet</span></span>](worksheet.md)|<span data-ttu-id="26976-p105">向工作簿添加新工作表。将工作表添加到现有工作表的末尾。</span><span class="sxs-lookup"><span data-stu-id="26976-p105">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets.</span></span> |
|<span data-ttu-id="26976-153">List pivotTables</span><span class="sxs-lookup"><span data-stu-id="26976-153">[List pivotTables](../api/workbookworksheet-list-pivottables.md)</span></span> |<span data-ttu-id="26976-154">workbookPivotTable 集合</span><span class="sxs-lookup"><span data-stu-id="26976-154">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="26976-155">获取一组 workbookPivotTable 对象。</span><span class="sxs-lookup"><span data-stu-id="26976-155">Get a workbookPivotTable object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="26976-156">属性</span><span class="sxs-lookup"><span data-stu-id="26976-156">Properties</span></span>
| <span data-ttu-id="26976-157">属性</span><span class="sxs-lookup"><span data-stu-id="26976-157">Property</span></span>     | <span data-ttu-id="26976-158">类型</span><span class="sxs-lookup"><span data-stu-id="26976-158">Type</span></span>   |<span data-ttu-id="26976-159">说明</span><span class="sxs-lookup"><span data-stu-id="26976-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26976-160">id</span><span class="sxs-lookup"><span data-stu-id="26976-160">id</span></span>|<span data-ttu-id="26976-161">string</span><span class="sxs-lookup"><span data-stu-id="26976-161">string</span></span>|<span data-ttu-id="26976-p106">返回用于唯一标识指定工作簿中工作表的值。即使工作表被重命名或移动，标识符的值仍然相同。只读。</span><span class="sxs-lookup"><span data-stu-id="26976-p106">Returns a value that uniquely identifies the worksheet in a given workbook. The value of the identifier remains the same even when the worksheet is renamed or moved. Read-only.</span></span>|
|<span data-ttu-id="26976-165">name</span><span class="sxs-lookup"><span data-stu-id="26976-165">name</span></span>|<span data-ttu-id="26976-166">string</span><span class="sxs-lookup"><span data-stu-id="26976-166">string</span></span>|<span data-ttu-id="26976-167">工作表的显示名称。</span><span class="sxs-lookup"><span data-stu-id="26976-167">The display name of the worksheet.</span></span>|
|<span data-ttu-id="26976-168">position</span><span class="sxs-lookup"><span data-stu-id="26976-168">position</span></span>|<span data-ttu-id="26976-169">int</span><span class="sxs-lookup"><span data-stu-id="26976-169">int</span></span>|<span data-ttu-id="26976-170">工作表在工作簿中的位置，从零开始。</span><span class="sxs-lookup"><span data-stu-id="26976-170">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="26976-171">visibility</span><span class="sxs-lookup"><span data-stu-id="26976-171">visibility</span></span>|<span data-ttu-id="26976-172">string</span><span class="sxs-lookup"><span data-stu-id="26976-172">string</span></span>|<span data-ttu-id="26976-p107">工作表的可见性。可能的值是：`Visible`、`Hidden`、`VeryHidden`。</span><span class="sxs-lookup"><span data-stu-id="26976-p107">The Visibility of the worksheet. Possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26976-175">关系</span><span class="sxs-lookup"><span data-stu-id="26976-175">Relationships</span></span>
| <span data-ttu-id="26976-176">关系</span><span class="sxs-lookup"><span data-stu-id="26976-176">Relationship</span></span> | <span data-ttu-id="26976-177">类型</span><span class="sxs-lookup"><span data-stu-id="26976-177">Type</span></span>   |<span data-ttu-id="26976-178">说明</span><span class="sxs-lookup"><span data-stu-id="26976-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26976-179">图表</span><span class="sxs-lookup"><span data-stu-id="26976-179">charts</span></span>|<span data-ttu-id="26976-180">[图表](chart.md) 集合</span><span class="sxs-lookup"><span data-stu-id="26976-180">[Chart](chart.md) collection</span></span>|<span data-ttu-id="26976-p108">返回属于工作表的图表的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="26976-p108">Returns collection of charts that are part of the worksheet. Read-only.</span></span>|
|<span data-ttu-id="26976-183">names</span><span class="sxs-lookup"><span data-stu-id="26976-183">names</span></span>|<span data-ttu-id="26976-184">[NamedItem](nameditem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="26976-184">[NamedItem](nameditem.md) collection</span></span>|<span data-ttu-id="26976-p109">返回与该工作表关联的名称集合。只读。</span><span class="sxs-lookup"><span data-stu-id="26976-p109">Returns collection of names that are associated with the worksheet. Read-only.</span></span>|
|<span data-ttu-id="26976-187">pivotTables</span><span class="sxs-lookup"><span data-stu-id="26976-187">pivotTables</span></span>|<span data-ttu-id="26976-188">[workbookPivotTable](workbookpivottable.md) 集合</span><span class="sxs-lookup"><span data-stu-id="26976-188">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="26976-189">一组属于工作表的数据透视表对象。</span><span class="sxs-lookup"><span data-stu-id="26976-189">Collection of PivotTables that are part of the worksheet.</span></span> |
|<span data-ttu-id="26976-190">protection</span><span class="sxs-lookup"><span data-stu-id="26976-190">protection</span></span>|[<span data-ttu-id="26976-191">WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="26976-191">WorksheetProtection</span></span>](worksheetprotection.md)|<span data-ttu-id="26976-p110">返回表工作表的工作表保护对象。只读。</span><span class="sxs-lookup"><span data-stu-id="26976-p110">Returns sheet protection object for a worksheet. Read-only.</span></span>|
|<span data-ttu-id="26976-194">表格</span><span class="sxs-lookup"><span data-stu-id="26976-194">tables</span></span>|<span data-ttu-id="26976-195">[Table](table.md) 集合</span><span class="sxs-lookup"><span data-stu-id="26976-195">[Table](table.md) collection</span></span>|<span data-ttu-id="26976-p111">属于工作表的表的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="26976-p111">Collection of tables that are part of the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="26976-198">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="26976-198">JSON representation</span></span>

<span data-ttu-id="26976-199">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26976-199">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.worksheet"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/worksheet.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
