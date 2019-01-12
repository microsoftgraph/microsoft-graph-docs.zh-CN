---
title: ChartDataLabels 资源类型
description: 表示图表点上的所有数据标签的集合。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 48d6cb0d35e82fc0117a24aad1c5e171bc869870
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961414"
---
# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="d0e97-103">ChartDataLabels 资源类型</span><span class="sxs-lookup"><span data-stu-id="d0e97-103">ChartDataLabels resource type</span></span>

<span data-ttu-id="d0e97-104">表示图表点上的所有数据标签的集合。</span><span class="sxs-lookup"><span data-stu-id="d0e97-104">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="d0e97-105">方法</span><span class="sxs-lookup"><span data-stu-id="d0e97-105">Methods</span></span>

| <span data-ttu-id="d0e97-106">方法</span><span class="sxs-lookup"><span data-stu-id="d0e97-106">Method</span></span>           | <span data-ttu-id="d0e97-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="d0e97-107">Return Type</span></span>    |<span data-ttu-id="d0e97-108">说明</span><span class="sxs-lookup"><span data-stu-id="d0e97-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d0e97-109">获取 ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="d0e97-109">Get ChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="d0e97-110">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="d0e97-110">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="d0e97-111">读取 chartDataLabels 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d0e97-111">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="d0e97-112">Update</span><span class="sxs-lookup"><span data-stu-id="d0e97-112">Update</span></span>](../api/chartdatalabels-update.md) | [<span data-ttu-id="d0e97-113">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="d0e97-113">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="d0e97-114">更新 ChartDataLabels 对象</span><span class="sxs-lookup"><span data-stu-id="d0e97-114">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d0e97-115">属性</span><span class="sxs-lookup"><span data-stu-id="d0e97-115">Properties</span></span>
| <span data-ttu-id="d0e97-116">属性</span><span class="sxs-lookup"><span data-stu-id="d0e97-116">Property</span></span>     | <span data-ttu-id="d0e97-117">类型</span><span class="sxs-lookup"><span data-stu-id="d0e97-117">Type</span></span>   |<span data-ttu-id="d0e97-118">说明</span><span class="sxs-lookup"><span data-stu-id="d0e97-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0e97-119">position</span><span class="sxs-lookup"><span data-stu-id="d0e97-119">position</span></span>|<span data-ttu-id="d0e97-120">string</span><span class="sxs-lookup"><span data-stu-id="d0e97-120">string</span></span>|<span data-ttu-id="d0e97-121">DataLabelPosition 值，它代表数据标签的位置。</span><span class="sxs-lookup"><span data-stu-id="d0e97-121">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="d0e97-122">可能的值为： `None`， `Center`， `InsideEnd`， `InsideBase`， `OutsideEnd`， `Left`， `Right`， `Top`， `Bottom`， `BestFit`， `Callout`。</span><span class="sxs-lookup"><span data-stu-id="d0e97-122">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="d0e97-123">separator</span><span class="sxs-lookup"><span data-stu-id="d0e97-123">separator</span></span>|<span data-ttu-id="d0e97-124">string</span><span class="sxs-lookup"><span data-stu-id="d0e97-124">string</span></span>|<span data-ttu-id="d0e97-125">表示用于图表中数据标签的分隔符的字符串。</span><span class="sxs-lookup"><span data-stu-id="d0e97-125">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="d0e97-126">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="d0e97-126">showBubbleSize</span></span>|<span data-ttu-id="d0e97-127">boolean</span><span class="sxs-lookup"><span data-stu-id="d0e97-127">boolean</span></span>|<span data-ttu-id="d0e97-128">表示数据标签气泡大小是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="d0e97-128">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="d0e97-129">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="d0e97-129">showCategoryName</span></span>|<span data-ttu-id="d0e97-130">boolean</span><span class="sxs-lookup"><span data-stu-id="d0e97-130">boolean</span></span>|<span data-ttu-id="d0e97-131">表示数据标签类别名称是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="d0e97-131">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="d0e97-132">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="d0e97-132">showLegendKey</span></span>|<span data-ttu-id="d0e97-133">boolean</span><span class="sxs-lookup"><span data-stu-id="d0e97-133">boolean</span></span>|<span data-ttu-id="d0e97-134">表示数据标签图例标示是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="d0e97-134">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="d0e97-135">showPercentage</span><span class="sxs-lookup"><span data-stu-id="d0e97-135">showPercentage</span></span>|<span data-ttu-id="d0e97-136">boolean</span><span class="sxs-lookup"><span data-stu-id="d0e97-136">boolean</span></span>|<span data-ttu-id="d0e97-137">表示数据标签百分比是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="d0e97-137">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="d0e97-138">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="d0e97-138">showSeriesName</span></span>|<span data-ttu-id="d0e97-139">boolean</span><span class="sxs-lookup"><span data-stu-id="d0e97-139">boolean</span></span>|<span data-ttu-id="d0e97-140">表示数据标签系列名称是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="d0e97-140">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="d0e97-141">showValue</span><span class="sxs-lookup"><span data-stu-id="d0e97-141">showValue</span></span>|<span data-ttu-id="d0e97-142">boolean</span><span class="sxs-lookup"><span data-stu-id="d0e97-142">boolean</span></span>|<span data-ttu-id="d0e97-143">表示数据标签值是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="d0e97-143">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0e97-144">Relationships</span><span class="sxs-lookup"><span data-stu-id="d0e97-144">Relationships</span></span>
| <span data-ttu-id="d0e97-145">关系</span><span class="sxs-lookup"><span data-stu-id="d0e97-145">Relationship</span></span> | <span data-ttu-id="d0e97-146">类型</span><span class="sxs-lookup"><span data-stu-id="d0e97-146">Type</span></span>   |<span data-ttu-id="d0e97-147">说明</span><span class="sxs-lookup"><span data-stu-id="d0e97-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0e97-148">format</span><span class="sxs-lookup"><span data-stu-id="d0e97-148">format</span></span>|[<span data-ttu-id="d0e97-149">WorkbookChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="d0e97-149">WorkbookChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="d0e97-p102">表示图表数据标签的格式，包括填充和字体格式。只读。</span><span class="sxs-lookup"><span data-stu-id="d0e97-p102">Represents the format of chart data labels, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d0e97-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d0e97-152">JSON representation</span></span>

<span data-ttu-id="d0e97-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d0e97-153">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartDataLabels"
}-->

```json
{
  "position": "string",
  "separator": "string",
  "showBubbleSize": true,
  "showCategoryName": true,
  "showLegendKey": true,
  "showPercentage": true,
  "showSeriesName": true,
  "showValue": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartDataLabels resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
