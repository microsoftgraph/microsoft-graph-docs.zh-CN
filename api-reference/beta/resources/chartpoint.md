---
title: ChartPoint 资源类型
description: 表示图表中某个系列的点。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: e8ede39ef53bfc39574ebfc86c8138a70fc31ad6
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573065"
---
# <a name="chartpoint-resource-type"></a><span data-ttu-id="cffad-103">ChartPoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="cffad-103">ChartPoint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cffad-104">表示图表中某个系列的点。</span><span class="sxs-lookup"><span data-stu-id="cffad-104">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="cffad-105">方法</span><span class="sxs-lookup"><span data-stu-id="cffad-105">Methods</span></span>

| <span data-ttu-id="cffad-106">方法</span><span class="sxs-lookup"><span data-stu-id="cffad-106">Method</span></span>           | <span data-ttu-id="cffad-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="cffad-107">Return Type</span></span>    |<span data-ttu-id="cffad-108">说明</span><span class="sxs-lookup"><span data-stu-id="cffad-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cffad-109">获取 ChartPoint</span><span class="sxs-lookup"><span data-stu-id="cffad-109">Get ChartPoint</span></span>](../api/chartpoint-get.md) | [<span data-ttu-id="cffad-110">workbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="cffad-110">workbookChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="cffad-111">读取 chartPoint 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cffad-111">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="cffad-112">List</span><span class="sxs-lookup"><span data-stu-id="cffad-112">List</span></span>](../api/chartpoint-list.md) | <span data-ttu-id="cffad-113">[workbookChartPoint](chartpoint.md)集合</span><span class="sxs-lookup"><span data-stu-id="cffad-113">[workbookChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="cffad-114">获取 chartPoint 对象集合。</span><span class="sxs-lookup"><span data-stu-id="cffad-114">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="cffad-115">ItemAt</span><span class="sxs-lookup"><span data-stu-id="cffad-115">ItemAt</span></span>](../api/chartpointscollection-itemat.md)|[<span data-ttu-id="cffad-116">workbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="cffad-116">workbookChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="cffad-117">根据其在系列中的位置检索点。</span><span class="sxs-lookup"><span data-stu-id="cffad-117">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="cffad-118">属性</span><span class="sxs-lookup"><span data-stu-id="cffad-118">Properties</span></span>
| <span data-ttu-id="cffad-119">属性</span><span class="sxs-lookup"><span data-stu-id="cffad-119">Property</span></span>     | <span data-ttu-id="cffad-120">类型</span><span class="sxs-lookup"><span data-stu-id="cffad-120">Type</span></span>   |<span data-ttu-id="cffad-121">说明</span><span class="sxs-lookup"><span data-stu-id="cffad-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cffad-122">value</span><span class="sxs-lookup"><span data-stu-id="cffad-122">value</span></span>|<span data-ttu-id="cffad-123">Json</span><span class="sxs-lookup"><span data-stu-id="cffad-123">Json</span></span>|<span data-ttu-id="cffad-p101">返回图表点的值。只读。</span><span class="sxs-lookup"><span data-stu-id="cffad-p101">Returns the value of a chart point. Read-only.</span></span>|
|<span data-ttu-id="cffad-126">id</span><span class="sxs-lookup"><span data-stu-id="cffad-126">id</span></span>|<span data-ttu-id="cffad-127">string</span><span class="sxs-lookup"><span data-stu-id="cffad-127">string</span></span>|<span data-ttu-id="cffad-128">唯一标识符</span><span class="sxs-lookup"><span data-stu-id="cffad-128">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="cffad-129">关系</span><span class="sxs-lookup"><span data-stu-id="cffad-129">Relationships</span></span>
| <span data-ttu-id="cffad-130">关系</span><span class="sxs-lookup"><span data-stu-id="cffad-130">Relationship</span></span> | <span data-ttu-id="cffad-131">类型</span><span class="sxs-lookup"><span data-stu-id="cffad-131">Type</span></span>   |<span data-ttu-id="cffad-132">说明</span><span class="sxs-lookup"><span data-stu-id="cffad-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cffad-133">format</span><span class="sxs-lookup"><span data-stu-id="cffad-133">format</span></span>|[<span data-ttu-id="cffad-134">workbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="cffad-134">workbookChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="cffad-p102">封装图表点的格式属性。只读。</span><span class="sxs-lookup"><span data-stu-id="cffad-p102">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cffad-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cffad-137">JSON representation</span></span>

<span data-ttu-id="cffad-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cffad-138">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartpoint.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
