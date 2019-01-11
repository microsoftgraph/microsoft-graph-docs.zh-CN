---
title: ChartSeries 资源类型
description: 代表图表上的系列。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: a3a19793629a5e100830565e224541930e2180de
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834893"
---
# <a name="chartseries-resource-type"></a><span data-ttu-id="f62bb-103">ChartSeries 资源类型</span><span class="sxs-lookup"><span data-stu-id="f62bb-103">ChartSeries resource type</span></span>

<span data-ttu-id="f62bb-104">代表图表上的系列。</span><span class="sxs-lookup"><span data-stu-id="f62bb-104">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="f62bb-105">方法</span><span class="sxs-lookup"><span data-stu-id="f62bb-105">Methods</span></span>

| <span data-ttu-id="f62bb-106">方法</span><span class="sxs-lookup"><span data-stu-id="f62bb-106">Method</span></span>           | <span data-ttu-id="f62bb-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="f62bb-107">Return Type</span></span>    |<span data-ttu-id="f62bb-108">说明</span><span class="sxs-lookup"><span data-stu-id="f62bb-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f62bb-109">获取 ChartSeries</span><span class="sxs-lookup"><span data-stu-id="f62bb-109">Get ChartSeries</span></span>](../api/chartseries-get.md) | [<span data-ttu-id="f62bb-110">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="f62bb-110">WorkbookChartSeries</span></span>](chartseries.md) |<span data-ttu-id="f62bb-111">读取 chartSeries 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f62bb-111">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="f62bb-112">创建 ChartPoints</span><span class="sxs-lookup"><span data-stu-id="f62bb-112">Create ChartPoints</span></span>](../api/chartseries-post-points.md) |[<span data-ttu-id="f62bb-113">ChartPoints</span><span class="sxs-lookup"><span data-stu-id="f62bb-113">ChartPoints</span></span>](chartpoint.md)| <span data-ttu-id="f62bb-114">通过发布到点集合创建新的 ChartPoints。</span><span class="sxs-lookup"><span data-stu-id="f62bb-114">Create a new ChartPoints by posting to the points collection.</span></span>|
|[<span data-ttu-id="f62bb-115">列出 points</span><span class="sxs-lookup"><span data-stu-id="f62bb-115">List points</span></span>](../api/chartseries-list-points.md) |<span data-ttu-id="f62bb-116">[ChartPoints](chartpoint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f62bb-116">[ChartPoints](chartpoint.md) collection</span></span>| <span data-ttu-id="f62bb-117">获取 ChartPoints 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f62bb-117">Get a ChartPoints object collection.</span></span>|
|[<span data-ttu-id="f62bb-118">Update</span><span class="sxs-lookup"><span data-stu-id="f62bb-118">Update</span></span>](../api/chartseries-update.md) | [<span data-ttu-id="f62bb-119">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="f62bb-119">WorkbookChartSeries</span></span>](chartseries.md) |<span data-ttu-id="f62bb-120">更新 ChartSeries 对象。</span><span class="sxs-lookup"><span data-stu-id="f62bb-120">Update ChartSeries object.</span></span> |
|[<span data-ttu-id="f62bb-121">List</span><span class="sxs-lookup"><span data-stu-id="f62bb-121">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="f62bb-122">[WorkbookChartSeries](chartseries.md)集合</span><span class="sxs-lookup"><span data-stu-id="f62bb-122">[WorkbookChartSeries](chartseries.md) collection</span></span> |<span data-ttu-id="f62bb-123">获取 chartSeries 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f62bb-123">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="f62bb-124">ItemAt</span><span class="sxs-lookup"><span data-stu-id="f62bb-124">ItemAt</span></span>](../api/chartseriescollection-itemat.md)|[<span data-ttu-id="f62bb-125">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="f62bb-125">WorkbookChartSeries</span></span>](chartseries.md)|<span data-ttu-id="f62bb-126">根据其在集合中的位置检索系列</span><span class="sxs-lookup"><span data-stu-id="f62bb-126">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="f62bb-127">属性</span><span class="sxs-lookup"><span data-stu-id="f62bb-127">Properties</span></span>
| <span data-ttu-id="f62bb-128">属性</span><span class="sxs-lookup"><span data-stu-id="f62bb-128">Property</span></span>     | <span data-ttu-id="f62bb-129">类型</span><span class="sxs-lookup"><span data-stu-id="f62bb-129">Type</span></span>   |<span data-ttu-id="f62bb-130">说明</span><span class="sxs-lookup"><span data-stu-id="f62bb-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f62bb-131">name</span><span class="sxs-lookup"><span data-stu-id="f62bb-131">name</span></span>|<span data-ttu-id="f62bb-132">string</span><span class="sxs-lookup"><span data-stu-id="f62bb-132">string</span></span>|<span data-ttu-id="f62bb-133">表示图表中某个系列的名称。</span><span class="sxs-lookup"><span data-stu-id="f62bb-133">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f62bb-134">Relationships</span><span class="sxs-lookup"><span data-stu-id="f62bb-134">Relationships</span></span>
| <span data-ttu-id="f62bb-135">关系</span><span class="sxs-lookup"><span data-stu-id="f62bb-135">Relationship</span></span> | <span data-ttu-id="f62bb-136">类型</span><span class="sxs-lookup"><span data-stu-id="f62bb-136">Type</span></span>   |<span data-ttu-id="f62bb-137">说明</span><span class="sxs-lookup"><span data-stu-id="f62bb-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f62bb-138">format</span><span class="sxs-lookup"><span data-stu-id="f62bb-138">format</span></span>|[<span data-ttu-id="f62bb-139">WorkbookChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="f62bb-139">WorkbookChartSeriesFormat</span></span>](chartseriesformat.md)|<span data-ttu-id="f62bb-p101">表示图表系列的格式，包括填充和线条格式。只读。</span><span class="sxs-lookup"><span data-stu-id="f62bb-p101">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="f62bb-142">points</span><span class="sxs-lookup"><span data-stu-id="f62bb-142">points</span></span>|<span data-ttu-id="f62bb-143">[WorkbookChartPoint](chartpoint.md)集合</span><span class="sxs-lookup"><span data-stu-id="f62bb-143">[WorkbookChartPoint](chartpoint.md) collection</span></span>|<span data-ttu-id="f62bb-p102">表示系列中所有数据点的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="f62bb-p102">Represents a collection of all points in the series. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f62bb-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f62bb-146">JSON representation</span></span>

<span data-ttu-id="f62bb-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f62bb-147">Here is a JSON representation of the resource.</span></span>

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
