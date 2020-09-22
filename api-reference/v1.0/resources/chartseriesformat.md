---
title: ChartSeriesFormat 资源类型
description: 封装图表系列的格式属性
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 3b6003df060fbb657dc3c67375f2c942ad8cff57
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059227"
---
# <a name="chartseriesformat-resource-type"></a><span data-ttu-id="e4793-103">ChartSeriesFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="e4793-103">ChartSeriesFormat resource type</span></span>

<span data-ttu-id="e4793-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4793-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e4793-105">封装图表系列的格式属性</span><span class="sxs-lookup"><span data-stu-id="e4793-105">encapsulates the format properties for the chart series</span></span>


## <a name="methods"></a><span data-ttu-id="e4793-106">方法</span><span class="sxs-lookup"><span data-stu-id="e4793-106">Methods</span></span>
<span data-ttu-id="e4793-107">无</span><span class="sxs-lookup"><span data-stu-id="e4793-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="e4793-108">属性</span><span class="sxs-lookup"><span data-stu-id="e4793-108">Properties</span></span>
<span data-ttu-id="e4793-109">无</span><span class="sxs-lookup"><span data-stu-id="e4793-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="e4793-110">关系</span><span class="sxs-lookup"><span data-stu-id="e4793-110">Relationships</span></span>
| <span data-ttu-id="e4793-111">关系</span><span class="sxs-lookup"><span data-stu-id="e4793-111">Relationship</span></span> | <span data-ttu-id="e4793-112">类型</span><span class="sxs-lookup"><span data-stu-id="e4793-112">Type</span></span>   |<span data-ttu-id="e4793-113">说明</span><span class="sxs-lookup"><span data-stu-id="e4793-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4793-114">fill</span><span class="sxs-lookup"><span data-stu-id="e4793-114">fill</span></span>|[<span data-ttu-id="e4793-115">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="e4793-115">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="e4793-p101">表示图表系列的填充格式，包括背景格式信息。只读。</span><span class="sxs-lookup"><span data-stu-id="e4793-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="e4793-118">line</span><span class="sxs-lookup"><span data-stu-id="e4793-118">line</span></span>|[<span data-ttu-id="e4793-119">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="e4793-119">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="e4793-120">表示线条格式。</span><span class="sxs-lookup"><span data-stu-id="e4793-120">Represents line formatting.</span></span> <span data-ttu-id="e4793-121">只读。</span><span class="sxs-lookup"><span data-stu-id="e4793-121">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e4793-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e4793-122">JSON representation</span></span>

<span data-ttu-id="e4793-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4793-123">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartSeriesFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeriesFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

