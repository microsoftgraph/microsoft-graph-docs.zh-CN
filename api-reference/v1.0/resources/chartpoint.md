---
title: ChartPoint 资源类型
description: 表示图表中某个系列的点。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3318415094a36100851b1c604cba2507de31f558
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569086"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="caee5-103">ChartPoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="caee5-103">ChartPoint resource type</span></span>

<span data-ttu-id="caee5-104">表示图表中某个系列的点。</span><span class="sxs-lookup"><span data-stu-id="caee5-104">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="caee5-105">方法</span><span class="sxs-lookup"><span data-stu-id="caee5-105">Methods</span></span>

| <span data-ttu-id="caee5-106">方法</span><span class="sxs-lookup"><span data-stu-id="caee5-106">Method</span></span>           | <span data-ttu-id="caee5-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="caee5-107">Return Type</span></span>    |<span data-ttu-id="caee5-108">说明</span><span class="sxs-lookup"><span data-stu-id="caee5-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="caee5-109">获取 ChartPoint</span><span class="sxs-lookup"><span data-stu-id="caee5-109">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="caee5-110">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="caee5-110">WorkbookChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="caee5-111">读取 chartPoint 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="caee5-111">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="caee5-112">列出</span><span class="sxs-lookup"><span data-stu-id="caee5-112">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="caee5-113">[WorkbookChartPoint](chartpoint.md)集合</span><span class="sxs-lookup"><span data-stu-id="caee5-113">[WorkbookChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="caee5-114">获取 chartPoint 对象集合。</span><span class="sxs-lookup"><span data-stu-id="caee5-114">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="caee5-115">ItemAt</span><span class="sxs-lookup"><span data-stu-id="caee5-115">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="caee5-116">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="caee5-116">WorkbookChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="caee5-117">根据其在系列中的位置检索点。</span><span class="sxs-lookup"><span data-stu-id="caee5-117">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="caee5-118">属性</span><span class="sxs-lookup"><span data-stu-id="caee5-118">Properties</span></span>
| <span data-ttu-id="caee5-119">属性</span><span class="sxs-lookup"><span data-stu-id="caee5-119">Property</span></span>     | <span data-ttu-id="caee5-120">类型</span><span class="sxs-lookup"><span data-stu-id="caee5-120">Type</span></span>   |<span data-ttu-id="caee5-121">说明</span><span class="sxs-lookup"><span data-stu-id="caee5-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="caee5-122">值</span><span class="sxs-lookup"><span data-stu-id="caee5-122">value</span></span>|<span data-ttu-id="caee5-123">Json</span><span class="sxs-lookup"><span data-stu-id="caee5-123">Json</span></span>|<span data-ttu-id="caee5-124">返回图表点的值。</span><span class="sxs-lookup"><span data-stu-id="caee5-124">Returns the value of a chart point.</span></span> <span data-ttu-id="caee5-125">只读。</span><span class="sxs-lookup"><span data-stu-id="caee5-125">Read-only.</span></span>|
|<span data-ttu-id="caee5-126">id</span><span class="sxs-lookup"><span data-stu-id="caee5-126">id</span></span>|<span data-ttu-id="caee5-127">string</span><span class="sxs-lookup"><span data-stu-id="caee5-127">string</span></span>|<span data-ttu-id="caee5-128">唯一标识符</span><span class="sxs-lookup"><span data-stu-id="caee5-128">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="caee5-129">关系</span><span class="sxs-lookup"><span data-stu-id="caee5-129">Relationships</span></span>
| <span data-ttu-id="caee5-130">关系</span><span class="sxs-lookup"><span data-stu-id="caee5-130">Relationship</span></span> | <span data-ttu-id="caee5-131">类型</span><span class="sxs-lookup"><span data-stu-id="caee5-131">Type</span></span>   |<span data-ttu-id="caee5-132">说明</span><span class="sxs-lookup"><span data-stu-id="caee5-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="caee5-133">format</span><span class="sxs-lookup"><span data-stu-id="caee5-133">format</span></span>|[<span data-ttu-id="caee5-134">WorkbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="caee5-134">WorkbookChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="caee5-135">封装图表点的格式属性。</span><span class="sxs-lookup"><span data-stu-id="caee5-135">Encapsulates the format properties chart point.</span></span> <span data-ttu-id="caee5-136">只读。</span><span class="sxs-lookup"><span data-stu-id="caee5-136">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="caee5-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="caee5-137">JSON representation</span></span>

<span data-ttu-id="caee5-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="caee5-138">Here is a JSON representation of the resource.</span></span>

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
