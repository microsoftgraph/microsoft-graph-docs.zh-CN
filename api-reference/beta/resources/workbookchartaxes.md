---
title: workbookChartAxes 资源类型
description: 表示图表坐标轴。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 15e63af1e7b648288dba813790302f1dee6536ba
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348562"
---
# <a name="workbookchartaxes-resource-type"></a><span data-ttu-id="6dd34-103">workbookChartAxes 资源类型</span><span class="sxs-lookup"><span data-stu-id="6dd34-103">workbookChartAxes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6dd34-104">表示图表坐标轴。</span><span class="sxs-lookup"><span data-stu-id="6dd34-104">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="6dd34-105">方法</span><span class="sxs-lookup"><span data-stu-id="6dd34-105">Methods</span></span>
<span data-ttu-id="6dd34-106">无</span><span class="sxs-lookup"><span data-stu-id="6dd34-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="6dd34-107">属性</span><span class="sxs-lookup"><span data-stu-id="6dd34-107">Properties</span></span>
<span data-ttu-id="6dd34-108">无</span><span class="sxs-lookup"><span data-stu-id="6dd34-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="6dd34-109">关系</span><span class="sxs-lookup"><span data-stu-id="6dd34-109">Relationships</span></span>
| <span data-ttu-id="6dd34-110">关系</span><span class="sxs-lookup"><span data-stu-id="6dd34-110">Relationship</span></span> | <span data-ttu-id="6dd34-111">类型</span><span class="sxs-lookup"><span data-stu-id="6dd34-111">Type</span></span>   |<span data-ttu-id="6dd34-112">说明</span><span class="sxs-lookup"><span data-stu-id="6dd34-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6dd34-113">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="6dd34-113">categoryAxis</span></span>|[<span data-ttu-id="6dd34-114">workbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="6dd34-114">workbookChartAxis</span></span>](workbookchartaxis.md)|<span data-ttu-id="6dd34-p101">表示图表中的类别轴。只读。</span><span class="sxs-lookup"><span data-stu-id="6dd34-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="6dd34-117">seriesAxis</span><span class="sxs-lookup"><span data-stu-id="6dd34-117">seriesAxis</span></span>|[<span data-ttu-id="6dd34-118">workbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="6dd34-118">workbookChartAxis</span></span>](workbookchartaxis.md)|<span data-ttu-id="6dd34-p102">表示三维图表的系列轴。只读。</span><span class="sxs-lookup"><span data-stu-id="6dd34-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="6dd34-121">值坐标轴</span><span class="sxs-lookup"><span data-stu-id="6dd34-121">valueAxis</span></span>|[<span data-ttu-id="6dd34-122">workbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="6dd34-122">workbookChartAxis</span></span>](workbookchartaxis.md)|<span data-ttu-id="6dd34-123">表示坐标轴中的数值轴。</span><span class="sxs-lookup"><span data-stu-id="6dd34-123">Represents the value axis in an axis.</span></span> <span data-ttu-id="6dd34-124">只读。</span><span class="sxs-lookup"><span data-stu-id="6dd34-124">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6dd34-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6dd34-125">JSON representation</span></span>

<span data-ttu-id="6dd34-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6dd34-126">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
