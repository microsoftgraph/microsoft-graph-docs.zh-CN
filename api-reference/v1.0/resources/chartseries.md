---
title: ChartSeries 资源类型
description: 代表图表上的系列。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: f7d42633321c78eb03942072731b0636a8ca73b7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531824"
---
# <a name="chartseries-resource-type"></a><span data-ttu-id="a2bdb-103">ChartSeries 资源类型</span><span class="sxs-lookup"><span data-stu-id="a2bdb-103">ChartSeries resource type</span></span>

<span data-ttu-id="a2bdb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2bdb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a2bdb-105">代表图表上的系列。</span><span class="sxs-lookup"><span data-stu-id="a2bdb-105">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="a2bdb-106">Methods</span><span class="sxs-lookup"><span data-stu-id="a2bdb-106">Methods</span></span>

| <span data-ttu-id="a2bdb-107">方法</span><span class="sxs-lookup"><span data-stu-id="a2bdb-107">Method</span></span>           | <span data-ttu-id="a2bdb-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="a2bdb-108">Return Type</span></span>    |<span data-ttu-id="a2bdb-109">说明</span><span class="sxs-lookup"><span data-stu-id="a2bdb-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a2bdb-110">获取 ChartSeries</span><span class="sxs-lookup"><span data-stu-id="a2bdb-110">Get ChartSeries</span></span>](../api/chartseries-get.md) | [<span data-ttu-id="a2bdb-111">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="a2bdb-111">WorkbookChartSeries</span></span>](chartseries.md) |<span data-ttu-id="a2bdb-112">读取 chartSeries 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a2bdb-112">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="a2bdb-113">创建 ChartPoints</span><span class="sxs-lookup"><span data-stu-id="a2bdb-113">Create ChartPoints</span></span>](../api/chartseries-post-points.md) |[<span data-ttu-id="a2bdb-114">ChartPoints</span><span class="sxs-lookup"><span data-stu-id="a2bdb-114">ChartPoints</span></span>](chartpoint.md)| <span data-ttu-id="a2bdb-115">通过发布到点集合创建新的 ChartPoints。</span><span class="sxs-lookup"><span data-stu-id="a2bdb-115">Create a new ChartPoints by posting to the points collection.</span></span>|
|[<span data-ttu-id="a2bdb-116">列出 points</span><span class="sxs-lookup"><span data-stu-id="a2bdb-116">List points</span></span>](../api/chartseries-list-points.md) |<span data-ttu-id="a2bdb-117">[ChartPoints](chartpoint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a2bdb-117">[ChartPoints](chartpoint.md) collection</span></span>| <span data-ttu-id="a2bdb-118">获取 ChartPoints 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a2bdb-118">Get a ChartPoints object collection.</span></span>|
|[<span data-ttu-id="a2bdb-119">更新</span><span class="sxs-lookup"><span data-stu-id="a2bdb-119">Update</span></span>](../api/chartseries-update.md) | [<span data-ttu-id="a2bdb-120">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="a2bdb-120">WorkbookChartSeries</span></span>](chartseries.md) |<span data-ttu-id="a2bdb-121">更新 ChartSeries 对象。</span><span class="sxs-lookup"><span data-stu-id="a2bdb-121">Update ChartSeries object.</span></span> |
|[<span data-ttu-id="a2bdb-122">列出</span><span class="sxs-lookup"><span data-stu-id="a2bdb-122">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="a2bdb-123">[WorkbookChartSeries](chartseries.md)集合</span><span class="sxs-lookup"><span data-stu-id="a2bdb-123">[WorkbookChartSeries](chartseries.md) collection</span></span> |<span data-ttu-id="a2bdb-124">获取 chartSeries 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a2bdb-124">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="a2bdb-125">ItemAt</span><span class="sxs-lookup"><span data-stu-id="a2bdb-125">ItemAt</span></span>](../api/chartseriescollection-itemat.md)|[<span data-ttu-id="a2bdb-126">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="a2bdb-126">WorkbookChartSeries</span></span>](chartseries.md)|<span data-ttu-id="a2bdb-127">根据其在集合中的位置检索系列</span><span class="sxs-lookup"><span data-stu-id="a2bdb-127">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="a2bdb-128">属性</span><span class="sxs-lookup"><span data-stu-id="a2bdb-128">Properties</span></span>
| <span data-ttu-id="a2bdb-129">属性</span><span class="sxs-lookup"><span data-stu-id="a2bdb-129">Property</span></span>     | <span data-ttu-id="a2bdb-130">类型</span><span class="sxs-lookup"><span data-stu-id="a2bdb-130">Type</span></span>   |<span data-ttu-id="a2bdb-131">说明</span><span class="sxs-lookup"><span data-stu-id="a2bdb-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2bdb-132">name</span><span class="sxs-lookup"><span data-stu-id="a2bdb-132">name</span></span>|<span data-ttu-id="a2bdb-133">string</span><span class="sxs-lookup"><span data-stu-id="a2bdb-133">string</span></span>|<span data-ttu-id="a2bdb-134">表示图表中某个系列的名称。</span><span class="sxs-lookup"><span data-stu-id="a2bdb-134">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2bdb-135">关系</span><span class="sxs-lookup"><span data-stu-id="a2bdb-135">Relationships</span></span>
| <span data-ttu-id="a2bdb-136">关系</span><span class="sxs-lookup"><span data-stu-id="a2bdb-136">Relationship</span></span> | <span data-ttu-id="a2bdb-137">类型</span><span class="sxs-lookup"><span data-stu-id="a2bdb-137">Type</span></span>   |<span data-ttu-id="a2bdb-138">说明</span><span class="sxs-lookup"><span data-stu-id="a2bdb-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2bdb-139">format</span><span class="sxs-lookup"><span data-stu-id="a2bdb-139">format</span></span>|[<span data-ttu-id="a2bdb-140">WorkbookChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="a2bdb-140">WorkbookChartSeriesFormat</span></span>](chartseriesformat.md)|<span data-ttu-id="a2bdb-p101">表示图表系列的格式，包括填充和线条格式。只读。</span><span class="sxs-lookup"><span data-stu-id="a2bdb-p101">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="a2bdb-143">points</span><span class="sxs-lookup"><span data-stu-id="a2bdb-143">points</span></span>|<span data-ttu-id="a2bdb-144">[WorkbookChartPoint](chartpoint.md)集合</span><span class="sxs-lookup"><span data-stu-id="a2bdb-144">[WorkbookChartPoint](chartpoint.md) collection</span></span>|<span data-ttu-id="a2bdb-145">表示系列中所有数据点的集合。</span><span class="sxs-lookup"><span data-stu-id="a2bdb-145">Represents a collection of all points in the series.</span></span> <span data-ttu-id="a2bdb-146">只读。</span><span class="sxs-lookup"><span data-stu-id="a2bdb-146">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a2bdb-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a2bdb-147">JSON representation</span></span>

<span data-ttu-id="a2bdb-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2bdb-148">Here is a JSON representation of the resource.</span></span>

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
