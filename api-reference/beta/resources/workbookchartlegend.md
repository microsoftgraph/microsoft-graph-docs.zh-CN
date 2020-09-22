---
title: workbookChartLegend 资源类型
description: 表示图表中的图例。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: dc269a041358a8b85a97224fa1bc880a38fa91e6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971457"
---
# <a name="workbookchartlegend-resource-type"></a><span data-ttu-id="8ae84-103">workbookChartLegend 资源类型</span><span class="sxs-lookup"><span data-stu-id="8ae84-103">workbookChartLegend resource type</span></span>

<span data-ttu-id="8ae84-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ae84-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ae84-105">表示图表中的图例。</span><span class="sxs-lookup"><span data-stu-id="8ae84-105">Represents the legend in a chart.</span></span>

## <a name="methods"></a><span data-ttu-id="8ae84-106">方法</span><span class="sxs-lookup"><span data-stu-id="8ae84-106">Methods</span></span>

| <span data-ttu-id="8ae84-107">方法</span><span class="sxs-lookup"><span data-stu-id="8ae84-107">Method</span></span>           | <span data-ttu-id="8ae84-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="8ae84-108">Return Type</span></span>    |<span data-ttu-id="8ae84-109">说明</span><span class="sxs-lookup"><span data-stu-id="8ae84-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8ae84-110">获取 workbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="8ae84-110">Get workbookChartLegend</span></span>](../api/chartlegend-get.md) | [<span data-ttu-id="8ae84-111">workbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="8ae84-111">workbookChartLegend</span></span>](workbookchartlegend.md) |<span data-ttu-id="8ae84-112">读取 chartlegend 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8ae84-112">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="8ae84-113">更新</span><span class="sxs-lookup"><span data-stu-id="8ae84-113">Update</span></span>](../api/chartlegend-update.md) | [<span data-ttu-id="8ae84-114">workbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="8ae84-114">workbookChartLegend</span></span>](workbookchartlegend.md) |<span data-ttu-id="8ae84-115">更新 chartlegend 对象。</span><span class="sxs-lookup"><span data-stu-id="8ae84-115">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8ae84-116">属性</span><span class="sxs-lookup"><span data-stu-id="8ae84-116">Properties</span></span>
| <span data-ttu-id="8ae84-117">属性</span><span class="sxs-lookup"><span data-stu-id="8ae84-117">Property</span></span>     | <span data-ttu-id="8ae84-118">类型</span><span class="sxs-lookup"><span data-stu-id="8ae84-118">Type</span></span>   |<span data-ttu-id="8ae84-119">说明</span><span class="sxs-lookup"><span data-stu-id="8ae84-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ae84-120">overlay</span><span class="sxs-lookup"><span data-stu-id="8ae84-120">overlay</span></span>|<span data-ttu-id="8ae84-121">布尔</span><span class="sxs-lookup"><span data-stu-id="8ae84-121">boolean</span></span>|<span data-ttu-id="8ae84-122">表示图表图例是否应该与图表主体重叠的布尔值。</span><span class="sxs-lookup"><span data-stu-id="8ae84-122">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="8ae84-123">position</span><span class="sxs-lookup"><span data-stu-id="8ae84-123">position</span></span>|<span data-ttu-id="8ae84-124">string</span><span class="sxs-lookup"><span data-stu-id="8ae84-124">string</span></span>|<span data-ttu-id="8ae84-125">表示图例在图表上的位置。</span><span class="sxs-lookup"><span data-stu-id="8ae84-125">Represents the position of the legend on the chart.</span></span> <span data-ttu-id="8ae84-126">可能的值包括 `Top`、`Bottom`、`Left`、`Right`、`Corner`、`Custom`。</span><span class="sxs-lookup"><span data-stu-id="8ae84-126">The possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="8ae84-127">visible</span><span class="sxs-lookup"><span data-stu-id="8ae84-127">visible</span></span>|<span data-ttu-id="8ae84-128">布尔</span><span class="sxs-lookup"><span data-stu-id="8ae84-128">boolean</span></span>|<span data-ttu-id="8ae84-129">表示 ChartLegend 对象的可见性的布尔值。</span><span class="sxs-lookup"><span data-stu-id="8ae84-129">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ae84-130">关系</span><span class="sxs-lookup"><span data-stu-id="8ae84-130">Relationships</span></span>
| <span data-ttu-id="8ae84-131">关系</span><span class="sxs-lookup"><span data-stu-id="8ae84-131">Relationship</span></span> | <span data-ttu-id="8ae84-132">类型</span><span class="sxs-lookup"><span data-stu-id="8ae84-132">Type</span></span>   |<span data-ttu-id="8ae84-133">说明</span><span class="sxs-lookup"><span data-stu-id="8ae84-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ae84-134">format</span><span class="sxs-lookup"><span data-stu-id="8ae84-134">format</span></span>|[<span data-ttu-id="8ae84-135">workbookChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="8ae84-135">workbookChartLegendFormat</span></span>](workbookchartlegendformat.md)|<span data-ttu-id="8ae84-136">表示图表图例的格式，包括填充和字体格式。</span><span class="sxs-lookup"><span data-stu-id="8ae84-136">Represents the formatting of a chart legend, which includes fill and font formatting.</span></span> <span data-ttu-id="8ae84-137">只读。</span><span class="sxs-lookup"><span data-stu-id="8ae84-137">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8ae84-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8ae84-138">JSON representation</span></span>

<span data-ttu-id="8ae84-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8ae84-139">Here is a JSON representation of the resource.</span></span>

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


