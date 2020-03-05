---
title: workbookChartLegend 资源类型
description: 表示图表中的图例。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 60d37ab606668fbe6828293112997980c7e4580c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519307"
---
# <a name="workbookchartlegend-resource-type"></a><span data-ttu-id="0fb6d-103">workbookChartLegend 资源类型</span><span class="sxs-lookup"><span data-stu-id="0fb6d-103">workbookChartLegend resource type</span></span>

<span data-ttu-id="0fb6d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0fb6d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0fb6d-105">表示图表中的图例。</span><span class="sxs-lookup"><span data-stu-id="0fb6d-105">Represents the legend in a chart.</span></span>

## <a name="methods"></a><span data-ttu-id="0fb6d-106">方法</span><span class="sxs-lookup"><span data-stu-id="0fb6d-106">Methods</span></span>

| <span data-ttu-id="0fb6d-107">方法</span><span class="sxs-lookup"><span data-stu-id="0fb6d-107">Method</span></span>           | <span data-ttu-id="0fb6d-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="0fb6d-108">Return Type</span></span>    |<span data-ttu-id="0fb6d-109">说明</span><span class="sxs-lookup"><span data-stu-id="0fb6d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0fb6d-110">获取 workbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="0fb6d-110">Get workbookChartLegend</span></span>](../api/chartlegend-get.md) | [<span data-ttu-id="0fb6d-111">workbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="0fb6d-111">workbookChartLegend</span></span>](workbookchartlegend.md) |<span data-ttu-id="0fb6d-112">读取 chartlegend 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0fb6d-112">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="0fb6d-113">更新</span><span class="sxs-lookup"><span data-stu-id="0fb6d-113">Update</span></span>](../api/chartlegend-update.md) | [<span data-ttu-id="0fb6d-114">workbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="0fb6d-114">workbookChartLegend</span></span>](workbookchartlegend.md) |<span data-ttu-id="0fb6d-115">更新 chartlegend 对象。</span><span class="sxs-lookup"><span data-stu-id="0fb6d-115">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0fb6d-116">属性</span><span class="sxs-lookup"><span data-stu-id="0fb6d-116">Properties</span></span>
| <span data-ttu-id="0fb6d-117">属性</span><span class="sxs-lookup"><span data-stu-id="0fb6d-117">Property</span></span>     | <span data-ttu-id="0fb6d-118">类型</span><span class="sxs-lookup"><span data-stu-id="0fb6d-118">Type</span></span>   |<span data-ttu-id="0fb6d-119">说明</span><span class="sxs-lookup"><span data-stu-id="0fb6d-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0fb6d-120">overlay</span><span class="sxs-lookup"><span data-stu-id="0fb6d-120">overlay</span></span>|<span data-ttu-id="0fb6d-121">布尔</span><span class="sxs-lookup"><span data-stu-id="0fb6d-121">boolean</span></span>|<span data-ttu-id="0fb6d-122">表示图表图例是否应该与图表主体重叠的布尔值。</span><span class="sxs-lookup"><span data-stu-id="0fb6d-122">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="0fb6d-123">position</span><span class="sxs-lookup"><span data-stu-id="0fb6d-123">position</span></span>|<span data-ttu-id="0fb6d-124">string</span><span class="sxs-lookup"><span data-stu-id="0fb6d-124">string</span></span>|<span data-ttu-id="0fb6d-125">表示图例在图表上的位置。</span><span class="sxs-lookup"><span data-stu-id="0fb6d-125">Represents the position of the legend on the chart.</span></span> <span data-ttu-id="0fb6d-126">可能的值包括 `Top`、`Bottom`、`Left`、`Right`、`Corner`、`Custom`。</span><span class="sxs-lookup"><span data-stu-id="0fb6d-126">The possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="0fb6d-127">visible</span><span class="sxs-lookup"><span data-stu-id="0fb6d-127">visible</span></span>|<span data-ttu-id="0fb6d-128">布尔</span><span class="sxs-lookup"><span data-stu-id="0fb6d-128">boolean</span></span>|<span data-ttu-id="0fb6d-129">表示 ChartLegend 对象的可见性的布尔值。</span><span class="sxs-lookup"><span data-stu-id="0fb6d-129">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0fb6d-130">关系</span><span class="sxs-lookup"><span data-stu-id="0fb6d-130">Relationships</span></span>
| <span data-ttu-id="0fb6d-131">关系</span><span class="sxs-lookup"><span data-stu-id="0fb6d-131">Relationship</span></span> | <span data-ttu-id="0fb6d-132">类型</span><span class="sxs-lookup"><span data-stu-id="0fb6d-132">Type</span></span>   |<span data-ttu-id="0fb6d-133">说明</span><span class="sxs-lookup"><span data-stu-id="0fb6d-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0fb6d-134">format</span><span class="sxs-lookup"><span data-stu-id="0fb6d-134">format</span></span>|[<span data-ttu-id="0fb6d-135">workbookChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="0fb6d-135">workbookChartLegendFormat</span></span>](workbookchartlegendformat.md)|<span data-ttu-id="0fb6d-136">表示图表图例的格式，包括填充和字体格式。</span><span class="sxs-lookup"><span data-stu-id="0fb6d-136">Represents the formatting of a chart legend, which includes fill and font formatting.</span></span> <span data-ttu-id="0fb6d-137">只读。</span><span class="sxs-lookup"><span data-stu-id="0fb6d-137">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0fb6d-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0fb6d-138">JSON representation</span></span>

<span data-ttu-id="0fb6d-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0fb6d-139">Here is a JSON representation of the resource.</span></span>

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
