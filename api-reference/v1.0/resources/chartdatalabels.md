---
title: ChartDataLabels 资源类型
description: 表示图表点上的所有数据标签的集合。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 502f18fdf03eb28bde4b6f8620bb274f6f2052dd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988434"
---
# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="9ed83-103">ChartDataLabels 资源类型</span><span class="sxs-lookup"><span data-stu-id="9ed83-103">ChartDataLabels resource type</span></span>

<span data-ttu-id="9ed83-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ed83-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9ed83-105">表示图表点上的所有数据标签的集合。</span><span class="sxs-lookup"><span data-stu-id="9ed83-105">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="9ed83-106">方法</span><span class="sxs-lookup"><span data-stu-id="9ed83-106">Methods</span></span>

| <span data-ttu-id="9ed83-107">方法</span><span class="sxs-lookup"><span data-stu-id="9ed83-107">Method</span></span>           | <span data-ttu-id="9ed83-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="9ed83-108">Return Type</span></span>    |<span data-ttu-id="9ed83-109">说明</span><span class="sxs-lookup"><span data-stu-id="9ed83-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9ed83-110">获取 ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="9ed83-110">Get ChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="9ed83-111">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="9ed83-111">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="9ed83-112">读取 chartDataLabels 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9ed83-112">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="9ed83-113">更新</span><span class="sxs-lookup"><span data-stu-id="9ed83-113">Update</span></span>](../api/chartdatalabels-update.md) | [<span data-ttu-id="9ed83-114">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="9ed83-114">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="9ed83-115">更新 ChartDataLabels 对象</span><span class="sxs-lookup"><span data-stu-id="9ed83-115">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9ed83-116">属性</span><span class="sxs-lookup"><span data-stu-id="9ed83-116">Properties</span></span>
| <span data-ttu-id="9ed83-117">属性</span><span class="sxs-lookup"><span data-stu-id="9ed83-117">Property</span></span>     | <span data-ttu-id="9ed83-118">类型</span><span class="sxs-lookup"><span data-stu-id="9ed83-118">Type</span></span>   |<span data-ttu-id="9ed83-119">说明</span><span class="sxs-lookup"><span data-stu-id="9ed83-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ed83-120">position</span><span class="sxs-lookup"><span data-stu-id="9ed83-120">position</span></span>|<span data-ttu-id="9ed83-121">string</span><span class="sxs-lookup"><span data-stu-id="9ed83-121">string</span></span>|<span data-ttu-id="9ed83-122">表示数据标签的位置的 DataLabelPosition 值。</span><span class="sxs-lookup"><span data-stu-id="9ed83-122">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="9ed83-123">可能的值为：、、、、、、、、、、 `None` `Center` `InsideEnd` `InsideBase` `OutsideEnd` `Left` `Right` `Top` `Bottom` `BestFit` `Callout` 。</span><span class="sxs-lookup"><span data-stu-id="9ed83-123">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="9ed83-124">Separator</span><span class="sxs-lookup"><span data-stu-id="9ed83-124">separator</span></span>|<span data-ttu-id="9ed83-125">string</span><span class="sxs-lookup"><span data-stu-id="9ed83-125">string</span></span>|<span data-ttu-id="9ed83-126">表示用于图表中数据标签的分隔符的字符串。</span><span class="sxs-lookup"><span data-stu-id="9ed83-126">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="9ed83-127">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="9ed83-127">showBubbleSize</span></span>|<span data-ttu-id="9ed83-128">布尔</span><span class="sxs-lookup"><span data-stu-id="9ed83-128">boolean</span></span>|<span data-ttu-id="9ed83-129">表示数据标签气泡大小是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="9ed83-129">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="9ed83-130">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="9ed83-130">showCategoryName</span></span>|<span data-ttu-id="9ed83-131">布尔</span><span class="sxs-lookup"><span data-stu-id="9ed83-131">boolean</span></span>|<span data-ttu-id="9ed83-132">表示数据标签类别名称是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="9ed83-132">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="9ed83-133">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="9ed83-133">showLegendKey</span></span>|<span data-ttu-id="9ed83-134">布尔</span><span class="sxs-lookup"><span data-stu-id="9ed83-134">boolean</span></span>|<span data-ttu-id="9ed83-135">表示数据标签图例标示是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="9ed83-135">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="9ed83-136">showPercentage</span><span class="sxs-lookup"><span data-stu-id="9ed83-136">showPercentage</span></span>|<span data-ttu-id="9ed83-137">布尔</span><span class="sxs-lookup"><span data-stu-id="9ed83-137">boolean</span></span>|<span data-ttu-id="9ed83-138">表示数据标签百分比是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="9ed83-138">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="9ed83-139">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="9ed83-139">showSeriesName</span></span>|<span data-ttu-id="9ed83-140">布尔</span><span class="sxs-lookup"><span data-stu-id="9ed83-140">boolean</span></span>|<span data-ttu-id="9ed83-141">表示数据标签系列名称是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="9ed83-141">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="9ed83-142">showValue</span><span class="sxs-lookup"><span data-stu-id="9ed83-142">showValue</span></span>|<span data-ttu-id="9ed83-143">布尔</span><span class="sxs-lookup"><span data-stu-id="9ed83-143">boolean</span></span>|<span data-ttu-id="9ed83-144">表示数据标签值是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="9ed83-144">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ed83-145">关系</span><span class="sxs-lookup"><span data-stu-id="9ed83-145">Relationships</span></span>
| <span data-ttu-id="9ed83-146">关系</span><span class="sxs-lookup"><span data-stu-id="9ed83-146">Relationship</span></span> | <span data-ttu-id="9ed83-147">类型</span><span class="sxs-lookup"><span data-stu-id="9ed83-147">Type</span></span>   |<span data-ttu-id="9ed83-148">说明</span><span class="sxs-lookup"><span data-stu-id="9ed83-148">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ed83-149">format</span><span class="sxs-lookup"><span data-stu-id="9ed83-149">format</span></span>|[<span data-ttu-id="9ed83-150">WorkbookChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="9ed83-150">WorkbookChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="9ed83-151">表示图表数据标签的格式，包括填充和字体格式。</span><span class="sxs-lookup"><span data-stu-id="9ed83-151">Represents the format of chart data labels, which includes fill and font formatting.</span></span> <span data-ttu-id="9ed83-152">只读。</span><span class="sxs-lookup"><span data-stu-id="9ed83-152">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9ed83-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9ed83-153">JSON representation</span></span>

<span data-ttu-id="9ed83-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ed83-154">Here is a JSON representation of the resource.</span></span>

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

