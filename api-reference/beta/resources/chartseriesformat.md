---
title: ChartSeriesFormat 资源类型
description: 封装图表系列的格式属性
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c5fdfffdf5bcf6aeefc5068392f689cbf66d683d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573583"
---
# <a name="chartseriesformat-resource-type"></a><span data-ttu-id="7b891-103">ChartSeriesFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="7b891-103">ChartSeriesFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b891-104">封装图表系列的格式属性</span><span class="sxs-lookup"><span data-stu-id="7b891-104">encapsulates the format properties for the chart series</span></span>


## <a name="methods"></a><span data-ttu-id="7b891-105">方法</span><span class="sxs-lookup"><span data-stu-id="7b891-105">Methods</span></span>
<span data-ttu-id="7b891-106">无</span><span class="sxs-lookup"><span data-stu-id="7b891-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="7b891-107">属性</span><span class="sxs-lookup"><span data-stu-id="7b891-107">Properties</span></span>
<span data-ttu-id="7b891-108">无</span><span class="sxs-lookup"><span data-stu-id="7b891-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="7b891-109">关系</span><span class="sxs-lookup"><span data-stu-id="7b891-109">Relationships</span></span>
| <span data-ttu-id="7b891-110">关系</span><span class="sxs-lookup"><span data-stu-id="7b891-110">Relationship</span></span> | <span data-ttu-id="7b891-111">类型</span><span class="sxs-lookup"><span data-stu-id="7b891-111">Type</span></span>   |<span data-ttu-id="7b891-112">说明</span><span class="sxs-lookup"><span data-stu-id="7b891-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b891-113">fill</span><span class="sxs-lookup"><span data-stu-id="7b891-113">fill</span></span>|[<span data-ttu-id="7b891-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="7b891-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="7b891-p101">表示图表系列的填充格式，包括背景格式信息。只读。</span><span class="sxs-lookup"><span data-stu-id="7b891-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="7b891-117">line</span><span class="sxs-lookup"><span data-stu-id="7b891-117">line</span></span>|[<span data-ttu-id="7b891-118">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="7b891-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="7b891-p102">表示线条格式。只读。</span><span class="sxs-lookup"><span data-stu-id="7b891-p102">Represents line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="7b891-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7b891-121">JSON representation</span></span>

<span data-ttu-id="7b891-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7b891-122">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/chartseriesformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
