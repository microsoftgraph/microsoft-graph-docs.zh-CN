---
title: workbookChartSeriesFormat 资源类型
description: 封装图表系列的格式属性
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 739a874545047c2ed6927cb4e31d2e006f4e6ba4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007163"
---
# <a name="workbookchartseriesformat-resource-type"></a><span data-ttu-id="725ee-103">workbookChartSeriesFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="725ee-103">workbookChartSeriesFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="725ee-104">封装图表系列的格式属性</span><span class="sxs-lookup"><span data-stu-id="725ee-104">Encapsulates the format properties for the chart series.</span></span>


## <a name="methods"></a><span data-ttu-id="725ee-105">方法</span><span class="sxs-lookup"><span data-stu-id="725ee-105">Methods</span></span>
<span data-ttu-id="725ee-106">无</span><span class="sxs-lookup"><span data-stu-id="725ee-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="725ee-107">属性</span><span class="sxs-lookup"><span data-stu-id="725ee-107">Properties</span></span>
<span data-ttu-id="725ee-108">无</span><span class="sxs-lookup"><span data-stu-id="725ee-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="725ee-109">关系</span><span class="sxs-lookup"><span data-stu-id="725ee-109">Relationships</span></span>
| <span data-ttu-id="725ee-110">关系</span><span class="sxs-lookup"><span data-stu-id="725ee-110">Relationship</span></span> | <span data-ttu-id="725ee-111">类型</span><span class="sxs-lookup"><span data-stu-id="725ee-111">Type</span></span>   |<span data-ttu-id="725ee-112">说明</span><span class="sxs-lookup"><span data-stu-id="725ee-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="725ee-113">fill</span><span class="sxs-lookup"><span data-stu-id="725ee-113">fill</span></span>|[<span data-ttu-id="725ee-114">workbookChartFill</span><span class="sxs-lookup"><span data-stu-id="725ee-114">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="725ee-p101">表示图表系列的填充格式，包括背景格式信息。只读。</span><span class="sxs-lookup"><span data-stu-id="725ee-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="725ee-117">line</span><span class="sxs-lookup"><span data-stu-id="725ee-117">line</span></span>|[<span data-ttu-id="725ee-118">workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="725ee-118">workbookChartLineFormat</span></span>](workbookchartlineformat.md)|<span data-ttu-id="725ee-119">表示线条格式。</span><span class="sxs-lookup"><span data-stu-id="725ee-119">Represents line formatting.</span></span> <span data-ttu-id="725ee-120">只读。</span><span class="sxs-lookup"><span data-stu-id="725ee-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="725ee-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="725ee-121">JSON representation</span></span>

<span data-ttu-id="725ee-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="725ee-122">Here is a JSON representation of the resource.</span></span>

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
