---
title: ChartAxes 资源类型
description: 表示图表坐标轴。
ms.openlocfilehash: 4fc801ecdba147a26b30f07a2487eabe11acfb3c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008538"
---
# <a name="chartaxes-resource-type"></a><span data-ttu-id="9e767-103">ChartAxes 资源类型</span><span class="sxs-lookup"><span data-stu-id="9e767-103">ChartAxes resource type</span></span>

<span data-ttu-id="9e767-104">表示图表坐标轴。</span><span class="sxs-lookup"><span data-stu-id="9e767-104">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="9e767-105">方法</span><span class="sxs-lookup"><span data-stu-id="9e767-105">Methods</span></span>
<span data-ttu-id="9e767-106">无</span><span class="sxs-lookup"><span data-stu-id="9e767-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="9e767-107">属性</span><span class="sxs-lookup"><span data-stu-id="9e767-107">Properties</span></span>
<span data-ttu-id="9e767-108">无</span><span class="sxs-lookup"><span data-stu-id="9e767-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="9e767-109">Relationships</span><span class="sxs-lookup"><span data-stu-id="9e767-109">Relationships</span></span>
| <span data-ttu-id="9e767-110">关系</span><span class="sxs-lookup"><span data-stu-id="9e767-110">Relationship</span></span> | <span data-ttu-id="9e767-111">类型</span><span class="sxs-lookup"><span data-stu-id="9e767-111">Type</span></span>   |<span data-ttu-id="9e767-112">说明</span><span class="sxs-lookup"><span data-stu-id="9e767-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e767-113">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="9e767-113">categoryAxis</span></span>|[<span data-ttu-id="9e767-114">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="9e767-114">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="9e767-p101">表示图表中的类别轴。只读。</span><span class="sxs-lookup"><span data-stu-id="9e767-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="9e767-117">seriesAxis</span><span class="sxs-lookup"><span data-stu-id="9e767-117">seriesAxis</span></span>|[<span data-ttu-id="9e767-118">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="9e767-118">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="9e767-p102">表示三维图表的系列轴。只读。</span><span class="sxs-lookup"><span data-stu-id="9e767-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="9e767-121">valueAxis</span><span class="sxs-lookup"><span data-stu-id="9e767-121">valueAxis</span></span>|[<span data-ttu-id="9e767-122">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="9e767-122">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="9e767-p103">表示坐标轴中的数值轴。只读。</span><span class="sxs-lookup"><span data-stu-id="9e767-p103">Represents the value axis in an axis. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9e767-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9e767-125">JSON representation</span></span>

<span data-ttu-id="9e767-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e767-126">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->