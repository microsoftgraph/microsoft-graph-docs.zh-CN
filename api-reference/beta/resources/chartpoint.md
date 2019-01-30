---
title: ChartPoint 资源类型
description: 表示图表中某个系列的点。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4fd50e2e0b0f289f719dd6636eab16544e6a80f5
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641965"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="33ac8-103">ChartPoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="33ac8-103">ChartPoint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33ac8-104">表示图表中某个系列的点。</span><span class="sxs-lookup"><span data-stu-id="33ac8-104">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="33ac8-105">方法</span><span class="sxs-lookup"><span data-stu-id="33ac8-105">Methods</span></span>

| <span data-ttu-id="33ac8-106">方法</span><span class="sxs-lookup"><span data-stu-id="33ac8-106">Method</span></span>           | <span data-ttu-id="33ac8-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="33ac8-107">Return Type</span></span>    |<span data-ttu-id="33ac8-108">说明</span><span class="sxs-lookup"><span data-stu-id="33ac8-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="33ac8-109">获取 ChartPoint</span><span class="sxs-lookup"><span data-stu-id="33ac8-109">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="33ac8-110">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="33ac8-110">ChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="33ac8-111">读取 chartPoint 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="33ac8-111">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="33ac8-112">List</span><span class="sxs-lookup"><span data-stu-id="33ac8-112">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="33ac8-113">[ChartPoint](chartpoint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="33ac8-113">[ChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="33ac8-114">获取 chartPoint 对象集合。</span><span class="sxs-lookup"><span data-stu-id="33ac8-114">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="33ac8-115">Itemat</span><span class="sxs-lookup"><span data-stu-id="33ac8-115">Itemat</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="33ac8-116">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="33ac8-116">ChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="33ac8-117">根据其在系列中的位置检索点。</span><span class="sxs-lookup"><span data-stu-id="33ac8-117">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="33ac8-118">属性</span><span class="sxs-lookup"><span data-stu-id="33ac8-118">Properties</span></span>
| <span data-ttu-id="33ac8-119">属性</span><span class="sxs-lookup"><span data-stu-id="33ac8-119">Property</span></span>     | <span data-ttu-id="33ac8-120">类型</span><span class="sxs-lookup"><span data-stu-id="33ac8-120">Type</span></span>   |<span data-ttu-id="33ac8-121">说明</span><span class="sxs-lookup"><span data-stu-id="33ac8-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="33ac8-122">value</span><span class="sxs-lookup"><span data-stu-id="33ac8-122">value</span></span>|<span data-ttu-id="33ac8-123">对象</span><span class="sxs-lookup"><span data-stu-id="33ac8-123">object</span></span>|<span data-ttu-id="33ac8-p101">返回图表点的值。只读。</span><span class="sxs-lookup"><span data-stu-id="33ac8-p101">Returns the value of a chart point. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="33ac8-126">关系</span><span class="sxs-lookup"><span data-stu-id="33ac8-126">Relationships</span></span>
| <span data-ttu-id="33ac8-127">关系</span><span class="sxs-lookup"><span data-stu-id="33ac8-127">Relationship</span></span> | <span data-ttu-id="33ac8-128">类型</span><span class="sxs-lookup"><span data-stu-id="33ac8-128">Type</span></span>   |<span data-ttu-id="33ac8-129">说明</span><span class="sxs-lookup"><span data-stu-id="33ac8-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="33ac8-130">format</span><span class="sxs-lookup"><span data-stu-id="33ac8-130">format</span></span>|[<span data-ttu-id="33ac8-131">ChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="33ac8-131">ChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="33ac8-p102">封装图表点的格式属性。只读。</span><span class="sxs-lookup"><span data-stu-id="33ac8-p102">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="33ac8-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="33ac8-134">JSON representation</span></span>

<span data-ttu-id="33ac8-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="33ac8-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartPoint"
}-->

```json
{
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartpoint.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
