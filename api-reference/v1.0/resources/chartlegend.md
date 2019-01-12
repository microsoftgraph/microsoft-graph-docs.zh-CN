---
title: ChartLegend 资源类型
description: 表示图表中的图例。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 8eea71707d622f0dc28cc8072fa984de64a8427f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967222"
---
# <a name="chartlegend-resource-type"></a><span data-ttu-id="32464-103">ChartLegend 资源类型</span><span class="sxs-lookup"><span data-stu-id="32464-103">ChartLegend resource type</span></span>

<span data-ttu-id="32464-104">表示图表中的图例。</span><span class="sxs-lookup"><span data-stu-id="32464-104">Represents the legend in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="32464-105">方法</span><span class="sxs-lookup"><span data-stu-id="32464-105">Methods</span></span>

| <span data-ttu-id="32464-106">方法</span><span class="sxs-lookup"><span data-stu-id="32464-106">Method</span></span>           | <span data-ttu-id="32464-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="32464-107">Return Type</span></span>    |<span data-ttu-id="32464-108">说明</span><span class="sxs-lookup"><span data-stu-id="32464-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="32464-109">获取 ChartLegend</span><span class="sxs-lookup"><span data-stu-id="32464-109">Get ChartLegend</span></span>](../api/chartlegend-get.md) | [<span data-ttu-id="32464-110">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="32464-110">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="32464-111">读取 chartlegend 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="32464-111">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="32464-112">Update</span><span class="sxs-lookup"><span data-stu-id="32464-112">Update</span></span>](../api/chartlegend-update.md) | [<span data-ttu-id="32464-113">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="32464-113">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="32464-114">更新 chartlegend 对象。</span><span class="sxs-lookup"><span data-stu-id="32464-114">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="32464-115">属性</span><span class="sxs-lookup"><span data-stu-id="32464-115">Properties</span></span>
| <span data-ttu-id="32464-116">属性</span><span class="sxs-lookup"><span data-stu-id="32464-116">Property</span></span>     | <span data-ttu-id="32464-117">类型</span><span class="sxs-lookup"><span data-stu-id="32464-117">Type</span></span>   |<span data-ttu-id="32464-118">说明</span><span class="sxs-lookup"><span data-stu-id="32464-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32464-119">overlay</span><span class="sxs-lookup"><span data-stu-id="32464-119">overlay</span></span>|<span data-ttu-id="32464-120">boolean</span><span class="sxs-lookup"><span data-stu-id="32464-120">boolean</span></span>|<span data-ttu-id="32464-121">表示图表图例是否应该与图表主体重叠的布尔值。</span><span class="sxs-lookup"><span data-stu-id="32464-121">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="32464-122">position</span><span class="sxs-lookup"><span data-stu-id="32464-122">position</span></span>|<span data-ttu-id="32464-123">string</span><span class="sxs-lookup"><span data-stu-id="32464-123">string</span></span>|<span data-ttu-id="32464-124">代表图表上图例的位置。</span><span class="sxs-lookup"><span data-stu-id="32464-124">Represents the position of the legend on the chart.</span></span> <span data-ttu-id="32464-125">可能的值为： `Top`， `Bottom`， `Left`， `Right`， `Corner`， `Custom`。</span><span class="sxs-lookup"><span data-stu-id="32464-125">The possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="32464-126">visible</span><span class="sxs-lookup"><span data-stu-id="32464-126">visible</span></span>|<span data-ttu-id="32464-127">boolean</span><span class="sxs-lookup"><span data-stu-id="32464-127">boolean</span></span>|<span data-ttu-id="32464-128">表示 ChartLegend 对象的可见性的布尔值。</span><span class="sxs-lookup"><span data-stu-id="32464-128">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="32464-129">Relationships</span><span class="sxs-lookup"><span data-stu-id="32464-129">Relationships</span></span>
| <span data-ttu-id="32464-130">关系</span><span class="sxs-lookup"><span data-stu-id="32464-130">Relationship</span></span> | <span data-ttu-id="32464-131">类型</span><span class="sxs-lookup"><span data-stu-id="32464-131">Type</span></span>   |<span data-ttu-id="32464-132">说明</span><span class="sxs-lookup"><span data-stu-id="32464-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32464-133">format</span><span class="sxs-lookup"><span data-stu-id="32464-133">format</span></span>|[<span data-ttu-id="32464-134">WorkbookChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="32464-134">WorkbookChartLegendFormat</span></span>](chartlegendformat.md)|<span data-ttu-id="32464-p102">表示图表图例的格式，包括填充和字体格式。只读。</span><span class="sxs-lookup"><span data-stu-id="32464-p102">Represents the formatting of a chart legend, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="32464-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="32464-137">JSON representation</span></span>

<span data-ttu-id="32464-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32464-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartLegend"
}-->

```json
{
  "overlay": true,
  "position": "string",
  "visible": true,
  "format": {"@odata.type":"microsoft.graph.workbookChartLegendFormat"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLegend resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
