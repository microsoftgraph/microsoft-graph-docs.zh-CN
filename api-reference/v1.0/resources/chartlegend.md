---
title: ChartLegend 资源类型
description: 表示图表中的图例。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 8b05e4c130eebe3ffc23af2389feb2846ef1474e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069174"
---
# <a name="chartlegend-resource-type"></a><span data-ttu-id="9de13-103">ChartLegend 资源类型</span><span class="sxs-lookup"><span data-stu-id="9de13-103">ChartLegend resource type</span></span>

<span data-ttu-id="9de13-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9de13-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9de13-105">表示图表中的图例。</span><span class="sxs-lookup"><span data-stu-id="9de13-105">Represents the legend in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="9de13-106">方法</span><span class="sxs-lookup"><span data-stu-id="9de13-106">Methods</span></span>

| <span data-ttu-id="9de13-107">方法</span><span class="sxs-lookup"><span data-stu-id="9de13-107">Method</span></span>           | <span data-ttu-id="9de13-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="9de13-108">Return Type</span></span>    |<span data-ttu-id="9de13-109">说明</span><span class="sxs-lookup"><span data-stu-id="9de13-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9de13-110">获取 ChartLegend</span><span class="sxs-lookup"><span data-stu-id="9de13-110">Get ChartLegend</span></span>](../api/chartlegend-get.md) | [<span data-ttu-id="9de13-111">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="9de13-111">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="9de13-112">读取 chartlegend 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9de13-112">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="9de13-113">更新</span><span class="sxs-lookup"><span data-stu-id="9de13-113">Update</span></span>](../api/chartlegend-update.md) | [<span data-ttu-id="9de13-114">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="9de13-114">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="9de13-115">更新 chartlegend 对象。</span><span class="sxs-lookup"><span data-stu-id="9de13-115">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9de13-116">属性</span><span class="sxs-lookup"><span data-stu-id="9de13-116">Properties</span></span>
| <span data-ttu-id="9de13-117">属性</span><span class="sxs-lookup"><span data-stu-id="9de13-117">Property</span></span>     | <span data-ttu-id="9de13-118">类型</span><span class="sxs-lookup"><span data-stu-id="9de13-118">Type</span></span>   |<span data-ttu-id="9de13-119">说明</span><span class="sxs-lookup"><span data-stu-id="9de13-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9de13-120">overlay</span><span class="sxs-lookup"><span data-stu-id="9de13-120">overlay</span></span>|<span data-ttu-id="9de13-121">布尔</span><span class="sxs-lookup"><span data-stu-id="9de13-121">boolean</span></span>|<span data-ttu-id="9de13-122">表示图表图例是否应该与图表主体重叠的布尔值。</span><span class="sxs-lookup"><span data-stu-id="9de13-122">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="9de13-123">position</span><span class="sxs-lookup"><span data-stu-id="9de13-123">position</span></span>|<span data-ttu-id="9de13-124">string</span><span class="sxs-lookup"><span data-stu-id="9de13-124">string</span></span>|<span data-ttu-id="9de13-125">表示图例在图表上的位置。</span><span class="sxs-lookup"><span data-stu-id="9de13-125">Represents the position of the legend on the chart.</span></span> <span data-ttu-id="9de13-126">可能的值包括 `Top`、`Bottom`、`Left`、`Right`、`Corner`、`Custom`。</span><span class="sxs-lookup"><span data-stu-id="9de13-126">The possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="9de13-127">visible</span><span class="sxs-lookup"><span data-stu-id="9de13-127">visible</span></span>|<span data-ttu-id="9de13-128">布尔</span><span class="sxs-lookup"><span data-stu-id="9de13-128">boolean</span></span>|<span data-ttu-id="9de13-129">表示 ChartLegend 对象的可见性的布尔值。</span><span class="sxs-lookup"><span data-stu-id="9de13-129">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9de13-130">关系</span><span class="sxs-lookup"><span data-stu-id="9de13-130">Relationships</span></span>
| <span data-ttu-id="9de13-131">关系</span><span class="sxs-lookup"><span data-stu-id="9de13-131">Relationship</span></span> | <span data-ttu-id="9de13-132">类型</span><span class="sxs-lookup"><span data-stu-id="9de13-132">Type</span></span>   |<span data-ttu-id="9de13-133">说明</span><span class="sxs-lookup"><span data-stu-id="9de13-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9de13-134">format</span><span class="sxs-lookup"><span data-stu-id="9de13-134">format</span></span>|[<span data-ttu-id="9de13-135">WorkbookChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="9de13-135">WorkbookChartLegendFormat</span></span>](chartlegendformat.md)|<span data-ttu-id="9de13-136">表示图表图例的格式，包括填充和字体格式。</span><span class="sxs-lookup"><span data-stu-id="9de13-136">Represents the formatting of a chart legend, which includes fill and font formatting.</span></span> <span data-ttu-id="9de13-137">只读。</span><span class="sxs-lookup"><span data-stu-id="9de13-137">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9de13-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9de13-138">JSON representation</span></span>

<span data-ttu-id="9de13-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9de13-139">Here is a JSON representation of the resource.</span></span>

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

