---
title: workbookChartDataLabels 资源类型
description: 表示图表点上的所有数据标签的集合。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: c5e469f5d95065fa3b5a161d510ca023e17f807a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007289"
---
# <a name="workbookchartdatalabels-resource-type"></a><span data-ttu-id="ea337-103">workbookChartDataLabels 资源类型</span><span class="sxs-lookup"><span data-stu-id="ea337-103">workbookChartDataLabels resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea337-104">表示图表点上的所有数据标签的集合。</span><span class="sxs-lookup"><span data-stu-id="ea337-104">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="ea337-105">方法</span><span class="sxs-lookup"><span data-stu-id="ea337-105">Methods</span></span>

| <span data-ttu-id="ea337-106">方法</span><span class="sxs-lookup"><span data-stu-id="ea337-106">Method</span></span>           | <span data-ttu-id="ea337-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="ea337-107">Return Type</span></span>    |<span data-ttu-id="ea337-108">说明</span><span class="sxs-lookup"><span data-stu-id="ea337-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ea337-109">获取 workbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="ea337-109">Get workbookChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="ea337-110">workbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="ea337-110">workbookChartDataLabels</span></span>](workbookchartdatalabels.md) |<span data-ttu-id="ea337-111">读取 chartDataLabels 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ea337-111">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="ea337-112">更新</span><span class="sxs-lookup"><span data-stu-id="ea337-112">Update</span></span>](../api/chartdatalabels-update.md) | [<span data-ttu-id="ea337-113">workbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="ea337-113">workbookChartDataLabels</span></span>](workbookchartdatalabels.md) |<span data-ttu-id="ea337-114">更新 ChartDataLabels 对象</span><span class="sxs-lookup"><span data-stu-id="ea337-114">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ea337-115">属性</span><span class="sxs-lookup"><span data-stu-id="ea337-115">Properties</span></span>
| <span data-ttu-id="ea337-116">属性</span><span class="sxs-lookup"><span data-stu-id="ea337-116">Property</span></span>     | <span data-ttu-id="ea337-117">类型</span><span class="sxs-lookup"><span data-stu-id="ea337-117">Type</span></span>   |<span data-ttu-id="ea337-118">说明</span><span class="sxs-lookup"><span data-stu-id="ea337-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea337-119">position</span><span class="sxs-lookup"><span data-stu-id="ea337-119">position</span></span>|<span data-ttu-id="ea337-120">字符串</span><span class="sxs-lookup"><span data-stu-id="ea337-120">string</span></span>|<span data-ttu-id="ea337-121">表示数据标签的位置的 DataLabelPosition 值。</span><span class="sxs-lookup"><span data-stu-id="ea337-121">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="ea337-122">可能的值为: `None`、 `Center`、 `InsideEnd` `InsideBase` `OutsideEnd` `Left` `Right` `Top` `Bottom`、、、、、、、、 `Callout` `BestFit`。</span><span class="sxs-lookup"><span data-stu-id="ea337-122">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="ea337-123">Separator</span><span class="sxs-lookup"><span data-stu-id="ea337-123">separator</span></span>|<span data-ttu-id="ea337-124">string</span><span class="sxs-lookup"><span data-stu-id="ea337-124">string</span></span>|<span data-ttu-id="ea337-125">表示用于图表中数据标签的分隔符的字符串。</span><span class="sxs-lookup"><span data-stu-id="ea337-125">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="ea337-126">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="ea337-126">showBubbleSize</span></span>|<span data-ttu-id="ea337-127">boolean</span><span class="sxs-lookup"><span data-stu-id="ea337-127">boolean</span></span>|<span data-ttu-id="ea337-128">表示数据标签气泡大小是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="ea337-128">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="ea337-129">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="ea337-129">showCategoryName</span></span>|<span data-ttu-id="ea337-130">boolean</span><span class="sxs-lookup"><span data-stu-id="ea337-130">boolean</span></span>|<span data-ttu-id="ea337-131">表示数据标签类别名称是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="ea337-131">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="ea337-132">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="ea337-132">showLegendKey</span></span>|<span data-ttu-id="ea337-133">boolean</span><span class="sxs-lookup"><span data-stu-id="ea337-133">boolean</span></span>|<span data-ttu-id="ea337-134">表示数据标签图例标示是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="ea337-134">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="ea337-135">showPercentage</span><span class="sxs-lookup"><span data-stu-id="ea337-135">showPercentage</span></span>|<span data-ttu-id="ea337-136">boolean</span><span class="sxs-lookup"><span data-stu-id="ea337-136">boolean</span></span>|<span data-ttu-id="ea337-137">表示数据标签百分比是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="ea337-137">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="ea337-138">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="ea337-138">showSeriesName</span></span>|<span data-ttu-id="ea337-139">boolean</span><span class="sxs-lookup"><span data-stu-id="ea337-139">boolean</span></span>|<span data-ttu-id="ea337-140">表示数据标签系列名称是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="ea337-140">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="ea337-141">showValue</span><span class="sxs-lookup"><span data-stu-id="ea337-141">showValue</span></span>|<span data-ttu-id="ea337-142">布尔</span><span class="sxs-lookup"><span data-stu-id="ea337-142">boolean</span></span>|<span data-ttu-id="ea337-143">表示数据标签值是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="ea337-143">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea337-144">关系</span><span class="sxs-lookup"><span data-stu-id="ea337-144">Relationships</span></span>
| <span data-ttu-id="ea337-145">关系</span><span class="sxs-lookup"><span data-stu-id="ea337-145">Relationship</span></span> | <span data-ttu-id="ea337-146">类型</span><span class="sxs-lookup"><span data-stu-id="ea337-146">Type</span></span>   |<span data-ttu-id="ea337-147">说明</span><span class="sxs-lookup"><span data-stu-id="ea337-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea337-148">format</span><span class="sxs-lookup"><span data-stu-id="ea337-148">format</span></span>|[<span data-ttu-id="ea337-149">workbookChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="ea337-149">workbookChartDataLabelFormat</span></span>](workbookchartdatalabelformat.md)|<span data-ttu-id="ea337-150">表示图表数据标签的格式，包括填充和字体格式。</span><span class="sxs-lookup"><span data-stu-id="ea337-150">Represents the format of chart data labels, which includes fill and font formatting.</span></span> <span data-ttu-id="ea337-151">只读。</span><span class="sxs-lookup"><span data-stu-id="ea337-151">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ea337-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ea337-152">JSON representation</span></span>

<span data-ttu-id="ea337-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea337-153">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "workbookChartDataLabels resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
