---
title: 图表资源类型
description: 表示工作簿中的 chart 对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4bc0ad0d31981e7e84241519e92569ab25c2cf18
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460938"
---
# <a name="chart-resource-type"></a><span data-ttu-id="95b1a-103">图表资源类型</span><span class="sxs-lookup"><span data-stu-id="95b1a-103">Chart resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95b1a-104">表示工作簿中的 chart 对象。</span><span class="sxs-lookup"><span data-stu-id="95b1a-104">Represents a chart object in a workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="95b1a-105">方法</span><span class="sxs-lookup"><span data-stu-id="95b1a-105">Methods</span></span>

| <span data-ttu-id="95b1a-106">方法</span><span class="sxs-lookup"><span data-stu-id="95b1a-106">Method</span></span>           | <span data-ttu-id="95b1a-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="95b1a-107">Return Type</span></span>    |<span data-ttu-id="95b1a-108">说明</span><span class="sxs-lookup"><span data-stu-id="95b1a-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="95b1a-109">获取图表</span><span class="sxs-lookup"><span data-stu-id="95b1a-109">Get Chart</span></span>](../api/chart-get.md) | [<span data-ttu-id="95b1a-110">Chart</span><span class="sxs-lookup"><span data-stu-id="95b1a-110">Chart</span></span>](chart.md) |<span data-ttu-id="95b1a-111">读取 chart 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="95b1a-111">Read properties and relationships of chart object.</span></span>|
|[<span data-ttu-id="95b1a-112">创建 ChartSeries</span><span class="sxs-lookup"><span data-stu-id="95b1a-112">Create ChartSeries</span></span>](../api/chart-post-series.md) |[<span data-ttu-id="95b1a-113">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="95b1a-113">ChartSeries</span></span>](chartseries.md)| <span data-ttu-id="95b1a-114">通过发布到序列集合创建新的 ChartSeries。</span><span class="sxs-lookup"><span data-stu-id="95b1a-114">Create a new ChartSeries by posting to the series collection.</span></span>|
|[<span data-ttu-id="95b1a-115">创建系列</span><span class="sxs-lookup"><span data-stu-id="95b1a-115">List series</span></span>](../api/chart-list-series.md) |<span data-ttu-id="95b1a-116">[ChartSeries](chartseries.md) 集合</span><span class="sxs-lookup"><span data-stu-id="95b1a-116">[ChartSeries](chartseries.md) collection</span></span>| <span data-ttu-id="95b1a-117">获取 ChartSeries 对象集合。</span><span class="sxs-lookup"><span data-stu-id="95b1a-117">Get a ChartSeries object collection.</span></span>|
|[<span data-ttu-id="95b1a-118">更新</span><span class="sxs-lookup"><span data-stu-id="95b1a-118">Update</span></span>](../api/chart-update.md) | [<span data-ttu-id="95b1a-119">Chart</span><span class="sxs-lookup"><span data-stu-id="95b1a-119">Chart</span></span>](chart.md)   |<span data-ttu-id="95b1a-120">更新 Chart 对象。</span><span class="sxs-lookup"><span data-stu-id="95b1a-120">Update Chart object.</span></span> |
|[<span data-ttu-id="95b1a-121">图像</span><span class="sxs-lookup"><span data-stu-id="95b1a-121">Image</span></span>](../api/chart-image.md)|<span data-ttu-id="95b1a-122">图像 base64 编码字符串</span><span class="sxs-lookup"><span data-stu-id="95b1a-122">Image base64 encoded string</span></span>|<span data-ttu-id="95b1a-123">通过缩放图表适应指定的尺寸，将图表呈现为 base64 编码的图像。</span><span class="sxs-lookup"><span data-stu-id="95b1a-123">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>|
|[<span data-ttu-id="95b1a-124">Delete</span><span class="sxs-lookup"><span data-stu-id="95b1a-124">Delete</span></span>](../api/chart-delete.md)|<span data-ttu-id="95b1a-125">无</span><span class="sxs-lookup"><span data-stu-id="95b1a-125">None</span></span>|<span data-ttu-id="95b1a-126">删除 chart 对象。</span><span class="sxs-lookup"><span data-stu-id="95b1a-126">Deletes the chart object.</span></span>|
|[<span data-ttu-id="95b1a-127">Setdata</span><span class="sxs-lookup"><span data-stu-id="95b1a-127">Setdata</span></span>](../api/chart-setdata.md)|<span data-ttu-id="95b1a-128">无</span><span class="sxs-lookup"><span data-stu-id="95b1a-128">None</span></span>|<span data-ttu-id="95b1a-129">重置图表的源数据。</span><span class="sxs-lookup"><span data-stu-id="95b1a-129">Resets the source data for the chart.</span></span>|
|[<span data-ttu-id="95b1a-130">Setposition</span><span class="sxs-lookup"><span data-stu-id="95b1a-130">Setposition</span></span>](../api/chart-setposition.md)|<span data-ttu-id="95b1a-131">无</span><span class="sxs-lookup"><span data-stu-id="95b1a-131">None</span></span>|<span data-ttu-id="95b1a-132">相对于工作表上的单元格放置图表。</span><span class="sxs-lookup"><span data-stu-id="95b1a-132">Positions the chart relative to cells on the worksheet.</span></span>|
|[<span data-ttu-id="95b1a-133">列出</span><span class="sxs-lookup"><span data-stu-id="95b1a-133">List</span></span>](../api/chart-list.md) | <span data-ttu-id="95b1a-134">[图表](chart.md) 集合</span><span class="sxs-lookup"><span data-stu-id="95b1a-134">[Chart](chart.md) collection</span></span> |<span data-ttu-id="95b1a-135">获取 chart 对象集合。</span><span class="sxs-lookup"><span data-stu-id="95b1a-135">Get chart object collection.</span></span> |
|[<span data-ttu-id="95b1a-136">Itemat</span><span class="sxs-lookup"><span data-stu-id="95b1a-136">Itemat</span></span>](../api/chartcollection-itemat.md)|[<span data-ttu-id="95b1a-137">Chart</span><span class="sxs-lookup"><span data-stu-id="95b1a-137">Chart</span></span>](chart.md)|<span data-ttu-id="95b1a-138">根据其在集合中的位置获取图表。</span><span class="sxs-lookup"><span data-stu-id="95b1a-138">Gets a chart based on its position in the collection.</span></span>|
|[<span data-ttu-id="95b1a-139">添加</span><span class="sxs-lookup"><span data-stu-id="95b1a-139">Add</span></span>](../api/chartcollection-add.md)|[<span data-ttu-id="95b1a-140">图表</span><span class="sxs-lookup"><span data-stu-id="95b1a-140">Chart</span></span>](chart.md)|<span data-ttu-id="95b1a-141">创建新图表。</span><span class="sxs-lookup"><span data-stu-id="95b1a-141">Creates a new chart.</span></span>|

## <a name="properties"></a><span data-ttu-id="95b1a-142">属性</span><span class="sxs-lookup"><span data-stu-id="95b1a-142">Properties</span></span>
| <span data-ttu-id="95b1a-143">属性</span><span class="sxs-lookup"><span data-stu-id="95b1a-143">Property</span></span>     | <span data-ttu-id="95b1a-144">类型</span><span class="sxs-lookup"><span data-stu-id="95b1a-144">Type</span></span>   |<span data-ttu-id="95b1a-145">说明</span><span class="sxs-lookup"><span data-stu-id="95b1a-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95b1a-146">高度</span><span class="sxs-lookup"><span data-stu-id="95b1a-146">height</span></span>|<span data-ttu-id="95b1a-147">double</span><span class="sxs-lookup"><span data-stu-id="95b1a-147">double</span></span>|<span data-ttu-id="95b1a-148">表示 chart 对象的高度，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="95b1a-148">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="95b1a-149">id</span><span class="sxs-lookup"><span data-stu-id="95b1a-149">id</span></span>|<span data-ttu-id="95b1a-150">string</span><span class="sxs-lookup"><span data-stu-id="95b1a-150">string</span></span>|<span data-ttu-id="95b1a-p101">根据其在集合中的位置获取图表。只读。</span><span class="sxs-lookup"><span data-stu-id="95b1a-p101">Gets a chart based on its position in the collection. Read-only.</span></span>|
|<span data-ttu-id="95b1a-153">left</span><span class="sxs-lookup"><span data-stu-id="95b1a-153">left</span></span>|<span data-ttu-id="95b1a-154">double</span><span class="sxs-lookup"><span data-stu-id="95b1a-154">double</span></span>|<span data-ttu-id="95b1a-155">从图表左侧到工作表原点的距离，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="95b1a-155">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="95b1a-156">name</span><span class="sxs-lookup"><span data-stu-id="95b1a-156">name</span></span>|<span data-ttu-id="95b1a-157">string</span><span class="sxs-lookup"><span data-stu-id="95b1a-157">string</span></span>|<span data-ttu-id="95b1a-158">表示 chart 对象的名称。</span><span class="sxs-lookup"><span data-stu-id="95b1a-158">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="95b1a-159">top</span><span class="sxs-lookup"><span data-stu-id="95b1a-159">top</span></span>|<span data-ttu-id="95b1a-160">double</span><span class="sxs-lookup"><span data-stu-id="95b1a-160">double</span></span>|<span data-ttu-id="95b1a-161">表示从对象左边界至第 1 行顶部（在工作表上）或图表区域顶部（在图表上）的距离，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="95b1a-161">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="95b1a-162">width</span><span class="sxs-lookup"><span data-stu-id="95b1a-162">width</span></span>|<span data-ttu-id="95b1a-163">double</span><span class="sxs-lookup"><span data-stu-id="95b1a-163">double</span></span>|<span data-ttu-id="95b1a-164">表示 chart 对象的宽度，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="95b1a-164">Represents the width, in points, of the chart object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95b1a-165">关系</span><span class="sxs-lookup"><span data-stu-id="95b1a-165">Relationships</span></span>
| <span data-ttu-id="95b1a-166">关系</span><span class="sxs-lookup"><span data-stu-id="95b1a-166">Relationship</span></span> | <span data-ttu-id="95b1a-167">类型</span><span class="sxs-lookup"><span data-stu-id="95b1a-167">Type</span></span>   |<span data-ttu-id="95b1a-168">说明</span><span class="sxs-lookup"><span data-stu-id="95b1a-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95b1a-169">axes</span><span class="sxs-lookup"><span data-stu-id="95b1a-169">axes</span></span>|[<span data-ttu-id="95b1a-170">ChartAxes</span><span class="sxs-lookup"><span data-stu-id="95b1a-170">ChartAxes</span></span>](chartaxes.md)|<span data-ttu-id="95b1a-p102">表示图表坐标轴。只读。</span><span class="sxs-lookup"><span data-stu-id="95b1a-p102">Represents chart axes. Read-only.</span></span>|
|<span data-ttu-id="95b1a-173">dataLabels</span><span class="sxs-lookup"><span data-stu-id="95b1a-173">dataLabels</span></span>|[<span data-ttu-id="95b1a-174">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="95b1a-174">ChartDataLabels</span></span>](chartdatalabels.md)|<span data-ttu-id="95b1a-p103">表示图表上的数据标签。只读。</span><span class="sxs-lookup"><span data-stu-id="95b1a-p103">Represents the datalabels on the chart. Read-only.</span></span>|
|<span data-ttu-id="95b1a-177">format</span><span class="sxs-lookup"><span data-stu-id="95b1a-177">format</span></span>|[<span data-ttu-id="95b1a-178">ChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="95b1a-178">ChartAreaFormat</span></span>](chartareaformat.md)|<span data-ttu-id="95b1a-p104">封装图表区域的格式属性。只读。</span><span class="sxs-lookup"><span data-stu-id="95b1a-p104">Encapsulates the format properties for the chart area. Read-only.</span></span>|
|<span data-ttu-id="95b1a-181">legend</span><span class="sxs-lookup"><span data-stu-id="95b1a-181">legend</span></span>|[<span data-ttu-id="95b1a-182">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="95b1a-182">ChartLegend</span></span>](chartlegend.md)|<span data-ttu-id="95b1a-p105">表示图表的图例。只读。</span><span class="sxs-lookup"><span data-stu-id="95b1a-p105">Represents the legend for the chart. Read-only.</span></span>|
|<span data-ttu-id="95b1a-185">系列</span><span class="sxs-lookup"><span data-stu-id="95b1a-185">series</span></span>|<span data-ttu-id="95b1a-186">[ChartSeries](chartseries.md) 集合</span><span class="sxs-lookup"><span data-stu-id="95b1a-186">[ChartSeries](chartseries.md) collection</span></span>|<span data-ttu-id="95b1a-p106">表示单个系列或图表中的系列集合。只读。</span><span class="sxs-lookup"><span data-stu-id="95b1a-p106">Represents either a single series or collection of series in the chart. Read-only.</span></span>|
|<span data-ttu-id="95b1a-189">职位</span><span class="sxs-lookup"><span data-stu-id="95b1a-189">title</span></span>|[<span data-ttu-id="95b1a-190">ChartTitle</span><span class="sxs-lookup"><span data-stu-id="95b1a-190">ChartTitle</span></span>](charttitle.md)|<span data-ttu-id="95b1a-p107">表示指定图表的标题，包括标题的文本、可见性、位置和格式。只读。</span><span class="sxs-lookup"><span data-stu-id="95b1a-p107">Represents the title of the specified chart, including the text, visibility, position and formating of the title. Read-only.</span></span>|
|<span data-ttu-id="95b1a-193">工作表</span><span class="sxs-lookup"><span data-stu-id="95b1a-193">worksheet</span></span>|[<span data-ttu-id="95b1a-194">Worksheet</span><span class="sxs-lookup"><span data-stu-id="95b1a-194">Worksheet</span></span>](worksheet.md)|<span data-ttu-id="95b1a-p108">包含当前 chart 的 worksheet 对象。只读。</span><span class="sxs-lookup"><span data-stu-id="95b1a-p108">The worksheet containing the current chart. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="95b1a-197">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="95b1a-197">JSON representation</span></span>

<span data-ttu-id="95b1a-198">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95b1a-198">Here is a JSON representation of the resource.</span></span>

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
