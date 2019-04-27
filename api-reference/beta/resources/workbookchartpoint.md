---
title: workbookChartPoint 资源类型
description: 表示图表中某个系列的点。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e12cc2f9a700ef66ec47a72aa88a2c30f2c2c3f6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348619"
---
# <a name="workbookchartpoint-resource-type"></a><span data-ttu-id="90936-103">workbookChartPoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="90936-103">workbookChartPoint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90936-104">表示图表中某个系列的点。</span><span class="sxs-lookup"><span data-stu-id="90936-104">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="90936-105">方法</span><span class="sxs-lookup"><span data-stu-id="90936-105">Methods</span></span>

| <span data-ttu-id="90936-106">方法</span><span class="sxs-lookup"><span data-stu-id="90936-106">Method</span></span>           | <span data-ttu-id="90936-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="90936-107">Return Type</span></span>    |<span data-ttu-id="90936-108">说明</span><span class="sxs-lookup"><span data-stu-id="90936-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="90936-109">获取 workbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="90936-109">Get workbookChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="90936-110">workbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="90936-110">workbookChartPoint</span></span>](workbookchartpoint.md) |<span data-ttu-id="90936-111">读取 chartPoint 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="90936-111">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="90936-112">列出</span><span class="sxs-lookup"><span data-stu-id="90936-112">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="90936-113">[workbookChartPoint](workbookchartpoint.md)集合</span><span class="sxs-lookup"><span data-stu-id="90936-113">[workbookChartPoint](workbookchartpoint.md) collection</span></span> |<span data-ttu-id="90936-114">获取 chartPoint 对象集合。</span><span class="sxs-lookup"><span data-stu-id="90936-114">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="90936-115">ItemAt</span><span class="sxs-lookup"><span data-stu-id="90936-115">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="90936-116">workbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="90936-116">workbookChartPoint</span></span>](workbookchartpoint.md)|<span data-ttu-id="90936-117">根据其在系列中的位置检索点。</span><span class="sxs-lookup"><span data-stu-id="90936-117">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="90936-118">属性</span><span class="sxs-lookup"><span data-stu-id="90936-118">Properties</span></span>
| <span data-ttu-id="90936-119">属性</span><span class="sxs-lookup"><span data-stu-id="90936-119">Property</span></span>     | <span data-ttu-id="90936-120">类型</span><span class="sxs-lookup"><span data-stu-id="90936-120">Type</span></span>   |<span data-ttu-id="90936-121">说明</span><span class="sxs-lookup"><span data-stu-id="90936-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90936-122">值</span><span class="sxs-lookup"><span data-stu-id="90936-122">value</span></span>|<span data-ttu-id="90936-123">Json</span><span class="sxs-lookup"><span data-stu-id="90936-123">Json</span></span>|<span data-ttu-id="90936-124">返回图表点的值。</span><span class="sxs-lookup"><span data-stu-id="90936-124">Returns the value of a chart point.</span></span> <span data-ttu-id="90936-125">只读。</span><span class="sxs-lookup"><span data-stu-id="90936-125">Read-only.</span></span>|
|<span data-ttu-id="90936-126">id</span><span class="sxs-lookup"><span data-stu-id="90936-126">id</span></span>|<span data-ttu-id="90936-127">string</span><span class="sxs-lookup"><span data-stu-id="90936-127">string</span></span>|<span data-ttu-id="90936-128">唯一标识符</span><span class="sxs-lookup"><span data-stu-id="90936-128">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="90936-129">关系</span><span class="sxs-lookup"><span data-stu-id="90936-129">Relationships</span></span>
| <span data-ttu-id="90936-130">关系</span><span class="sxs-lookup"><span data-stu-id="90936-130">Relationship</span></span> | <span data-ttu-id="90936-131">类型</span><span class="sxs-lookup"><span data-stu-id="90936-131">Type</span></span>   |<span data-ttu-id="90936-132">说明</span><span class="sxs-lookup"><span data-stu-id="90936-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90936-133">format</span><span class="sxs-lookup"><span data-stu-id="90936-133">format</span></span>|[<span data-ttu-id="90936-134">workbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="90936-134">workbookChartPointFormat</span></span>](workbookchartpointformat.md)|<span data-ttu-id="90936-135">封装图表点的格式属性。</span><span class="sxs-lookup"><span data-stu-id="90936-135">Encapsulates the format properties chart point.</span></span> <span data-ttu-id="90936-136">只读。</span><span class="sxs-lookup"><span data-stu-id="90936-136">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="90936-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="90936-137">JSON representation</span></span>

<span data-ttu-id="90936-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90936-138">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "format"
    ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPoint"
}-->

```json
{
  "value": "string",
  "id": "string",
  "format": {"@odata.type": "microsoft.graph.workbookChartPointFormat"}
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
  "suppressions": []
}
-->
