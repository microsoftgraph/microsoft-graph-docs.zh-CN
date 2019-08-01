---
title: ChartPoint 资源类型
description: 表示图表中某个系列的点。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 5e0a9d9fe558f53fe87ae8e3a0a447a5bd93aa71
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032947"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="53ac3-103">ChartPoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="53ac3-103">ChartPoint resource type</span></span>

<span data-ttu-id="53ac3-104">表示图表中某个系列的点。</span><span class="sxs-lookup"><span data-stu-id="53ac3-104">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="53ac3-105">方法</span><span class="sxs-lookup"><span data-stu-id="53ac3-105">Methods</span></span>

| <span data-ttu-id="53ac3-106">方法</span><span class="sxs-lookup"><span data-stu-id="53ac3-106">Method</span></span>           | <span data-ttu-id="53ac3-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="53ac3-107">Return Type</span></span>    |<span data-ttu-id="53ac3-108">说明</span><span class="sxs-lookup"><span data-stu-id="53ac3-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="53ac3-109">获取 ChartPoint</span><span class="sxs-lookup"><span data-stu-id="53ac3-109">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="53ac3-110">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="53ac3-110">WorkbookChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="53ac3-111">读取 chartPoint 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="53ac3-111">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="53ac3-112">列出</span><span class="sxs-lookup"><span data-stu-id="53ac3-112">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="53ac3-113">[WorkbookChartPoint](chartpoint.md)集合</span><span class="sxs-lookup"><span data-stu-id="53ac3-113">[WorkbookChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="53ac3-114">获取 chartPoint 对象集合。</span><span class="sxs-lookup"><span data-stu-id="53ac3-114">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="53ac3-115">ItemAt</span><span class="sxs-lookup"><span data-stu-id="53ac3-115">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="53ac3-116">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="53ac3-116">WorkbookChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="53ac3-117">根据其在系列中的位置检索点。</span><span class="sxs-lookup"><span data-stu-id="53ac3-117">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="53ac3-118">属性</span><span class="sxs-lookup"><span data-stu-id="53ac3-118">Properties</span></span>
| <span data-ttu-id="53ac3-119">属性</span><span class="sxs-lookup"><span data-stu-id="53ac3-119">Property</span></span>     | <span data-ttu-id="53ac3-120">类型</span><span class="sxs-lookup"><span data-stu-id="53ac3-120">Type</span></span>   |<span data-ttu-id="53ac3-121">说明</span><span class="sxs-lookup"><span data-stu-id="53ac3-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53ac3-122">值</span><span class="sxs-lookup"><span data-stu-id="53ac3-122">value</span></span>|<span data-ttu-id="53ac3-123">Json</span><span class="sxs-lookup"><span data-stu-id="53ac3-123">Json</span></span>|<span data-ttu-id="53ac3-124">返回图表点的值。</span><span class="sxs-lookup"><span data-stu-id="53ac3-124">Returns the value of a chart point.</span></span> <span data-ttu-id="53ac3-125">只读。</span><span class="sxs-lookup"><span data-stu-id="53ac3-125">Read-only.</span></span>|
|<span data-ttu-id="53ac3-126">id</span><span class="sxs-lookup"><span data-stu-id="53ac3-126">id</span></span>|<span data-ttu-id="53ac3-127">string</span><span class="sxs-lookup"><span data-stu-id="53ac3-127">string</span></span>|<span data-ttu-id="53ac3-128">唯一标识符</span><span class="sxs-lookup"><span data-stu-id="53ac3-128">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="53ac3-129">关系</span><span class="sxs-lookup"><span data-stu-id="53ac3-129">Relationships</span></span>
| <span data-ttu-id="53ac3-130">关系</span><span class="sxs-lookup"><span data-stu-id="53ac3-130">Relationship</span></span> | <span data-ttu-id="53ac3-131">类型</span><span class="sxs-lookup"><span data-stu-id="53ac3-131">Type</span></span>   |<span data-ttu-id="53ac3-132">说明</span><span class="sxs-lookup"><span data-stu-id="53ac3-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53ac3-133">format</span><span class="sxs-lookup"><span data-stu-id="53ac3-133">format</span></span>|[<span data-ttu-id="53ac3-134">WorkbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="53ac3-134">WorkbookChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="53ac3-135">封装图表点的格式属性。</span><span class="sxs-lookup"><span data-stu-id="53ac3-135">Encapsulates the format properties chart point.</span></span> <span data-ttu-id="53ac3-136">只读。</span><span class="sxs-lookup"><span data-stu-id="53ac3-136">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="53ac3-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="53ac3-137">JSON representation</span></span>

<span data-ttu-id="53ac3-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53ac3-138">Here is a JSON representation of the resource.</span></span>

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
