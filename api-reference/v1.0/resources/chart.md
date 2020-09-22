---
title: 图表资源类型
description: 表示工作簿中的 chart 对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 2aedb1869a0dee1cc9e0d13fa85ca3c06bcc1d1c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032822"
---
# <a name="chart-resource-type"></a><span data-ttu-id="823ba-103">图表资源类型</span><span class="sxs-lookup"><span data-stu-id="823ba-103">Chart resource type</span></span>

<span data-ttu-id="823ba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="823ba-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="823ba-105">表示工作簿中的 chart 对象。</span><span class="sxs-lookup"><span data-stu-id="823ba-105">Represents a chart object in a workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="823ba-106">方法</span><span class="sxs-lookup"><span data-stu-id="823ba-106">Methods</span></span>

| <span data-ttu-id="823ba-107">方法</span><span class="sxs-lookup"><span data-stu-id="823ba-107">Method</span></span>           | <span data-ttu-id="823ba-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="823ba-108">Return Type</span></span>    |<span data-ttu-id="823ba-109">说明</span><span class="sxs-lookup"><span data-stu-id="823ba-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="823ba-110">获取图表</span><span class="sxs-lookup"><span data-stu-id="823ba-110">Get Chart</span></span>](../api/chart-get.md) | [<span data-ttu-id="823ba-111">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="823ba-111">WorkbookChart</span></span>](chart.md) |<span data-ttu-id="823ba-112">读取 chart 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="823ba-112">Read properties and relationships of chart object.</span></span>|
|[<span data-ttu-id="823ba-113">创建 ChartSeries</span><span class="sxs-lookup"><span data-stu-id="823ba-113">Create ChartSeries</span></span>](../api/chart-post-series.md) |[<span data-ttu-id="823ba-114">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="823ba-114">WorkbookChartSeries</span></span>](chartseries.md)| <span data-ttu-id="823ba-115">通过发布到序列集合创建新的 ChartSeries。</span><span class="sxs-lookup"><span data-stu-id="823ba-115">Create a new ChartSeries by posting to the series collection.</span></span>|
|[<span data-ttu-id="823ba-116">创建系列</span><span class="sxs-lookup"><span data-stu-id="823ba-116">List series</span></span>](../api/chart-list-series.md) |<span data-ttu-id="823ba-117">[WorkbookChartSeries](chartseries.md) 集合</span><span class="sxs-lookup"><span data-stu-id="823ba-117">[WorkbookChartSeries](chartseries.md) collection</span></span>| <span data-ttu-id="823ba-118">获取 ChartSeries 对象集合。</span><span class="sxs-lookup"><span data-stu-id="823ba-118">Get a ChartSeries object collection.</span></span>|
|[<span data-ttu-id="823ba-119">更新</span><span class="sxs-lookup"><span data-stu-id="823ba-119">Update</span></span>](../api/chart-update.md) | [<span data-ttu-id="823ba-120">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="823ba-120">WorkbookChart</span></span>](chart.md)   |<span data-ttu-id="823ba-121">更新 Chart 对象。</span><span class="sxs-lookup"><span data-stu-id="823ba-121">Update Chart object.</span></span> |
|[<span data-ttu-id="823ba-122">图像</span><span class="sxs-lookup"><span data-stu-id="823ba-122">Image</span></span>](../api/chart-image.md)|<span data-ttu-id="823ba-123">图像 base64 编码字符串</span><span class="sxs-lookup"><span data-stu-id="823ba-123">Image base64 encoded string</span></span>|<span data-ttu-id="823ba-124">通过缩放图表适应指定的尺寸，将图表呈现为 base64 编码的图像。</span><span class="sxs-lookup"><span data-stu-id="823ba-124">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>|
|[<span data-ttu-id="823ba-125">删除</span><span class="sxs-lookup"><span data-stu-id="823ba-125">Delete</span></span>](../api/chart-delete.md)|<span data-ttu-id="823ba-126">无</span><span class="sxs-lookup"><span data-stu-id="823ba-126">None</span></span>|<span data-ttu-id="823ba-127">删除 chart 对象。</span><span class="sxs-lookup"><span data-stu-id="823ba-127">Deletes the chart object.</span></span>|
|[<span data-ttu-id="823ba-128">Setdata</span><span class="sxs-lookup"><span data-stu-id="823ba-128">Setdata</span></span>](../api/chart-setdata.md)|<span data-ttu-id="823ba-129">无</span><span class="sxs-lookup"><span data-stu-id="823ba-129">None</span></span>|<span data-ttu-id="823ba-130">重置图表的源数据。</span><span class="sxs-lookup"><span data-stu-id="823ba-130">Resets the source data for the chart.</span></span>|
|[<span data-ttu-id="823ba-131">Setposition</span><span class="sxs-lookup"><span data-stu-id="823ba-131">Setposition</span></span>](../api/chart-setposition.md)|<span data-ttu-id="823ba-132">无</span><span class="sxs-lookup"><span data-stu-id="823ba-132">None</span></span>|<span data-ttu-id="823ba-133">相对于工作表上的单元格放置图表。</span><span class="sxs-lookup"><span data-stu-id="823ba-133">Positions the chart relative to cells on the worksheet.</span></span>|
|[<span data-ttu-id="823ba-134">列出</span><span class="sxs-lookup"><span data-stu-id="823ba-134">List</span></span>](../api/chart-list.md) | <span data-ttu-id="823ba-135">[WorkbookChart](chart.md) 集合</span><span class="sxs-lookup"><span data-stu-id="823ba-135">[WorkbookChart](chart.md) collection</span></span> |<span data-ttu-id="823ba-136">获取 chart 对象集合。</span><span class="sxs-lookup"><span data-stu-id="823ba-136">Get chart object collection.</span></span> |
|[<span data-ttu-id="823ba-137">Itemat</span><span class="sxs-lookup"><span data-stu-id="823ba-137">Itemat</span></span>](../api/chartcollection-itemat.md)|[<span data-ttu-id="823ba-138">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="823ba-138">WorkbookChart</span></span>](chart.md)|<span data-ttu-id="823ba-139">根据其在集合中的位置获取图表。</span><span class="sxs-lookup"><span data-stu-id="823ba-139">Gets a chart based on its position in the collection.</span></span>|
|[<span data-ttu-id="823ba-140">添加</span><span class="sxs-lookup"><span data-stu-id="823ba-140">Add</span></span>](../api/chartcollection-add.md)|[<span data-ttu-id="823ba-141">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="823ba-141">WorkbookChart</span></span>](chart.md)|<span data-ttu-id="823ba-142">创建新图表。</span><span class="sxs-lookup"><span data-stu-id="823ba-142">Creates a new chart.</span></span>|

## <a name="properties"></a><span data-ttu-id="823ba-143">属性</span><span class="sxs-lookup"><span data-stu-id="823ba-143">Properties</span></span>
| <span data-ttu-id="823ba-144">属性</span><span class="sxs-lookup"><span data-stu-id="823ba-144">Property</span></span>     | <span data-ttu-id="823ba-145">类型</span><span class="sxs-lookup"><span data-stu-id="823ba-145">Type</span></span>   |<span data-ttu-id="823ba-146">说明</span><span class="sxs-lookup"><span data-stu-id="823ba-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="823ba-147">高度</span><span class="sxs-lookup"><span data-stu-id="823ba-147">height</span></span>|<span data-ttu-id="823ba-148">double</span><span class="sxs-lookup"><span data-stu-id="823ba-148">double</span></span>|<span data-ttu-id="823ba-149">表示 chart 对象的高度，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="823ba-149">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="823ba-150">id</span><span class="sxs-lookup"><span data-stu-id="823ba-150">id</span></span>|<span data-ttu-id="823ba-151">string</span><span class="sxs-lookup"><span data-stu-id="823ba-151">string</span></span>|<span data-ttu-id="823ba-p101">根据其在集合中的位置获取图表。只读。</span><span class="sxs-lookup"><span data-stu-id="823ba-p101">Gets a chart based on its position in the collection. Read-only.</span></span>|
|<span data-ttu-id="823ba-154">left</span><span class="sxs-lookup"><span data-stu-id="823ba-154">left</span></span>|<span data-ttu-id="823ba-155">double</span><span class="sxs-lookup"><span data-stu-id="823ba-155">double</span></span>|<span data-ttu-id="823ba-156">从图表左侧到工作表原点的距离，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="823ba-156">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="823ba-157">name</span><span class="sxs-lookup"><span data-stu-id="823ba-157">name</span></span>|<span data-ttu-id="823ba-158">string</span><span class="sxs-lookup"><span data-stu-id="823ba-158">string</span></span>|<span data-ttu-id="823ba-159">表示 chart 对象的名称。</span><span class="sxs-lookup"><span data-stu-id="823ba-159">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="823ba-160">top</span><span class="sxs-lookup"><span data-stu-id="823ba-160">top</span></span>|<span data-ttu-id="823ba-161">double</span><span class="sxs-lookup"><span data-stu-id="823ba-161">double</span></span>|<span data-ttu-id="823ba-162">表示从对象左边界至第 1 行顶部（在工作表上）或图表区域顶部（在图表上）的距离，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="823ba-162">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="823ba-163">width</span><span class="sxs-lookup"><span data-stu-id="823ba-163">width</span></span>|<span data-ttu-id="823ba-164">double</span><span class="sxs-lookup"><span data-stu-id="823ba-164">double</span></span>|<span data-ttu-id="823ba-165">表示 chart 对象的宽度，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="823ba-165">Represents the width, in points, of the chart object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="823ba-166">关系</span><span class="sxs-lookup"><span data-stu-id="823ba-166">Relationships</span></span>
| <span data-ttu-id="823ba-167">关系</span><span class="sxs-lookup"><span data-stu-id="823ba-167">Relationship</span></span> | <span data-ttu-id="823ba-168">类型</span><span class="sxs-lookup"><span data-stu-id="823ba-168">Type</span></span>   |<span data-ttu-id="823ba-169">说明</span><span class="sxs-lookup"><span data-stu-id="823ba-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="823ba-170">axes</span><span class="sxs-lookup"><span data-stu-id="823ba-170">axes</span></span>|[<span data-ttu-id="823ba-171">WorkbookChartAxes</span><span class="sxs-lookup"><span data-stu-id="823ba-171">WorkbookChartAxes</span></span>](chartaxes.md)|<span data-ttu-id="823ba-p102">表示图表坐标轴。只读。</span><span class="sxs-lookup"><span data-stu-id="823ba-p102">Represents chart axes. Read-only.</span></span>|
|<span data-ttu-id="823ba-174">dataLabels</span><span class="sxs-lookup"><span data-stu-id="823ba-174">dataLabels</span></span>|[<span data-ttu-id="823ba-175">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="823ba-175">WorkbookChartDataLabels</span></span>](chartdatalabels.md)|<span data-ttu-id="823ba-p103">表示图表上的数据标签。只读。</span><span class="sxs-lookup"><span data-stu-id="823ba-p103">Represents the datalabels on the chart. Read-only.</span></span>|
|<span data-ttu-id="823ba-178">format</span><span class="sxs-lookup"><span data-stu-id="823ba-178">format</span></span>|[<span data-ttu-id="823ba-179">WorkbookChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="823ba-179">WorkbookChartAreaFormat</span></span>](chartareaformat.md)|<span data-ttu-id="823ba-p104">封装图表区域的格式属性。只读。</span><span class="sxs-lookup"><span data-stu-id="823ba-p104">Encapsulates the format properties for the chart area. Read-only.</span></span>|
|<span data-ttu-id="823ba-182">legend</span><span class="sxs-lookup"><span data-stu-id="823ba-182">legend</span></span>|[<span data-ttu-id="823ba-183">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="823ba-183">WorkbookChartLegend</span></span>](chartlegend.md)|<span data-ttu-id="823ba-p105">表示图表的图例。只读。</span><span class="sxs-lookup"><span data-stu-id="823ba-p105">Represents the legend for the chart. Read-only.</span></span>|
|<span data-ttu-id="823ba-186">series</span><span class="sxs-lookup"><span data-stu-id="823ba-186">series</span></span>|<span data-ttu-id="823ba-187">[WorkbookChartSeries](chartseries.md) 集合</span><span class="sxs-lookup"><span data-stu-id="823ba-187">[WorkbookChartSeries](chartseries.md) collection</span></span>|<span data-ttu-id="823ba-p106">表示单个系列或图表中的系列集合。只读。</span><span class="sxs-lookup"><span data-stu-id="823ba-p106">Represents either a single series or collection of series in the chart. Read-only.</span></span>|
|<span data-ttu-id="823ba-190">职位</span><span class="sxs-lookup"><span data-stu-id="823ba-190">title</span></span>|[<span data-ttu-id="823ba-191">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="823ba-191">WorkbookChartTitle</span></span>](charttitle.md)|<span data-ttu-id="823ba-p107">表示指定图表的标题，包括标题的文本、可见性、位置和格式。只读。</span><span class="sxs-lookup"><span data-stu-id="823ba-p107">Represents the title of the specified chart, including the text, visibility, position and formating of the title. Read-only.</span></span>|
|<span data-ttu-id="823ba-194">worksheet</span><span class="sxs-lookup"><span data-stu-id="823ba-194">worksheet</span></span>|[<span data-ttu-id="823ba-195">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="823ba-195">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="823ba-196">包含当前 chart 的 worksheet 对象。</span><span class="sxs-lookup"><span data-stu-id="823ba-196">The worksheet containing the current chart.</span></span> <span data-ttu-id="823ba-197">只读。</span><span class="sxs-lookup"><span data-stu-id="823ba-197">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="823ba-198">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="823ba-198">JSON representation</span></span>

<span data-ttu-id="823ba-199">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="823ba-199">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChart"
}-->

```json
{
  "height": 1024,
  "id": "string",
  "left": 1024,
  "name": "string",
  "top": 1024,
  "width": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

