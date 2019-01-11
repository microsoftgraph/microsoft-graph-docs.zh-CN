---
title: 工作表资源类型
description: Excel 工作表是由单元格组成的网格。它可以包含数据、表、图表等。
localization_priority: Normal
ms.openlocfilehash: 690596bfe6df5f6bfd98f7f5bd37021e47132152
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807796"
---
# <a name="worksheet-resource-type"></a><span data-ttu-id="83af5-104">工作表资源类型</span><span class="sxs-lookup"><span data-stu-id="83af5-104">Worksheet resource type</span></span>

> <span data-ttu-id="83af5-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="83af5-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="83af5-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="83af5-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="83af5-p103">Excel 工作表是由单元格组成的网格。它可以包含数据、表、图表等。</span><span class="sxs-lookup"><span data-stu-id="83af5-p103">An Excel worksheet is a grid of cells. It can contain data, tables, charts, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="83af5-109">方法</span><span class="sxs-lookup"><span data-stu-id="83af5-109">Methods</span></span>

| <span data-ttu-id="83af5-110">方法</span><span class="sxs-lookup"><span data-stu-id="83af5-110">Method</span></span>           | <span data-ttu-id="83af5-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="83af5-111">Return Type</span></span>    |<span data-ttu-id="83af5-112">说明</span><span class="sxs-lookup"><span data-stu-id="83af5-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="83af5-113">获取工作表</span><span class="sxs-lookup"><span data-stu-id="83af5-113">Get Worksheet</span></span>](../api/worksheet-get.md) | [<span data-ttu-id="83af5-114">Worksheet</span><span class="sxs-lookup"><span data-stu-id="83af5-114">Worksheet</span></span>](worksheet.md) |<span data-ttu-id="83af5-115">读取 worksheet 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="83af5-115">Read properties and relationships of worksheet object.</span></span>|
|[<span data-ttu-id="83af5-116">创建图表</span><span class="sxs-lookup"><span data-stu-id="83af5-116">Create Chart</span></span>](../api/worksheet-post-charts.md) |[<span data-ttu-id="83af5-117">Chart</span><span class="sxs-lookup"><span data-stu-id="83af5-117">Chart</span></span>](chart.md)| <span data-ttu-id="83af5-118">通过发布到图表集合创建新的图表。</span><span class="sxs-lookup"><span data-stu-id="83af5-118">Create a new Chart by posting to the charts collection.</span></span>|
|[<span data-ttu-id="83af5-119">列出名称</span><span class="sxs-lookup"><span data-stu-id="83af5-119">List names</span></span>](../api/worksheet-list-names.md) |<span data-ttu-id="83af5-120">[NamedItem](nameditem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="83af5-120">[NamedItem](nameditem.md) collection</span></span>| <span data-ttu-id="83af5-121">获取与工作表关联的命名项的集合。</span><span class="sxs-lookup"><span data-stu-id="83af5-121">Get named item collection associated with the worksheet.</span></span>|
|[<span data-ttu-id="83af5-122">列出图表</span><span class="sxs-lookup"><span data-stu-id="83af5-122">List charts</span></span>](../api/worksheet-list-charts.md) |<span data-ttu-id="83af5-123">[图表](chart.md) 集合</span><span class="sxs-lookup"><span data-stu-id="83af5-123">[Chart](chart.md) collection</span></span>| <span data-ttu-id="83af5-124">获取 Chart 对象集合。</span><span class="sxs-lookup"><span data-stu-id="83af5-124">Get a Chart object collection.</span></span>|
|[<span data-ttu-id="83af5-125">创建表</span><span class="sxs-lookup"><span data-stu-id="83af5-125">Create Table</span></span>](../api/worksheet-post-tables.md) |[<span data-ttu-id="83af5-126">Table</span><span class="sxs-lookup"><span data-stu-id="83af5-126">Table</span></span>](table.md)| <span data-ttu-id="83af5-127">通过发布到表集合创建新表。</span><span class="sxs-lookup"><span data-stu-id="83af5-127">Create a new Table by posting to the tables collection.</span></span>|
|[<span data-ttu-id="83af5-128">列出表</span><span class="sxs-lookup"><span data-stu-id="83af5-128">List tables</span></span>](../api/worksheet-list-tables.md) |<span data-ttu-id="83af5-129">[表](table.md) 集合</span><span class="sxs-lookup"><span data-stu-id="83af5-129">[Table](table.md) collection</span></span>| <span data-ttu-id="83af5-130">获取 Table 对象集合。</span><span class="sxs-lookup"><span data-stu-id="83af5-130">Get a Table object collection.</span></span>|
|[<span data-ttu-id="83af5-131">Update</span><span class="sxs-lookup"><span data-stu-id="83af5-131">Update</span></span>](../api/worksheet-update.md) | [<span data-ttu-id="83af5-132">Worksheet</span><span class="sxs-lookup"><span data-stu-id="83af5-132">Worksheet</span></span>](worksheet.md)   |<span data-ttu-id="83af5-133">更新 Worksheet 对象。</span><span class="sxs-lookup"><span data-stu-id="83af5-133">Update Worksheet object.</span></span> |
|[<span data-ttu-id="83af5-134">Cell</span><span class="sxs-lookup"><span data-stu-id="83af5-134">Cell</span></span>](../api/worksheet-cell.md)|[<span data-ttu-id="83af5-135">Range</span><span class="sxs-lookup"><span data-stu-id="83af5-135">Range</span></span>](range.md)|<span data-ttu-id="83af5-p104">根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。</span><span class="sxs-lookup"><span data-stu-id="83af5-p104">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>|
|[<span data-ttu-id="83af5-138">区域</span><span class="sxs-lookup"><span data-stu-id="83af5-138">Range</span></span>](../api/worksheet-range.md)|[<span data-ttu-id="83af5-139">Range</span><span class="sxs-lookup"><span data-stu-id="83af5-139">Range</span></span>](range.md)|<span data-ttu-id="83af5-140">获取地址或名称指定的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="83af5-140">Gets the range object specified by the address or name.</span></span>|
|[<span data-ttu-id="83af5-141">Usedrange</span><span class="sxs-lookup"><span data-stu-id="83af5-141">Usedrange</span></span>](../api/worksheet-usedrange.md)|[<span data-ttu-id="83af5-142">Range</span><span class="sxs-lookup"><span data-stu-id="83af5-142">Range</span></span>](range.md)|<span data-ttu-id="83af5-p105">使用的区域是包含分配了值或格式化的任何单元格的最小区域。如果工作表为空，此函数将返回左上角的单元格。</span><span class="sxs-lookup"><span data-stu-id="83af5-p105">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>|
|[<span data-ttu-id="83af5-145">删除</span><span class="sxs-lookup"><span data-stu-id="83af5-145">Delete</span></span>](../api/worksheet-delete.md)|<span data-ttu-id="83af5-146">无</span><span class="sxs-lookup"><span data-stu-id="83af5-146">None</span></span>|<span data-ttu-id="83af5-147">从工作簿中删除工作表。</span><span class="sxs-lookup"><span data-stu-id="83af5-147">Deletes the worksheet from the workbook.</span></span>|
|[<span data-ttu-id="83af5-148">List</span><span class="sxs-lookup"><span data-stu-id="83af5-148">List</span></span>](../api/worksheet-list.md) | <span data-ttu-id="83af5-149">[Worksheet](worksheet.md) 集合</span><span class="sxs-lookup"><span data-stu-id="83af5-149">[Worksheet](worksheet.md) collection</span></span> |<span data-ttu-id="83af5-150">获取 worksheet 对象集合。</span><span class="sxs-lookup"><span data-stu-id="83af5-150">Get worksheet object collection.</span></span> |
|[<span data-ttu-id="83af5-151">Add</span><span class="sxs-lookup"><span data-stu-id="83af5-151">Add</span></span>](../api/worksheetcollection-add.md)|[<span data-ttu-id="83af5-152">Worksheet</span><span class="sxs-lookup"><span data-stu-id="83af5-152">Worksheet</span></span>](worksheet.md)|<span data-ttu-id="83af5-p106">向工作簿添加新工作表。将工作表添加到现有工作表的末尾。</span><span class="sxs-lookup"><span data-stu-id="83af5-p106">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets.</span></span> |
|[<span data-ttu-id="83af5-155">List pivotTables</span><span class="sxs-lookup"><span data-stu-id="83af5-155">List pivotTables</span></span>](../api/workbookworksheet-list-pivottables.md) |<span data-ttu-id="83af5-156">[workbookPivotTable](workbookpivottable.md) 集合</span><span class="sxs-lookup"><span data-stu-id="83af5-156">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="83af5-157">获取一组 workbookPivotTable 对象。</span><span class="sxs-lookup"><span data-stu-id="83af5-157">Get a workbookPivotTable object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="83af5-158">属性</span><span class="sxs-lookup"><span data-stu-id="83af5-158">Properties</span></span>
| <span data-ttu-id="83af5-159">属性</span><span class="sxs-lookup"><span data-stu-id="83af5-159">Property</span></span>     | <span data-ttu-id="83af5-160">类型</span><span class="sxs-lookup"><span data-stu-id="83af5-160">Type</span></span>   |<span data-ttu-id="83af5-161">说明</span><span class="sxs-lookup"><span data-stu-id="83af5-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="83af5-162">ID</span><span class="sxs-lookup"><span data-stu-id="83af5-162">id</span></span>|<span data-ttu-id="83af5-163">string</span><span class="sxs-lookup"><span data-stu-id="83af5-163">string</span></span>|<span data-ttu-id="83af5-p107">返回用于唯一标识指定工作簿中工作表的值。即使工作表被重命名或移动，标识符的值仍然相同。只读。</span><span class="sxs-lookup"><span data-stu-id="83af5-p107">Returns a value that uniquely identifies the worksheet in a given workbook. The value of the identifier remains the same even when the worksheet is renamed or moved. Read-only.</span></span>|
|<span data-ttu-id="83af5-167">name</span><span class="sxs-lookup"><span data-stu-id="83af5-167">name</span></span>|<span data-ttu-id="83af5-168">string</span><span class="sxs-lookup"><span data-stu-id="83af5-168">string</span></span>|<span data-ttu-id="83af5-169">工作表的显示名称。</span><span class="sxs-lookup"><span data-stu-id="83af5-169">The display name of the worksheet.</span></span>|
|<span data-ttu-id="83af5-170">position</span><span class="sxs-lookup"><span data-stu-id="83af5-170">position</span></span>|<span data-ttu-id="83af5-171">int</span><span class="sxs-lookup"><span data-stu-id="83af5-171">int</span></span>|<span data-ttu-id="83af5-172">工作表在工作簿中的位置，从零开始。</span><span class="sxs-lookup"><span data-stu-id="83af5-172">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="83af5-173">visibility</span><span class="sxs-lookup"><span data-stu-id="83af5-173">visibility</span></span>|<span data-ttu-id="83af5-174">string</span><span class="sxs-lookup"><span data-stu-id="83af5-174">string</span></span>|<span data-ttu-id="83af5-p108">工作表的可见性。可能的值是：`Visible`、`Hidden`、`VeryHidden`。</span><span class="sxs-lookup"><span data-stu-id="83af5-p108">The Visibility of the worksheet. Possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="83af5-177">Relationships</span><span class="sxs-lookup"><span data-stu-id="83af5-177">Relationships</span></span>
| <span data-ttu-id="83af5-178">关系</span><span class="sxs-lookup"><span data-stu-id="83af5-178">Relationship</span></span> | <span data-ttu-id="83af5-179">类型</span><span class="sxs-lookup"><span data-stu-id="83af5-179">Type</span></span>   |<span data-ttu-id="83af5-180">说明</span><span class="sxs-lookup"><span data-stu-id="83af5-180">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="83af5-181">图表</span><span class="sxs-lookup"><span data-stu-id="83af5-181">charts</span></span>|<span data-ttu-id="83af5-182">[图表](chart.md) 集合</span><span class="sxs-lookup"><span data-stu-id="83af5-182">[Chart](chart.md) collection</span></span>|<span data-ttu-id="83af5-p109">返回属于工作表的图表的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="83af5-p109">Returns collection of charts that are part of the worksheet. Read-only.</span></span>|
|<span data-ttu-id="83af5-185">names</span><span class="sxs-lookup"><span data-stu-id="83af5-185">names</span></span>|<span data-ttu-id="83af5-186">[NamedItem](nameditem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="83af5-186">[NamedItem](nameditem.md) collection</span></span>|<span data-ttu-id="83af5-p110">返回与该工作表关联的名称集合。只读。</span><span class="sxs-lookup"><span data-stu-id="83af5-p110">Returns collection of names that are associated with the worksheet. Read-only.</span></span>|
|<span data-ttu-id="83af5-189">pivotTables</span><span class="sxs-lookup"><span data-stu-id="83af5-189">pivotTables</span></span>|<span data-ttu-id="83af5-190">[workbookPivotTable](workbookpivottable.md) 集合</span><span class="sxs-lookup"><span data-stu-id="83af5-190">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="83af5-191">一组属于工作表的数据透视表对象。</span><span class="sxs-lookup"><span data-stu-id="83af5-191">Collection of PivotTables that are part of the worksheet.</span></span> |
|<span data-ttu-id="83af5-192">protection</span><span class="sxs-lookup"><span data-stu-id="83af5-192">protection</span></span>|[<span data-ttu-id="83af5-193">WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="83af5-193">WorksheetProtection</span></span>](worksheetprotection.md)|<span data-ttu-id="83af5-p111">返回表工作表的工作表保护对象。只读。</span><span class="sxs-lookup"><span data-stu-id="83af5-p111">Returns sheet protection object for a worksheet. Read-only.</span></span>|
|<span data-ttu-id="83af5-196">表格</span><span class="sxs-lookup"><span data-stu-id="83af5-196">tables</span></span>|<span data-ttu-id="83af5-197">[Table](table.md) 集合</span><span class="sxs-lookup"><span data-stu-id="83af5-197">[Table](table.md) collection</span></span>|<span data-ttu-id="83af5-p112">属于工作表的表的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="83af5-p112">Collection of tables that are part of the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="83af5-200">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="83af5-200">JSON representation</span></span>

<span data-ttu-id="83af5-201">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83af5-201">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
