---
title: 图表资源类型
description: 表示工作簿中的 chart 对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4bc0ad0d31981e7e84241519e92569ab25c2cf18
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529521"
---
# <a name="chart-resource-type"></a><span data-ttu-id="30c7e-103">图表资源类型</span><span class="sxs-lookup"><span data-stu-id="30c7e-103">Chart resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30c7e-104">表示工作簿中的 chart 对象。</span><span class="sxs-lookup"><span data-stu-id="30c7e-104">Represents a chart object in a workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="30c7e-105">方法</span><span class="sxs-lookup"><span data-stu-id="30c7e-105">Methods</span></span>

| <span data-ttu-id="30c7e-106">方法</span><span class="sxs-lookup"><span data-stu-id="30c7e-106">Method</span></span>           | <span data-ttu-id="30c7e-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="30c7e-107">Return Type</span></span>    |<span data-ttu-id="30c7e-108">说明</span><span class="sxs-lookup"><span data-stu-id="30c7e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30c7e-109">获取图表</span><span class="sxs-lookup"><span data-stu-id="30c7e-109">[Get Chart](../api/chart-get.md)</span></span> | [<span data-ttu-id="30c7e-110">Chart</span><span class="sxs-lookup"><span data-stu-id="30c7e-110">Chart</span></span>](chart.md) |<span data-ttu-id="30c7e-111">读取 chart 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="30c7e-111">Read properties and relationships of chart object.</span></span>|
|<span data-ttu-id="30c7e-112">创建 ChartSeries</span><span class="sxs-lookup"><span data-stu-id="30c7e-112">[Create ChartSeries](../api/chart-post-series.md)</span></span> |[<span data-ttu-id="30c7e-113">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="30c7e-113">ChartSeries</span></span>](chartseries.md)| <span data-ttu-id="30c7e-114">通过发布到序列集合创建新的 ChartSeries。</span><span class="sxs-lookup"><span data-stu-id="30c7e-114">Create a new ChartSeries by posting to the series collection.</span></span>|
|<span data-ttu-id="30c7e-115">创建系列</span><span class="sxs-lookup"><span data-stu-id="30c7e-115">[List series](../api/chart-list-series.md)</span></span> |<span data-ttu-id="30c7e-116">ChartSeries 集合</span><span class="sxs-lookup"><span data-stu-id="30c7e-116">[ChartSeries](chartseries.md) collection</span></span>| <span data-ttu-id="30c7e-117">获取 ChartSeries 对象集合。</span><span class="sxs-lookup"><span data-stu-id="30c7e-117">Get a ChartSeries object collection.</span></span>|
|[<span data-ttu-id="30c7e-118">Update</span><span class="sxs-lookup"><span data-stu-id="30c7e-118">Update</span></span>](../api/chart-update.md) | [<span data-ttu-id="30c7e-119">Chart</span><span class="sxs-lookup"><span data-stu-id="30c7e-119">Chart</span></span>](chart.md)   |<span data-ttu-id="30c7e-120">更新 Chart 对象。</span><span class="sxs-lookup"><span data-stu-id="30c7e-120">Update Chart object.</span></span> |
|[<span data-ttu-id="30c7e-121">Image</span><span class="sxs-lookup"><span data-stu-id="30c7e-121">Image</span></span>](../api/chart-image.md)|<span data-ttu-id="30c7e-122">图像 base64 编码字符串</span><span class="sxs-lookup"><span data-stu-id="30c7e-122">Image base64 encoded string</span></span>|<span data-ttu-id="30c7e-123">通过缩放图表适应指定的尺寸，将图表呈现为 base64 编码的图像。</span><span class="sxs-lookup"><span data-stu-id="30c7e-123">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>|
|[<span data-ttu-id="30c7e-124">删除</span><span class="sxs-lookup"><span data-stu-id="30c7e-124">Delete</span></span>](../api/chart-delete.md)|<span data-ttu-id="30c7e-125">无</span><span class="sxs-lookup"><span data-stu-id="30c7e-125">None</span></span>|<span data-ttu-id="30c7e-126">删除 chart 对象。</span><span class="sxs-lookup"><span data-stu-id="30c7e-126">Deletes the chart object.</span></span>|
|[<span data-ttu-id="30c7e-127">Setdata</span><span class="sxs-lookup"><span data-stu-id="30c7e-127">Setdata</span></span>](../api/chart-setdata.md)|<span data-ttu-id="30c7e-128">无</span><span class="sxs-lookup"><span data-stu-id="30c7e-128">None</span></span>|<span data-ttu-id="30c7e-129">重置图表的源数据。</span><span class="sxs-lookup"><span data-stu-id="30c7e-129">Resets the source data for the chart.</span></span>|
|[<span data-ttu-id="30c7e-130">Setposition</span><span class="sxs-lookup"><span data-stu-id="30c7e-130">Setposition</span></span>](../api/chart-setposition.md)|<span data-ttu-id="30c7e-131">无</span><span class="sxs-lookup"><span data-stu-id="30c7e-131">None</span></span>|<span data-ttu-id="30c7e-132">相对于工作表上的单元格放置图表。</span><span class="sxs-lookup"><span data-stu-id="30c7e-132">Positions the chart relative to cells on the worksheet.</span></span>|
|[<span data-ttu-id="30c7e-133">List</span><span class="sxs-lookup"><span data-stu-id="30c7e-133">List</span></span>](../api/chart-list.md) | <span data-ttu-id="30c7e-134">图表 集合</span><span class="sxs-lookup"><span data-stu-id="30c7e-134">[Chart](chart.md) collection</span></span> |<span data-ttu-id="30c7e-135">获取 chart 对象集合。</span><span class="sxs-lookup"><span data-stu-id="30c7e-135">Get chart object collection.</span></span> |
|[<span data-ttu-id="30c7e-136">Itemat</span><span class="sxs-lookup"><span data-stu-id="30c7e-136">Itemat</span></span>](../api/chartcollection-itemat.md)|[<span data-ttu-id="30c7e-137">Chart</span><span class="sxs-lookup"><span data-stu-id="30c7e-137">Chart</span></span>](chart.md)|<span data-ttu-id="30c7e-138">按图表在集合中的位置获取此对象。</span><span class="sxs-lookup"><span data-stu-id="30c7e-138">Gets a chart based on its position in the collection.</span></span>|
|[<span data-ttu-id="30c7e-139">Add</span><span class="sxs-lookup"><span data-stu-id="30c7e-139">Add</span></span>](../api/chartcollection-add.md)|[<span data-ttu-id="30c7e-140">Chart</span><span class="sxs-lookup"><span data-stu-id="30c7e-140">Chart</span></span>](chart.md)|<span data-ttu-id="30c7e-141">创建新图表。</span><span class="sxs-lookup"><span data-stu-id="30c7e-141">Creates a new chart.</span></span>|

## <a name="properties"></a><span data-ttu-id="30c7e-142">属性</span><span class="sxs-lookup"><span data-stu-id="30c7e-142">Properties</span></span>
| <span data-ttu-id="30c7e-143">属性</span><span class="sxs-lookup"><span data-stu-id="30c7e-143">Property</span></span>     | <span data-ttu-id="30c7e-144">类型</span><span class="sxs-lookup"><span data-stu-id="30c7e-144">Type</span></span>   |<span data-ttu-id="30c7e-145">说明</span><span class="sxs-lookup"><span data-stu-id="30c7e-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30c7e-146">height</span><span class="sxs-lookup"><span data-stu-id="30c7e-146">height</span></span>|<span data-ttu-id="30c7e-147">double</span><span class="sxs-lookup"><span data-stu-id="30c7e-147">double</span></span>|<span data-ttu-id="30c7e-148">表示 chart 对象的高度，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="30c7e-148">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="30c7e-149">id</span><span class="sxs-lookup"><span data-stu-id="30c7e-149">id</span></span>|<span data-ttu-id="30c7e-150">string</span><span class="sxs-lookup"><span data-stu-id="30c7e-150">string</span></span>|<span data-ttu-id="30c7e-p101">根据其在集合中的位置获取图表。只读。</span><span class="sxs-lookup"><span data-stu-id="30c7e-p101">Gets a chart based on its position in the collection. Read-only.</span></span>|
|<span data-ttu-id="30c7e-153">left</span><span class="sxs-lookup"><span data-stu-id="30c7e-153">left</span></span>|<span data-ttu-id="30c7e-154">double</span><span class="sxs-lookup"><span data-stu-id="30c7e-154">double</span></span>|<span data-ttu-id="30c7e-155">从图表左侧到工作表原点的距离，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="30c7e-155">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="30c7e-156">name</span><span class="sxs-lookup"><span data-stu-id="30c7e-156">name</span></span>|<span data-ttu-id="30c7e-157">string</span><span class="sxs-lookup"><span data-stu-id="30c7e-157">string</span></span>|<span data-ttu-id="30c7e-158">表示 chart 对象的名称。</span><span class="sxs-lookup"><span data-stu-id="30c7e-158">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="30c7e-159">top</span><span class="sxs-lookup"><span data-stu-id="30c7e-159">top</span></span>|<span data-ttu-id="30c7e-160">double</span><span class="sxs-lookup"><span data-stu-id="30c7e-160">double</span></span>|<span data-ttu-id="30c7e-161">表示从对象左边界至第 1 行顶部（在工作表上）或图表区域顶部（在图表上）的距离，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="30c7e-161">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="30c7e-162">width</span><span class="sxs-lookup"><span data-stu-id="30c7e-162">width</span></span>|<span data-ttu-id="30c7e-163">double</span><span class="sxs-lookup"><span data-stu-id="30c7e-163">double</span></span>|<span data-ttu-id="30c7e-164">表示 chart 对象的宽度，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="30c7e-164">Represents the width, in points, of the chart object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="30c7e-165">关系</span><span class="sxs-lookup"><span data-stu-id="30c7e-165">Relationships</span></span>
| <span data-ttu-id="30c7e-166">关系</span><span class="sxs-lookup"><span data-stu-id="30c7e-166">Relationship</span></span> | <span data-ttu-id="30c7e-167">类型</span><span class="sxs-lookup"><span data-stu-id="30c7e-167">Type</span></span>   |<span data-ttu-id="30c7e-168">说明</span><span class="sxs-lookup"><span data-stu-id="30c7e-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30c7e-169">axes</span><span class="sxs-lookup"><span data-stu-id="30c7e-169">axes</span></span>|[<span data-ttu-id="30c7e-170">ChartAxes</span><span class="sxs-lookup"><span data-stu-id="30c7e-170">ChartAxes</span></span>](chartaxes.md)|<span data-ttu-id="30c7e-p102">表示图表坐标轴。只读。</span><span class="sxs-lookup"><span data-stu-id="30c7e-p102">Represents chart axes. Read-only.</span></span>|
|<span data-ttu-id="30c7e-173">dataLabels</span><span class="sxs-lookup"><span data-stu-id="30c7e-173">dataLabels</span></span>|[<span data-ttu-id="30c7e-174">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="30c7e-174">ChartDataLabels</span></span>](chartdatalabels.md)|<span data-ttu-id="30c7e-p103">表示图表上的数据标签。只读。</span><span class="sxs-lookup"><span data-stu-id="30c7e-p103">Represents the datalabels on the chart. Read-only.</span></span>|
|<span data-ttu-id="30c7e-177">format</span><span class="sxs-lookup"><span data-stu-id="30c7e-177">format</span></span>|[<span data-ttu-id="30c7e-178">ChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="30c7e-178">ChartAreaFormat</span></span>](chartareaformat.md)|<span data-ttu-id="30c7e-p104">封装图表区域的格式属性。只读。</span><span class="sxs-lookup"><span data-stu-id="30c7e-p104">Encapsulates the format properties for the chart area. Read-only.</span></span>|
|<span data-ttu-id="30c7e-181">legend</span><span class="sxs-lookup"><span data-stu-id="30c7e-181">legend</span></span>|[<span data-ttu-id="30c7e-182">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="30c7e-182">ChartLegend</span></span>](chartlegend.md)|<span data-ttu-id="30c7e-p105">表示图表的图例。只读。</span><span class="sxs-lookup"><span data-stu-id="30c7e-p105">Represents the legend for the chart. Read-only.</span></span>|
|<span data-ttu-id="30c7e-185">series</span><span class="sxs-lookup"><span data-stu-id="30c7e-185">series</span></span>|<span data-ttu-id="30c7e-186">[ChartSeries](chartseries.md) 集合</span><span class="sxs-lookup"><span data-stu-id="30c7e-186">[ChartSeries](chartseries.md) collection</span></span>|<span data-ttu-id="30c7e-p106">表示单个系列或图表中的系列集合。只读。</span><span class="sxs-lookup"><span data-stu-id="30c7e-p106">Represents either a single series or collection of series in the chart. Read-only.</span></span>|
|<span data-ttu-id="30c7e-189">title</span><span class="sxs-lookup"><span data-stu-id="30c7e-189">title</span></span>|[<span data-ttu-id="30c7e-190">ChartTitle</span><span class="sxs-lookup"><span data-stu-id="30c7e-190">ChartTitle</span></span>](charttitle.md)|<span data-ttu-id="30c7e-p107">表示指定图表的标题，包括标题的文本、可见性、位置和格式。只读。</span><span class="sxs-lookup"><span data-stu-id="30c7e-p107">Represents the title of the specified chart, including the text, visibility, position and formating of the title. Read-only.</span></span>|
|<span data-ttu-id="30c7e-193">worksheet</span><span class="sxs-lookup"><span data-stu-id="30c7e-193">worksheet</span></span>|[<span data-ttu-id="30c7e-194">工作表</span><span class="sxs-lookup"><span data-stu-id="30c7e-194">Worksheet</span></span>](worksheet.md)|<span data-ttu-id="30c7e-p108">包含当前图表的工作表。只读。</span><span class="sxs-lookup"><span data-stu-id="30c7e-p108">The worksheet containing the current chart. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="30c7e-197">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="30c7e-197">JSON representation</span></span>

<span data-ttu-id="30c7e-198">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="30c7e-198">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Chart resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chart.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
