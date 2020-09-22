---
title: workbookChartSeries 资源类型
description: 代表图表上的系列。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 22ce2138da7ae8163304978370ada1f71abe7026
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979229"
---
# <a name="workbookchartseries-resource-type"></a><span data-ttu-id="c93be-103">workbookChartSeries 资源类型</span><span class="sxs-lookup"><span data-stu-id="c93be-103">workbookChartSeries resource type</span></span>

<span data-ttu-id="c93be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c93be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c93be-105">代表图表上的系列。</span><span class="sxs-lookup"><span data-stu-id="c93be-105">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="c93be-106">方法</span><span class="sxs-lookup"><span data-stu-id="c93be-106">Methods</span></span>

| <span data-ttu-id="c93be-107">方法</span><span class="sxs-lookup"><span data-stu-id="c93be-107">Method</span></span>           | <span data-ttu-id="c93be-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="c93be-108">Return Type</span></span>    |<span data-ttu-id="c93be-109">说明</span><span class="sxs-lookup"><span data-stu-id="c93be-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c93be-110">获取 ChartSeries</span><span class="sxs-lookup"><span data-stu-id="c93be-110">Get ChartSeries</span></span>](../api/chartseries-get.md) | [<span data-ttu-id="c93be-111">workbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="c93be-111">workbookChartSeries</span></span>](workbookchartseries.md) |<span data-ttu-id="c93be-112">读取 chartSeries 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c93be-112">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="c93be-113">创建 ChartPoint</span><span class="sxs-lookup"><span data-stu-id="c93be-113">Create ChartPoint</span></span>](../api/chartseries-post-points.md) |[<span data-ttu-id="c93be-114">chartPoints</span><span class="sxs-lookup"><span data-stu-id="c93be-114">chartPoints</span></span>](workbookchartpoint.md)| <span data-ttu-id="c93be-115">通过发布到点集合创建新的 chartPoint。</span><span class="sxs-lookup"><span data-stu-id="c93be-115">Create a new chartPoint by posting to the points collection.</span></span>|
|[<span data-ttu-id="c93be-116">列出 points</span><span class="sxs-lookup"><span data-stu-id="c93be-116">List points</span></span>](../api/chartseries-list-points.md) |<span data-ttu-id="c93be-117">[workbookChartPoints](workbookchartpoint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c93be-117">[workbookChartPoints](workbookchartpoint.md) collection</span></span>| <span data-ttu-id="c93be-118">获取 chartPoints 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c93be-118">Get a chartPoints object collection.</span></span>|
|[<span data-ttu-id="c93be-119">更新</span><span class="sxs-lookup"><span data-stu-id="c93be-119">Update</span></span>](../api/chartseries-update.md) | [<span data-ttu-id="c93be-120">workbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="c93be-120">workbookChartSeries</span></span>](workbookchartseries.md) |<span data-ttu-id="c93be-121">更新 chartSeries 对象。</span><span class="sxs-lookup"><span data-stu-id="c93be-121">Update chartSeries object.</span></span> |
|[<span data-ttu-id="c93be-122">List</span><span class="sxs-lookup"><span data-stu-id="c93be-122">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="c93be-123">[workbookChartSeries](workbookchartseries.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c93be-123">[workbookChartSeries](workbookchartseries.md) collection</span></span> |<span data-ttu-id="c93be-124">获取 chartSeries 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c93be-124">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="c93be-125">ItemAt</span><span class="sxs-lookup"><span data-stu-id="c93be-125">ItemAt</span></span>](../api/chartseriescollection-itemat.md)|[<span data-ttu-id="c93be-126">workbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="c93be-126">workbookChartSeries</span></span>](workbookchartseries.md)|<span data-ttu-id="c93be-127">根据其在集合中的位置检索系列</span><span class="sxs-lookup"><span data-stu-id="c93be-127">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="c93be-128">属性</span><span class="sxs-lookup"><span data-stu-id="c93be-128">Properties</span></span>
| <span data-ttu-id="c93be-129">属性</span><span class="sxs-lookup"><span data-stu-id="c93be-129">Property</span></span>     | <span data-ttu-id="c93be-130">类型</span><span class="sxs-lookup"><span data-stu-id="c93be-130">Type</span></span>   |<span data-ttu-id="c93be-131">说明</span><span class="sxs-lookup"><span data-stu-id="c93be-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c93be-132">name</span><span class="sxs-lookup"><span data-stu-id="c93be-132">name</span></span>|<span data-ttu-id="c93be-133">string</span><span class="sxs-lookup"><span data-stu-id="c93be-133">string</span></span>|<span data-ttu-id="c93be-134">表示图表中某个系列的名称。</span><span class="sxs-lookup"><span data-stu-id="c93be-134">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c93be-135">关系</span><span class="sxs-lookup"><span data-stu-id="c93be-135">Relationships</span></span>
| <span data-ttu-id="c93be-136">关系</span><span class="sxs-lookup"><span data-stu-id="c93be-136">Relationship</span></span> | <span data-ttu-id="c93be-137">类型</span><span class="sxs-lookup"><span data-stu-id="c93be-137">Type</span></span>   |<span data-ttu-id="c93be-138">说明</span><span class="sxs-lookup"><span data-stu-id="c93be-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c93be-139">format</span><span class="sxs-lookup"><span data-stu-id="c93be-139">format</span></span>|[<span data-ttu-id="c93be-140">workbookChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="c93be-140">workbookChartSeriesFormat</span></span>](workbookchartseriesformat.md)|<span data-ttu-id="c93be-p101">表示图表系列的格式，包括填充和线条格式。只读。</span><span class="sxs-lookup"><span data-stu-id="c93be-p101">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="c93be-143">points</span><span class="sxs-lookup"><span data-stu-id="c93be-143">points</span></span>|<span data-ttu-id="c93be-144">[workbookChartPoint](workbookchartpoint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c93be-144">[workbookChartPoint](workbookchartpoint.md) collection</span></span>|<span data-ttu-id="c93be-145">表示系列中所有数据点的集合。</span><span class="sxs-lookup"><span data-stu-id="c93be-145">Represents a collection of all points in the series.</span></span> <span data-ttu-id="c93be-146">只读。</span><span class="sxs-lookup"><span data-stu-id="c93be-146">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c93be-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c93be-147">JSON representation</span></span>

<span data-ttu-id="c93be-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c93be-148">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartSeries resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


