---
title: ChartLegend 资源类型
description: 表示图表中的图例。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 13c054403eb93afce03775138c151e67bc2f57d7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543758"
---
# <a name="chartlegend-resource-type"></a><span data-ttu-id="02eeb-103">ChartLegend 资源类型</span><span class="sxs-lookup"><span data-stu-id="02eeb-103">ChartLegend resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02eeb-104">表示图表中的图例。</span><span class="sxs-lookup"><span data-stu-id="02eeb-104">Represents the legend in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="02eeb-105">方法</span><span class="sxs-lookup"><span data-stu-id="02eeb-105">Methods</span></span>

| <span data-ttu-id="02eeb-106">方法</span><span class="sxs-lookup"><span data-stu-id="02eeb-106">Method</span></span>           | <span data-ttu-id="02eeb-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="02eeb-107">Return Type</span></span>    |<span data-ttu-id="02eeb-108">说明</span><span class="sxs-lookup"><span data-stu-id="02eeb-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="02eeb-109">获取 ChartLegend</span><span class="sxs-lookup"><span data-stu-id="02eeb-109">Get ChartLegend</span></span>](../api/chartlegend-get.md) | [<span data-ttu-id="02eeb-110">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="02eeb-110">ChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="02eeb-111">读取 chartlegend 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="02eeb-111">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="02eeb-112">更新</span><span class="sxs-lookup"><span data-stu-id="02eeb-112">Update</span></span>](../api/chartlegend-update.md) | [<span data-ttu-id="02eeb-113">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="02eeb-113">ChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="02eeb-114">更新 chartlegend 对象。</span><span class="sxs-lookup"><span data-stu-id="02eeb-114">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="02eeb-115">属性</span><span class="sxs-lookup"><span data-stu-id="02eeb-115">Properties</span></span>
| <span data-ttu-id="02eeb-116">属性</span><span class="sxs-lookup"><span data-stu-id="02eeb-116">Property</span></span>     | <span data-ttu-id="02eeb-117">类型</span><span class="sxs-lookup"><span data-stu-id="02eeb-117">Type</span></span>   |<span data-ttu-id="02eeb-118">说明</span><span class="sxs-lookup"><span data-stu-id="02eeb-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02eeb-119">overlay</span><span class="sxs-lookup"><span data-stu-id="02eeb-119">overlay</span></span>|<span data-ttu-id="02eeb-120">布尔</span><span class="sxs-lookup"><span data-stu-id="02eeb-120">boolean</span></span>|<span data-ttu-id="02eeb-121">表示图表图例是否应该与图表主体重叠的布尔值。</span><span class="sxs-lookup"><span data-stu-id="02eeb-121">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="02eeb-122">position</span><span class="sxs-lookup"><span data-stu-id="02eeb-122">position</span></span>|<span data-ttu-id="02eeb-123">string</span><span class="sxs-lookup"><span data-stu-id="02eeb-123">string</span></span>|<span data-ttu-id="02eeb-p101">表示图例在图表上的位置。可能的值是：`Top`、`Bottom`、`Left`、`Right`、`Corner`、`Custom`。</span><span class="sxs-lookup"><span data-stu-id="02eeb-p101">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="02eeb-126">visible</span><span class="sxs-lookup"><span data-stu-id="02eeb-126">visible</span></span>|<span data-ttu-id="02eeb-127">布尔</span><span class="sxs-lookup"><span data-stu-id="02eeb-127">boolean</span></span>|<span data-ttu-id="02eeb-128">表示 ChartLegend 对象的可见性的布尔值。</span><span class="sxs-lookup"><span data-stu-id="02eeb-128">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="02eeb-129">关系</span><span class="sxs-lookup"><span data-stu-id="02eeb-129">Relationships</span></span>
| <span data-ttu-id="02eeb-130">关系</span><span class="sxs-lookup"><span data-stu-id="02eeb-130">Relationship</span></span> | <span data-ttu-id="02eeb-131">类型</span><span class="sxs-lookup"><span data-stu-id="02eeb-131">Type</span></span>   |<span data-ttu-id="02eeb-132">说明</span><span class="sxs-lookup"><span data-stu-id="02eeb-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02eeb-133">format</span><span class="sxs-lookup"><span data-stu-id="02eeb-133">format</span></span>|[<span data-ttu-id="02eeb-134">ChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="02eeb-134">ChartLegendFormat</span></span>](chartlegendformat.md)|<span data-ttu-id="02eeb-p102">表示图表图例的格式，包括填充和字体格式。只读。</span><span class="sxs-lookup"><span data-stu-id="02eeb-p102">Represents the formatting of a chart legend, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="02eeb-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="02eeb-137">JSON representation</span></span>

<span data-ttu-id="02eeb-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="02eeb-138">Here is a JSON representation of the resource.</span></span>

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
