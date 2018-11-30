---
title: ChartPoint 资源类型
description: 表示图表中某个系列的点。
ms.openlocfilehash: 3d1bcc26fdc78bd7b844c870d40346a5f1f0496f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046182"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="ad2a5-103">ChartPoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="ad2a5-103">ChartPoint resource type</span></span>

> <span data-ttu-id="ad2a5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ad2a5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad2a5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ad2a5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ad2a5-106">表示图表中某个系列的点。</span><span class="sxs-lookup"><span data-stu-id="ad2a5-106">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="ad2a5-107">方法</span><span class="sxs-lookup"><span data-stu-id="ad2a5-107">Methods</span></span>

| <span data-ttu-id="ad2a5-108">方法</span><span class="sxs-lookup"><span data-stu-id="ad2a5-108">Method</span></span>           | <span data-ttu-id="ad2a5-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="ad2a5-109">Return Type</span></span>    |<span data-ttu-id="ad2a5-110">说明</span><span class="sxs-lookup"><span data-stu-id="ad2a5-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ad2a5-111">获取 ChartPoint</span><span class="sxs-lookup"><span data-stu-id="ad2a5-111">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="ad2a5-112">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="ad2a5-112">ChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="ad2a5-113">读取 chartPoint 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ad2a5-113">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="ad2a5-114">List</span><span class="sxs-lookup"><span data-stu-id="ad2a5-114">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="ad2a5-115">[ChartPoint](chartpoint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ad2a5-115">[ChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="ad2a5-116">获取 chartPoint 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ad2a5-116">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="ad2a5-117">Itemat</span><span class="sxs-lookup"><span data-stu-id="ad2a5-117">Itemat</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="ad2a5-118">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="ad2a5-118">ChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="ad2a5-119">根据其在系列中的位置检索点。</span><span class="sxs-lookup"><span data-stu-id="ad2a5-119">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="ad2a5-120">属性</span><span class="sxs-lookup"><span data-stu-id="ad2a5-120">Properties</span></span>
| <span data-ttu-id="ad2a5-121">属性</span><span class="sxs-lookup"><span data-stu-id="ad2a5-121">Property</span></span>     | <span data-ttu-id="ad2a5-122">类型</span><span class="sxs-lookup"><span data-stu-id="ad2a5-122">Type</span></span>   |<span data-ttu-id="ad2a5-123">说明</span><span class="sxs-lookup"><span data-stu-id="ad2a5-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad2a5-124">value</span><span class="sxs-lookup"><span data-stu-id="ad2a5-124">value</span></span>|<span data-ttu-id="ad2a5-125">对象</span><span class="sxs-lookup"><span data-stu-id="ad2a5-125">object</span></span>|<span data-ttu-id="ad2a5-p102">返回图表点的值。只读。</span><span class="sxs-lookup"><span data-stu-id="ad2a5-p102">Returns the value of a chart point. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad2a5-128">Relationships</span><span class="sxs-lookup"><span data-stu-id="ad2a5-128">Relationships</span></span>
| <span data-ttu-id="ad2a5-129">关系</span><span class="sxs-lookup"><span data-stu-id="ad2a5-129">Relationship</span></span> | <span data-ttu-id="ad2a5-130">类型</span><span class="sxs-lookup"><span data-stu-id="ad2a5-130">Type</span></span>   |<span data-ttu-id="ad2a5-131">说明</span><span class="sxs-lookup"><span data-stu-id="ad2a5-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad2a5-132">format</span><span class="sxs-lookup"><span data-stu-id="ad2a5-132">format</span></span>|[<span data-ttu-id="ad2a5-133">ChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="ad2a5-133">ChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="ad2a5-p103">封装图表点的格式属性。只读。</span><span class="sxs-lookup"><span data-stu-id="ad2a5-p103">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ad2a5-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ad2a5-136">JSON representation</span></span>

<span data-ttu-id="ad2a5-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ad2a5-137">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->