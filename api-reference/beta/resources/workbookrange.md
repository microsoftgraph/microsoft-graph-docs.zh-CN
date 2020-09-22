---
title: workbookRange 资源类型
description: 区域表示一个或多个相邻的单元格，如单元格、行、列、单元格块等。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: b0f4afa72c4662f3f1254371a2c0170792a14196
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046216"
---
# <a name="workbookrange-resource-type"></a><span data-ttu-id="b79bb-103">workbookRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="b79bb-103">workbookRange resource type</span></span>

<span data-ttu-id="b79bb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b79bb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b79bb-105">区域表示一个或多个相邻的单元格，如单元格、行、列、单元格块等。</span><span class="sxs-lookup"><span data-stu-id="b79bb-105">Range represents a set of one or more contiguous cells such as a cell, a row, a column, block of cells, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="b79bb-106">方法</span><span class="sxs-lookup"><span data-stu-id="b79bb-106">Methods</span></span>

| <span data-ttu-id="b79bb-107">方法</span><span class="sxs-lookup"><span data-stu-id="b79bb-107">Method</span></span>           | <span data-ttu-id="b79bb-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="b79bb-108">Return Type</span></span>    |<span data-ttu-id="b79bb-109">说明</span><span class="sxs-lookup"><span data-stu-id="b79bb-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b79bb-110">获取区域</span><span class="sxs-lookup"><span data-stu-id="b79bb-110">Get Range</span></span>](../api/range-get.md) | [<span data-ttu-id="b79bb-111">workbookRange</span><span class="sxs-lookup"><span data-stu-id="b79bb-111">workbookRange</span></span>](workbookrange.md) |<span data-ttu-id="b79bb-112">读取 range 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b79bb-112">Read properties and relationships of range object.</span></span>|
|[<span data-ttu-id="b79bb-113">更新</span><span class="sxs-lookup"><span data-stu-id="b79bb-113">Update</span></span>](../api/range-update.md) | [<span data-ttu-id="b79bb-114">workbookRange</span><span class="sxs-lookup"><span data-stu-id="b79bb-114">workbookRange</span></span>](workbookrange.md)   |<span data-ttu-id="b79bb-115">更新 Range 对象。</span><span class="sxs-lookup"><span data-stu-id="b79bb-115">Update Range object.</span></span> |
|[<span data-ttu-id="b79bb-116">Boundingrect</span><span class="sxs-lookup"><span data-stu-id="b79bb-116">Boundingrect</span></span>](../api/range-boundingrect.md)|[<span data-ttu-id="b79bb-117">workbookRange</span><span class="sxs-lookup"><span data-stu-id="b79bb-117">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="b79bb-p101">获取包含指定区域的最小 range 对象。例如，“B2:C5”和“D10:E15”的 GetBoundingRect 为“B2:E16”。</span><span class="sxs-lookup"><span data-stu-id="b79bb-p101">Gets the smallest range object that encompasses the given ranges. For example, the GetBoundingRect of "B2:C5" and "D10:E15" is "B2:E16".</span></span>|
|[<span data-ttu-id="b79bb-120">单元格</span><span class="sxs-lookup"><span data-stu-id="b79bb-120">Cell</span></span>](../api/range-cell.md)|[<span data-ttu-id="b79bb-121">workbookRange</span><span class="sxs-lookup"><span data-stu-id="b79bb-121">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="b79bb-p102">根据行和列编号获取包含单个单元格的 range 对象。单元格可以位于父区域外部，只要其保持在工作表网格内即可。返回的单元格位于相对于区域左上角的单元格的位置。</span><span class="sxs-lookup"><span data-stu-id="b79bb-p102">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid. The returned cell is located relative to the top left cell of the range.</span></span>|
|[<span data-ttu-id="b79bb-125">列</span><span class="sxs-lookup"><span data-stu-id="b79bb-125">Column</span></span>](../api/range-column.md)|[<span data-ttu-id="b79bb-126">workbookRange</span><span class="sxs-lookup"><span data-stu-id="b79bb-126">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="b79bb-127">获取范围中包含的列。</span><span class="sxs-lookup"><span data-stu-id="b79bb-127">Gets a column contained in the range.</span></span>|
|[<span data-ttu-id="b79bb-128">Columnsafter</span><span class="sxs-lookup"><span data-stu-id="b79bb-128">Columnsafter</span></span>](../api/workbookrange-columnsafter.md)|[<span data-ttu-id="b79bb-129">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="b79bb-129">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="b79bb-130">获取给定范围右侧的一定数量的列。</span><span class="sxs-lookup"><span data-stu-id="b79bb-130">Gets a certain number of columns to the right of the given range.</span></span>|
|[<span data-ttu-id="b79bb-131">Columnsbefore</span><span class="sxs-lookup"><span data-stu-id="b79bb-131">Columnsbefore</span></span>](../api/workbookrange-columnsbefore.md)|[<span data-ttu-id="b79bb-132">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="b79bb-132">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="b79bb-133">获取给定范围左侧的一定数量的列。</span><span class="sxs-lookup"><span data-stu-id="b79bb-133">Gets a certain number of columns to the left of the given range.</span></span>|
|[<span data-ttu-id="b79bb-134">Entirecolumn</span><span class="sxs-lookup"><span data-stu-id="b79bb-134">Entirecolumn</span></span>](../api/range-entirecolumn.md)|[<span data-ttu-id="b79bb-135">workbookRange</span><span class="sxs-lookup"><span data-stu-id="b79bb-135">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="b79bb-136">获取表示区域整列的对象。</span><span class="sxs-lookup"><span data-stu-id="b79bb-136">Gets an object that represents the entire column of the range.</span></span>|
|[<span data-ttu-id="b79bb-137">Entirerow</span><span class="sxs-lookup"><span data-stu-id="b79bb-137">Entirerow</span></span>](../api/range-entirerow.md)|[<span data-ttu-id="b79bb-138">workbookRange</span><span class="sxs-lookup"><span data-stu-id="b79bb-138">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="b79bb-139">获取表示区域整行的对象。</span><span class="sxs-lookup"><span data-stu-id="b79bb-139">Gets an object that represents the entire row of the range.</span></span>|
|[<span data-ttu-id="b79bb-140">Intersection</span><span class="sxs-lookup"><span data-stu-id="b79bb-140">Intersection</span></span>](../api/range-intersection.md)|[<span data-ttu-id="b79bb-141">workbookRange</span><span class="sxs-lookup"><span data-stu-id="b79bb-141">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="b79bb-142">获取表示指定区域的矩形交集的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="b79bb-142">Gets the range object that represents the rectangular intersection of the given ranges.</span></span>|
|[<span data-ttu-id="b79bb-143">Lastcell</span><span class="sxs-lookup"><span data-stu-id="b79bb-143">Lastcell</span></span>](../api/range-lastcell.md)|[<span data-ttu-id="b79bb-144">区域</span><span class="sxs-lookup"><span data-stu-id="b79bb-144">Range</span></span>](workbookrange.md)|<span data-ttu-id="b79bb-p103">获取区域内的最后一个单元格。例如，“B2:D5”的最后一个单元格是“D5”。</span><span class="sxs-lookup"><span data-stu-id="b79bb-p103">Gets the last cell within the range. For example, the last cell of "B2:D5" is "D5".</span></span>|
|[<span data-ttu-id="b79bb-147">Lastcolumn</span><span class="sxs-lookup"><span data-stu-id="b79bb-147">Lastcolumn</span></span>](../api/range-lastcolumn.md)|[<span data-ttu-id="b79bb-148">workbookRange</span><span class="sxs-lookup"><span data-stu-id="b79bb-148">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="b79bb-p104">获取区域内的最后一列。例如，“B2:D5”的最后一列是“D2:D5”。</span><span class="sxs-lookup"><span data-stu-id="b79bb-p104">Gets the last column within the range. For example, the last column of "B2:D5" is "D2:D5".</span></span>|
|[<span data-ttu-id="b79bb-151">Lastrow</span><span class="sxs-lookup"><span data-stu-id="b79bb-151">Lastrow</span></span>](../api/range-lastrow.md)|[<span data-ttu-id="b79bb-152">区域</span><span class="sxs-lookup"><span data-stu-id="b79bb-152">Range</span></span>](workbookrange.md)|<span data-ttu-id="b79bb-p105">获取区域内的最后一行。例如，“B2:D5”的最后一行是“B5:D5”。</span><span class="sxs-lookup"><span data-stu-id="b79bb-p105">Gets the last row within the range. For example, the last row of "B2:D5" is "B5:D5".</span></span>|
|[<span data-ttu-id="b79bb-155">Offsetrange</span><span class="sxs-lookup"><span data-stu-id="b79bb-155">Offsetrange</span></span>](../api/range-offsetrange.md)|[<span data-ttu-id="b79bb-156">workbookRange</span><span class="sxs-lookup"><span data-stu-id="b79bb-156">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="b79bb-p106">获取表示与指定区域偏移的区域的对象。返回的区域的尺寸将与该区域匹配。如果强制使生成的区域位于工作表网格的边界之外，则会引发异常。</span><span class="sxs-lookup"><span data-stu-id="b79bb-p106">Gets an object which represents a range that's offset from the specified range. The dimension of the returned range will match this range. If the resulting range is forced outside the bounds of the worksheet grid, an exception will be thrown.</span></span>|
|[<span data-ttu-id="b79bb-160">行</span><span class="sxs-lookup"><span data-stu-id="b79bb-160">Row</span></span>](../api/range-row.md)|[<span data-ttu-id="b79bb-161">区域</span><span class="sxs-lookup"><span data-stu-id="b79bb-161">Range</span></span>](workbookrange.md)|<span data-ttu-id="b79bb-162">获取范围中包含的行。</span><span class="sxs-lookup"><span data-stu-id="b79bb-162">Gets a row contained in the range.</span></span>|
|[<span data-ttu-id="b79bb-163">Rowsabove</span><span class="sxs-lookup"><span data-stu-id="b79bb-163">Rowsabove</span></span>](../api/workbookrange-rowsabove.md)|[<span data-ttu-id="b79bb-164">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="b79bb-164">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="b79bb-165">获取给定范围上方的一定数量的行。</span><span class="sxs-lookup"><span data-stu-id="b79bb-165">Gets a certain number of rows above a given range.</span></span>|
|[<span data-ttu-id="b79bb-166">Rowsbelow</span><span class="sxs-lookup"><span data-stu-id="b79bb-166">Rowsbelow</span></span>](../api/workbookrange-rowsbelow.md)|[<span data-ttu-id="b79bb-167">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="b79bb-167">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="b79bb-168">获取给定范围下方的一定数量的行。</span><span class="sxs-lookup"><span data-stu-id="b79bb-168">Gets a certain number of rows below a given range.</span></span>|
|[<span data-ttu-id="b79bb-169">Usedrange</span><span class="sxs-lookup"><span data-stu-id="b79bb-169">Usedrange</span></span>](../api/range-usedrange.md)|[<span data-ttu-id="b79bb-170">workbookRange</span><span class="sxs-lookup"><span data-stu-id="b79bb-170">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="b79bb-171">返回指定 range 对象的所用区域。</span><span class="sxs-lookup"><span data-stu-id="b79bb-171">Returns the used range of the given range object.</span></span>|
|[<span data-ttu-id="b79bb-172">清除</span><span class="sxs-lookup"><span data-stu-id="b79bb-172">Clear</span></span>](../api/range-clear.md)|<span data-ttu-id="b79bb-173">None</span><span class="sxs-lookup"><span data-stu-id="b79bb-173">None</span></span>|<span data-ttu-id="b79bb-174">清除区域值、格式、填充、边框等。</span><span class="sxs-lookup"><span data-stu-id="b79bb-174">Clear range values, format, fill, border, etc.</span></span>|
|[<span data-ttu-id="b79bb-175">删除</span><span class="sxs-lookup"><span data-stu-id="b79bb-175">Delete</span></span>](../api/range-delete.md)|<span data-ttu-id="b79bb-176">None</span><span class="sxs-lookup"><span data-stu-id="b79bb-176">None</span></span>|<span data-ttu-id="b79bb-177">删除与区域相关的单元格。</span><span class="sxs-lookup"><span data-stu-id="b79bb-177">Deletes the cells associated with the range.</span></span>|
|[<span data-ttu-id="b79bb-178">插入</span><span class="sxs-lookup"><span data-stu-id="b79bb-178">Insert</span></span>](../api/range-insert.md)|[<span data-ttu-id="b79bb-179">workbookRange</span><span class="sxs-lookup"><span data-stu-id="b79bb-179">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="b79bb-p107">将单个单元格或一系列单元格插入到工作表中取代此区域，并移动其他单元格以留出空间。在现在空白的空间返回新的 Range 对象。</span><span class="sxs-lookup"><span data-stu-id="b79bb-p107">Inserts a cell or a range of cells into the worksheet in place of this range, and shifts the other cells to make space. Returns a new Range object at the now blank space.</span></span>|
|[<span data-ttu-id="b79bb-182">合并</span><span class="sxs-lookup"><span data-stu-id="b79bb-182">Merge</span></span>](../api/range-merge.md)|<span data-ttu-id="b79bb-183">None</span><span class="sxs-lookup"><span data-stu-id="b79bb-183">None</span></span>|<span data-ttu-id="b79bb-184">将范围单元格合并到工作表的一个区域内。</span><span class="sxs-lookup"><span data-stu-id="b79bb-184">Merge the range cells into one region in the worksheet.</span></span>|
|[<span data-ttu-id="b79bb-185">Resizedrange</span><span class="sxs-lookup"><span data-stu-id="b79bb-185">Resizedrange</span></span>](../api/workbookrange-resizedrange.md)|[<span data-ttu-id="b79bb-186">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="b79bb-186">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="b79bb-187">获取与当前范围对象类似的范围对象，但其右下角可通过一定数量的行和列进行展开（或合拢）。</span><span class="sxs-lookup"><span data-stu-id="b79bb-187">Gets a range object similar to the current range object, but with its bottom-right corner expanded (or contracted) by some number of rows and columns.</span></span>|
|[<span data-ttu-id="b79bb-188">Unmerge</span><span class="sxs-lookup"><span data-stu-id="b79bb-188">Unmerge</span></span>](../api/range-unmerge.md)|<span data-ttu-id="b79bb-189">None</span><span class="sxs-lookup"><span data-stu-id="b79bb-189">None</span></span>|<span data-ttu-id="b79bb-190">将范围单元格取消合并为各个单元格。</span><span class="sxs-lookup"><span data-stu-id="b79bb-190">Unmerge the range cells into separate cells.</span></span>|
|[<span data-ttu-id="b79bb-191">Visibleview</span><span class="sxs-lookup"><span data-stu-id="b79bb-191">Visibleview</span></span>](../api/workbookrange-visibleview.md)|[<span data-ttu-id="b79bb-192">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="b79bb-192">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="b79bb-193">获取筛选的范围中的可见范围。</span><span class="sxs-lookup"><span data-stu-id="b79bb-193">Get the range visible from a filtered range.</span></span>|

## <a name="properties"></a><span data-ttu-id="b79bb-194">属性</span><span class="sxs-lookup"><span data-stu-id="b79bb-194">Properties</span></span>
| <span data-ttu-id="b79bb-195">属性</span><span class="sxs-lookup"><span data-stu-id="b79bb-195">Property</span></span>     | <span data-ttu-id="b79bb-196">类型</span><span class="sxs-lookup"><span data-stu-id="b79bb-196">Type</span></span>   |<span data-ttu-id="b79bb-197">说明</span><span class="sxs-lookup"><span data-stu-id="b79bb-197">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b79bb-198">address</span><span class="sxs-lookup"><span data-stu-id="b79bb-198">address</span></span>|<span data-ttu-id="b79bb-199">string</span><span class="sxs-lookup"><span data-stu-id="b79bb-199">string</span></span>|<span data-ttu-id="b79bb-p108">表示 A1 样式的区域引用。地址值将包含工作表引用（如 Sheet1!A1:B4）。只读。</span><span class="sxs-lookup"><span data-stu-id="b79bb-p108">Represents the range reference in A1-style. Address value will contain the Sheet reference (e.g. Sheet1!A1:B4). Read-only.</span></span>|
|<span data-ttu-id="b79bb-203">addressLocal</span><span class="sxs-lookup"><span data-stu-id="b79bb-203">addressLocal</span></span>|<span data-ttu-id="b79bb-204">string</span><span class="sxs-lookup"><span data-stu-id="b79bb-204">string</span></span>|<span data-ttu-id="b79bb-p109">以用户语言表示对指定区域的区域引用。只读。</span><span class="sxs-lookup"><span data-stu-id="b79bb-p109">Represents range reference for the specified range in the language of the user. Read-only.</span></span>|
|<span data-ttu-id="b79bb-207">cellCount</span><span class="sxs-lookup"><span data-stu-id="b79bb-207">cellCount</span></span>|<span data-ttu-id="b79bb-208">int</span><span class="sxs-lookup"><span data-stu-id="b79bb-208">int</span></span>|<span data-ttu-id="b79bb-p110">区域中的单元格数目。只读。</span><span class="sxs-lookup"><span data-stu-id="b79bb-p110">Number of cells in the range. Read-only.</span></span>|
|<span data-ttu-id="b79bb-211">columnCount</span><span class="sxs-lookup"><span data-stu-id="b79bb-211">columnCount</span></span>|<span data-ttu-id="b79bb-212">int</span><span class="sxs-lookup"><span data-stu-id="b79bb-212">int</span></span>|<span data-ttu-id="b79bb-p111">表示区域中的列总数。只读。</span><span class="sxs-lookup"><span data-stu-id="b79bb-p111">Represents the total number of columns in the range. Read-only.</span></span>|
|<span data-ttu-id="b79bb-215">columnHidden</span><span class="sxs-lookup"><span data-stu-id="b79bb-215">columnHidden</span></span>|<span data-ttu-id="b79bb-216">boolean</span><span class="sxs-lookup"><span data-stu-id="b79bb-216">boolean</span></span>|<span data-ttu-id="b79bb-217">表示当前区域中的所有列是否隐藏。</span><span class="sxs-lookup"><span data-stu-id="b79bb-217">Represents if all columns of the current range are hidden.</span></span>|
|<span data-ttu-id="b79bb-218">columnIndex</span><span class="sxs-lookup"><span data-stu-id="b79bb-218">columnIndex</span></span>|<span data-ttu-id="b79bb-219">int</span><span class="sxs-lookup"><span data-stu-id="b79bb-219">int</span></span>|<span data-ttu-id="b79bb-p112">表示区域中第一个单元格的列编号。从零开始编制索引。只读。</span><span class="sxs-lookup"><span data-stu-id="b79bb-p112">Represents the column number of the first cell in the range. Zero-indexed. Read-only.</span></span>|
|<span data-ttu-id="b79bb-223">formulas</span><span class="sxs-lookup"><span data-stu-id="b79bb-223">formulas</span></span>|<span data-ttu-id="b79bb-224">Json</span><span class="sxs-lookup"><span data-stu-id="b79bb-224">Json</span></span>|<span data-ttu-id="b79bb-225">表示采用 A1 表示法的公式。</span><span class="sxs-lookup"><span data-stu-id="b79bb-225">Represents the formula in A1-style notation.</span></span>|
|<span data-ttu-id="b79bb-226">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="b79bb-226">formulasLocal</span></span>|<span data-ttu-id="b79bb-227">Json</span><span class="sxs-lookup"><span data-stu-id="b79bb-227">Json</span></span>|<span data-ttu-id="b79bb-p113">表示采用 A1 样式表示法的公式，使用用户的语言和数字格式区域设置。例如，英语中的公式 "=SUM(A1, 1.5)" 在德语中将变为 "=SUMME(A1; 1,5)"。</span><span class="sxs-lookup"><span data-stu-id="b79bb-p113">Represents the formula in A1-style notation, in the user's language and number-formatting locale.  For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>|
|<span data-ttu-id="b79bb-230">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="b79bb-230">formulasR1C1</span></span>|<span data-ttu-id="b79bb-231">Json</span><span class="sxs-lookup"><span data-stu-id="b79bb-231">Json</span></span>|<span data-ttu-id="b79bb-232">表示采用 R1C1 样式表示法的公式。</span><span class="sxs-lookup"><span data-stu-id="b79bb-232">Represents the formula in R1C1-style notation.</span></span>|
|<span data-ttu-id="b79bb-233">hidden</span><span class="sxs-lookup"><span data-stu-id="b79bb-233">hidden</span></span>|<span data-ttu-id="b79bb-234">boolean</span><span class="sxs-lookup"><span data-stu-id="b79bb-234">boolean</span></span>|<span data-ttu-id="b79bb-p114">表示当前区域中的所有单元格是否隐藏。只读。</span><span class="sxs-lookup"><span data-stu-id="b79bb-p114">Represents if all cells of the current range are hidden. Read-only.</span></span>|
|<span data-ttu-id="b79bb-237">numberFormat</span><span class="sxs-lookup"><span data-stu-id="b79bb-237">numberFormat</span></span>|<span data-ttu-id="b79bb-238">Json</span><span class="sxs-lookup"><span data-stu-id="b79bb-238">Json</span></span>|<span data-ttu-id="b79bb-239">表示 Excel 中指定单元格的数字格式代码。</span><span class="sxs-lookup"><span data-stu-id="b79bb-239">Represents Excel's number format code for the given cell.</span></span>|
|<span data-ttu-id="b79bb-240">rowCount</span><span class="sxs-lookup"><span data-stu-id="b79bb-240">rowCount</span></span>|<span data-ttu-id="b79bb-241">int</span><span class="sxs-lookup"><span data-stu-id="b79bb-241">int</span></span>|<span data-ttu-id="b79bb-p115">返回区域中的总行数。只读。</span><span class="sxs-lookup"><span data-stu-id="b79bb-p115">Returns the total number of rows in the range. Read-only.</span></span>|
|<span data-ttu-id="b79bb-244">rowHidden</span><span class="sxs-lookup"><span data-stu-id="b79bb-244">rowHidden</span></span>|<span data-ttu-id="b79bb-245">boolean</span><span class="sxs-lookup"><span data-stu-id="b79bb-245">boolean</span></span>|<span data-ttu-id="b79bb-246">表示当前区域中的所有行是否隐藏。</span><span class="sxs-lookup"><span data-stu-id="b79bb-246">Represents if all rows of the current range are hidden.</span></span>|
|<span data-ttu-id="b79bb-247">rowIndex</span><span class="sxs-lookup"><span data-stu-id="b79bb-247">rowIndex</span></span>|<span data-ttu-id="b79bb-248">int</span><span class="sxs-lookup"><span data-stu-id="b79bb-248">int</span></span>|<span data-ttu-id="b79bb-p116">返回区域中第一个单元格的行编号。从零开始编制索引。只读。</span><span class="sxs-lookup"><span data-stu-id="b79bb-p116">Returns the row number of the first cell in the range. Zero-indexed. Read-only.</span></span>|
|<span data-ttu-id="b79bb-252">text</span><span class="sxs-lookup"><span data-stu-id="b79bb-252">text</span></span>|<span data-ttu-id="b79bb-253">Json</span><span class="sxs-lookup"><span data-stu-id="b79bb-253">Json</span></span>|<span data-ttu-id="b79bb-p117">指定区域的文本值。文本值与单元格宽度无关。在 Excel UI 中替代 # 符号不会影响 API 返回的文本值。只读。</span><span class="sxs-lookup"><span data-stu-id="b79bb-p117">Text values of the specified range. The Text value will not depend on the cell width. The # sign substitution that happens in Excel UI will not affect the text value returned by the API. Read-only.</span></span>|
|<span data-ttu-id="b79bb-258">valueTypes</span><span class="sxs-lookup"><span data-stu-id="b79bb-258">valueTypes</span></span>|<span data-ttu-id="b79bb-259">string</span><span class="sxs-lookup"><span data-stu-id="b79bb-259">string</span></span>|<span data-ttu-id="b79bb-p118">表示每个单元格的数据类型。可能的值是：`Unknown`、`Empty`、`String`、`Integer`、`Double`、`Boolean`、`Error`。只读。</span><span class="sxs-lookup"><span data-stu-id="b79bb-p118">Represents the type of data of each cell. Possible values are: `Unknown`, `Empty`, `String`, `Integer`, `Double`, `Boolean`, `Error`. Read-only.</span></span>|
|<span data-ttu-id="b79bb-263">values</span><span class="sxs-lookup"><span data-stu-id="b79bb-263">values</span></span>|<span data-ttu-id="b79bb-264">Json</span><span class="sxs-lookup"><span data-stu-id="b79bb-264">Json</span></span>|<span data-ttu-id="b79bb-p119">表示指定区域的原始值。返回的数据类型可能是字符串、数字或布尔值。包含一个将返回错误字符串的错误的单元格。</span><span class="sxs-lookup"><span data-stu-id="b79bb-p119">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b79bb-268">关系</span><span class="sxs-lookup"><span data-stu-id="b79bb-268">Relationships</span></span>
| <span data-ttu-id="b79bb-269">关系</span><span class="sxs-lookup"><span data-stu-id="b79bb-269">Relationship</span></span> | <span data-ttu-id="b79bb-270">类型</span><span class="sxs-lookup"><span data-stu-id="b79bb-270">Type</span></span>   |<span data-ttu-id="b79bb-271">说明</span><span class="sxs-lookup"><span data-stu-id="b79bb-271">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b79bb-272">format</span><span class="sxs-lookup"><span data-stu-id="b79bb-272">format</span></span>|[<span data-ttu-id="b79bb-273">workbookRangeFormat</span><span class="sxs-lookup"><span data-stu-id="b79bb-273">workbookRangeFormat</span></span>](workbookrangeformat.md)|<span data-ttu-id="b79bb-p120">返回一个格式对象，其中封装了区域的字体、填充、边框、对齐方式和其他属性。只读。</span><span class="sxs-lookup"><span data-stu-id="b79bb-p120">Returns a format object, encapsulating the range's font, fill, borders, alignment, and other properties. Read-only.</span></span>|
|<span data-ttu-id="b79bb-276">sort</span><span class="sxs-lookup"><span data-stu-id="b79bb-276">sort</span></span>|[<span data-ttu-id="b79bb-277">workbookRangeSort</span><span class="sxs-lookup"><span data-stu-id="b79bb-277">workbookRangeSort</span></span>](workbookrangesort.md)|<span data-ttu-id="b79bb-p121">包含当前区域的工作表。只读。</span><span class="sxs-lookup"><span data-stu-id="b79bb-p121">The worksheet containing the current range. Read-only.</span></span>|
|<span data-ttu-id="b79bb-280">worksheet</span><span class="sxs-lookup"><span data-stu-id="b79bb-280">worksheet</span></span>|[<span data-ttu-id="b79bb-281">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="b79bb-281">workbookWorksheet</span></span>](workbookworksheet.md)|<span data-ttu-id="b79bb-p122">包含当前区域的工作表。只读。</span><span class="sxs-lookup"><span data-stu-id="b79bb-p122">The worksheet containing the current range. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b79bb-284">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b79bb-284">JSON representation</span></span>

<span data-ttu-id="b79bb-285">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b79bb-285">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRange"
}-->

```json
{
  "id": "string",
  "address": "string",
  "addressLocal": "string",
  "cellCount": 1024,
  "columnCount": 1024,
  "columnHidden": true,
  "columnIndex": 1024,
  "formulas": "Json",
  "formulasLocal": "Json",
  "formulasR1C1": "Json",
  "hidden": true,
  "numberFormat": "Json",
  "rowCount": 1024,
  "rowHidden": true,
  "rowIndex": 1024,
  "text": "Json",
  "valueTypes": "string",
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Range resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


