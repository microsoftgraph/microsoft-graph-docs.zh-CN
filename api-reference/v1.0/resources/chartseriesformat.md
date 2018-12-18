---
title: ChartSeriesFormat 资源类型
description: 封装图表系列的格式属性
author: lumine2008
ms.openlocfilehash: 9c27a20c6be6987c31579ca88d546ee80c86d3ea
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354059"
---
# <a name="chartseriesformat-resource-type"></a><span data-ttu-id="94801-103">ChartSeriesFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="94801-103">ChartSeriesFormat resource type</span></span>

<span data-ttu-id="94801-104">封装图表系列的格式属性</span><span class="sxs-lookup"><span data-stu-id="94801-104">encapsulates the format properties for the chart series</span></span>


## <a name="methods"></a><span data-ttu-id="94801-105">方法</span><span class="sxs-lookup"><span data-stu-id="94801-105">Methods</span></span>
<span data-ttu-id="94801-106">无</span><span class="sxs-lookup"><span data-stu-id="94801-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="94801-107">属性</span><span class="sxs-lookup"><span data-stu-id="94801-107">Properties</span></span>
<span data-ttu-id="94801-108">无</span><span class="sxs-lookup"><span data-stu-id="94801-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="94801-109">Relationships</span><span class="sxs-lookup"><span data-stu-id="94801-109">Relationships</span></span>
| <span data-ttu-id="94801-110">关系</span><span class="sxs-lookup"><span data-stu-id="94801-110">Relationship</span></span> | <span data-ttu-id="94801-111">类型</span><span class="sxs-lookup"><span data-stu-id="94801-111">Type</span></span>   |<span data-ttu-id="94801-112">说明</span><span class="sxs-lookup"><span data-stu-id="94801-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94801-113">fill</span><span class="sxs-lookup"><span data-stu-id="94801-113">fill</span></span>|[<span data-ttu-id="94801-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="94801-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="94801-p101">表示图表系列的填充格式，包括背景格式信息。只读。</span><span class="sxs-lookup"><span data-stu-id="94801-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="94801-117">line</span><span class="sxs-lookup"><span data-stu-id="94801-117">line</span></span>|[<span data-ttu-id="94801-118">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="94801-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="94801-p102">表示线条格式。只读。</span><span class="sxs-lookup"><span data-stu-id="94801-p102">Represents line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="94801-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94801-121">JSON representation</span></span>

<span data-ttu-id="94801-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94801-122">Here is a JSON representation of the resource.</span></span>

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