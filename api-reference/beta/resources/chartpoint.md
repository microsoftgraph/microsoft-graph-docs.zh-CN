---
title: ChartPoint 资源类型
description: 表示图表中某个系列的点。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 66c58e08063bd9757ad9c174e81f35328dd2722b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912755"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="19f3f-103">ChartPoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="19f3f-103">ChartPoint resource type</span></span>

> <span data-ttu-id="19f3f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="19f3f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19f3f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="19f3f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="19f3f-106">表示图表中某个系列的点。</span><span class="sxs-lookup"><span data-stu-id="19f3f-106">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="19f3f-107">方法</span><span class="sxs-lookup"><span data-stu-id="19f3f-107">Methods</span></span>

| <span data-ttu-id="19f3f-108">方法</span><span class="sxs-lookup"><span data-stu-id="19f3f-108">Method</span></span>           | <span data-ttu-id="19f3f-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="19f3f-109">Return Type</span></span>    |<span data-ttu-id="19f3f-110">说明</span><span class="sxs-lookup"><span data-stu-id="19f3f-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="19f3f-111">获取 ChartPoint</span><span class="sxs-lookup"><span data-stu-id="19f3f-111">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="19f3f-112">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="19f3f-112">ChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="19f3f-113">读取 chartPoint 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="19f3f-113">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="19f3f-114">List</span><span class="sxs-lookup"><span data-stu-id="19f3f-114">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="19f3f-115">[ChartPoint](chartpoint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="19f3f-115">[ChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="19f3f-116">获取 chartPoint 对象集合。</span><span class="sxs-lookup"><span data-stu-id="19f3f-116">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="19f3f-117">Itemat</span><span class="sxs-lookup"><span data-stu-id="19f3f-117">Itemat</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="19f3f-118">ChartPoint</span><span class="sxs-lookup"><span data-stu-id="19f3f-118">ChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="19f3f-119">根据其在系列中的位置检索点。</span><span class="sxs-lookup"><span data-stu-id="19f3f-119">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="19f3f-120">属性</span><span class="sxs-lookup"><span data-stu-id="19f3f-120">Properties</span></span>
| <span data-ttu-id="19f3f-121">属性</span><span class="sxs-lookup"><span data-stu-id="19f3f-121">Property</span></span>     | <span data-ttu-id="19f3f-122">类型</span><span class="sxs-lookup"><span data-stu-id="19f3f-122">Type</span></span>   |<span data-ttu-id="19f3f-123">说明</span><span class="sxs-lookup"><span data-stu-id="19f3f-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19f3f-124">value</span><span class="sxs-lookup"><span data-stu-id="19f3f-124">value</span></span>|<span data-ttu-id="19f3f-125">对象</span><span class="sxs-lookup"><span data-stu-id="19f3f-125">object</span></span>|<span data-ttu-id="19f3f-p102">返回图表点的值。只读。</span><span class="sxs-lookup"><span data-stu-id="19f3f-p102">Returns the value of a chart point. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="19f3f-128">Relationships</span><span class="sxs-lookup"><span data-stu-id="19f3f-128">Relationships</span></span>
| <span data-ttu-id="19f3f-129">关系</span><span class="sxs-lookup"><span data-stu-id="19f3f-129">Relationship</span></span> | <span data-ttu-id="19f3f-130">类型</span><span class="sxs-lookup"><span data-stu-id="19f3f-130">Type</span></span>   |<span data-ttu-id="19f3f-131">说明</span><span class="sxs-lookup"><span data-stu-id="19f3f-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19f3f-132">format</span><span class="sxs-lookup"><span data-stu-id="19f3f-132">format</span></span>|[<span data-ttu-id="19f3f-133">ChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="19f3f-133">ChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="19f3f-p103">封装图表点的格式属性。只读。</span><span class="sxs-lookup"><span data-stu-id="19f3f-p103">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="19f3f-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="19f3f-136">JSON representation</span></span>

<span data-ttu-id="19f3f-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="19f3f-137">Here is a JSON representation of the resource.</span></span>

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
