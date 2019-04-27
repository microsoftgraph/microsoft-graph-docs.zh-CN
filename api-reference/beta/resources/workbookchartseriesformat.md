---
title: workbookChartSeriesFormat 资源类型
description: 封装图表系列的格式属性
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5d07dbaf17fd715b93dcd039fe3fb9e264bd7f63
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348616"
---
# <a name="workbookchartseriesformat-resource-type"></a><span data-ttu-id="497e3-103">workbookChartSeriesFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="497e3-103">workbookChartSeriesFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="497e3-104">封装图表系列的格式属性</span><span class="sxs-lookup"><span data-stu-id="497e3-104">Encapsulates the format properties for the chart series.</span></span>


## <a name="methods"></a><span data-ttu-id="497e3-105">方法</span><span class="sxs-lookup"><span data-stu-id="497e3-105">Methods</span></span>
<span data-ttu-id="497e3-106">无</span><span class="sxs-lookup"><span data-stu-id="497e3-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="497e3-107">属性</span><span class="sxs-lookup"><span data-stu-id="497e3-107">Properties</span></span>
<span data-ttu-id="497e3-108">无</span><span class="sxs-lookup"><span data-stu-id="497e3-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="497e3-109">关系</span><span class="sxs-lookup"><span data-stu-id="497e3-109">Relationships</span></span>
| <span data-ttu-id="497e3-110">关系</span><span class="sxs-lookup"><span data-stu-id="497e3-110">Relationship</span></span> | <span data-ttu-id="497e3-111">类型</span><span class="sxs-lookup"><span data-stu-id="497e3-111">Type</span></span>   |<span data-ttu-id="497e3-112">说明</span><span class="sxs-lookup"><span data-stu-id="497e3-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="497e3-113">fill</span><span class="sxs-lookup"><span data-stu-id="497e3-113">fill</span></span>|[<span data-ttu-id="497e3-114">workbookChartFill</span><span class="sxs-lookup"><span data-stu-id="497e3-114">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="497e3-p101">表示图表系列的填充格式，包括背景格式信息。只读。</span><span class="sxs-lookup"><span data-stu-id="497e3-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="497e3-117">line</span><span class="sxs-lookup"><span data-stu-id="497e3-117">line</span></span>|[<span data-ttu-id="497e3-118">workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="497e3-118">workbookChartLineFormat</span></span>](workbookchartlineformat.md)|<span data-ttu-id="497e3-119">表示线条格式。</span><span class="sxs-lookup"><span data-stu-id="497e3-119">Represents line formatting.</span></span> <span data-ttu-id="497e3-120">只读。</span><span class="sxs-lookup"><span data-stu-id="497e3-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="497e3-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="497e3-121">JSON representation</span></span>

<span data-ttu-id="497e3-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="497e3-122">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartSeriesFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
