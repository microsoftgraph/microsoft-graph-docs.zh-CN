---
title: ChartDataLabels 资源类型
description: 表示图表点上的所有数据标签的集合。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: bda2c1849f154435608f311671026e224b0c7e3c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543727"
---
# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="0acfe-103">ChartDataLabels 资源类型</span><span class="sxs-lookup"><span data-stu-id="0acfe-103">ChartDataLabels resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0acfe-104">表示图表点上的所有数据标签的集合。</span><span class="sxs-lookup"><span data-stu-id="0acfe-104">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="0acfe-105">方法</span><span class="sxs-lookup"><span data-stu-id="0acfe-105">Methods</span></span>

| <span data-ttu-id="0acfe-106">方法</span><span class="sxs-lookup"><span data-stu-id="0acfe-106">Method</span></span>           | <span data-ttu-id="0acfe-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="0acfe-107">Return Type</span></span>    |<span data-ttu-id="0acfe-108">说明</span><span class="sxs-lookup"><span data-stu-id="0acfe-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0acfe-109">获取 ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="0acfe-109">Get ChartDataLabels</span></span>](../api/chartdatalabels-get.md) | [<span data-ttu-id="0acfe-110">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="0acfe-110">ChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="0acfe-111">读取 chartDataLabels 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0acfe-111">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="0acfe-112">更新</span><span class="sxs-lookup"><span data-stu-id="0acfe-112">Update</span></span>](../api/chartdatalabels-update.md) | [<span data-ttu-id="0acfe-113">ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="0acfe-113">ChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="0acfe-114">更新 ChartDataLabels 对象</span><span class="sxs-lookup"><span data-stu-id="0acfe-114">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0acfe-115">属性</span><span class="sxs-lookup"><span data-stu-id="0acfe-115">Properties</span></span>
| <span data-ttu-id="0acfe-116">属性</span><span class="sxs-lookup"><span data-stu-id="0acfe-116">Property</span></span>     | <span data-ttu-id="0acfe-117">类型</span><span class="sxs-lookup"><span data-stu-id="0acfe-117">Type</span></span>   |<span data-ttu-id="0acfe-118">说明</span><span class="sxs-lookup"><span data-stu-id="0acfe-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0acfe-119">position</span><span class="sxs-lookup"><span data-stu-id="0acfe-119">position</span></span>|<span data-ttu-id="0acfe-120">字符串</span><span class="sxs-lookup"><span data-stu-id="0acfe-120">string</span></span>|<span data-ttu-id="0acfe-p101">表示数据标签位置的 DataLabelPosition 值。可能的值是：`None`、`Center`、`InsideEnd`、`InsideBase`、`OutsideEnd`、`Left`、`Right`、`Top`、`Bottom`、`BestFit`、`Callout`。</span><span class="sxs-lookup"><span data-stu-id="0acfe-p101">DataLabelPosition value that represents the position of the data label. Possible values are: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span></span>|
|<span data-ttu-id="0acfe-123">separator</span><span class="sxs-lookup"><span data-stu-id="0acfe-123">separator</span></span>|<span data-ttu-id="0acfe-124">string</span><span class="sxs-lookup"><span data-stu-id="0acfe-124">string</span></span>|<span data-ttu-id="0acfe-125">表示用于图表中数据标签的分隔符的字符串。</span><span class="sxs-lookup"><span data-stu-id="0acfe-125">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="0acfe-126">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="0acfe-126">showBubbleSize</span></span>|<span data-ttu-id="0acfe-127">布尔</span><span class="sxs-lookup"><span data-stu-id="0acfe-127">boolean</span></span>|<span data-ttu-id="0acfe-128">表示数据标签气泡大小是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="0acfe-128">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="0acfe-129">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="0acfe-129">showCategoryName</span></span>|<span data-ttu-id="0acfe-130">布尔</span><span class="sxs-lookup"><span data-stu-id="0acfe-130">boolean</span></span>|<span data-ttu-id="0acfe-131">表示数据标签类别名称是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="0acfe-131">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="0acfe-132">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="0acfe-132">showLegendKey</span></span>|<span data-ttu-id="0acfe-133">布尔</span><span class="sxs-lookup"><span data-stu-id="0acfe-133">boolean</span></span>|<span data-ttu-id="0acfe-134">表示数据标签图例标示是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="0acfe-134">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="0acfe-135">showPercentage</span><span class="sxs-lookup"><span data-stu-id="0acfe-135">showPercentage</span></span>|<span data-ttu-id="0acfe-136">布尔</span><span class="sxs-lookup"><span data-stu-id="0acfe-136">boolean</span></span>|<span data-ttu-id="0acfe-137">表示数据标签百分比是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="0acfe-137">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="0acfe-138">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="0acfe-138">showSeriesName</span></span>|<span data-ttu-id="0acfe-139">布尔</span><span class="sxs-lookup"><span data-stu-id="0acfe-139">boolean</span></span>|<span data-ttu-id="0acfe-140">表示数据标签系列名称是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="0acfe-140">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="0acfe-141">showValue</span><span class="sxs-lookup"><span data-stu-id="0acfe-141">showValue</span></span>|<span data-ttu-id="0acfe-142">布尔</span><span class="sxs-lookup"><span data-stu-id="0acfe-142">boolean</span></span>|<span data-ttu-id="0acfe-143">表示数据标签值是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="0acfe-143">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0acfe-144">关系</span><span class="sxs-lookup"><span data-stu-id="0acfe-144">Relationships</span></span>
| <span data-ttu-id="0acfe-145">关系</span><span class="sxs-lookup"><span data-stu-id="0acfe-145">Relationship</span></span> | <span data-ttu-id="0acfe-146">类型</span><span class="sxs-lookup"><span data-stu-id="0acfe-146">Type</span></span>   |<span data-ttu-id="0acfe-147">说明</span><span class="sxs-lookup"><span data-stu-id="0acfe-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0acfe-148">format</span><span class="sxs-lookup"><span data-stu-id="0acfe-148">format</span></span>|[<span data-ttu-id="0acfe-149">ChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="0acfe-149">ChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="0acfe-p102">表示图表数据标签的格式，包括填充和字体格式。只读。</span><span class="sxs-lookup"><span data-stu-id="0acfe-p102">Represents the format of chart data labels, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0acfe-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0acfe-152">JSON representation</span></span>

<span data-ttu-id="0acfe-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0acfe-153">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartDataLabels resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartdatalabels.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
