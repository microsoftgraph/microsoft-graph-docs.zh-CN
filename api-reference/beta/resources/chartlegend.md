---
title: ChartLegend 资源类型
description: 表示图表中的图例。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 13c054403eb93afce03775138c151e67bc2f57d7
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640243"
---
# <a name="chartlegend-resource-type"></a><span data-ttu-id="0a66e-103">ChartLegend 资源类型</span><span class="sxs-lookup"><span data-stu-id="0a66e-103">ChartLegend resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a66e-104">表示图表中的图例。</span><span class="sxs-lookup"><span data-stu-id="0a66e-104">Represents the legend in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="0a66e-105">方法</span><span class="sxs-lookup"><span data-stu-id="0a66e-105">Methods</span></span>

| <span data-ttu-id="0a66e-106">方法</span><span class="sxs-lookup"><span data-stu-id="0a66e-106">Method</span></span>           | <span data-ttu-id="0a66e-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="0a66e-107">Return Type</span></span>    |<span data-ttu-id="0a66e-108">说明</span><span class="sxs-lookup"><span data-stu-id="0a66e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0a66e-109">获取 ChartLegend</span><span class="sxs-lookup"><span data-stu-id="0a66e-109">Get ChartLegend</span></span>](../api/chartlegend-get.md) | [<span data-ttu-id="0a66e-110">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="0a66e-110">ChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="0a66e-111">读取 chartlegend 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0a66e-111">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="0a66e-112">更新</span><span class="sxs-lookup"><span data-stu-id="0a66e-112">Update</span></span>](../api/chartlegend-update.md) | [<span data-ttu-id="0a66e-113">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="0a66e-113">ChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="0a66e-114">更新 chartlegend 对象。</span><span class="sxs-lookup"><span data-stu-id="0a66e-114">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0a66e-115">属性</span><span class="sxs-lookup"><span data-stu-id="0a66e-115">Properties</span></span>
| <span data-ttu-id="0a66e-116">属性</span><span class="sxs-lookup"><span data-stu-id="0a66e-116">Property</span></span>     | <span data-ttu-id="0a66e-117">类型</span><span class="sxs-lookup"><span data-stu-id="0a66e-117">Type</span></span>   |<span data-ttu-id="0a66e-118">说明</span><span class="sxs-lookup"><span data-stu-id="0a66e-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a66e-119">overlay</span><span class="sxs-lookup"><span data-stu-id="0a66e-119">overlay</span></span>|<span data-ttu-id="0a66e-120">boolean</span><span class="sxs-lookup"><span data-stu-id="0a66e-120">boolean</span></span>|<span data-ttu-id="0a66e-121">表示图表图例是否应该与图表主体重叠的布尔值。</span><span class="sxs-lookup"><span data-stu-id="0a66e-121">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="0a66e-122">position</span><span class="sxs-lookup"><span data-stu-id="0a66e-122">position</span></span>|<span data-ttu-id="0a66e-123">string</span><span class="sxs-lookup"><span data-stu-id="0a66e-123">string</span></span>|<span data-ttu-id="0a66e-p101">表示图例在图表上的位置。可能的值是：`Top`、`Bottom`、`Left`、`Right`、`Corner`、`Custom`。</span><span class="sxs-lookup"><span data-stu-id="0a66e-p101">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="0a66e-126">visible</span><span class="sxs-lookup"><span data-stu-id="0a66e-126">visible</span></span>|<span data-ttu-id="0a66e-127">boolean</span><span class="sxs-lookup"><span data-stu-id="0a66e-127">boolean</span></span>|<span data-ttu-id="0a66e-128">表示 ChartLegend 对象的可见性的布尔值。</span><span class="sxs-lookup"><span data-stu-id="0a66e-128">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a66e-129">关系</span><span class="sxs-lookup"><span data-stu-id="0a66e-129">Relationships</span></span>
| <span data-ttu-id="0a66e-130">关系</span><span class="sxs-lookup"><span data-stu-id="0a66e-130">Relationship</span></span> | <span data-ttu-id="0a66e-131">类型</span><span class="sxs-lookup"><span data-stu-id="0a66e-131">Type</span></span>   |<span data-ttu-id="0a66e-132">说明</span><span class="sxs-lookup"><span data-stu-id="0a66e-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a66e-133">format</span><span class="sxs-lookup"><span data-stu-id="0a66e-133">format</span></span>|[<span data-ttu-id="0a66e-134">ChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="0a66e-134">ChartLegendFormat</span></span>](chartlegendformat.md)|<span data-ttu-id="0a66e-p102">表示图表图例的格式，包括填充和字体格式。只读。</span><span class="sxs-lookup"><span data-stu-id="0a66e-p102">Represents the formatting of a chart legend, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0a66e-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0a66e-137">JSON representation</span></span>

<span data-ttu-id="0a66e-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0a66e-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartLegend"
}-->

```json
{
  "overlay": true,
  "position": "string",
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartLegend resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartlegend.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
