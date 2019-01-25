---
title: ChartSeries 资源类型
description: 代表图表上的系列。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e5606516092633ff14d23947f73626adc6d83c2c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519659"
---
# <a name="chartseries-resource-type"></a><span data-ttu-id="a3d68-103">ChartSeries 资源类型</span><span class="sxs-lookup"><span data-stu-id="a3d68-103">ChartSeries resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3d68-104">代表图表上的系列。</span><span class="sxs-lookup"><span data-stu-id="a3d68-104">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="a3d68-105">方法</span><span class="sxs-lookup"><span data-stu-id="a3d68-105">Methods</span></span>

| <span data-ttu-id="a3d68-106">方法</span><span class="sxs-lookup"><span data-stu-id="a3d68-106">Method</span></span>           | <span data-ttu-id="a3d68-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="a3d68-107">Return Type</span></span>    |<span data-ttu-id="a3d68-108">说明</span><span class="sxs-lookup"><span data-stu-id="a3d68-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a3d68-109">获取 ChartSeries</span><span class="sxs-lookup"><span data-stu-id="a3d68-109">[Get ChartSeries](../api/chartseries-get.md)</span></span> | [<span data-ttu-id="a3d68-110">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="a3d68-110">ChartSeries</span></span>](chartseries.md) |<span data-ttu-id="a3d68-111">读取 chartSeries 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a3d68-111">Read properties and relationships of chartSeries object.</span></span>|
|<span data-ttu-id="a3d68-112">创建 ChartPoints</span><span class="sxs-lookup"><span data-stu-id="a3d68-112">[Create ChartPoints](../api/chartseries-post-points.md)</span></span> |<span data-ttu-id="a3d68-113">ChartPoints</span><span class="sxs-lookup"><span data-stu-id="a3d68-113">[ChartPoints](chartpoint.md)</span></span>| <span data-ttu-id="a3d68-114">通过发布到点集合创建新的 ChartPoints。</span><span class="sxs-lookup"><span data-stu-id="a3d68-114">Create a new ChartPoints by posting to the points collection.</span></span>|
|<span data-ttu-id="a3d68-115">列出 points</span><span class="sxs-lookup"><span data-stu-id="a3d68-115">[List points](../api/chartseries-list-points.md)</span></span> |<span data-ttu-id="a3d68-116">ChartPoints 集合</span><span class="sxs-lookup"><span data-stu-id="a3d68-116">[ChartPoints](chartpoint.md) collection</span></span>| <span data-ttu-id="a3d68-117">获取 ChartPoints 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a3d68-117">Get a ChartPoints object collection.</span></span>|
|[<span data-ttu-id="a3d68-118">Update</span><span class="sxs-lookup"><span data-stu-id="a3d68-118">Update</span></span>](../api/chartseries-update.md) | [<span data-ttu-id="a3d68-119">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="a3d68-119">ChartSeries</span></span>](chartseries.md) |<span data-ttu-id="a3d68-120">更新 ChartSeries 对象。</span><span class="sxs-lookup"><span data-stu-id="a3d68-120">Update ChartSeries object.</span></span> |
|[<span data-ttu-id="a3d68-121">List</span><span class="sxs-lookup"><span data-stu-id="a3d68-121">List</span></span>](../api/chartseries-list.md) | <span data-ttu-id="a3d68-122">ChartSeries 集合</span><span class="sxs-lookup"><span data-stu-id="a3d68-122">[ChartSeries](chartseries.md) collection</span></span> |<span data-ttu-id="a3d68-123">获取 chartSeries 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a3d68-123">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="a3d68-124">Itemat</span><span class="sxs-lookup"><span data-stu-id="a3d68-124">Itemat</span></span>](../api/chartseriescollection-itemat.md)|[<span data-ttu-id="a3d68-125">ChartSeries</span><span class="sxs-lookup"><span data-stu-id="a3d68-125">ChartSeries</span></span>](chartseries.md)|<span data-ttu-id="a3d68-126">根据其在集合中的位置检索系列</span><span class="sxs-lookup"><span data-stu-id="a3d68-126">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="a3d68-127">属性</span><span class="sxs-lookup"><span data-stu-id="a3d68-127">Properties</span></span>
| <span data-ttu-id="a3d68-128">属性</span><span class="sxs-lookup"><span data-stu-id="a3d68-128">Property</span></span>     | <span data-ttu-id="a3d68-129">类型</span><span class="sxs-lookup"><span data-stu-id="a3d68-129">Type</span></span>   |<span data-ttu-id="a3d68-130">说明</span><span class="sxs-lookup"><span data-stu-id="a3d68-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a3d68-131">name</span><span class="sxs-lookup"><span data-stu-id="a3d68-131">name</span></span>|<span data-ttu-id="a3d68-132">string</span><span class="sxs-lookup"><span data-stu-id="a3d68-132">string</span></span>|<span data-ttu-id="a3d68-133">表示图表中某个系列的名称。</span><span class="sxs-lookup"><span data-stu-id="a3d68-133">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3d68-134">关系</span><span class="sxs-lookup"><span data-stu-id="a3d68-134">Relationships</span></span>
| <span data-ttu-id="a3d68-135">关系</span><span class="sxs-lookup"><span data-stu-id="a3d68-135">Relationship</span></span> | <span data-ttu-id="a3d68-136">类型</span><span class="sxs-lookup"><span data-stu-id="a3d68-136">Type</span></span>   |<span data-ttu-id="a3d68-137">说明</span><span class="sxs-lookup"><span data-stu-id="a3d68-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a3d68-138">format</span><span class="sxs-lookup"><span data-stu-id="a3d68-138">format</span></span>|[<span data-ttu-id="a3d68-139">ChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="a3d68-139">ChartSeriesFormat</span></span>](chartseriesformat.md)|<span data-ttu-id="a3d68-p101">表示图表系列的格式，包括填充和线条格式。只读。</span><span class="sxs-lookup"><span data-stu-id="a3d68-p101">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="a3d68-142">points</span><span class="sxs-lookup"><span data-stu-id="a3d68-142">points</span></span>|<span data-ttu-id="a3d68-143">[ChartPoints](chartpoint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a3d68-143">[ChartPoints](chartpoint.md) collection</span></span>|<span data-ttu-id="a3d68-p102">表示系列中所有数据点的集合。只读。</span><span class="sxs-lookup"><span data-stu-id="a3d68-p102">Represents a collection of all points in the series. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a3d68-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a3d68-146">JSON representation</span></span>

<span data-ttu-id="a3d68-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3d68-147">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartSeries resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartseries.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
