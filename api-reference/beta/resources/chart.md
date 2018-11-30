---
title: 图表资源类型
description: 表示工作簿中的 chart 对象。
ms.openlocfilehash: 3305c674bf299fa68ce139ba16b3174965b694ac
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047597"
---
# <a name="chart-resource-type"></a><span data-ttu-id="8bde4-103">图表资源类型</span><span class="sxs-lookup"><span data-stu-id="8bde4-103">Chart resource type</span></span>

> <span data-ttu-id="8bde4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8bde4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8bde4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8bde4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8bde4-106">表示工作簿中的 chart 对象。</span><span class="sxs-lookup"><span data-stu-id="8bde4-106">Represents a chart object in a workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="8bde4-107">方法</span><span class="sxs-lookup"><span data-stu-id="8bde4-107">Methods</span></span>

| <span data-ttu-id="8bde4-108">方法</span><span class="sxs-lookup"><span data-stu-id="8bde4-108">Method</span></span>           | <span data-ttu-id="8bde4-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="8bde4-109">Return Type</span></span>    |<span data-ttu-id="8bde4-110">说明</span><span class="sxs-lookup"><span data-stu-id="8bde4-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8bde4-111">获取图表</span><span class="sxs-lookup"><span data-stu-id="8bde4-111">Get Chart</span></span>](../api/chart-get.md) | [<span data-ttu-id="8bde4-112">Chart</span><span class="sxs-lookup"><span data-stu-id="8bde4-112">Chart</span></span>](chart.md) |<span data-ttu-id="8bde4-113">读取 chart 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8bde4-113">Read properties and relationships of chart object.</span></span>|
|[<span data-ttu-id="8bde4-114">创建 ChartSeries</span><span class="sxs-lookup"><span data-stu-id="8bde4-114">Create ChartSeries</span></span>](../api/chart-post-series.md) |[<span data-ttu-id="8bde4-115">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="8bde4-115">ChartSeries</span></span>](chartseries.md)| <span data-ttu-id="8bde4-116">通过发布到序列集合创建新的 ChartSeries。</span><span class="sxs-lookup"><span data-stu-id="8bde4-116">Create a new ChartSeries by posting to the series collection.</span></span>|
|[<span data-ttu-id="8bde4-117">创建系列</span><span class="sxs-lookup"><span data-stu-id="8bde4-117">List series</span></span>](../api/chart-list-series.md) |<span data-ttu-id="8bde4-118">[ChartSeries](chartseries.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8bde4-118">[ChartSeries](chartseries.md) collection</span></span>| <span data-ttu-id="8bde4-119">获取 ChartSeries 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8bde4-119">Get a ChartSeries object collection.</span></span>|
|[<span data-ttu-id="8bde4-120">Update</span><span class="sxs-lookup"><span data-stu-id="8bde4-120">Update</span></span>](../api/chart-update.md) | [<span data-ttu-id="8bde4-121">Chart</span><span class="sxs-lookup"><span data-stu-id="8bde4-121">Chart</span></span>](chart.md)   |<span data-ttu-id="8bde4-122">更新 Chart 对象。</span><span class="sxs-lookup"><span data-stu-id="8bde4-122">Update Chart object.</span></span> |
|[<span data-ttu-id="8bde4-123">图像</span><span class="sxs-lookup"><span data-stu-id="8bde4-123">Image</span></span>](../api/chart-image.md)|<span data-ttu-id="8bde4-124">图像 base64 编码字符串</span><span class="sxs-lookup"><span data-stu-id="8bde4-124">Image base64 encoded string</span></span>|<span data-ttu-id="8bde4-125">通过缩放图表适应指定的尺寸，将图表呈现为 base64 编码的图像。</span><span class="sxs-lookup"><span data-stu-id="8bde4-125">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>|
|[<span data-ttu-id="8bde4-126">删除</span><span class="sxs-lookup"><span data-stu-id="8bde4-126">Delete</span></span>](../api/chart-delete.md)|<span data-ttu-id="8bde4-127">无</span><span class="sxs-lookup"><span data-stu-id="8bde4-127">None</span></span>|<span data-ttu-id="8bde4-128">删除 chart 对象。</span><span class="sxs-lookup"><span data-stu-id="8bde4-128">Deletes the chart object.</span></span>|
|[<span data-ttu-id="8bde4-129">Setdata</span><span class="sxs-lookup"><span data-stu-id="8bde4-129">Setdata</span></span>](../api/chart-setdata.md)|<span data-ttu-id="8bde4-130">无</span><span class="sxs-lookup"><span data-stu-id="8bde4-130">None</span></span>|<span data-ttu-id="8bde4-131">重置图表的源数据。</span><span class="sxs-lookup"><span data-stu-id="8bde4-131">Resets the source data for the chart.</span></span>|
|[<span data-ttu-id="8bde4-132">Setposition</span><span class="sxs-lookup"><span data-stu-id="8bde4-132">Setposition</span></span>](../api/chart-setposition.md)|<span data-ttu-id="8bde4-133">无</span><span class="sxs-lookup"><span data-stu-id="8bde4-133">None</span></span>|<span data-ttu-id="8bde4-134">相对于工作表上的单元格放置图表。</span><span class="sxs-lookup"><span data-stu-id="8bde4-134">Positions the chart relative to cells on the worksheet.</span></span>|
|[<span data-ttu-id="8bde4-135">List</span><span class="sxs-lookup"><span data-stu-id="8bde4-135">List</span></span>](../api/chart-list.md) | <span data-ttu-id="8bde4-136">[图表](chart.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8bde4-136">[Chart](chart.md) collection</span></span> |<span data-ttu-id="8bde4-137">获取 chart 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8bde4-137">Get chart object collection.</span></span> |
|[<span data-ttu-id="8bde4-138">Itemat</span><span class="sxs-lookup"><span data-stu-id="8bde4-138">Itemat</span></span>](../api/chartcollection-itemat.md)|[<span data-ttu-id="8bde4-139">Chart</span><span class="sxs-lookup"><span data-stu-id="8bde4-139">Chart</span></span>](chart.md)|<span data-ttu-id="8bde4-140">按图表在集合中的位置获取此对象。</span><span class="sxs-lookup"><span data-stu-id="8bde4-140">Gets a chart based on its position in the collection.</span></span>|
|[<span data-ttu-id="8bde4-141">Add</span><span class="sxs-lookup"><span data-stu-id="8bde4-141">Add</span></span>](../api/chartcollection-add.md)|[<span data-ttu-id="8bde4-142">Chart</span><span class="sxs-lookup"><span data-stu-id="8bde4-142">Chart</span></span>](chart.md)|<span data-ttu-id="8bde4-143">创建新图表。</span><span class="sxs-lookup"><span data-stu-id="8bde4-143">Creates a new chart.</span></span>|

## <a name="properties"></a><span data-ttu-id="8bde4-144">属性</span><span class="sxs-lookup"><span data-stu-id="8bde4-144">Properties</span></span>
| <span data-ttu-id="8bde4-145">属性</span><span class="sxs-lookup"><span data-stu-id="8bde4-145">Property</span></span>     | <span data-ttu-id="8bde4-146">类型</span><span class="sxs-lookup"><span data-stu-id="8bde4-146">Type</span></span>   |<span data-ttu-id="8bde4-147">说明</span><span class="sxs-lookup"><span data-stu-id="8bde4-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8bde4-148">height</span><span class="sxs-lookup"><span data-stu-id="8bde4-148">height</span></span>|<span data-ttu-id="8bde4-149">double</span><span class="sxs-lookup"><span data-stu-id="8bde4-149">double</span></span>|<span data-ttu-id="8bde4-150">表示 chart 对象的高度，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="8bde4-150">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="8bde4-151">id</span><span class="sxs-lookup"><span data-stu-id="8bde4-151">id</span></span>|<span data-ttu-id="8bde4-152">string</span><span class="sxs-lookup"><span data-stu-id="8bde4-152">string</span></span>|<span data-ttu-id="8bde4-p102">根据其在集合中的位置获取图表。只读。</span><span class="sxs-lookup"><span data-stu-id="8bde4-p102">Gets a chart based on its position in the collection. Read-only.</span></span>|
|<span data-ttu-id="8bde4-155">left</span><span class="sxs-lookup"><span data-stu-id="8bde4-155">left</span></span>|<span data-ttu-id="8bde4-156">double</span><span class="sxs-lookup"><span data-stu-id="8bde4-156">double</span></span>|<span data-ttu-id="8bde4-157">从图表左侧到工作表原点的距离，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="8bde4-157">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="8bde4-158">name</span><span class="sxs-lookup"><span data-stu-id="8bde4-158">name</span></span>|<span data-ttu-id="8bde4-159">string</span><span class="sxs-lookup"><span data-stu-id="8bde4-159">string</span></span>|<span data-ttu-id="8bde4-160">表示 chart 对象的名称。</span><span class="sxs-lookup"><span data-stu-id="8bde4-160">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="8bde4-161">top</span><span class="sxs-lookup"><span data-stu-id="8bde4-161">top</span></span>|<span data-ttu-id="8bde4-162">double</span><span class="sxs-lookup"><span data-stu-id="8bde4-162">double</span></span>|<span data-ttu-id="8bde4-163">表示从对象左边界至第 1 行顶部（在工作表上）或图表区域顶部（在图表上）的距离，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="8bde4-163">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="8bde4-164">width</span><span class="sxs-lookup"><span data-stu-id="8bde4-164">width</span></span>|<span data-ttu-id="8bde4-165">double</span><span class="sxs-lookup"><span data-stu-id="8bde4-165">double</span></span>|<span data-ttu-id="8bde4-166">表示 chart 对象的宽度，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="8bde4-166">Represents the width, in points, of the chart object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8bde4-167">Relationships</span><span class="sxs-lookup"><span data-stu-id="8bde4-167">Relationships</span></span>
| <span data-ttu-id="8bde4-168">关系</span><span class="sxs-lookup"><span data-stu-id="8bde4-168">Relationship</span></span> | <span data-ttu-id="8bde4-169">类型</span><span class="sxs-lookup"><span data-stu-id="8bde4-169">Type</span></span>   |<span data-ttu-id="8bde4-170">说明</span><span class="sxs-lookup"><span data-stu-id="8bde4-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8bde4-171">axes</span><span class="sxs-lookup"><span data-stu-id="8bde4-171">axes</span></span>|[<span data-ttu-id="8bde4-172">ChartAxes</span><span class="sxs-lookup"><span data-stu-id="8bde4-172">ChartAxes</span></span>](chartaxes.md)|<span data-ttu-id="8bde4-p103">表示图表坐标轴。只读。</span><span class="sxs-lookup"><span data-stu-id="8bde4-p103">Represents chart axes. Read-only.</span></span>|
|<span data-ttu-id="8bde4-175">dataLabels</span><span class="sxs-lookup"><span data-stu-id="8bde4-175">dataLabels</span></span>|[<span data-ttu-id="8bde4-176">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="8bde4-176">ChartDataLabels</span></span>](chartdatalabels.md)|<span data-ttu-id="8bde4-p104">表示图表上的数据标签。只读。</span><span class="sxs-lookup"><span data-stu-id="8bde4-p104">Represents the datalabels on the chart. Read-only.</span></span>|
|<span data-ttu-id="8bde4-179">format</span><span class="sxs-lookup"><span data-stu-id="8bde4-179">format</span></span>|[<span data-ttu-id="8bde4-180">ChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="8bde4-180">ChartAreaFormat</span></span>](chartareaformat.md)|<span data-ttu-id="8bde4-p105">封装图表区域的格式属性。只读。</span><span class="sxs-lookup"><span data-stu-id="8bde4-p105">Encapsulates the format properties for the chart area. Read-only.</span></span>|
|<span data-ttu-id="8bde4-183">legend</span><span class="sxs-lookup"><span data-stu-id="8bde4-183">legend</span></span>|[<span data-ttu-id="8bde4-184">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="8bde4-184">ChartLegend</span></span>](chartlegend.md)|<span data-ttu-id="8bde4-p106">表示图表的图例。只读。</span><span class="sxs-lookup"><span data-stu-id="8bde4-p106">Represents the legend for the chart. Read-only.</span></span>|
|<span data-ttu-id="8bde4-187">series</span><span class="sxs-lookup"><span data-stu-id="8bde4-187">series</span></span>|<span data-ttu-id="8bde4-188">[ChartSeries](chartseries.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8bde4-188">[ChartSeries](chartseries.md) collection</span></span>|<span data-ttu-id="8bde4-p107">表示单个系列或图表中的系列集合。只读。</span><span class="sxs-lookup"><span data-stu-id="8bde4-p107">Represents either a single series or collection of series in the chart. Read-only.</span></span>|
|<span data-ttu-id="8bde4-191">title</span><span class="sxs-lookup"><span data-stu-id="8bde4-191">title</span></span>|[<span data-ttu-id="8bde4-192">ChartTitle</span><span class="sxs-lookup"><span data-stu-id="8bde4-192">ChartTitle</span></span>](charttitle.md)|<span data-ttu-id="8bde4-p108">表示指定图表的标题，包括标题的文本、可见性、位置和格式。只读。</span><span class="sxs-lookup"><span data-stu-id="8bde4-p108">Represents the title of the specified chart, including the text, visibility, position and formating of the title. Read-only.</span></span>|
|<span data-ttu-id="8bde4-195">工作表</span><span class="sxs-lookup"><span data-stu-id="8bde4-195">worksheet</span></span>|[<span data-ttu-id="8bde4-196">工作表</span><span class="sxs-lookup"><span data-stu-id="8bde4-196">Worksheet</span></span>](worksheet.md)|<span data-ttu-id="8bde4-p109">包含当前图表的工作表。只读。</span><span class="sxs-lookup"><span data-stu-id="8bde4-p109">The worksheet containing the current chart. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8bde4-199">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8bde4-199">JSON representation</span></span>

<span data-ttu-id="8bde4-200">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8bde4-200">Here is a JSON representation of the resource.</span></span>

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