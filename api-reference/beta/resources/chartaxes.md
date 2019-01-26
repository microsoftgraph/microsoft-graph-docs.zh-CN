---
title: ChartAxes 资源类型
description: 表示图表坐标轴。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f2a3744e38ffebef0c28784c0fd4be8f35b8af23
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570860"
---
# <a name="chartaxes-resource-type"></a><span data-ttu-id="5f55d-103">ChartAxes 资源类型</span><span class="sxs-lookup"><span data-stu-id="5f55d-103">ChartAxes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f55d-104">表示图表坐标轴。</span><span class="sxs-lookup"><span data-stu-id="5f55d-104">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="5f55d-105">方法</span><span class="sxs-lookup"><span data-stu-id="5f55d-105">Methods</span></span>
<span data-ttu-id="5f55d-106">无</span><span class="sxs-lookup"><span data-stu-id="5f55d-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="5f55d-107">属性</span><span class="sxs-lookup"><span data-stu-id="5f55d-107">Properties</span></span>
<span data-ttu-id="5f55d-108">无</span><span class="sxs-lookup"><span data-stu-id="5f55d-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="5f55d-109">关系</span><span class="sxs-lookup"><span data-stu-id="5f55d-109">Relationships</span></span>
| <span data-ttu-id="5f55d-110">关系</span><span class="sxs-lookup"><span data-stu-id="5f55d-110">Relationship</span></span> | <span data-ttu-id="5f55d-111">类型</span><span class="sxs-lookup"><span data-stu-id="5f55d-111">Type</span></span>   |<span data-ttu-id="5f55d-112">说明</span><span class="sxs-lookup"><span data-stu-id="5f55d-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5f55d-113">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="5f55d-113">categoryAxis</span></span>|[<span data-ttu-id="5f55d-114">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="5f55d-114">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="5f55d-p101">表示图表中的类别轴。只读。</span><span class="sxs-lookup"><span data-stu-id="5f55d-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="5f55d-117">seriesAxis</span><span class="sxs-lookup"><span data-stu-id="5f55d-117">seriesAxis</span></span>|[<span data-ttu-id="5f55d-118">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="5f55d-118">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="5f55d-p102">表示三维图表的系列轴。只读。</span><span class="sxs-lookup"><span data-stu-id="5f55d-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="5f55d-121">valueAxis</span><span class="sxs-lookup"><span data-stu-id="5f55d-121">valueAxis</span></span>|[<span data-ttu-id="5f55d-122">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="5f55d-122">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="5f55d-p103">表示坐标轴中的数值轴。只读。</span><span class="sxs-lookup"><span data-stu-id="5f55d-p103">Represents the value axis in an axis. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5f55d-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5f55d-125">JSON representation</span></span>

<span data-ttu-id="5f55d-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f55d-126">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxes"
}-->

```json
{
  "categoryAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"},
  "seriesAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"},
  "valueAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartaxes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
