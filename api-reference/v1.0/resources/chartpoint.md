---
title: ChartPoint 资源类型
description: 表示图表中某个系列的点。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 208f4eb90763210639540c9fd15bdaec89b7466c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988378"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="74abb-103">ChartPoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="74abb-103">ChartPoint resource type</span></span>

<span data-ttu-id="74abb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74abb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="74abb-105">表示图表中某个系列的点。</span><span class="sxs-lookup"><span data-stu-id="74abb-105">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="74abb-106">方法</span><span class="sxs-lookup"><span data-stu-id="74abb-106">Methods</span></span>

| <span data-ttu-id="74abb-107">方法</span><span class="sxs-lookup"><span data-stu-id="74abb-107">Method</span></span>           | <span data-ttu-id="74abb-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="74abb-108">Return Type</span></span>    |<span data-ttu-id="74abb-109">说明</span><span class="sxs-lookup"><span data-stu-id="74abb-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="74abb-110">获取 ChartPoint</span><span class="sxs-lookup"><span data-stu-id="74abb-110">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="74abb-111">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="74abb-111">WorkbookChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="74abb-112">读取 chartPoint 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="74abb-112">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="74abb-113">列出</span><span class="sxs-lookup"><span data-stu-id="74abb-113">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="74abb-114">[WorkbookChartPoint](chartpoint.md) 集合</span><span class="sxs-lookup"><span data-stu-id="74abb-114">[WorkbookChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="74abb-115">获取 chartPoint 对象集合。</span><span class="sxs-lookup"><span data-stu-id="74abb-115">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="74abb-116">ItemAt</span><span class="sxs-lookup"><span data-stu-id="74abb-116">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="74abb-117">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="74abb-117">WorkbookChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="74abb-118">根据其在系列中的位置检索点。</span><span class="sxs-lookup"><span data-stu-id="74abb-118">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="74abb-119">属性</span><span class="sxs-lookup"><span data-stu-id="74abb-119">Properties</span></span>
| <span data-ttu-id="74abb-120">属性</span><span class="sxs-lookup"><span data-stu-id="74abb-120">Property</span></span>     | <span data-ttu-id="74abb-121">类型</span><span class="sxs-lookup"><span data-stu-id="74abb-121">Type</span></span>   |<span data-ttu-id="74abb-122">说明</span><span class="sxs-lookup"><span data-stu-id="74abb-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74abb-123">值</span><span class="sxs-lookup"><span data-stu-id="74abb-123">value</span></span>|<span data-ttu-id="74abb-124">Json</span><span class="sxs-lookup"><span data-stu-id="74abb-124">Json</span></span>|<span data-ttu-id="74abb-125">返回图表点的值。</span><span class="sxs-lookup"><span data-stu-id="74abb-125">Returns the value of a chart point.</span></span> <span data-ttu-id="74abb-126">只读。</span><span class="sxs-lookup"><span data-stu-id="74abb-126">Read-only.</span></span>|
|<span data-ttu-id="74abb-127">id</span><span class="sxs-lookup"><span data-stu-id="74abb-127">id</span></span>|<span data-ttu-id="74abb-128">string</span><span class="sxs-lookup"><span data-stu-id="74abb-128">string</span></span>|<span data-ttu-id="74abb-129">唯一标识符</span><span class="sxs-lookup"><span data-stu-id="74abb-129">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="74abb-130">关系</span><span class="sxs-lookup"><span data-stu-id="74abb-130">Relationships</span></span>
| <span data-ttu-id="74abb-131">关系</span><span class="sxs-lookup"><span data-stu-id="74abb-131">Relationship</span></span> | <span data-ttu-id="74abb-132">类型</span><span class="sxs-lookup"><span data-stu-id="74abb-132">Type</span></span>   |<span data-ttu-id="74abb-133">说明</span><span class="sxs-lookup"><span data-stu-id="74abb-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74abb-134">format</span><span class="sxs-lookup"><span data-stu-id="74abb-134">format</span></span>|[<span data-ttu-id="74abb-135">WorkbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="74abb-135">WorkbookChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="74abb-136">封装图表点的格式属性。</span><span class="sxs-lookup"><span data-stu-id="74abb-136">Encapsulates the format properties chart point.</span></span> <span data-ttu-id="74abb-137">只读。</span><span class="sxs-lookup"><span data-stu-id="74abb-137">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="74abb-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="74abb-138">JSON representation</span></span>

<span data-ttu-id="74abb-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="74abb-139">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPoint"
}-->

```json
{
  "value": "string",
  "id": "string"
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

