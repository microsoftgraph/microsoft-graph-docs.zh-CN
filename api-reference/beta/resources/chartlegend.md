---
title: ChartLegend 资源类型
description: 表示图表中的图例。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c76fd21700616ec6c353644de93bddd0a47ac7dd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980878"
---
# <a name="chartlegend-resource-type"></a><span data-ttu-id="cc754-103">ChartLegend 资源类型</span><span class="sxs-lookup"><span data-stu-id="cc754-103">ChartLegend resource type</span></span>

> <span data-ttu-id="cc754-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cc754-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc754-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cc754-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cc754-106">表示图表中的图例。</span><span class="sxs-lookup"><span data-stu-id="cc754-106">Represents the legend in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="cc754-107">方法</span><span class="sxs-lookup"><span data-stu-id="cc754-107">Methods</span></span>

| <span data-ttu-id="cc754-108">方法</span><span class="sxs-lookup"><span data-stu-id="cc754-108">Method</span></span>           | <span data-ttu-id="cc754-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="cc754-109">Return Type</span></span>    |<span data-ttu-id="cc754-110">说明</span><span class="sxs-lookup"><span data-stu-id="cc754-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cc754-111">获取 ChartLegend</span><span class="sxs-lookup"><span data-stu-id="cc754-111">Get ChartLegend</span></span>](../api/chartlegend-get.md) | [<span data-ttu-id="cc754-112">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="cc754-112">ChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="cc754-113">读取 chartlegend 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cc754-113">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="cc754-114">Update</span><span class="sxs-lookup"><span data-stu-id="cc754-114">Update</span></span>](../api/chartlegend-update.md) | [<span data-ttu-id="cc754-115">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="cc754-115">ChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="cc754-116">更新 chartlegend 对象。</span><span class="sxs-lookup"><span data-stu-id="cc754-116">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="cc754-117">属性</span><span class="sxs-lookup"><span data-stu-id="cc754-117">Properties</span></span>
| <span data-ttu-id="cc754-118">属性</span><span class="sxs-lookup"><span data-stu-id="cc754-118">Property</span></span>     | <span data-ttu-id="cc754-119">类型</span><span class="sxs-lookup"><span data-stu-id="cc754-119">Type</span></span>   |<span data-ttu-id="cc754-120">说明</span><span class="sxs-lookup"><span data-stu-id="cc754-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc754-121">overlay</span><span class="sxs-lookup"><span data-stu-id="cc754-121">overlay</span></span>|<span data-ttu-id="cc754-122">boolean</span><span class="sxs-lookup"><span data-stu-id="cc754-122">boolean</span></span>|<span data-ttu-id="cc754-123">表示图表图例是否应该与图表主体重叠的布尔值。</span><span class="sxs-lookup"><span data-stu-id="cc754-123">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="cc754-124">position</span><span class="sxs-lookup"><span data-stu-id="cc754-124">position</span></span>|<span data-ttu-id="cc754-125">string</span><span class="sxs-lookup"><span data-stu-id="cc754-125">string</span></span>|<span data-ttu-id="cc754-p102">表示图例在图表上的位置。可能的值是：`Top`、`Bottom`、`Left`、`Right`、`Corner`、`Custom`。</span><span class="sxs-lookup"><span data-stu-id="cc754-p102">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="cc754-128">visible</span><span class="sxs-lookup"><span data-stu-id="cc754-128">visible</span></span>|<span data-ttu-id="cc754-129">boolean</span><span class="sxs-lookup"><span data-stu-id="cc754-129">boolean</span></span>|<span data-ttu-id="cc754-130">表示 ChartLegend 对象的可见性的布尔值。</span><span class="sxs-lookup"><span data-stu-id="cc754-130">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc754-131">Relationships</span><span class="sxs-lookup"><span data-stu-id="cc754-131">Relationships</span></span>
| <span data-ttu-id="cc754-132">关系</span><span class="sxs-lookup"><span data-stu-id="cc754-132">Relationship</span></span> | <span data-ttu-id="cc754-133">类型</span><span class="sxs-lookup"><span data-stu-id="cc754-133">Type</span></span>   |<span data-ttu-id="cc754-134">说明</span><span class="sxs-lookup"><span data-stu-id="cc754-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc754-135">format</span><span class="sxs-lookup"><span data-stu-id="cc754-135">format</span></span>|[<span data-ttu-id="cc754-136">ChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="cc754-136">ChartLegendFormat</span></span>](chartlegendformat.md)|<span data-ttu-id="cc754-p103">表示图表图例的格式，包括填充和字体格式。只读。</span><span class="sxs-lookup"><span data-stu-id="cc754-p103">Represents the formatting of a chart legend, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cc754-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cc754-139">JSON representation</span></span>

<span data-ttu-id="cc754-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc754-140">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartLegend resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
