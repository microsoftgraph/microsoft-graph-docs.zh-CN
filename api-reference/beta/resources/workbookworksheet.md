---
title: workbookWorksheet 资源类型
description: Excel 工作表是由单元格组成的网格。 它可以包含数据、表、图表等。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: edb6e13c975c0dc65c19604aef7256d63a409141
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519104"
---
# <a name="workbookworksheet-resource-type"></a><span data-ttu-id="2b231-104">workbookWorksheet 资源类型</span><span class="sxs-lookup"><span data-stu-id="2b231-104">workbookWorksheet resource type</span></span>

<span data-ttu-id="2b231-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="2b231-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b231-106">Excel 工作表是由单元格组成的网格。</span><span class="sxs-lookup"><span data-stu-id="2b231-106">An Excel worksheet is a grid of cells.</span></span> <span data-ttu-id="2b231-107">它可以包含数据、表、图表等。</span><span class="sxs-lookup"><span data-stu-id="2b231-107">It can contain data, tables, charts, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="2b231-108">方法</span><span class="sxs-lookup"><span data-stu-id="2b231-108">Methods</span></span>

| <span data-ttu-id="2b231-109">方法</span><span class="sxs-lookup"><span data-stu-id="2b231-109">Method</span></span>           | <span data-ttu-id="2b231-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="2b231-110">Return Type</span></span>    |<span data-ttu-id="2b231-111">说明</span><span class="sxs-lookup"><span data-stu-id="2b231-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2b231-112">获取工作表</span><span class="sxs-lookup"><span data-stu-id="2b231-112">Get Worksheet</span></span>](../api/worksheet-get.md) | [<span data-ttu-id="2b231-113">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="2b231-113">workbookWorksheet</span></span>](workbookworksheet.md) |<span data-ttu-id="2b231-114">读取 worksheet 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2b231-114">Read properties and relationships of worksheet object.</span></span>|
|[<span data-ttu-id="2b231-115">创建图表</span><span class="sxs-lookup"><span data-stu-id="2b231-115">Create Chart</span></span>](../api/worksheet-post-charts.md) |[<span data-ttu-id="2b231-116">workbookChart</span><span class="sxs-lookup"><span data-stu-id="2b231-116">workbookChart</span></span>](workbookchart.md)| <span data-ttu-id="2b231-117">通过发布到图表集合创建新的图表。</span><span class="sxs-lookup"><span data-stu-id="2b231-117">Create a new Chart by posting to the charts collection.</span></span>|
|[<span data-ttu-id="2b231-118">列出名称</span><span class="sxs-lookup"><span data-stu-id="2b231-118">List names</span></span>](../api/worksheet-list-names.md) |<span data-ttu-id="2b231-119">[workbookNamedItem](workbooknameditem.md)集合</span><span class="sxs-lookup"><span data-stu-id="2b231-119">[workbookNamedItem](workbooknameditem.md) collection</span></span>| <span data-ttu-id="2b231-120">获取与工作表关联的命名项的集合。</span><span class="sxs-lookup"><span data-stu-id="2b231-120">Get named item collection associated with the worksheet.</span></span>|
|[<span data-ttu-id="2b231-121">列出图表</span><span class="sxs-lookup"><span data-stu-id="2b231-121">List charts</span></span>](../api/worksheet-list-charts.md) |<span data-ttu-id="2b231-122">[workbookChart](workbookchart.md)集合</span><span class="sxs-lookup"><span data-stu-id="2b231-122">[workbookChart](workbookchart.md) collection</span></span>| <span data-ttu-id="2b231-123">获取 Chart 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2b231-123">Get a Chart object collection.</span></span>|
|[<span data-ttu-id="2b231-124">创建表</span><span class="sxs-lookup"><span data-stu-id="2b231-124">Create Table</span></span>](../api/worksheet-post-tables.md) |[<span data-ttu-id="2b231-125">workbookTable</span><span class="sxs-lookup"><span data-stu-id="2b231-125">workbookTable</span></span>](workbooktable.md)| <span data-ttu-id="2b231-126">通过发布到表集合创建新表。</span><span class="sxs-lookup"><span data-stu-id="2b231-126">Create a new Table by posting to the tables collection.</span></span>|
|[<span data-ttu-id="2b231-127">列出表</span><span class="sxs-lookup"><span data-stu-id="2b231-127">List tables</span></span>](../api/worksheet-list-tables.md) |<span data-ttu-id="2b231-128">[workbookTable](workbooktable.md)集合</span><span class="sxs-lookup"><span data-stu-id="2b231-128">[workbookTable](workbooktable.md) collection</span></span>| <span data-ttu-id="2b231-129">获取 Table 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2b231-129">Get a Table object collection.</span></span>|
|[<span data-ttu-id="2b231-130">更新</span><span class="sxs-lookup"><span data-stu-id="2b231-130">Update</span></span>](../api/worksheet-update.md) | [<span data-ttu-id="2b231-131">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="2b231-131">workbookWorksheet</span></span>](workbookworksheet.md)   |<span data-ttu-id="2b231-132">更新 Worksheet 对象。</span><span class="sxs-lookup"><span data-stu-id="2b231-132">Update Worksheet object.</span></span> |
|[<span data-ttu-id="2b231-133">单元格</span><span class="sxs-lookup"><span data-stu-id="2b231-133">Cell</span></span>](../api/worksheet-cell.md)|[<span data-ttu-id="2b231-134">workbookRange</span><span class="sxs-lookup"><span data-stu-id="2b231-134">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="2b231-p103">根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。</span><span class="sxs-lookup"><span data-stu-id="2b231-p103">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>|
|[<span data-ttu-id="2b231-137">区域</span><span class="sxs-lookup"><span data-stu-id="2b231-137">Range</span></span>](../api/worksheet-range.md)|[<span data-ttu-id="2b231-138">workbookRange</span><span class="sxs-lookup"><span data-stu-id="2b231-138">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="2b231-139">获取地址或名称指定的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="2b231-139">Gets the range object specified by the address or name.</span></span>|
|[<span data-ttu-id="2b231-140">Usedrange</span><span class="sxs-lookup"><span data-stu-id="2b231-140">Usedrange</span></span>](../api/worksheet-usedrange.md)|[<span data-ttu-id="2b231-141">workbookRange</span><span class="sxs-lookup"><span data-stu-id="2b231-141">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="2b231-p104">使用的区域是包含分配了值或格式化的任何单元格的最小区域。如果工作表为空，此函数将返回左上角的单元格。</span><span class="sxs-lookup"><span data-stu-id="2b231-p104">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>|
|[<span data-ttu-id="2b231-144">删除</span><span class="sxs-lookup"><span data-stu-id="2b231-144">Delete</span></span>](../api/worksheet-delete.md)|<span data-ttu-id="2b231-145">无</span><span class="sxs-lookup"><span data-stu-id="2b231-145">None</span></span>|<span data-ttu-id="2b231-146">从工作簿中删除工作表。</span><span class="sxs-lookup"><span data-stu-id="2b231-146">Deletes the worksheet from the workbook.</span></span>|
|[<span data-ttu-id="2b231-147">List</span><span class="sxs-lookup"><span data-stu-id="2b231-147">List</span></span>](../api/worksheet-list.md) | <span data-ttu-id="2b231-148">[workbookWorksheet](workbookworksheet.md)集合</span><span class="sxs-lookup"><span data-stu-id="2b231-148">[workbookWorksheet](workbookworksheet.md) collection</span></span> |<span data-ttu-id="2b231-149">获取 worksheet 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2b231-149">Get worksheet object collection.</span></span> |
|[<span data-ttu-id="2b231-150">Add</span><span class="sxs-lookup"><span data-stu-id="2b231-150">Add</span></span>](../api/worksheetcollection-add.md)|[<span data-ttu-id="2b231-151">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="2b231-151">workbookWorksheet</span></span>](workbookworksheet.md)|<span data-ttu-id="2b231-p105">向工作簿添加新工作表。将工作表添加到现有工作表的末尾。</span><span class="sxs-lookup"><span data-stu-id="2b231-p105">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets.</span></span> |
|[<span data-ttu-id="2b231-154">List pivotTables</span><span class="sxs-lookup"><span data-stu-id="2b231-154">List pivotTables</span></span>](../api/workbookworksheet-list-pivottables.md) |<span data-ttu-id="2b231-155">[workbookPivotTable](workbookpivottable.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2b231-155">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="2b231-156">获取一组 workbookPivotTable 对象。</span><span class="sxs-lookup"><span data-stu-id="2b231-156">Get a workbookPivotTable object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="2b231-157">属性</span><span class="sxs-lookup"><span data-stu-id="2b231-157">Properties</span></span>
| <span data-ttu-id="2b231-158">属性</span><span class="sxs-lookup"><span data-stu-id="2b231-158">Property</span></span>     | <span data-ttu-id="2b231-159">类型</span><span class="sxs-lookup"><span data-stu-id="2b231-159">Type</span></span>   |<span data-ttu-id="2b231-160">说明</span><span class="sxs-lookup"><span data-stu-id="2b231-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b231-161">id</span><span class="sxs-lookup"><span data-stu-id="2b231-161">id</span></span>|<span data-ttu-id="2b231-162">string</span><span class="sxs-lookup"><span data-stu-id="2b231-162">string</span></span>|<span data-ttu-id="2b231-p106">返回用于唯一标识指定工作簿中工作表的值。即使工作表被重命名或移动，标识符的值仍然相同。只读。</span><span class="sxs-lookup"><span data-stu-id="2b231-p106">Returns a value that uniquely identifies the worksheet in a given workbook. The value of the identifier remains the same even when the worksheet is renamed or moved. Read-only.</span></span>|
|<span data-ttu-id="2b231-166">name</span><span class="sxs-lookup"><span data-stu-id="2b231-166">name</span></span>|<span data-ttu-id="2b231-167">string</span><span class="sxs-lookup"><span data-stu-id="2b231-167">string</span></span>|<span data-ttu-id="2b231-168">工作表的显示名称。</span><span class="sxs-lookup"><span data-stu-id="2b231-168">The display name of the worksheet.</span></span>|
|<span data-ttu-id="2b231-169">position</span><span class="sxs-lookup"><span data-stu-id="2b231-169">position</span></span>|<span data-ttu-id="2b231-170">int</span><span class="sxs-lookup"><span data-stu-id="2b231-170">int</span></span>|<span data-ttu-id="2b231-171">工作表在工作簿中的位置，从零开始。</span><span class="sxs-lookup"><span data-stu-id="2b231-171">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="2b231-172">visibility</span><span class="sxs-lookup"><span data-stu-id="2b231-172">visibility</span></span>|<span data-ttu-id="2b231-173">string</span><span class="sxs-lookup"><span data-stu-id="2b231-173">string</span></span>|<span data-ttu-id="2b231-174">工作表的可见性。</span><span class="sxs-lookup"><span data-stu-id="2b231-174">The Visibility of the worksheet.</span></span> <span data-ttu-id="2b231-175">可能的值包括 `Visible`、`Hidden`、`VeryHidden`。</span><span class="sxs-lookup"><span data-stu-id="2b231-175">The possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b231-176">关系</span><span class="sxs-lookup"><span data-stu-id="2b231-176">Relationships</span></span>
| <span data-ttu-id="2b231-177">关系</span><span class="sxs-lookup"><span data-stu-id="2b231-177">Relationship</span></span> | <span data-ttu-id="2b231-178">类型</span><span class="sxs-lookup"><span data-stu-id="2b231-178">Type</span></span>   |<span data-ttu-id="2b231-179">说明</span><span class="sxs-lookup"><span data-stu-id="2b231-179">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b231-180">图表</span><span class="sxs-lookup"><span data-stu-id="2b231-180">charts</span></span>|<span data-ttu-id="2b231-181">[workbookChart](workbookchart.md)集合</span><span class="sxs-lookup"><span data-stu-id="2b231-181">[workbookChart](workbookchart.md) collection</span></span>|<span data-ttu-id="2b231-182">返回属于工作表的图表的集合。</span><span class="sxs-lookup"><span data-stu-id="2b231-182">Returns collection of charts that are part of the worksheet.</span></span> <span data-ttu-id="2b231-183">只读。</span><span class="sxs-lookup"><span data-stu-id="2b231-183">Read-only.</span></span>|
|<span data-ttu-id="2b231-184">names</span><span class="sxs-lookup"><span data-stu-id="2b231-184">names</span></span>|<span data-ttu-id="2b231-185">[workbookNamedItem](workbooknameditem.md)集合</span><span class="sxs-lookup"><span data-stu-id="2b231-185">[workbookNamedItem](workbooknameditem.md) collection</span></span>|<span data-ttu-id="2b231-186">返回与该工作表关联的名称集合。</span><span class="sxs-lookup"><span data-stu-id="2b231-186">Returns collection of names that are associated with the worksheet.</span></span> <span data-ttu-id="2b231-187">只读。</span><span class="sxs-lookup"><span data-stu-id="2b231-187">Read-only.</span></span>|
|<span data-ttu-id="2b231-188">pivotTables</span><span class="sxs-lookup"><span data-stu-id="2b231-188">pivotTables</span></span>|<span data-ttu-id="2b231-189">[workbookPivotTable](workbookpivottable.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2b231-189">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="2b231-190">一组属于工作表的数据透视表对象。</span><span class="sxs-lookup"><span data-stu-id="2b231-190">Collection of PivotTables that are part of the worksheet.</span></span> |
|<span data-ttu-id="2b231-191">保护</span><span class="sxs-lookup"><span data-stu-id="2b231-191">protection</span></span>|[<span data-ttu-id="2b231-192">workbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="2b231-192">workbookWorksheetProtection</span></span>](workbookworksheetprotection.md)|<span data-ttu-id="2b231-p110">返回表工作表的工作表保护对象。只读。</span><span class="sxs-lookup"><span data-stu-id="2b231-p110">Returns sheet protection object for a worksheet. Read-only.</span></span>|
|<span data-ttu-id="2b231-195">表格</span><span class="sxs-lookup"><span data-stu-id="2b231-195">tables</span></span>|<span data-ttu-id="2b231-196">[workbookTable](workbooktable.md)集合</span><span class="sxs-lookup"><span data-stu-id="2b231-196">[workbookTable](workbooktable.md) collection</span></span>|<span data-ttu-id="2b231-197">属于工作表的表的集合。</span><span class="sxs-lookup"><span data-stu-id="2b231-197">Collection of tables that are part of the worksheet.</span></span> <span data-ttu-id="2b231-198">只读。</span><span class="sxs-lookup"><span data-stu-id="2b231-198">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2b231-199">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2b231-199">JSON representation</span></span>

<span data-ttu-id="2b231-200">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b231-200">Here is a JSON representation of the resource.</span></span>

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
