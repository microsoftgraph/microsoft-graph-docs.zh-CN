---
title: workbookChartAxes 资源类型
description: 表示图表坐标轴。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 89d9a45f0f9e992ac8a93cde6114fc8c9f073359
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519384"
---
# <a name="workbookchartaxes-resource-type"></a><span data-ttu-id="5a2f8-103">workbookChartAxes 资源类型</span><span class="sxs-lookup"><span data-stu-id="5a2f8-103">workbookChartAxes resource type</span></span>

<span data-ttu-id="5a2f8-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="5a2f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a2f8-105">表示图表坐标轴。</span><span class="sxs-lookup"><span data-stu-id="5a2f8-105">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="5a2f8-106">方法</span><span class="sxs-lookup"><span data-stu-id="5a2f8-106">Methods</span></span>
<span data-ttu-id="5a2f8-107">无</span><span class="sxs-lookup"><span data-stu-id="5a2f8-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="5a2f8-108">属性</span><span class="sxs-lookup"><span data-stu-id="5a2f8-108">Properties</span></span>
<span data-ttu-id="5a2f8-109">无</span><span class="sxs-lookup"><span data-stu-id="5a2f8-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="5a2f8-110">关系</span><span class="sxs-lookup"><span data-stu-id="5a2f8-110">Relationships</span></span>
| <span data-ttu-id="5a2f8-111">关系</span><span class="sxs-lookup"><span data-stu-id="5a2f8-111">Relationship</span></span> | <span data-ttu-id="5a2f8-112">类型</span><span class="sxs-lookup"><span data-stu-id="5a2f8-112">Type</span></span>   |<span data-ttu-id="5a2f8-113">说明</span><span class="sxs-lookup"><span data-stu-id="5a2f8-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a2f8-114">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="5a2f8-114">categoryAxis</span></span>|[<span data-ttu-id="5a2f8-115">workbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="5a2f8-115">workbookChartAxis</span></span>](workbookchartaxis.md)|<span data-ttu-id="5a2f8-p101">表示图表中的类别轴。只读。</span><span class="sxs-lookup"><span data-stu-id="5a2f8-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="5a2f8-118">seriesAxis</span><span class="sxs-lookup"><span data-stu-id="5a2f8-118">seriesAxis</span></span>|[<span data-ttu-id="5a2f8-119">workbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="5a2f8-119">workbookChartAxis</span></span>](workbookchartaxis.md)|<span data-ttu-id="5a2f8-p102">表示三维图表的系列轴。只读。</span><span class="sxs-lookup"><span data-stu-id="5a2f8-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="5a2f8-122">值坐标轴</span><span class="sxs-lookup"><span data-stu-id="5a2f8-122">valueAxis</span></span>|[<span data-ttu-id="5a2f8-123">workbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="5a2f8-123">workbookChartAxis</span></span>](workbookchartaxis.md)|<span data-ttu-id="5a2f8-124">表示坐标轴中的数值轴。</span><span class="sxs-lookup"><span data-stu-id="5a2f8-124">Represents the value axis in an axis.</span></span> <span data-ttu-id="5a2f8-125">只读。</span><span class="sxs-lookup"><span data-stu-id="5a2f8-125">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5a2f8-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5a2f8-126">JSON representation</span></span>

<span data-ttu-id="5a2f8-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5a2f8-127">Here is a JSON representation of the resource.</span></span>

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
