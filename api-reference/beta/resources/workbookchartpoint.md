---
title: workbookChartPoint 资源类型
description: 表示图表中某个系列的点。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 54342227c15eeb1b11c3ddfb157e1ef3bc83390e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519286"
---
# <a name="workbookchartpoint-resource-type"></a><span data-ttu-id="7ee7e-103">workbookChartPoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="7ee7e-103">workbookChartPoint resource type</span></span>

<span data-ttu-id="7ee7e-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="7ee7e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ee7e-105">表示图表中某个系列的点。</span><span class="sxs-lookup"><span data-stu-id="7ee7e-105">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="7ee7e-106">方法</span><span class="sxs-lookup"><span data-stu-id="7ee7e-106">Methods</span></span>

| <span data-ttu-id="7ee7e-107">方法</span><span class="sxs-lookup"><span data-stu-id="7ee7e-107">Method</span></span>           | <span data-ttu-id="7ee7e-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="7ee7e-108">Return Type</span></span>    |<span data-ttu-id="7ee7e-109">说明</span><span class="sxs-lookup"><span data-stu-id="7ee7e-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7ee7e-110">获取 workbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="7ee7e-110">Get workbookChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="7ee7e-111">workbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="7ee7e-111">workbookChartPoint</span></span>](workbookchartpoint.md) |<span data-ttu-id="7ee7e-112">读取 chartPoint 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7ee7e-112">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="7ee7e-113">列出</span><span class="sxs-lookup"><span data-stu-id="7ee7e-113">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="7ee7e-114">[workbookChartPoint](workbookchartpoint.md)集合</span><span class="sxs-lookup"><span data-stu-id="7ee7e-114">[workbookChartPoint](workbookchartpoint.md) collection</span></span> |<span data-ttu-id="7ee7e-115">获取 chartPoint 对象集合。</span><span class="sxs-lookup"><span data-stu-id="7ee7e-115">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="7ee7e-116">ItemAt</span><span class="sxs-lookup"><span data-stu-id="7ee7e-116">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="7ee7e-117">workbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="7ee7e-117">workbookChartPoint</span></span>](workbookchartpoint.md)|<span data-ttu-id="7ee7e-118">根据其在系列中的位置检索点。</span><span class="sxs-lookup"><span data-stu-id="7ee7e-118">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="7ee7e-119">属性</span><span class="sxs-lookup"><span data-stu-id="7ee7e-119">Properties</span></span>
| <span data-ttu-id="7ee7e-120">属性</span><span class="sxs-lookup"><span data-stu-id="7ee7e-120">Property</span></span>     | <span data-ttu-id="7ee7e-121">类型</span><span class="sxs-lookup"><span data-stu-id="7ee7e-121">Type</span></span>   |<span data-ttu-id="7ee7e-122">说明</span><span class="sxs-lookup"><span data-stu-id="7ee7e-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7ee7e-123">值</span><span class="sxs-lookup"><span data-stu-id="7ee7e-123">value</span></span>|<span data-ttu-id="7ee7e-124">Json</span><span class="sxs-lookup"><span data-stu-id="7ee7e-124">Json</span></span>|<span data-ttu-id="7ee7e-125">返回图表点的值。</span><span class="sxs-lookup"><span data-stu-id="7ee7e-125">Returns the value of a chart point.</span></span> <span data-ttu-id="7ee7e-126">只读。</span><span class="sxs-lookup"><span data-stu-id="7ee7e-126">Read-only.</span></span>|
|<span data-ttu-id="7ee7e-127">id</span><span class="sxs-lookup"><span data-stu-id="7ee7e-127">id</span></span>|<span data-ttu-id="7ee7e-128">string</span><span class="sxs-lookup"><span data-stu-id="7ee7e-128">string</span></span>|<span data-ttu-id="7ee7e-129">唯一标识符</span><span class="sxs-lookup"><span data-stu-id="7ee7e-129">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ee7e-130">关系</span><span class="sxs-lookup"><span data-stu-id="7ee7e-130">Relationships</span></span>
| <span data-ttu-id="7ee7e-131">关系</span><span class="sxs-lookup"><span data-stu-id="7ee7e-131">Relationship</span></span> | <span data-ttu-id="7ee7e-132">类型</span><span class="sxs-lookup"><span data-stu-id="7ee7e-132">Type</span></span>   |<span data-ttu-id="7ee7e-133">说明</span><span class="sxs-lookup"><span data-stu-id="7ee7e-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7ee7e-134">format</span><span class="sxs-lookup"><span data-stu-id="7ee7e-134">format</span></span>|[<span data-ttu-id="7ee7e-135">workbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="7ee7e-135">workbookChartPointFormat</span></span>](workbookchartpointformat.md)|<span data-ttu-id="7ee7e-136">封装图表点的格式属性。</span><span class="sxs-lookup"><span data-stu-id="7ee7e-136">Encapsulates the format properties chart point.</span></span> <span data-ttu-id="7ee7e-137">只读。</span><span class="sxs-lookup"><span data-stu-id="7ee7e-137">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7ee7e-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ee7e-138">JSON representation</span></span>

<span data-ttu-id="7ee7e-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ee7e-139">Here is a JSON representation of the resource.</span></span>

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
