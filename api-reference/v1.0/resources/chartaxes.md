---
title: ChartAxes 资源类型
description: 表示图表坐标轴。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 483a69f11425f3b8991305e6acdf6b970d0e2db1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976385"
---
# <a name="chartaxes-resource-type"></a><span data-ttu-id="f5dce-103">ChartAxes 资源类型</span><span class="sxs-lookup"><span data-stu-id="f5dce-103">ChartAxes resource type</span></span>

<span data-ttu-id="f5dce-104">表示图表坐标轴。</span><span class="sxs-lookup"><span data-stu-id="f5dce-104">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="f5dce-105">方法</span><span class="sxs-lookup"><span data-stu-id="f5dce-105">Methods</span></span>
<span data-ttu-id="f5dce-106">无</span><span class="sxs-lookup"><span data-stu-id="f5dce-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="f5dce-107">属性</span><span class="sxs-lookup"><span data-stu-id="f5dce-107">Properties</span></span>
<span data-ttu-id="f5dce-108">无</span><span class="sxs-lookup"><span data-stu-id="f5dce-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="f5dce-109">Relationships</span><span class="sxs-lookup"><span data-stu-id="f5dce-109">Relationships</span></span>
| <span data-ttu-id="f5dce-110">关系</span><span class="sxs-lookup"><span data-stu-id="f5dce-110">Relationship</span></span> | <span data-ttu-id="f5dce-111">类型</span><span class="sxs-lookup"><span data-stu-id="f5dce-111">Type</span></span>   |<span data-ttu-id="f5dce-112">说明</span><span class="sxs-lookup"><span data-stu-id="f5dce-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5dce-113">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="f5dce-113">categoryAxis</span></span>|[<span data-ttu-id="f5dce-114">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="f5dce-114">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="f5dce-p101">表示图表中的类别轴。只读。</span><span class="sxs-lookup"><span data-stu-id="f5dce-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="f5dce-117">seriesAxis</span><span class="sxs-lookup"><span data-stu-id="f5dce-117">seriesAxis</span></span>|[<span data-ttu-id="f5dce-118">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="f5dce-118">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="f5dce-p102">表示三维图表的系列轴。只读。</span><span class="sxs-lookup"><span data-stu-id="f5dce-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="f5dce-121">valueAxis</span><span class="sxs-lookup"><span data-stu-id="f5dce-121">valueAxis</span></span>|[<span data-ttu-id="f5dce-122">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="f5dce-122">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="f5dce-p103">表示坐标轴中的数值轴。只读。</span><span class="sxs-lookup"><span data-stu-id="f5dce-p103">Represents the value axis in an axis. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f5dce-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f5dce-125">JSON representation</span></span>

<span data-ttu-id="f5dce-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f5dce-126">Here is a JSON representation of the resource.</span></span>

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
