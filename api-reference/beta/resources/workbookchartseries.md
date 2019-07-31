---
title: workbookChartSeries 资源类型
description: 代表图表上的系列。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: c7f7c8108ac17e6705b8bf5f69b0e87f0dc96b31
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007247"
---
# <a name="workbookchartseries-resource-type"></a><span data-ttu-id="6003c-103">workbookChartSeries 资源类型</span><span class="sxs-lookup"><span data-stu-id="6003c-103">workbookChartSeries resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6003c-104">代表图表上的系列。</span><span class="sxs-lookup"><span data-stu-id="6003c-104">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="6003c-105">方法</span><span class="sxs-lookup"><span data-stu-id="6003c-105">Methods</span></span>

| <span data-ttu-id="6003c-106">方法</span><span class="sxs-lookup"><span data-stu-id="6003c-106">Method</span></span>           | <span data-ttu-id="6003c-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="6003c-107">Return Type</span></span>    |<span data-ttu-id="6003c-108">说明</span><span class="sxs-lookup"><span data-stu-id="6003c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6003c-109">获取 ChartSeries</span><span class="sxs-lookup"><span data-stu-id="6003c-109">Get ChartSeries</span></span>](../api/chartseries-get.md) | [<span data-ttu-id="6003c-110">workbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="6003c-110">workbookChartSeries</span></span>](workbookchartseries.md) |<span data-ttu-id="6003c-111">读取 chartSeries 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6003c-111">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="6003c-112">创建 ChartPoint</span><span class="sxs-lookup"><span data-stu-id="6003c-112">Create ChartPoint</span></span>](../api/chartseries-post-points.md) |[<span data-ttu-id="6003c-113">chartPoints</span><span class="sxs-lookup"><span data-stu-id="6003c-113">chartPoints</span></span>](workbookchartpoint.md)| <span data-ttu-id="6003c-114">通过发布到点集合创建新的 chartPoint。</span><span class="sxs-lookup"><span data-stu-id="6003c-114">Create a new chartPoint by posting to the points collection.</span></span>|
|[<span data-ttu-id="6003c-115">列出 points</span><span class="sxs-lookup"><span data-stu-id="6003c-115">List points</span></span>](../api/chartseries-list-points.md) |<span data-ttu-id="6003c-116">[workbookChartPoints](workbookchartpoint.md)集合</span><span class="sxs-lookup"><span data-stu-id="6003c-116">[workbookChartPoints](workbookchartpoint.md) collection</span></span>| <span data-ttu-id="6003c-117">获取 chartPoints 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6003c-117">Get a chartPoints object collection.</span></span>|
|[<span data-ttu-id="6003c-118">更新</span><span class="sxs-lookup"><span data-stu-id="6003c-118">Update</span></span>](../api/chartseries-update.md) | [<span data-ttu-id="6003c-119">workbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="6003c-119">workbookChartSeries</span></span>](workbookchartseries.md) |<span data-ttu-id="6003c-120">更新 chartSeries 对象。</span><span class="sxs-lookup"><span data-stu-id="6003c-120">Update chartSeries object.</span></span> |
|[<span data-ttu-id="6003c-121">List</span><span class="sxs-lookup"><span data-stu-id="6003c-121">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="6003c-122">[workbookChartSeries](workbookchartseries.md)集合</span><span class="sxs-lookup"><span data-stu-id="6003c-122">[workbookChartSeries](workbookchartseries.md) collection</span></span> |<span data-ttu-id="6003c-123">获取 chartSeries 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6003c-123">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="6003c-124">ItemAt</span><span class="sxs-lookup"><span data-stu-id="6003c-124">ItemAt</span></span>](../api/chartseriescollection-itemat.md)|[<span data-ttu-id="6003c-125">workbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="6003c-125">workbookChartSeries</span></span>](workbookchartseries.md)|<span data-ttu-id="6003c-126">根据其在集合中的位置检索系列</span><span class="sxs-lookup"><span data-stu-id="6003c-126">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="6003c-127">属性</span><span class="sxs-lookup"><span data-stu-id="6003c-127">Properties</span></span>
| <span data-ttu-id="6003c-128">属性</span><span class="sxs-lookup"><span data-stu-id="6003c-128">Property</span></span>     | <span data-ttu-id="6003c-129">类型</span><span class="sxs-lookup"><span data-stu-id="6003c-129">Type</span></span>   |<span data-ttu-id="6003c-130">说明</span><span class="sxs-lookup"><span data-stu-id="6003c-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6003c-131">name</span><span class="sxs-lookup"><span data-stu-id="6003c-131">name</span></span>|<span data-ttu-id="6003c-132">string</span><span class="sxs-lookup"><span data-stu-id="6003c-132">string</span></span>|<span data-ttu-id="6003c-133">表示图表中某个系列的名称。</span><span class="sxs-lookup"><span data-stu-id="6003c-133">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6003c-134">关系</span><span class="sxs-lookup"><span data-stu-id="6003c-134">Relationships</span></span>
| <span data-ttu-id="6003c-135">关系</span><span class="sxs-lookup"><span data-stu-id="6003c-135">Relationship</span></span> | <span data-ttu-id="6003c-136">类型</span><span class="sxs-lookup"><span data-stu-id="6003c-136">Type</span></span>   |<span data-ttu-id="6003c-137">说明</span><span class="sxs-lookup"><span data-stu-id="6003c-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6003c-138">format</span><span class="sxs-lookup"><span data-stu-id="6003c-138">format</span></span>|[<span data-ttu-id="6003c-139">workbookChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="6003c-139">workbookChartSeriesFormat</span></span>](workbookchartseriesformat.md)|<span data-ttu-id="6003c-p101">表示图表系列的格式，包括填充和线条格式。只读。</span><span class="sxs-lookup"><span data-stu-id="6003c-p101">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="6003c-142">points</span><span class="sxs-lookup"><span data-stu-id="6003c-142">points</span></span>|<span data-ttu-id="6003c-143">[workbookChartPoint](workbookchartpoint.md)集合</span><span class="sxs-lookup"><span data-stu-id="6003c-143">[workbookChartPoint](workbookchartpoint.md) collection</span></span>|<span data-ttu-id="6003c-144">表示系列中所有数据点的集合。</span><span class="sxs-lookup"><span data-stu-id="6003c-144">Represents a collection of all points in the series.</span></span> <span data-ttu-id="6003c-145">只读。</span><span class="sxs-lookup"><span data-stu-id="6003c-145">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6003c-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6003c-146">JSON representation</span></span>

<span data-ttu-id="6003c-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6003c-147">Here is a JSON representation of the resource.</span></span>

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
