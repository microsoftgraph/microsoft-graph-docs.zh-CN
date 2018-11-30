---
title: ChartLegend 资源类型
description: 表示图表中的图例。
ms.openlocfilehash: 9066e69da4100c711f9b0b19165a58d94a8bb142
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008778"
---
# <a name="chartlegend-resource-type"></a><span data-ttu-id="36ccd-103">ChartLegend 资源类型</span><span class="sxs-lookup"><span data-stu-id="36ccd-103">ChartLegend resource type</span></span>

<span data-ttu-id="36ccd-104">表示图表中的图例。</span><span class="sxs-lookup"><span data-stu-id="36ccd-104">Represents the legend in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="36ccd-105">方法</span><span class="sxs-lookup"><span data-stu-id="36ccd-105">Methods</span></span>

| <span data-ttu-id="36ccd-106">方法</span><span class="sxs-lookup"><span data-stu-id="36ccd-106">Method</span></span>           | <span data-ttu-id="36ccd-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="36ccd-107">Return Type</span></span>    |<span data-ttu-id="36ccd-108">说明</span><span class="sxs-lookup"><span data-stu-id="36ccd-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="36ccd-109">获取 ChartLegend</span><span class="sxs-lookup"><span data-stu-id="36ccd-109">Get ChartLegend</span></span>](../api/chartlegend-get.md) | [<span data-ttu-id="36ccd-110">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="36ccd-110">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="36ccd-111">读取 chartlegend 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="36ccd-111">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="36ccd-112">Update</span><span class="sxs-lookup"><span data-stu-id="36ccd-112">Update</span></span>](../api/chartlegend-update.md) | [<span data-ttu-id="36ccd-113">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="36ccd-113">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="36ccd-114">更新 chartlegend 对象。</span><span class="sxs-lookup"><span data-stu-id="36ccd-114">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="36ccd-115">属性</span><span class="sxs-lookup"><span data-stu-id="36ccd-115">Properties</span></span>
| <span data-ttu-id="36ccd-116">属性</span><span class="sxs-lookup"><span data-stu-id="36ccd-116">Property</span></span>     | <span data-ttu-id="36ccd-117">类型</span><span class="sxs-lookup"><span data-stu-id="36ccd-117">Type</span></span>   |<span data-ttu-id="36ccd-118">说明</span><span class="sxs-lookup"><span data-stu-id="36ccd-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36ccd-119">overlay</span><span class="sxs-lookup"><span data-stu-id="36ccd-119">overlay</span></span>|<span data-ttu-id="36ccd-120">boolean</span><span class="sxs-lookup"><span data-stu-id="36ccd-120">boolean</span></span>|<span data-ttu-id="36ccd-121">表示图表图例是否应该与图表主体重叠的布尔值。</span><span class="sxs-lookup"><span data-stu-id="36ccd-121">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="36ccd-122">position</span><span class="sxs-lookup"><span data-stu-id="36ccd-122">position</span></span>|<span data-ttu-id="36ccd-123">string</span><span class="sxs-lookup"><span data-stu-id="36ccd-123">string</span></span>|<span data-ttu-id="36ccd-124">代表图表上图例的位置。</span><span class="sxs-lookup"><span data-stu-id="36ccd-124">Represents the position of the legend on the chart.</span></span> <span data-ttu-id="36ccd-125">可能的值为： `Top`， `Bottom`， `Left`， `Right`， `Corner`， `Custom`。</span><span class="sxs-lookup"><span data-stu-id="36ccd-125">The possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="36ccd-126">visible</span><span class="sxs-lookup"><span data-stu-id="36ccd-126">visible</span></span>|<span data-ttu-id="36ccd-127">boolean</span><span class="sxs-lookup"><span data-stu-id="36ccd-127">boolean</span></span>|<span data-ttu-id="36ccd-128">表示 ChartLegend 对象的可见性的布尔值。</span><span class="sxs-lookup"><span data-stu-id="36ccd-128">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="36ccd-129">Relationships</span><span class="sxs-lookup"><span data-stu-id="36ccd-129">Relationships</span></span>
| <span data-ttu-id="36ccd-130">关系</span><span class="sxs-lookup"><span data-stu-id="36ccd-130">Relationship</span></span> | <span data-ttu-id="36ccd-131">类型</span><span class="sxs-lookup"><span data-stu-id="36ccd-131">Type</span></span>   |<span data-ttu-id="36ccd-132">说明</span><span class="sxs-lookup"><span data-stu-id="36ccd-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36ccd-133">format</span><span class="sxs-lookup"><span data-stu-id="36ccd-133">format</span></span>|[<span data-ttu-id="36ccd-134">WorkbookChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="36ccd-134">WorkbookChartLegendFormat</span></span>](chartlegendformat.md)|<span data-ttu-id="36ccd-p102">表示图表图例的格式，包括填充和字体格式。只读。</span><span class="sxs-lookup"><span data-stu-id="36ccd-p102">Represents the formatting of a chart legend, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="36ccd-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="36ccd-137">JSON representation</span></span>

<span data-ttu-id="36ccd-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="36ccd-138">Here is a JSON representation of the resource.</span></span>

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