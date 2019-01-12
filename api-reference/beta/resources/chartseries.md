---
title: ChartSeries 资源类型
description: 代表图表上的系列。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5a299c7140c2032a57cd47fb0880ae34620a920b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915814"
---
# <a name="chartseries-resource-type"></a><span data-ttu-id="09703-103">ChartSeries 资源类型</span><span class="sxs-lookup"><span data-stu-id="09703-103">ChartSeries resource type</span></span>

> <span data-ttu-id="09703-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="09703-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="09703-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="09703-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="09703-106">代表图表上的系列。</span><span class="sxs-lookup"><span data-stu-id="09703-106">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="09703-107">方法</span><span class="sxs-lookup"><span data-stu-id="09703-107">Methods</span></span>

| <span data-ttu-id="09703-108">方法</span><span class="sxs-lookup"><span data-stu-id="09703-108">Method</span></span>           | <span data-ttu-id="09703-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="09703-109">Return Type</span></span>    |<span data-ttu-id="09703-110">说明</span><span class="sxs-lookup"><span data-stu-id="09703-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="09703-111">获取 ChartSeries</span><span class="sxs-lookup"><span data-stu-id="09703-111">Get ChartSeries</span></span>](../api/chartseries-get.md) | [<span data-ttu-id="09703-112">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="09703-112">ChartSeries</span></span>](chartseries.md) |<span data-ttu-id="09703-113">读取 chartSeries 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="09703-113">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="09703-114">创建 ChartPoints</span><span class="sxs-lookup"><span data-stu-id="09703-114">Create ChartPoints</span></span>](../api/chartseries-post-points.md) |[<span data-ttu-id="09703-115">ChartPoints</span><span class="sxs-lookup"><span data-stu-id="09703-115">ChartPoints</span></span>](chartpoint.md)| <span data-ttu-id="09703-116">通过发布到点集合创建新的 ChartPoints。</span><span class="sxs-lookup"><span data-stu-id="09703-116">Create a new ChartPoints by posting to the points collection.</span></span>|
|[<span data-ttu-id="09703-117">列出 points</span><span class="sxs-lookup"><span data-stu-id="09703-117">List points</span></span>](../api/chartseries-list-points.md) |<span data-ttu-id="09703-118">[ChartPoints](chartpoint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="09703-118">[ChartPoints](chartpoint.md) collection</span></span>| <span data-ttu-id="09703-119">获取 ChartPoints 对象集合。</span><span class="sxs-lookup"><span data-stu-id="09703-119">Get a ChartPoints object collection.</span></span>|
|[<span data-ttu-id="09703-120">更新</span><span class="sxs-lookup"><span data-stu-id="09703-120">Update</span></span>](../api/chartseries-update.md) | [<span data-ttu-id="09703-121">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="09703-121">ChartSeries</span></span>](chartseries.md) |<span data-ttu-id="09703-122">更新 ChartSeries 对象。</span><span class="sxs-lookup"><span data-stu-id="09703-122">Update ChartSeries object.</span></span> |
|[<span data-ttu-id="09703-123">List</span><span class="sxs-lookup"><span data-stu-id="09703-123">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="09703-124">[ChartSeries](chartseries.md) 集合</span><span class="sxs-lookup"><span data-stu-id="09703-124">[ChartSeries](chartseries.md) collection</span></span> |<span data-ttu-id="09703-125">获取 chartSeries 对象集合。</span><span class="sxs-lookup"><span data-stu-id="09703-125">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="09703-126">Itemat</span><span class="sxs-lookup"><span data-stu-id="09703-126">Itemat</span></span>](../api/chartseriescollection-itemat.md)|[<span data-ttu-id="09703-127">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="09703-127">ChartSeries</span></span>](chartseries.md)|<span data-ttu-id="09703-128">根据其在集合中的位置检索系列</span><span class="sxs-lookup"><span data-stu-id="09703-128">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="09703-129">属性</span><span class="sxs-lookup"><span data-stu-id="09703-129">Properties</span></span>
| <span data-ttu-id="09703-130">属性</span><span class="sxs-lookup"><span data-stu-id="09703-130">Property</span></span>     | <span data-ttu-id="09703-131">类型</span><span class="sxs-lookup"><span data-stu-id="09703-131">Type</span></span>   |<span data-ttu-id="09703-132">说明</span><span class="sxs-lookup"><span data-stu-id="09703-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09703-133">name</span><span class="sxs-lookup"><span data-stu-id="09703-133">name</span></span>|<span data-ttu-id="09703-134">string</span><span class="sxs-lookup"><span data-stu-id="09703-134">string</span></span>|<span data-ttu-id="09703-135">表示图表中某个系列的名称。</span><span class="sxs-lookup"><span data-stu-id="09703-135">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09703-136">Relationships</span><span class="sxs-lookup"><span data-stu-id="09703-136">Relationships</span></span>
| <span data-ttu-id="09703-137">关系</span><span class="sxs-lookup"><span data-stu-id="09703-137">Relationship</span></span> | <span data-ttu-id="09703-138">类型</span><span class="sxs-lookup"><span data-stu-id="09703-138">Type</span></span>   |<span data-ttu-id="09703-139">说明</span><span class="sxs-lookup"><span data-stu-id="09703-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09703-140">format</span><span class="sxs-lookup"><span data-stu-id="09703-140">format</span></span>|[<span data-ttu-id="09703-141">ChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="09703-141">ChartSeriesFormat</span></span>](chartseriesformat.md)|<span data-ttu-id="09703-p102">表示图表系列的格式，包括填充和线条格式。只读。</span><span class="sxs-lookup"><span data-stu-id="09703-p102">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="09703-144">points</span><span class="sxs-lookup"><span data-stu-id="09703-144">points</span></span>|<span data-ttu-id="09703-145">[ChartPoints](chartpoint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="09703-145">[ChartPoints](chartpoint.md) collection</span></span>|<span data-ttu-id="09703-p103">表示系列中所有数据点的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="09703-p103">Represents a collection of all points in the series. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="09703-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="09703-148">JSON representation</span></span>

<span data-ttu-id="09703-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09703-149">Here is a JSON representation of the resource.</span></span>

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
