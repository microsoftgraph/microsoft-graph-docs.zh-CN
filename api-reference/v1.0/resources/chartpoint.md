---
title: ChartPoint 资源类型
description: 表示图表中某个系列的点。
ms.openlocfilehash: 93c89bca61f27924621df0376bdf50e925e25c86
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010963"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="728af-103">ChartPoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="728af-103">ChartPoint resource type</span></span>

<span data-ttu-id="728af-104">表示图表中某个系列的点。</span><span class="sxs-lookup"><span data-stu-id="728af-104">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="728af-105">方法</span><span class="sxs-lookup"><span data-stu-id="728af-105">Methods</span></span>

| <span data-ttu-id="728af-106">方法</span><span class="sxs-lookup"><span data-stu-id="728af-106">Method</span></span>           | <span data-ttu-id="728af-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="728af-107">Return Type</span></span>    |<span data-ttu-id="728af-108">说明</span><span class="sxs-lookup"><span data-stu-id="728af-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="728af-109">获取 ChartPoint</span><span class="sxs-lookup"><span data-stu-id="728af-109">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="728af-110">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="728af-110">WorkbookChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="728af-111">读取 chartPoint 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="728af-111">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="728af-112">List</span><span class="sxs-lookup"><span data-stu-id="728af-112">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="728af-113">[WorkbookChartPoint](chartpoint.md)集合</span><span class="sxs-lookup"><span data-stu-id="728af-113">[WorkbookChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="728af-114">获取 chartPoint 对象集合。</span><span class="sxs-lookup"><span data-stu-id="728af-114">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="728af-115">ItemAt</span><span class="sxs-lookup"><span data-stu-id="728af-115">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="728af-116">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="728af-116">WorkbookChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="728af-117">根据其在系列中的位置检索点。</span><span class="sxs-lookup"><span data-stu-id="728af-117">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="728af-118">属性</span><span class="sxs-lookup"><span data-stu-id="728af-118">Properties</span></span>
| <span data-ttu-id="728af-119">属性</span><span class="sxs-lookup"><span data-stu-id="728af-119">Property</span></span>     | <span data-ttu-id="728af-120">类型</span><span class="sxs-lookup"><span data-stu-id="728af-120">Type</span></span>   |<span data-ttu-id="728af-121">说明</span><span class="sxs-lookup"><span data-stu-id="728af-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="728af-122">value</span><span class="sxs-lookup"><span data-stu-id="728af-122">value</span></span>|<span data-ttu-id="728af-123">Json</span><span class="sxs-lookup"><span data-stu-id="728af-123">Json</span></span>|<span data-ttu-id="728af-p101">返回图表点的值。只读。</span><span class="sxs-lookup"><span data-stu-id="728af-p101">Returns the value of a chart point. Read-only.</span></span>|
|<span data-ttu-id="728af-126">id</span><span class="sxs-lookup"><span data-stu-id="728af-126">id</span></span>|<span data-ttu-id="728af-127">string</span><span class="sxs-lookup"><span data-stu-id="728af-127">string</span></span>|<span data-ttu-id="728af-128">唯一标识符</span><span class="sxs-lookup"><span data-stu-id="728af-128">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="728af-129">Relationships</span><span class="sxs-lookup"><span data-stu-id="728af-129">Relationships</span></span>
| <span data-ttu-id="728af-130">关系</span><span class="sxs-lookup"><span data-stu-id="728af-130">Relationship</span></span> | <span data-ttu-id="728af-131">类型</span><span class="sxs-lookup"><span data-stu-id="728af-131">Type</span></span>   |<span data-ttu-id="728af-132">说明</span><span class="sxs-lookup"><span data-stu-id="728af-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="728af-133">format</span><span class="sxs-lookup"><span data-stu-id="728af-133">format</span></span>|[<span data-ttu-id="728af-134">WorkbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="728af-134">WorkbookChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="728af-p102">封装图表点的格式属性。只读。</span><span class="sxs-lookup"><span data-stu-id="728af-p102">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="728af-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="728af-137">JSON representation</span></span>

<span data-ttu-id="728af-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="728af-138">Here is a JSON representation of the resource.</span></span>

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