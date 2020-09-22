---
title: ChartSeries 资源类型
description: 代表图表上的系列。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 173f9878daecd3443137800f143a2b3633a2fa20
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988371"
---
# <a name="chartseries-resource-type"></a><span data-ttu-id="77dd8-103">ChartSeries 资源类型</span><span class="sxs-lookup"><span data-stu-id="77dd8-103">ChartSeries resource type</span></span>

<span data-ttu-id="77dd8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77dd8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="77dd8-105">代表图表上的系列。</span><span class="sxs-lookup"><span data-stu-id="77dd8-105">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="77dd8-106">方法</span><span class="sxs-lookup"><span data-stu-id="77dd8-106">Methods</span></span>

| <span data-ttu-id="77dd8-107">方法</span><span class="sxs-lookup"><span data-stu-id="77dd8-107">Method</span></span>           | <span data-ttu-id="77dd8-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="77dd8-108">Return Type</span></span>    |<span data-ttu-id="77dd8-109">说明</span><span class="sxs-lookup"><span data-stu-id="77dd8-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="77dd8-110">获取 ChartSeries</span><span class="sxs-lookup"><span data-stu-id="77dd8-110">Get ChartSeries</span></span>](../api/chartseries-get.md) | [<span data-ttu-id="77dd8-111">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="77dd8-111">WorkbookChartSeries</span></span>](chartseries.md) |<span data-ttu-id="77dd8-112">读取 chartSeries 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="77dd8-112">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="77dd8-113">创建 ChartPoints</span><span class="sxs-lookup"><span data-stu-id="77dd8-113">Create ChartPoints</span></span>](../api/chartseries-post-points.md) |[<span data-ttu-id="77dd8-114">ChartPoints</span><span class="sxs-lookup"><span data-stu-id="77dd8-114">ChartPoints</span></span>](chartpoint.md)| <span data-ttu-id="77dd8-115">通过发布到点集合创建新的 ChartPoints。</span><span class="sxs-lookup"><span data-stu-id="77dd8-115">Create a new ChartPoints by posting to the points collection.</span></span>|
|[<span data-ttu-id="77dd8-116">列出 points</span><span class="sxs-lookup"><span data-stu-id="77dd8-116">List points</span></span>](../api/chartseries-list-points.md) |<span data-ttu-id="77dd8-117">[ChartPoints](chartpoint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="77dd8-117">[ChartPoints](chartpoint.md) collection</span></span>| <span data-ttu-id="77dd8-118">获取 ChartPoints 对象集合。</span><span class="sxs-lookup"><span data-stu-id="77dd8-118">Get a ChartPoints object collection.</span></span>|
|[<span data-ttu-id="77dd8-119">更新</span><span class="sxs-lookup"><span data-stu-id="77dd8-119">Update</span></span>](../api/chartseries-update.md) | [<span data-ttu-id="77dd8-120">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="77dd8-120">WorkbookChartSeries</span></span>](chartseries.md) |<span data-ttu-id="77dd8-121">更新 ChartSeries 对象。</span><span class="sxs-lookup"><span data-stu-id="77dd8-121">Update ChartSeries object.</span></span> |
|[<span data-ttu-id="77dd8-122">列出</span><span class="sxs-lookup"><span data-stu-id="77dd8-122">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="77dd8-123">[WorkbookChartSeries](chartseries.md) 集合</span><span class="sxs-lookup"><span data-stu-id="77dd8-123">[WorkbookChartSeries](chartseries.md) collection</span></span> |<span data-ttu-id="77dd8-124">获取 chartSeries 对象集合。</span><span class="sxs-lookup"><span data-stu-id="77dd8-124">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="77dd8-125">ItemAt</span><span class="sxs-lookup"><span data-stu-id="77dd8-125">ItemAt</span></span>](../api/chartseriescollection-itemat.md)|[<span data-ttu-id="77dd8-126">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="77dd8-126">WorkbookChartSeries</span></span>](chartseries.md)|<span data-ttu-id="77dd8-127">根据其在集合中的位置检索系列</span><span class="sxs-lookup"><span data-stu-id="77dd8-127">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="77dd8-128">属性</span><span class="sxs-lookup"><span data-stu-id="77dd8-128">Properties</span></span>
| <span data-ttu-id="77dd8-129">属性</span><span class="sxs-lookup"><span data-stu-id="77dd8-129">Property</span></span>     | <span data-ttu-id="77dd8-130">类型</span><span class="sxs-lookup"><span data-stu-id="77dd8-130">Type</span></span>   |<span data-ttu-id="77dd8-131">说明</span><span class="sxs-lookup"><span data-stu-id="77dd8-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77dd8-132">name</span><span class="sxs-lookup"><span data-stu-id="77dd8-132">name</span></span>|<span data-ttu-id="77dd8-133">string</span><span class="sxs-lookup"><span data-stu-id="77dd8-133">string</span></span>|<span data-ttu-id="77dd8-134">表示图表中某个系列的名称。</span><span class="sxs-lookup"><span data-stu-id="77dd8-134">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="77dd8-135">关系</span><span class="sxs-lookup"><span data-stu-id="77dd8-135">Relationships</span></span>
| <span data-ttu-id="77dd8-136">关系</span><span class="sxs-lookup"><span data-stu-id="77dd8-136">Relationship</span></span> | <span data-ttu-id="77dd8-137">类型</span><span class="sxs-lookup"><span data-stu-id="77dd8-137">Type</span></span>   |<span data-ttu-id="77dd8-138">说明</span><span class="sxs-lookup"><span data-stu-id="77dd8-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77dd8-139">format</span><span class="sxs-lookup"><span data-stu-id="77dd8-139">format</span></span>|[<span data-ttu-id="77dd8-140">WorkbookChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="77dd8-140">WorkbookChartSeriesFormat</span></span>](chartseriesformat.md)|<span data-ttu-id="77dd8-p101">表示图表系列的格式，包括填充和线条格式。只读。</span><span class="sxs-lookup"><span data-stu-id="77dd8-p101">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="77dd8-143">points</span><span class="sxs-lookup"><span data-stu-id="77dd8-143">points</span></span>|<span data-ttu-id="77dd8-144">[WorkbookChartPoint](chartpoint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="77dd8-144">[WorkbookChartPoint](chartpoint.md) collection</span></span>|<span data-ttu-id="77dd8-145">表示系列中所有数据点的集合。</span><span class="sxs-lookup"><span data-stu-id="77dd8-145">Represents a collection of all points in the series.</span></span> <span data-ttu-id="77dd8-146">只读。</span><span class="sxs-lookup"><span data-stu-id="77dd8-146">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="77dd8-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="77dd8-147">JSON representation</span></span>

<span data-ttu-id="77dd8-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="77dd8-148">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartSeries"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeries resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

