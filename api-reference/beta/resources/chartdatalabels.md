---
title: ChartDataLabels 资源类型
description: 表示图表点上的所有数据标签的集合。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 16e2e3acafc98a4066b8620f41f15c7cae1667cc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954678"
---
# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="d38a6-103">ChartDataLabels 资源类型</span><span class="sxs-lookup"><span data-stu-id="d38a6-103">ChartDataLabels resource type</span></span>

> <span data-ttu-id="d38a6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d38a6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d38a6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d38a6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d38a6-106">表示图表点上的所有数据标签的集合。</span><span class="sxs-lookup"><span data-stu-id="d38a6-106">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="d38a6-107">方法</span><span class="sxs-lookup"><span data-stu-id="d38a6-107">Methods</span></span>

| <span data-ttu-id="d38a6-108">方法</span><span class="sxs-lookup"><span data-stu-id="d38a6-108">Method</span></span>           | <span data-ttu-id="d38a6-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d38a6-109">Return Type</span></span>    |<span data-ttu-id="d38a6-110">说明</span><span class="sxs-lookup"><span data-stu-id="d38a6-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d38a6-111">获取 ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="d38a6-111">Get ChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="d38a6-112">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="d38a6-112">ChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="d38a6-113">读取 chartDataLabels 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d38a6-113">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="d38a6-114">Update</span><span class="sxs-lookup"><span data-stu-id="d38a6-114">Update</span></span>](../api/chartdatalabels-update.md) | [<span data-ttu-id="d38a6-115">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="d38a6-115">ChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="d38a6-116">更新 ChartDataLabels 对象</span><span class="sxs-lookup"><span data-stu-id="d38a6-116">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d38a6-117">属性</span><span class="sxs-lookup"><span data-stu-id="d38a6-117">Properties</span></span>
| <span data-ttu-id="d38a6-118">属性</span><span class="sxs-lookup"><span data-stu-id="d38a6-118">Property</span></span>     | <span data-ttu-id="d38a6-119">类型</span><span class="sxs-lookup"><span data-stu-id="d38a6-119">Type</span></span>   |<span data-ttu-id="d38a6-120">说明</span><span class="sxs-lookup"><span data-stu-id="d38a6-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d38a6-121">position</span><span class="sxs-lookup"><span data-stu-id="d38a6-121">position</span></span>|<span data-ttu-id="d38a6-122">string</span><span class="sxs-lookup"><span data-stu-id="d38a6-122">string</span></span>|<span data-ttu-id="d38a6-p102">表示数据标签位置的 DataLabelPosition 值。可能的值是：`None`、`Center`、`InsideEnd`、`InsideBase`、`OutsideEnd`、`Left`、`Right`、`Top`、`Bottom`、`BestFit`、`Callout`。</span><span class="sxs-lookup"><span data-stu-id="d38a6-p102">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="d38a6-125">separator</span><span class="sxs-lookup"><span data-stu-id="d38a6-125">separator</span></span>|<span data-ttu-id="d38a6-126">string</span><span class="sxs-lookup"><span data-stu-id="d38a6-126">string</span></span>|<span data-ttu-id="d38a6-127">表示用于图表中数据标签的分隔符的字符串。</span><span class="sxs-lookup"><span data-stu-id="d38a6-127">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="d38a6-128">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="d38a6-128">showBubbleSize</span></span>|<span data-ttu-id="d38a6-129">boolean</span><span class="sxs-lookup"><span data-stu-id="d38a6-129">boolean</span></span>|<span data-ttu-id="d38a6-130">表示数据标签气泡大小是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="d38a6-130">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="d38a6-131">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="d38a6-131">showCategoryName</span></span>|<span data-ttu-id="d38a6-132">boolean</span><span class="sxs-lookup"><span data-stu-id="d38a6-132">boolean</span></span>|<span data-ttu-id="d38a6-133">表示数据标签类别名称是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="d38a6-133">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="d38a6-134">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="d38a6-134">showLegendKey</span></span>|<span data-ttu-id="d38a6-135">boolean</span><span class="sxs-lookup"><span data-stu-id="d38a6-135">boolean</span></span>|<span data-ttu-id="d38a6-136">表示数据标签图例标示是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="d38a6-136">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="d38a6-137">showPercentage</span><span class="sxs-lookup"><span data-stu-id="d38a6-137">showPercentage</span></span>|<span data-ttu-id="d38a6-138">boolean</span><span class="sxs-lookup"><span data-stu-id="d38a6-138">boolean</span></span>|<span data-ttu-id="d38a6-139">表示数据标签百分比是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="d38a6-139">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="d38a6-140">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="d38a6-140">showSeriesName</span></span>|<span data-ttu-id="d38a6-141">boolean</span><span class="sxs-lookup"><span data-stu-id="d38a6-141">boolean</span></span>|<span data-ttu-id="d38a6-142">表示数据标签系列名称是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="d38a6-142">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="d38a6-143">showValue</span><span class="sxs-lookup"><span data-stu-id="d38a6-143">showValue</span></span>|<span data-ttu-id="d38a6-144">boolean</span><span class="sxs-lookup"><span data-stu-id="d38a6-144">boolean</span></span>|<span data-ttu-id="d38a6-145">表示数据标签值是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="d38a6-145">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d38a6-146">Relationships</span><span class="sxs-lookup"><span data-stu-id="d38a6-146">Relationships</span></span>
| <span data-ttu-id="d38a6-147">关系</span><span class="sxs-lookup"><span data-stu-id="d38a6-147">Relationship</span></span> | <span data-ttu-id="d38a6-148">类型</span><span class="sxs-lookup"><span data-stu-id="d38a6-148">Type</span></span>   |<span data-ttu-id="d38a6-149">说明</span><span class="sxs-lookup"><span data-stu-id="d38a6-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d38a6-150">format</span><span class="sxs-lookup"><span data-stu-id="d38a6-150">format</span></span>|[<span data-ttu-id="d38a6-151">ChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="d38a6-151">ChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="d38a6-p103">表示图表数据标签的格式，包括填充和字体格式。只读。</span><span class="sxs-lookup"><span data-stu-id="d38a6-p103">Represents the format of chart data labels, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d38a6-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d38a6-154">JSON representation</span></span>

<span data-ttu-id="d38a6-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d38a6-155">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartDataLabels"
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
