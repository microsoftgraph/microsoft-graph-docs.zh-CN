---
title: ChartGridlines 资源类型
description: 代表图表坐标轴的主要或次要网格线。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: b37bbc2b746d3dc2de4b55fa363b7b67f30f7191
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069181"
---
# <a name="chartgridlines-resource-type"></a><span data-ttu-id="86134-103">ChartGridlines 资源类型</span><span class="sxs-lookup"><span data-stu-id="86134-103">ChartGridlines resource type</span></span>

<span data-ttu-id="86134-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86134-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="86134-105">代表图表坐标轴的主要或次要网格线。</span><span class="sxs-lookup"><span data-stu-id="86134-105">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="86134-106">方法</span><span class="sxs-lookup"><span data-stu-id="86134-106">Methods</span></span>

| <span data-ttu-id="86134-107">方法</span><span class="sxs-lookup"><span data-stu-id="86134-107">Method</span></span>           | <span data-ttu-id="86134-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="86134-108">Return Type</span></span>    |<span data-ttu-id="86134-109">说明</span><span class="sxs-lookup"><span data-stu-id="86134-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="86134-110">获取 ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="86134-110">Get ChartGridlines</span></span>](../api/chartgridlines-get.md) | [<span data-ttu-id="86134-111">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="86134-111">WorkbookChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="86134-112">读取 chartGridlines 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="86134-112">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="86134-113">更新</span><span class="sxs-lookup"><span data-stu-id="86134-113">Update</span></span>](../api/chartgridlines-update.md) | [<span data-ttu-id="86134-114">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="86134-114">WorkbookChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="86134-115">更新 ChartGridlines 对象。</span><span class="sxs-lookup"><span data-stu-id="86134-115">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="86134-116">属性</span><span class="sxs-lookup"><span data-stu-id="86134-116">Properties</span></span>
| <span data-ttu-id="86134-117">属性</span><span class="sxs-lookup"><span data-stu-id="86134-117">Property</span></span>     | <span data-ttu-id="86134-118">类型</span><span class="sxs-lookup"><span data-stu-id="86134-118">Type</span></span>   |<span data-ttu-id="86134-119">说明</span><span class="sxs-lookup"><span data-stu-id="86134-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86134-120">visible</span><span class="sxs-lookup"><span data-stu-id="86134-120">visible</span></span>|<span data-ttu-id="86134-121">布尔</span><span class="sxs-lookup"><span data-stu-id="86134-121">boolean</span></span>|<span data-ttu-id="86134-122">表示坐标轴网格线是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="86134-122">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="86134-123">关系</span><span class="sxs-lookup"><span data-stu-id="86134-123">Relationships</span></span>
| <span data-ttu-id="86134-124">关系</span><span class="sxs-lookup"><span data-stu-id="86134-124">Relationship</span></span> | <span data-ttu-id="86134-125">类型</span><span class="sxs-lookup"><span data-stu-id="86134-125">Type</span></span>   |<span data-ttu-id="86134-126">说明</span><span class="sxs-lookup"><span data-stu-id="86134-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86134-127">format</span><span class="sxs-lookup"><span data-stu-id="86134-127">format</span></span>|[<span data-ttu-id="86134-128">WorkbookChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="86134-128">WorkbookChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="86134-129">表示图表网格线的格式。</span><span class="sxs-lookup"><span data-stu-id="86134-129">Represents the formatting of chart gridlines.</span></span> <span data-ttu-id="86134-130">只读。</span><span class="sxs-lookup"><span data-stu-id="86134-130">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="86134-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="86134-131">JSON representation</span></span>

<span data-ttu-id="86134-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="86134-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartGridlines"
}-->

```json
{
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartGridlines resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

