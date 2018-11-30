---
title: ChartSeries 资源类型
description: 代表图表上的系列。
ms.openlocfilehash: 301fd3ba3c299108836bbd92497f4d6f6af94b0a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049382"
---
# <a name="chartseries-resource-type"></a><span data-ttu-id="a30fc-103">ChartSeries 资源类型</span><span class="sxs-lookup"><span data-stu-id="a30fc-103">ChartSeries resource type</span></span>

> <span data-ttu-id="a30fc-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a30fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a30fc-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a30fc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a30fc-106">代表图表上的系列。</span><span class="sxs-lookup"><span data-stu-id="a30fc-106">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="a30fc-107">方法</span><span class="sxs-lookup"><span data-stu-id="a30fc-107">Methods</span></span>

| <span data-ttu-id="a30fc-108">方法</span><span class="sxs-lookup"><span data-stu-id="a30fc-108">Method</span></span>           | <span data-ttu-id="a30fc-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a30fc-109">Return Type</span></span>    |<span data-ttu-id="a30fc-110">说明</span><span class="sxs-lookup"><span data-stu-id="a30fc-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a30fc-111">获取 ChartSeries</span><span class="sxs-lookup"><span data-stu-id="a30fc-111">Get ChartSeries</span></span>](../api/chartseries-get.md) | [<span data-ttu-id="a30fc-112">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="a30fc-112">ChartSeries</span></span>](chartseries.md) |<span data-ttu-id="a30fc-113">读取 chartSeries 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a30fc-113">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="a30fc-114">创建 ChartPoints</span><span class="sxs-lookup"><span data-stu-id="a30fc-114">Create ChartPoints</span></span>](../api/chartseries-post-points.md) |[<span data-ttu-id="a30fc-115">ChartPoints</span><span class="sxs-lookup"><span data-stu-id="a30fc-115">ChartPoints</span></span>](chartpoint.md)| <span data-ttu-id="a30fc-116">通过发布到点集合创建新的 ChartPoints。</span><span class="sxs-lookup"><span data-stu-id="a30fc-116">Create a new ChartPoints by posting to the points collection.</span></span>|
|[<span data-ttu-id="a30fc-117">列出 points</span><span class="sxs-lookup"><span data-stu-id="a30fc-117">List points</span></span>](../api/chartseries-list-points.md) |<span data-ttu-id="a30fc-118">[ChartPoints](chartpoint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a30fc-118">[ChartPoints](chartpoint.md) collection</span></span>| <span data-ttu-id="a30fc-119">获取 ChartPoints 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a30fc-119">Get a ChartPoints object collection.</span></span>|
|[<span data-ttu-id="a30fc-120">Update</span><span class="sxs-lookup"><span data-stu-id="a30fc-120">Update</span></span>](../api/chartseries-update.md) | [<span data-ttu-id="a30fc-121">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="a30fc-121">ChartSeries</span></span>](chartseries.md) |<span data-ttu-id="a30fc-122">更新 ChartSeries 对象。</span><span class="sxs-lookup"><span data-stu-id="a30fc-122">Update ChartSeries object.</span></span> |
|[<span data-ttu-id="a30fc-123">List</span><span class="sxs-lookup"><span data-stu-id="a30fc-123">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="a30fc-124">[ChartSeries](chartseries.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a30fc-124">[ChartSeries](chartseries.md) collection</span></span> |<span data-ttu-id="a30fc-125">获取 chartSeries 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a30fc-125">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="a30fc-126">Itemat</span><span class="sxs-lookup"><span data-stu-id="a30fc-126">Itemat</span></span>](../api/chartseriescollection-itemat.md)|[<span data-ttu-id="a30fc-127">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="a30fc-127">ChartSeries</span></span>](chartseries.md)|<span data-ttu-id="a30fc-128">根据其在集合中的位置检索系列</span><span class="sxs-lookup"><span data-stu-id="a30fc-128">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="a30fc-129">属性</span><span class="sxs-lookup"><span data-stu-id="a30fc-129">Properties</span></span>
| <span data-ttu-id="a30fc-130">属性</span><span class="sxs-lookup"><span data-stu-id="a30fc-130">Property</span></span>     | <span data-ttu-id="a30fc-131">类型</span><span class="sxs-lookup"><span data-stu-id="a30fc-131">Type</span></span>   |<span data-ttu-id="a30fc-132">说明</span><span class="sxs-lookup"><span data-stu-id="a30fc-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a30fc-133">name</span><span class="sxs-lookup"><span data-stu-id="a30fc-133">name</span></span>|<span data-ttu-id="a30fc-134">string</span><span class="sxs-lookup"><span data-stu-id="a30fc-134">string</span></span>|<span data-ttu-id="a30fc-135">表示图表中某个系列的名称。</span><span class="sxs-lookup"><span data-stu-id="a30fc-135">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a30fc-136">Relationships</span><span class="sxs-lookup"><span data-stu-id="a30fc-136">Relationships</span></span>
| <span data-ttu-id="a30fc-137">关系</span><span class="sxs-lookup"><span data-stu-id="a30fc-137">Relationship</span></span> | <span data-ttu-id="a30fc-138">类型</span><span class="sxs-lookup"><span data-stu-id="a30fc-138">Type</span></span>   |<span data-ttu-id="a30fc-139">说明</span><span class="sxs-lookup"><span data-stu-id="a30fc-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a30fc-140">format</span><span class="sxs-lookup"><span data-stu-id="a30fc-140">format</span></span>|[<span data-ttu-id="a30fc-141">ChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="a30fc-141">ChartSeriesFormat</span></span>](chartseriesformat.md)|<span data-ttu-id="a30fc-p102">表示图表系列的格式，包括填充和线条格式。只读。</span><span class="sxs-lookup"><span data-stu-id="a30fc-p102">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="a30fc-144">points</span><span class="sxs-lookup"><span data-stu-id="a30fc-144">points</span></span>|<span data-ttu-id="a30fc-145">[ChartPoints](chartpoint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a30fc-145">[ChartPoints](chartpoint.md) collection</span></span>|<span data-ttu-id="a30fc-p103">表示系列中所有数据点的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="a30fc-p103">Represents a collection of all points in the series. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a30fc-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a30fc-148">JSON representation</span></span>

<span data-ttu-id="a30fc-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a30fc-149">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartSeries"
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