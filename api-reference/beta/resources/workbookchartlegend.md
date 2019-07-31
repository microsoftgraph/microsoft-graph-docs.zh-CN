---
title: workbookChartLegend 资源类型
description: 表示图表中的图例。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 42414f0089cf3e33529796ebbeb53b95bc1d4ef2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964022"
---
# <a name="workbookchartlegend-resource-type"></a><span data-ttu-id="5e796-103">workbookChartLegend 资源类型</span><span class="sxs-lookup"><span data-stu-id="5e796-103">workbookChartLegend resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e796-104">表示图表中的图例。</span><span class="sxs-lookup"><span data-stu-id="5e796-104">Represents the legend in a chart.</span></span>

## <a name="methods"></a><span data-ttu-id="5e796-105">方法</span><span class="sxs-lookup"><span data-stu-id="5e796-105">Methods</span></span>

| <span data-ttu-id="5e796-106">方法</span><span class="sxs-lookup"><span data-stu-id="5e796-106">Method</span></span>           | <span data-ttu-id="5e796-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="5e796-107">Return Type</span></span>    |<span data-ttu-id="5e796-108">说明</span><span class="sxs-lookup"><span data-stu-id="5e796-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5e796-109">获取 workbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="5e796-109">Get workbookChartLegend</span></span>](../api/chartlegend-get.md) | [<span data-ttu-id="5e796-110">workbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="5e796-110">workbookChartLegend</span></span>](workbookchartlegend.md) |<span data-ttu-id="5e796-111">读取 chartlegend 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5e796-111">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="5e796-112">更新</span><span class="sxs-lookup"><span data-stu-id="5e796-112">Update</span></span>](../api/chartlegend-update.md) | [<span data-ttu-id="5e796-113">workbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="5e796-113">workbookChartLegend</span></span>](workbookchartlegend.md) |<span data-ttu-id="5e796-114">更新 chartlegend 对象。</span><span class="sxs-lookup"><span data-stu-id="5e796-114">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5e796-115">属性</span><span class="sxs-lookup"><span data-stu-id="5e796-115">Properties</span></span>
| <span data-ttu-id="5e796-116">属性</span><span class="sxs-lookup"><span data-stu-id="5e796-116">Property</span></span>     | <span data-ttu-id="5e796-117">类型</span><span class="sxs-lookup"><span data-stu-id="5e796-117">Type</span></span>   |<span data-ttu-id="5e796-118">说明</span><span class="sxs-lookup"><span data-stu-id="5e796-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e796-119">overlay</span><span class="sxs-lookup"><span data-stu-id="5e796-119">overlay</span></span>|<span data-ttu-id="5e796-120">布尔</span><span class="sxs-lookup"><span data-stu-id="5e796-120">boolean</span></span>|<span data-ttu-id="5e796-121">表示图表图例是否应该与图表主体重叠的布尔值。</span><span class="sxs-lookup"><span data-stu-id="5e796-121">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="5e796-122">position</span><span class="sxs-lookup"><span data-stu-id="5e796-122">position</span></span>|<span data-ttu-id="5e796-123">string</span><span class="sxs-lookup"><span data-stu-id="5e796-123">string</span></span>|<span data-ttu-id="5e796-124">表示图例在图表上的位置。</span><span class="sxs-lookup"><span data-stu-id="5e796-124">Represents the position of the legend on the chart.</span></span> <span data-ttu-id="5e796-125">可能的值包括 `Top`、`Bottom`、`Left`、`Right`、`Corner`、`Custom`。</span><span class="sxs-lookup"><span data-stu-id="5e796-125">The possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="5e796-126">visible</span><span class="sxs-lookup"><span data-stu-id="5e796-126">visible</span></span>|<span data-ttu-id="5e796-127">布尔</span><span class="sxs-lookup"><span data-stu-id="5e796-127">boolean</span></span>|<span data-ttu-id="5e796-128">表示 ChartLegend 对象的可见性的布尔值。</span><span class="sxs-lookup"><span data-stu-id="5e796-128">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e796-129">关系</span><span class="sxs-lookup"><span data-stu-id="5e796-129">Relationships</span></span>
| <span data-ttu-id="5e796-130">关系</span><span class="sxs-lookup"><span data-stu-id="5e796-130">Relationship</span></span> | <span data-ttu-id="5e796-131">类型</span><span class="sxs-lookup"><span data-stu-id="5e796-131">Type</span></span>   |<span data-ttu-id="5e796-132">说明</span><span class="sxs-lookup"><span data-stu-id="5e796-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e796-133">format</span><span class="sxs-lookup"><span data-stu-id="5e796-133">format</span></span>|[<span data-ttu-id="5e796-134">workbookChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="5e796-134">workbookChartLegendFormat</span></span>](workbookchartlegendformat.md)|<span data-ttu-id="5e796-135">表示图表图例的格式，包括填充和字体格式。</span><span class="sxs-lookup"><span data-stu-id="5e796-135">Represents the formatting of a chart legend, which includes fill and font formatting.</span></span> <span data-ttu-id="5e796-136">只读。</span><span class="sxs-lookup"><span data-stu-id="5e796-136">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5e796-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5e796-137">JSON representation</span></span>

<span data-ttu-id="5e796-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e796-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [
    "format"        
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartLegend resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
