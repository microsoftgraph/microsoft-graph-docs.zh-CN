---
title: workbookChartSeries 资源类型
description: 代表图表上的系列。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e9ff478a5f7e91c3d116ca2dbd78e20699077aab
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348597"
---
# <a name="workbookchartseries-resource-type"></a><span data-ttu-id="bf25f-103">workbookChartSeries 资源类型</span><span class="sxs-lookup"><span data-stu-id="bf25f-103">workbookChartSeries resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf25f-104">代表图表上的系列。</span><span class="sxs-lookup"><span data-stu-id="bf25f-104">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="bf25f-105">方法</span><span class="sxs-lookup"><span data-stu-id="bf25f-105">Methods</span></span>

| <span data-ttu-id="bf25f-106">方法</span><span class="sxs-lookup"><span data-stu-id="bf25f-106">Method</span></span>           | <span data-ttu-id="bf25f-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="bf25f-107">Return Type</span></span>    |<span data-ttu-id="bf25f-108">说明</span><span class="sxs-lookup"><span data-stu-id="bf25f-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bf25f-109">获取 ChartSeries</span><span class="sxs-lookup"><span data-stu-id="bf25f-109">Get ChartSeries</span></span>](../api/chartseries-get.md) | [<span data-ttu-id="bf25f-110">workbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="bf25f-110">workbookChartSeries</span></span>](workbookchartseries.md) |<span data-ttu-id="bf25f-111">读取 chartSeries 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bf25f-111">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="bf25f-112">创建 ChartPoint</span><span class="sxs-lookup"><span data-stu-id="bf25f-112">Create ChartPoint</span></span>](../api/chartseries-post-points.md) |[<span data-ttu-id="bf25f-113">chartPoints</span><span class="sxs-lookup"><span data-stu-id="bf25f-113">chartPoints</span></span>](workbookchartpoint.md)| <span data-ttu-id="bf25f-114">通过发布到点集合创建新的 chartPoint。</span><span class="sxs-lookup"><span data-stu-id="bf25f-114">Create a new chartPoint by posting to the points collection.</span></span>|
|[<span data-ttu-id="bf25f-115">列出 points</span><span class="sxs-lookup"><span data-stu-id="bf25f-115">List points</span></span>](../api/chartseries-list-points.md) |<span data-ttu-id="bf25f-116">[workbookChartPoints](workbookchartpoint.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf25f-116">[workbookChartPoints](workbookchartpoint.md) collection</span></span>| <span data-ttu-id="bf25f-117">获取 chartPoints 对象集合。</span><span class="sxs-lookup"><span data-stu-id="bf25f-117">Get a chartPoints object collection.</span></span>|
|[<span data-ttu-id="bf25f-118">更新</span><span class="sxs-lookup"><span data-stu-id="bf25f-118">Update</span></span>](../api/chartseries-update.md) | [<span data-ttu-id="bf25f-119">workbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="bf25f-119">workbookChartSeries</span></span>](workbookchartseries.md) |<span data-ttu-id="bf25f-120">更新 chartSeries 对象。</span><span class="sxs-lookup"><span data-stu-id="bf25f-120">Update chartSeries object.</span></span> |
|[<span data-ttu-id="bf25f-121">List</span><span class="sxs-lookup"><span data-stu-id="bf25f-121">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="bf25f-122">[workbookChartSeries](workbookchartseries.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf25f-122">[workbookChartSeries](workbookchartseries.md) collection</span></span> |<span data-ttu-id="bf25f-123">获取 chartSeries 对象集合。</span><span class="sxs-lookup"><span data-stu-id="bf25f-123">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="bf25f-124">ItemAt</span><span class="sxs-lookup"><span data-stu-id="bf25f-124">ItemAt</span></span>](../api/chartseriescollection-itemat.md)|[<span data-ttu-id="bf25f-125">workbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="bf25f-125">workbookChartSeries</span></span>](workbookchartseries.md)|<span data-ttu-id="bf25f-126">根据其在集合中的位置检索系列</span><span class="sxs-lookup"><span data-stu-id="bf25f-126">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="bf25f-127">属性</span><span class="sxs-lookup"><span data-stu-id="bf25f-127">Properties</span></span>
| <span data-ttu-id="bf25f-128">属性</span><span class="sxs-lookup"><span data-stu-id="bf25f-128">Property</span></span>     | <span data-ttu-id="bf25f-129">类型</span><span class="sxs-lookup"><span data-stu-id="bf25f-129">Type</span></span>   |<span data-ttu-id="bf25f-130">说明</span><span class="sxs-lookup"><span data-stu-id="bf25f-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf25f-131">name</span><span class="sxs-lookup"><span data-stu-id="bf25f-131">name</span></span>|<span data-ttu-id="bf25f-132">string</span><span class="sxs-lookup"><span data-stu-id="bf25f-132">string</span></span>|<span data-ttu-id="bf25f-133">表示图表中某个系列的名称。</span><span class="sxs-lookup"><span data-stu-id="bf25f-133">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf25f-134">关系</span><span class="sxs-lookup"><span data-stu-id="bf25f-134">Relationships</span></span>
| <span data-ttu-id="bf25f-135">关系</span><span class="sxs-lookup"><span data-stu-id="bf25f-135">Relationship</span></span> | <span data-ttu-id="bf25f-136">类型</span><span class="sxs-lookup"><span data-stu-id="bf25f-136">Type</span></span>   |<span data-ttu-id="bf25f-137">说明</span><span class="sxs-lookup"><span data-stu-id="bf25f-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf25f-138">format</span><span class="sxs-lookup"><span data-stu-id="bf25f-138">format</span></span>|[<span data-ttu-id="bf25f-139">workbookChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="bf25f-139">workbookChartSeriesFormat</span></span>](workbookchartseriesformat.md)|<span data-ttu-id="bf25f-p101">表示图表系列的格式，包括填充和线条格式。只读。</span><span class="sxs-lookup"><span data-stu-id="bf25f-p101">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="bf25f-142">points</span><span class="sxs-lookup"><span data-stu-id="bf25f-142">points</span></span>|<span data-ttu-id="bf25f-143">[workbookChartPoint](workbookchartpoint.md)集合</span><span class="sxs-lookup"><span data-stu-id="bf25f-143">[workbookChartPoint](workbookchartpoint.md) collection</span></span>|<span data-ttu-id="bf25f-144">表示系列中所有数据点的集合。</span><span class="sxs-lookup"><span data-stu-id="bf25f-144">Represents a collection of all points in the series.</span></span> <span data-ttu-id="bf25f-145">只读。</span><span class="sxs-lookup"><span data-stu-id="bf25f-145">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bf25f-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bf25f-146">JSON representation</span></span>

<span data-ttu-id="bf25f-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bf25f-147">Here is a JSON representation of the resource.</span></span>

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
