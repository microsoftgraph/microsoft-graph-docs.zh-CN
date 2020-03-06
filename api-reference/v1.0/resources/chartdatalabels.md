---
title: ChartDataLabels 资源类型
description: 表示图表点上的所有数据标签的集合。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 7e45e9160573c7297285ebb6613be0bf405b0086
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531866"
---
# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="b394a-103">ChartDataLabels 资源类型</span><span class="sxs-lookup"><span data-stu-id="b394a-103">ChartDataLabels resource type</span></span>

<span data-ttu-id="b394a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b394a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b394a-105">表示图表点上的所有数据标签的集合。</span><span class="sxs-lookup"><span data-stu-id="b394a-105">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="b394a-106">Methods</span><span class="sxs-lookup"><span data-stu-id="b394a-106">Methods</span></span>

| <span data-ttu-id="b394a-107">方法</span><span class="sxs-lookup"><span data-stu-id="b394a-107">Method</span></span>           | <span data-ttu-id="b394a-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="b394a-108">Return Type</span></span>    |<span data-ttu-id="b394a-109">说明</span><span class="sxs-lookup"><span data-stu-id="b394a-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b394a-110">获取 ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="b394a-110">Get ChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="b394a-111">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="b394a-111">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="b394a-112">读取 chartDataLabels 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b394a-112">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="b394a-113">更新</span><span class="sxs-lookup"><span data-stu-id="b394a-113">Update</span></span>](../api/chartdatalabels-update.md) | [<span data-ttu-id="b394a-114">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="b394a-114">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="b394a-115">更新 ChartDataLabels 对象</span><span class="sxs-lookup"><span data-stu-id="b394a-115">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b394a-116">属性</span><span class="sxs-lookup"><span data-stu-id="b394a-116">Properties</span></span>
| <span data-ttu-id="b394a-117">属性</span><span class="sxs-lookup"><span data-stu-id="b394a-117">Property</span></span>     | <span data-ttu-id="b394a-118">类型</span><span class="sxs-lookup"><span data-stu-id="b394a-118">Type</span></span>   |<span data-ttu-id="b394a-119">说明</span><span class="sxs-lookup"><span data-stu-id="b394a-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b394a-120">position</span><span class="sxs-lookup"><span data-stu-id="b394a-120">position</span></span>|<span data-ttu-id="b394a-121">字符串</span><span class="sxs-lookup"><span data-stu-id="b394a-121">string</span></span>|<span data-ttu-id="b394a-122">表示数据标签的位置的 DataLabelPosition 值。</span><span class="sxs-lookup"><span data-stu-id="b394a-122">DataLabelPosition value that represents the position of the data label.</span></span> <span data-ttu-id="b394a-123">可能的值为： `None`、 `Center`、 `InsideEnd` `InsideBase` `OutsideEnd` `Left` `Right` `Top` `Bottom`、、、、、、、、 `Callout` `BestFit`。</span><span class="sxs-lookup"><span data-stu-id="b394a-123">The possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="b394a-124">Separator</span><span class="sxs-lookup"><span data-stu-id="b394a-124">separator</span></span>|<span data-ttu-id="b394a-125">string</span><span class="sxs-lookup"><span data-stu-id="b394a-125">string</span></span>|<span data-ttu-id="b394a-126">表示用于图表中数据标签的分隔符的字符串。</span><span class="sxs-lookup"><span data-stu-id="b394a-126">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="b394a-127">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="b394a-127">showBubbleSize</span></span>|<span data-ttu-id="b394a-128">boolean</span><span class="sxs-lookup"><span data-stu-id="b394a-128">boolean</span></span>|<span data-ttu-id="b394a-129">表示数据标签气泡大小是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="b394a-129">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="b394a-130">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="b394a-130">showCategoryName</span></span>|<span data-ttu-id="b394a-131">boolean</span><span class="sxs-lookup"><span data-stu-id="b394a-131">boolean</span></span>|<span data-ttu-id="b394a-132">表示数据标签类别名称是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="b394a-132">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="b394a-133">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="b394a-133">showLegendKey</span></span>|<span data-ttu-id="b394a-134">boolean</span><span class="sxs-lookup"><span data-stu-id="b394a-134">boolean</span></span>|<span data-ttu-id="b394a-135">表示数据标签图例标示是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="b394a-135">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="b394a-136">showPercentage</span><span class="sxs-lookup"><span data-stu-id="b394a-136">showPercentage</span></span>|<span data-ttu-id="b394a-137">boolean</span><span class="sxs-lookup"><span data-stu-id="b394a-137">boolean</span></span>|<span data-ttu-id="b394a-138">表示数据标签百分比是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="b394a-138">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="b394a-139">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="b394a-139">showSeriesName</span></span>|<span data-ttu-id="b394a-140">boolean</span><span class="sxs-lookup"><span data-stu-id="b394a-140">boolean</span></span>|<span data-ttu-id="b394a-141">表示数据标签系列名称是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="b394a-141">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="b394a-142">showValue</span><span class="sxs-lookup"><span data-stu-id="b394a-142">showValue</span></span>|<span data-ttu-id="b394a-143">布尔</span><span class="sxs-lookup"><span data-stu-id="b394a-143">boolean</span></span>|<span data-ttu-id="b394a-144">表示数据标签值是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="b394a-144">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b394a-145">关系</span><span class="sxs-lookup"><span data-stu-id="b394a-145">Relationships</span></span>
| <span data-ttu-id="b394a-146">关系</span><span class="sxs-lookup"><span data-stu-id="b394a-146">Relationship</span></span> | <span data-ttu-id="b394a-147">类型</span><span class="sxs-lookup"><span data-stu-id="b394a-147">Type</span></span>   |<span data-ttu-id="b394a-148">说明</span><span class="sxs-lookup"><span data-stu-id="b394a-148">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b394a-149">format</span><span class="sxs-lookup"><span data-stu-id="b394a-149">format</span></span>|[<span data-ttu-id="b394a-150">WorkbookChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="b394a-150">WorkbookChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="b394a-151">表示图表数据标签的格式，包括填充和字体格式。</span><span class="sxs-lookup"><span data-stu-id="b394a-151">Represents the format of chart data labels, which includes fill and font formatting.</span></span> <span data-ttu-id="b394a-152">只读。</span><span class="sxs-lookup"><span data-stu-id="b394a-152">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b394a-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b394a-153">JSON representation</span></span>

<span data-ttu-id="b394a-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b394a-154">Here is a JSON representation of the resource.</span></span>

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
