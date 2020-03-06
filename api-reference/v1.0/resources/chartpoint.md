---
title: ChartPoint 资源类型
description: 表示图表中某个系列的点。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: befa6f552fd343140d2aae10266c1445066266d5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531834"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="86465-103">ChartPoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="86465-103">ChartPoint resource type</span></span>

<span data-ttu-id="86465-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86465-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="86465-105">表示图表中某个系列的点。</span><span class="sxs-lookup"><span data-stu-id="86465-105">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="86465-106">Methods</span><span class="sxs-lookup"><span data-stu-id="86465-106">Methods</span></span>

| <span data-ttu-id="86465-107">方法</span><span class="sxs-lookup"><span data-stu-id="86465-107">Method</span></span>           | <span data-ttu-id="86465-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="86465-108">Return Type</span></span>    |<span data-ttu-id="86465-109">说明</span><span class="sxs-lookup"><span data-stu-id="86465-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="86465-110">获取 ChartPoint</span><span class="sxs-lookup"><span data-stu-id="86465-110">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="86465-111">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="86465-111">WorkbookChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="86465-112">读取 chartPoint 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="86465-112">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="86465-113">列出</span><span class="sxs-lookup"><span data-stu-id="86465-113">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="86465-114">[WorkbookChartPoint](chartpoint.md)集合</span><span class="sxs-lookup"><span data-stu-id="86465-114">[WorkbookChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="86465-115">获取 chartPoint 对象集合。</span><span class="sxs-lookup"><span data-stu-id="86465-115">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="86465-116">ItemAt</span><span class="sxs-lookup"><span data-stu-id="86465-116">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="86465-117">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="86465-117">WorkbookChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="86465-118">根据其在系列中的位置检索点。</span><span class="sxs-lookup"><span data-stu-id="86465-118">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="86465-119">属性</span><span class="sxs-lookup"><span data-stu-id="86465-119">Properties</span></span>
| <span data-ttu-id="86465-120">属性</span><span class="sxs-lookup"><span data-stu-id="86465-120">Property</span></span>     | <span data-ttu-id="86465-121">类型</span><span class="sxs-lookup"><span data-stu-id="86465-121">Type</span></span>   |<span data-ttu-id="86465-122">说明</span><span class="sxs-lookup"><span data-stu-id="86465-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86465-123">值</span><span class="sxs-lookup"><span data-stu-id="86465-123">value</span></span>|<span data-ttu-id="86465-124">Json</span><span class="sxs-lookup"><span data-stu-id="86465-124">Json</span></span>|<span data-ttu-id="86465-125">返回图表点的值。</span><span class="sxs-lookup"><span data-stu-id="86465-125">Returns the value of a chart point.</span></span> <span data-ttu-id="86465-126">只读。</span><span class="sxs-lookup"><span data-stu-id="86465-126">Read-only.</span></span>|
|<span data-ttu-id="86465-127">id</span><span class="sxs-lookup"><span data-stu-id="86465-127">id</span></span>|<span data-ttu-id="86465-128">string</span><span class="sxs-lookup"><span data-stu-id="86465-128">string</span></span>|<span data-ttu-id="86465-129">唯一标识符</span><span class="sxs-lookup"><span data-stu-id="86465-129">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="86465-130">关系</span><span class="sxs-lookup"><span data-stu-id="86465-130">Relationships</span></span>
| <span data-ttu-id="86465-131">关系</span><span class="sxs-lookup"><span data-stu-id="86465-131">Relationship</span></span> | <span data-ttu-id="86465-132">类型</span><span class="sxs-lookup"><span data-stu-id="86465-132">Type</span></span>   |<span data-ttu-id="86465-133">说明</span><span class="sxs-lookup"><span data-stu-id="86465-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86465-134">format</span><span class="sxs-lookup"><span data-stu-id="86465-134">format</span></span>|[<span data-ttu-id="86465-135">WorkbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="86465-135">WorkbookChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="86465-136">封装图表点的格式属性。</span><span class="sxs-lookup"><span data-stu-id="86465-136">Encapsulates the format properties chart point.</span></span> <span data-ttu-id="86465-137">只读。</span><span class="sxs-lookup"><span data-stu-id="86465-137">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="86465-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="86465-138">JSON representation</span></span>

<span data-ttu-id="86465-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="86465-139">Here is a JSON representation of the resource.</span></span>

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
