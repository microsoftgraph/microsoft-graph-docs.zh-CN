---
title: workbookChart 资源类型
description: 表示工作簿中的 chart 对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: c180d6d2649f7c55868ffa04a5318c5c5f522ddd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007380"
---
# <a name="workbookchart-resource-type"></a><span data-ttu-id="11715-103">workbookChart 资源类型</span><span class="sxs-lookup"><span data-stu-id="11715-103">workbookChart resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11715-104">表示工作簿中的 chart 对象。</span><span class="sxs-lookup"><span data-stu-id="11715-104">Represents a chart object in a workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="11715-105">方法</span><span class="sxs-lookup"><span data-stu-id="11715-105">Methods</span></span>

| <span data-ttu-id="11715-106">方法</span><span class="sxs-lookup"><span data-stu-id="11715-106">Method</span></span>           | <span data-ttu-id="11715-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="11715-107">Return Type</span></span>    |<span data-ttu-id="11715-108">说明</span><span class="sxs-lookup"><span data-stu-id="11715-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="11715-109">获取图表</span><span class="sxs-lookup"><span data-stu-id="11715-109">Get Chart</span></span>](../api/chart-get.md) | [<span data-ttu-id="11715-110">workbookChart</span><span class="sxs-lookup"><span data-stu-id="11715-110">workbookChart</span></span>](workbookchart.md) |<span data-ttu-id="11715-111">读取 chart 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="11715-111">Read properties and relationships of chart object.</span></span>|
|[<span data-ttu-id="11715-112">创建 ChartSeries</span><span class="sxs-lookup"><span data-stu-id="11715-112">Create ChartSeries</span></span>](../api/chart-post-series.md) |[<span data-ttu-id="11715-113">workbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="11715-113">workbookChartSeries</span></span>](workbookchartseries.md)| <span data-ttu-id="11715-114">通过发布到序列集合创建新的 ChartSeries。</span><span class="sxs-lookup"><span data-stu-id="11715-114">Create a new ChartSeries by posting to the series collection.</span></span>|
|[<span data-ttu-id="11715-115">创建系列</span><span class="sxs-lookup"><span data-stu-id="11715-115">List series</span></span>](../api/chart-list-series.md) |<span data-ttu-id="11715-116">[workbookChartSeries](workbookchartseries.md)集合</span><span class="sxs-lookup"><span data-stu-id="11715-116">[workbookChartSeries](workbookchartseries.md) collection</span></span>| <span data-ttu-id="11715-117">获取 ChartSeries 对象集合。</span><span class="sxs-lookup"><span data-stu-id="11715-117">Get a ChartSeries object collection.</span></span>|
|[<span data-ttu-id="11715-118">更新</span><span class="sxs-lookup"><span data-stu-id="11715-118">Update</span></span>](../api/chart-update.md) | [<span data-ttu-id="11715-119">workbookChart</span><span class="sxs-lookup"><span data-stu-id="11715-119">workbookChart</span></span>](workbookchart.md)   |<span data-ttu-id="11715-120">更新 Chart 对象。</span><span class="sxs-lookup"><span data-stu-id="11715-120">Update Chart object.</span></span> |
|[<span data-ttu-id="11715-121">图像</span><span class="sxs-lookup"><span data-stu-id="11715-121">Image</span></span>](../api/chart-image.md)|<span data-ttu-id="11715-122">图像 base64 编码字符串</span><span class="sxs-lookup"><span data-stu-id="11715-122">Image base64 encoded string</span></span>|<span data-ttu-id="11715-123">通过缩放图表适应指定的尺寸，将图表呈现为 base64 编码的图像。</span><span class="sxs-lookup"><span data-stu-id="11715-123">Renders the chart as a base64-encoded image by scaling the chart to fit the specified dimensions.</span></span>|
|[<span data-ttu-id="11715-124">删除</span><span class="sxs-lookup"><span data-stu-id="11715-124">Delete</span></span>](../api/chart-delete.md)|<span data-ttu-id="11715-125">无</span><span class="sxs-lookup"><span data-stu-id="11715-125">None</span></span>|<span data-ttu-id="11715-126">删除 chart 对象。</span><span class="sxs-lookup"><span data-stu-id="11715-126">Deletes the chart object.</span></span>|
|[<span data-ttu-id="11715-127">Setdata</span><span class="sxs-lookup"><span data-stu-id="11715-127">Setdata</span></span>](../api/chart-setdata.md)|<span data-ttu-id="11715-128">无</span><span class="sxs-lookup"><span data-stu-id="11715-128">None</span></span>|<span data-ttu-id="11715-129">重置图表的源数据。</span><span class="sxs-lookup"><span data-stu-id="11715-129">Resets the source data for the chart.</span></span>|
|[<span data-ttu-id="11715-130">Setposition</span><span class="sxs-lookup"><span data-stu-id="11715-130">Setposition</span></span>](../api/chart-setposition.md)|<span data-ttu-id="11715-131">无</span><span class="sxs-lookup"><span data-stu-id="11715-131">None</span></span>|<span data-ttu-id="11715-132">相对于工作表上的单元格放置图表。</span><span class="sxs-lookup"><span data-stu-id="11715-132">Positions the chart relative to cells on the worksheet.</span></span>|
|[<span data-ttu-id="11715-133">列出</span><span class="sxs-lookup"><span data-stu-id="11715-133">List</span></span>](../api/chart-list.md) | <span data-ttu-id="11715-134">[workbookChart](workbookchart.md)集合</span><span class="sxs-lookup"><span data-stu-id="11715-134">[workbookChart](workbookchart.md) collection</span></span> |<span data-ttu-id="11715-135">获取 chart 对象集合。</span><span class="sxs-lookup"><span data-stu-id="11715-135">Get chart object collection.</span></span> |
|[<span data-ttu-id="11715-136">Itemat</span><span class="sxs-lookup"><span data-stu-id="11715-136">Itemat</span></span>](../api/chartcollection-itemat.md)|[<span data-ttu-id="11715-137">workbookChart</span><span class="sxs-lookup"><span data-stu-id="11715-137">workbookChart</span></span>](workbookchart.md)|<span data-ttu-id="11715-138">根据其在集合中的位置获取图表。</span><span class="sxs-lookup"><span data-stu-id="11715-138">Gets a chart based on its position in the collection.</span></span>|
|[<span data-ttu-id="11715-139">添加</span><span class="sxs-lookup"><span data-stu-id="11715-139">Add</span></span>](../api/chartcollection-add.md)|[<span data-ttu-id="11715-140">workbookChart</span><span class="sxs-lookup"><span data-stu-id="11715-140">workbookChart</span></span>](workbookchart.md)|<span data-ttu-id="11715-141">创建新图表。</span><span class="sxs-lookup"><span data-stu-id="11715-141">Creates a new chart.</span></span>|

## <a name="properties"></a><span data-ttu-id="11715-142">属性</span><span class="sxs-lookup"><span data-stu-id="11715-142">Properties</span></span>
| <span data-ttu-id="11715-143">属性</span><span class="sxs-lookup"><span data-stu-id="11715-143">Property</span></span>     | <span data-ttu-id="11715-144">类型</span><span class="sxs-lookup"><span data-stu-id="11715-144">Type</span></span>   |<span data-ttu-id="11715-145">说明</span><span class="sxs-lookup"><span data-stu-id="11715-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11715-146">高度</span><span class="sxs-lookup"><span data-stu-id="11715-146">height</span></span>|<span data-ttu-id="11715-147">double</span><span class="sxs-lookup"><span data-stu-id="11715-147">double</span></span>|<span data-ttu-id="11715-148">表示 chart 对象的高度，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="11715-148">Represents the height, in points, of the chart object.</span></span>|
|<span data-ttu-id="11715-149">id</span><span class="sxs-lookup"><span data-stu-id="11715-149">id</span></span>|<span data-ttu-id="11715-150">string</span><span class="sxs-lookup"><span data-stu-id="11715-150">string</span></span>|<span data-ttu-id="11715-p101">根据其在集合中的位置获取图表。只读。</span><span class="sxs-lookup"><span data-stu-id="11715-p101">Gets a chart based on its position in the collection. Read-only.</span></span>|
|<span data-ttu-id="11715-153">left</span><span class="sxs-lookup"><span data-stu-id="11715-153">left</span></span>|<span data-ttu-id="11715-154">double</span><span class="sxs-lookup"><span data-stu-id="11715-154">double</span></span>|<span data-ttu-id="11715-155">从图表左侧到工作表原点的距离，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="11715-155">The distance, in points, from the left side of the chart to the worksheet origin.</span></span>|
|<span data-ttu-id="11715-156">name</span><span class="sxs-lookup"><span data-stu-id="11715-156">name</span></span>|<span data-ttu-id="11715-157">string</span><span class="sxs-lookup"><span data-stu-id="11715-157">string</span></span>|<span data-ttu-id="11715-158">表示 chart 对象的名称。</span><span class="sxs-lookup"><span data-stu-id="11715-158">Represents the name of a chart object.</span></span>|
|<span data-ttu-id="11715-159">top</span><span class="sxs-lookup"><span data-stu-id="11715-159">top</span></span>|<span data-ttu-id="11715-160">double</span><span class="sxs-lookup"><span data-stu-id="11715-160">double</span></span>|<span data-ttu-id="11715-161">表示从对象左边界至第 1 行顶部（在工作表上）或图表区域顶部（在图表上）的距离，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="11715-161">Represents the distance, in points, from the top edge of the object to the top of row 1 (on a worksheet) or the top of the chart area (on a chart).</span></span>|
|<span data-ttu-id="11715-162">width</span><span class="sxs-lookup"><span data-stu-id="11715-162">width</span></span>|<span data-ttu-id="11715-163">double</span><span class="sxs-lookup"><span data-stu-id="11715-163">double</span></span>|<span data-ttu-id="11715-164">表示 chart 对象的宽度，以磅值表示。</span><span class="sxs-lookup"><span data-stu-id="11715-164">Represents the width, in points, of the chart object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11715-165">关系</span><span class="sxs-lookup"><span data-stu-id="11715-165">Relationships</span></span>
| <span data-ttu-id="11715-166">关系</span><span class="sxs-lookup"><span data-stu-id="11715-166">Relationship</span></span> | <span data-ttu-id="11715-167">类型</span><span class="sxs-lookup"><span data-stu-id="11715-167">Type</span></span>   |<span data-ttu-id="11715-168">说明</span><span class="sxs-lookup"><span data-stu-id="11715-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11715-169">axes</span><span class="sxs-lookup"><span data-stu-id="11715-169">axes</span></span>|[<span data-ttu-id="11715-170">workbookChartAxes</span><span class="sxs-lookup"><span data-stu-id="11715-170">workbookChartAxes</span></span>](workbookchartaxes.md)|<span data-ttu-id="11715-p102">表示图表坐标轴。只读。</span><span class="sxs-lookup"><span data-stu-id="11715-p102">Represents chart axes. Read-only.</span></span>|
|<span data-ttu-id="11715-173">dataLabels</span><span class="sxs-lookup"><span data-stu-id="11715-173">dataLabels</span></span>|[<span data-ttu-id="11715-174">workbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="11715-174">workbookChartDataLabels</span></span>](workbookchartdatalabels.md)|<span data-ttu-id="11715-p103">表示图表上的数据标签。只读。</span><span class="sxs-lookup"><span data-stu-id="11715-p103">Represents the datalabels on the chart. Read-only.</span></span>|
|<span data-ttu-id="11715-177">format</span><span class="sxs-lookup"><span data-stu-id="11715-177">format</span></span>|[<span data-ttu-id="11715-178">workbookChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="11715-178">workbookChartAreaFormat</span></span>](workbookchartareaformat.md)|<span data-ttu-id="11715-p104">封装图表区域的格式属性。只读。</span><span class="sxs-lookup"><span data-stu-id="11715-p104">Encapsulates the format properties for the chart area. Read-only.</span></span>|
|<span data-ttu-id="11715-181">legend</span><span class="sxs-lookup"><span data-stu-id="11715-181">legend</span></span>|[<span data-ttu-id="11715-182">workbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="11715-182">workbookChartLegend</span></span>](workbookchartlegend.md)|<span data-ttu-id="11715-p105">表示图表的图例。只读。</span><span class="sxs-lookup"><span data-stu-id="11715-p105">Represents the legend for the chart. Read-only.</span></span>|
|<span data-ttu-id="11715-185">series</span><span class="sxs-lookup"><span data-stu-id="11715-185">series</span></span>|<span data-ttu-id="11715-186">[workbookChartSeries](workbookchartseries.md)集合</span><span class="sxs-lookup"><span data-stu-id="11715-186">[workbookChartSeries](workbookchartseries.md) collection</span></span>|<span data-ttu-id="11715-p106">表示单个系列或图表中的系列集合。只读。</span><span class="sxs-lookup"><span data-stu-id="11715-p106">Represents either a single series or collection of series in the chart. Read-only.</span></span>|
|<span data-ttu-id="11715-189">职位</span><span class="sxs-lookup"><span data-stu-id="11715-189">title</span></span>|[<span data-ttu-id="11715-190">workbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="11715-190">workbookChartTitle</span></span>](workbookcharttitle.md)|<span data-ttu-id="11715-p107">表示指定图表的标题，包括标题的文本、可见性、位置和格式。只读。</span><span class="sxs-lookup"><span data-stu-id="11715-p107">Represents the title of the specified chart, including the text, visibility, position and formating of the title. Read-only.</span></span>|
|<span data-ttu-id="11715-193">工作表</span><span class="sxs-lookup"><span data-stu-id="11715-193">worksheet</span></span>|[<span data-ttu-id="11715-194">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="11715-194">workbookWorksheet</span></span>](workbookworksheet.md)|<span data-ttu-id="11715-195">包含当前 chart 的 worksheet 对象。</span><span class="sxs-lookup"><span data-stu-id="11715-195">The worksheet containing the current chart.</span></span> <span data-ttu-id="11715-196">只读。</span><span class="sxs-lookup"><span data-stu-id="11715-196">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11715-197">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="11715-197">JSON representation</span></span>

<span data-ttu-id="11715-198">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="11715-198">Here is a JSON representation of the resource.</span></span>

<!-- {
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
<!--
{
  "type": "#page.annotation",
  "description": "workbookChart resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
