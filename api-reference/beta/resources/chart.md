---
title: 图表资源类型
description: 表示工作簿中的 chart 对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 09d5fd376cfdcd03517cc989708bbf17bcf49a72
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970673"
---
# <a name="chart-resource-type"></a><span data-ttu-id="bbe9c-103">图表资源类型</span><span class="sxs-lookup"><span data-stu-id="bbe9c-103">Chart resource type</span></span>

> <span data-ttu-id="bbe9c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bbe9c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bbe9c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bbe9c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bbe9c-106">表示工作簿中的 chart 对象。</span><span class="sxs-lookup"><span data-stu-id="bbe9c-106">Represents a chart object in a workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="bbe9c-107">方法</span><span class="sxs-lookup"><span data-stu-id="bbe9c-107">Methods</span></span>

| <span data-ttu-id="bbe9c-108">方法</span><span class="sxs-lookup"><span data-stu-id="bbe9c-108">Method</span></span>           | <span data-ttu-id="bbe9c-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="bbe9c-109">Return Type</span></span>    |<span data-ttu-id="bbe9c-110">说明</span><span class="sxs-lookup"><span data-stu-id="bbe9c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bbe9c-111">获取图表</span><span class="sxs-lookup"><span data-stu-id="bbe9c-111">Get Chart</span></span>](../api/chart-get.md) | [<span data-ttu-id="bbe9c-112">Chart</span><span class="sxs-lookup"><span data-stu-id="bbe9c-112">Chart</span></span>](chart.md) |<span data-ttu-id="bbe9c-113">读取 chart 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bbe9c-113">Read properties and relationships of chart object.</span></span>|
|[<span data-ttu-id="bbe9c-114">创建 ChartSeries</span><span class="sxs-lookup"><span data-stu-id="bbe9c-114">Create ChartSeries</span></span>](../api/chart-post-series.md) |[<span data-ttu-id="bbe9c-115">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="bbe9c-115">ChartSeries</span></span>](chartseries.md)| <span data-ttu-id="bbe9c-116">通过发布到序列集合创建新的 ChartSeries。</span><span class="sxs-lookup"><span data-stu-id="bbe9c-116">Create a new ChartSeries by posting to the series collection.</span></span>|
|[<span data-ttu-id="bbe9c-117">创建系列</span><span class="sxs-lookup"><span data-stu-id="bbe9c-117">List series</span></span>](../api/chart-list-series.md) |<span data-ttu-id="bbe9c-118">[ChartSeries](chartseries.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bbe9c-118">[ChartSeries](chartseries.md) collection</span></span>| <span data-ttu-id="bbe9c-119">获取 ChartSeries 对象集合。</span><span class="sxs-lookup"><span data-stu-id="bbe9c-119">Get a ChartSeries object collection.</span></span>|
|[<span data-ttu-id="bbe9c-120">更新</span><span class="sxs-lookup"><span data-stu-id="bbe9c-120">Update</span></span>](../api/chart-update.md) | [<span data-ttu-id="bbe9c-121">Chart</span><span class="sxs-lookup"><span data-stu-id="bbe9c-121">Chart</span></span>](chart.md)   |<span data-ttu-id="bbe9c-122">更新 Chart 对象。</span><span class="sxs-lookup"><span data-stu-id="bbe9c-122">Update Chart object.</span></span> |
|[<span data-ttu-id="bbe9c-123">Image</span><span class="sxs-lookup"><span data-stu-id="bbe9c-123">Image</span></span>](../api/chart-image.md)|<span data-ttu-id="bbe9c-124">图像 base64 编码字符串</span><span class="sxs-lookup"><span data-stu-id="bbe9c-124">Image base64 encoded string</span></span>|<span data-ttu-id="bbe9c-125">通过缩放图表适应指定的尺寸，将图表呈现为 base64 编码的图像。</span><span class="sxs-lookup"><span data-stu-id="bbe9c-125">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>|
|[<span data-ttu-id="bbe9c-126">删除</span><span class="sxs-lookup"><span data-stu-id="bbe9c-126">Delete</span></span>](../api/chart-delete.md)|<span data-ttu-id="bbe9c-127">无</span><span class="sxs-lookup"><span data-stu-id="bbe9c-127">None</span></span>|<span data-ttu-id="bbe9c-128">删除 chart 对象。</span><span class="sxs-lookup"><span data-stu-id="bbe9c-128">Deletes the chart object.</span></span>|
|[<span data-ttu-id="bbe9c-129">Setdata</span><span class="sxs-lookup"><span data-stu-id="bbe9c-129">Setdata</span></span>](../api/chart-setdata.md)|<span data-ttu-id="bbe9c-130">无</span><span class="sxs-lookup"><span data-stu-id="bbe9c-130">None</span></span>|<span data-ttu-id="bbe9c-131">重置图表的源数据。</span><span class="sxs-lookup"><span data-stu-id="bbe9c-131">Resets the source data for the chart.</span></span>|
|[<span data-ttu-id="bbe9c-132">Setposition</span><span class="sxs-lookup"><span data-stu-id="bbe9c-132">Setposition</span></span>](../api/chart-setposition.md)|<span data-ttu-id="bbe9c-133">无</span><span class="sxs-lookup"><span data-stu-id="bbe9c-133">None</span></span>|<span data-ttu-id="bbe9c-134">相对于工作表上的单元格放置图表。</span><span class="sxs-lookup"><span data-stu-id="bbe9c-134">Positions the chart relative to cells on the worksheet.</span></span>|
|[<span data-ttu-id="bbe9c-135">列出</span><span class="sxs-lookup"><span data-stu-id="bbe9c-135">List</span></span>](../api/chart-list.md) | <span data-ttu-id="bbe9c-136">[图表](chart.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bbe9c-136">[Chart](chart.md) collection</span></span> |<span data-ttu-id="bbe9c-137">获取 chart 对象集合。</span><span class="sxs-lookup"><span data-stu-id="bbe9c-137">Get chart object collection.</span></span> |
|[<span data-ttu-id="bbe9c-138">Itemat</span><span class="sxs-lookup"><span data-stu-id="bbe9c-138">Itemat</span></span>](../api/chartcollection-itemat.md)|[<span data-ttu-id="bbe9c-139">Chart</span><span class="sxs-lookup"><span data-stu-id="bbe9c-139">Chart</span></span>](chart.md)|<span data-ttu-id="bbe9c-140">按图表在集合中的位置获取此对象。</span><span class="sxs-lookup"><span data-stu-id="bbe9c-140">Gets a chart based on its position in the collection.</span></span>|
|[<span data-ttu-id="bbe9c-141">Add</span><span class="sxs-lookup"><span data-stu-id="bbe9c-141">Add</span></span>](../api/chartcollection-add.md)|[<span data-ttu-id="bbe9c-142">Chart</span><span class="sxs-lookup"><span data-stu-id="bbe9c-142">Chart</span></span>](chart.md)|<span data-ttu-id="bbe9c-143">创建新图表。</span><span class="sxs-lookup"><span data-stu-id="bbe9c-143">Creates a new chart.</span></span>|

## <a name="properties"></a><span data-ttu-id="bbe9c-144">属性</span><span class="sxs-lookup"><span data-stu-id="bbe9c-144">Properties</span></span>
| <span data-ttu-id="bbe9c-145">属性</span><span class="sxs-lookup"><span data-stu-id="bbe9c-145">Property</span></span>     | <span data-ttu-id="bbe9c-146">类型</span><span class="sxs-lookup"><span data-stu-id="bbe9c-146">Type</span></span>   |<span data-ttu-id="bbe9c-147">说明</span><span class="sxs-lookup"><span data-stu-id="bbe9c-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bbe9c-148">height</span><span class="sxs-lookup"><span data-stu-id="bbe9c-148">height</span></span>|<span data-ttu-id="bbe9c-149">double</span><span class="sxs-lookup"><span data-stu-id="bbe9c-149">double</span></span>|<span data-ttu-id="bbe9c-150">表示 chart 对象的高度，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="bbe9c-150">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="bbe9c-151">id</span><span class="sxs-lookup"><span data-stu-id="bbe9c-151">id</span></span>|<span data-ttu-id="bbe9c-152">string</span><span class="sxs-lookup"><span data-stu-id="bbe9c-152">string</span></span>|<span data-ttu-id="bbe9c-p102">根据其在集合中的位置获取图表。只读。</span><span class="sxs-lookup"><span data-stu-id="bbe9c-p102">Gets a chart based on its position in the collection. Read-only.</span></span>|
|<span data-ttu-id="bbe9c-155">left</span><span class="sxs-lookup"><span data-stu-id="bbe9c-155">left</span></span>|<span data-ttu-id="bbe9c-156">double</span><span class="sxs-lookup"><span data-stu-id="bbe9c-156">double</span></span>|<span data-ttu-id="bbe9c-157">从图表左侧到工作表原点的距离，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="bbe9c-157">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="bbe9c-158">name</span><span class="sxs-lookup"><span data-stu-id="bbe9c-158">name</span></span>|<span data-ttu-id="bbe9c-159">string</span><span class="sxs-lookup"><span data-stu-id="bbe9c-159">string</span></span>|<span data-ttu-id="bbe9c-160">表示 chart 对象的名称。</span><span class="sxs-lookup"><span data-stu-id="bbe9c-160">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="bbe9c-161">top</span><span class="sxs-lookup"><span data-stu-id="bbe9c-161">top</span></span>|<span data-ttu-id="bbe9c-162">double</span><span class="sxs-lookup"><span data-stu-id="bbe9c-162">double</span></span>|<span data-ttu-id="bbe9c-163">表示从对象左边界至第 1 行顶部（在工作表上）或图表区域顶部（在图表上）的距离，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="bbe9c-163">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="bbe9c-164">width</span><span class="sxs-lookup"><span data-stu-id="bbe9c-164">width</span></span>|<span data-ttu-id="bbe9c-165">double</span><span class="sxs-lookup"><span data-stu-id="bbe9c-165">double</span></span>|<span data-ttu-id="bbe9c-166">表示 chart 对象的宽度，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="bbe9c-166">Represents the width, in points, of the chart object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bbe9c-167">Relationships</span><span class="sxs-lookup"><span data-stu-id="bbe9c-167">Relationships</span></span>
| <span data-ttu-id="bbe9c-168">关系</span><span class="sxs-lookup"><span data-stu-id="bbe9c-168">Relationship</span></span> | <span data-ttu-id="bbe9c-169">类型</span><span class="sxs-lookup"><span data-stu-id="bbe9c-169">Type</span></span>   |<span data-ttu-id="bbe9c-170">说明</span><span class="sxs-lookup"><span data-stu-id="bbe9c-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bbe9c-171">axes</span><span class="sxs-lookup"><span data-stu-id="bbe9c-171">axes</span></span>|[<span data-ttu-id="bbe9c-172">ChartAxes</span><span class="sxs-lookup"><span data-stu-id="bbe9c-172">ChartAxes</span></span>](chartaxes.md)|<span data-ttu-id="bbe9c-p103">表示图表坐标轴。只读。</span><span class="sxs-lookup"><span data-stu-id="bbe9c-p103">Represents chart axes. Read-only.</span></span>|
|<span data-ttu-id="bbe9c-175">dataLabels</span><span class="sxs-lookup"><span data-stu-id="bbe9c-175">dataLabels</span></span>|[<span data-ttu-id="bbe9c-176">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="bbe9c-176">ChartDataLabels</span></span>](chartdatalabels.md)|<span data-ttu-id="bbe9c-p104">表示图表上的数据标签。只读。</span><span class="sxs-lookup"><span data-stu-id="bbe9c-p104">Represents the datalabels on the chart. Read-only.</span></span>|
|<span data-ttu-id="bbe9c-179">format</span><span class="sxs-lookup"><span data-stu-id="bbe9c-179">format</span></span>|[<span data-ttu-id="bbe9c-180">ChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="bbe9c-180">ChartAreaFormat</span></span>](chartareaformat.md)|<span data-ttu-id="bbe9c-p105">封装图表区域的格式属性。只读。</span><span class="sxs-lookup"><span data-stu-id="bbe9c-p105">Encapsulates the format properties for the chart area. Read-only.</span></span>|
|<span data-ttu-id="bbe9c-183">legend</span><span class="sxs-lookup"><span data-stu-id="bbe9c-183">legend</span></span>|[<span data-ttu-id="bbe9c-184">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="bbe9c-184">ChartLegend</span></span>](chartlegend.md)|<span data-ttu-id="bbe9c-p106">表示图表的图例。只读。</span><span class="sxs-lookup"><span data-stu-id="bbe9c-p106">Represents the legend for the chart. Read-only.</span></span>|
|<span data-ttu-id="bbe9c-187">series</span><span class="sxs-lookup"><span data-stu-id="bbe9c-187">series</span></span>|<span data-ttu-id="bbe9c-188">[ChartSeries](chartseries.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bbe9c-188">[ChartSeries](chartseries.md) collection</span></span>|<span data-ttu-id="bbe9c-p107">表示单个系列或图表中的系列集合。只读。</span><span class="sxs-lookup"><span data-stu-id="bbe9c-p107">Represents either a single series or collection of series in the chart. Read-only.</span></span>|
|<span data-ttu-id="bbe9c-191">title</span><span class="sxs-lookup"><span data-stu-id="bbe9c-191">title</span></span>|[<span data-ttu-id="bbe9c-192">ChartTitle</span><span class="sxs-lookup"><span data-stu-id="bbe9c-192">ChartTitle</span></span>](charttitle.md)|<span data-ttu-id="bbe9c-p108">表示指定图表的标题，包括标题的文本、可见性、位置和格式。只读。</span><span class="sxs-lookup"><span data-stu-id="bbe9c-p108">Represents the title of the specified chart, including the text, visibility, position and formating of the title. Read-only.</span></span>|
|<span data-ttu-id="bbe9c-195">worksheet</span><span class="sxs-lookup"><span data-stu-id="bbe9c-195">worksheet</span></span>|[<span data-ttu-id="bbe9c-196">工作表</span><span class="sxs-lookup"><span data-stu-id="bbe9c-196">Worksheet</span></span>](worksheet.md)|<span data-ttu-id="bbe9c-p109">包含当前图表的工作表。只读。</span><span class="sxs-lookup"><span data-stu-id="bbe9c-p109">The worksheet containing the current chart. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bbe9c-199">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bbe9c-199">JSON representation</span></span>

<span data-ttu-id="bbe9c-200">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bbe9c-200">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chart"
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
