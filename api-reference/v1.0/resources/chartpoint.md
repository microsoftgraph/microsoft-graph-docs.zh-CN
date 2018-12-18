---
title: ChartPoint 资源类型
description: 表示图表中某个系列的点。
author: lumine2008
ms.openlocfilehash: b2d1fab0c76100aae1a5606690772a0aa3854f42
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316224"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="8d1a6-103">ChartPoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="8d1a6-103">ChartPoint resource type</span></span>

<span data-ttu-id="8d1a6-104">表示图表中某个系列的点。</span><span class="sxs-lookup"><span data-stu-id="8d1a6-104">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="8d1a6-105">方法</span><span class="sxs-lookup"><span data-stu-id="8d1a6-105">Methods</span></span>

| <span data-ttu-id="8d1a6-106">方法</span><span class="sxs-lookup"><span data-stu-id="8d1a6-106">Method</span></span>           | <span data-ttu-id="8d1a6-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="8d1a6-107">Return Type</span></span>    |<span data-ttu-id="8d1a6-108">说明</span><span class="sxs-lookup"><span data-stu-id="8d1a6-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8d1a6-109">获取 ChartPoint</span><span class="sxs-lookup"><span data-stu-id="8d1a6-109">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="8d1a6-110">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="8d1a6-110">WorkbookChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="8d1a6-111">读取 chartPoint 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8d1a6-111">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="8d1a6-112">List</span><span class="sxs-lookup"><span data-stu-id="8d1a6-112">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="8d1a6-113">[WorkbookChartPoint](chartpoint.md)集合</span><span class="sxs-lookup"><span data-stu-id="8d1a6-113">[WorkbookChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="8d1a6-114">获取 chartPoint 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8d1a6-114">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="8d1a6-115">ItemAt</span><span class="sxs-lookup"><span data-stu-id="8d1a6-115">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="8d1a6-116">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="8d1a6-116">WorkbookChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="8d1a6-117">根据其在系列中的位置检索点。</span><span class="sxs-lookup"><span data-stu-id="8d1a6-117">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="8d1a6-118">属性</span><span class="sxs-lookup"><span data-stu-id="8d1a6-118">Properties</span></span>
| <span data-ttu-id="8d1a6-119">属性</span><span class="sxs-lookup"><span data-stu-id="8d1a6-119">Property</span></span>     | <span data-ttu-id="8d1a6-120">类型</span><span class="sxs-lookup"><span data-stu-id="8d1a6-120">Type</span></span>   |<span data-ttu-id="8d1a6-121">说明</span><span class="sxs-lookup"><span data-stu-id="8d1a6-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d1a6-122">value</span><span class="sxs-lookup"><span data-stu-id="8d1a6-122">value</span></span>|<span data-ttu-id="8d1a6-123">Json</span><span class="sxs-lookup"><span data-stu-id="8d1a6-123">Json</span></span>|<span data-ttu-id="8d1a6-p101">返回图表点的值。只读。</span><span class="sxs-lookup"><span data-stu-id="8d1a6-p101">Returns the value of a chart point. Read-only.</span></span>|
|<span data-ttu-id="8d1a6-126">id</span><span class="sxs-lookup"><span data-stu-id="8d1a6-126">id</span></span>|<span data-ttu-id="8d1a6-127">string</span><span class="sxs-lookup"><span data-stu-id="8d1a6-127">string</span></span>|<span data-ttu-id="8d1a6-128">唯一标识符</span><span class="sxs-lookup"><span data-stu-id="8d1a6-128">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d1a6-129">Relationships</span><span class="sxs-lookup"><span data-stu-id="8d1a6-129">Relationships</span></span>
| <span data-ttu-id="8d1a6-130">关系</span><span class="sxs-lookup"><span data-stu-id="8d1a6-130">Relationship</span></span> | <span data-ttu-id="8d1a6-131">类型</span><span class="sxs-lookup"><span data-stu-id="8d1a6-131">Type</span></span>   |<span data-ttu-id="8d1a6-132">说明</span><span class="sxs-lookup"><span data-stu-id="8d1a6-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d1a6-133">format</span><span class="sxs-lookup"><span data-stu-id="8d1a6-133">format</span></span>|[<span data-ttu-id="8d1a6-134">WorkbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="8d1a6-134">WorkbookChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="8d1a6-p102">封装图表点的格式属性。只读。</span><span class="sxs-lookup"><span data-stu-id="8d1a6-p102">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8d1a6-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8d1a6-137">JSON representation</span></span>

<span data-ttu-id="8d1a6-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d1a6-138">Here is a JSON representation of the resource.</span></span>

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