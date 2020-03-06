---
title: ChartSeriesFormat 资源类型
description: 封装图表系列的格式属性
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: a44392eb718c157f6422228405f7bb2a4b411733
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533101"
---
# <a name="chartseriesformat-resource-type"></a><span data-ttu-id="65d11-103">ChartSeriesFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="65d11-103">ChartSeriesFormat resource type</span></span>

<span data-ttu-id="65d11-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65d11-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="65d11-105">封装图表系列的格式属性</span><span class="sxs-lookup"><span data-stu-id="65d11-105">encapsulates the format properties for the chart series</span></span>


## <a name="methods"></a><span data-ttu-id="65d11-106">Methods</span><span class="sxs-lookup"><span data-stu-id="65d11-106">Methods</span></span>
<span data-ttu-id="65d11-107">无</span><span class="sxs-lookup"><span data-stu-id="65d11-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="65d11-108">属性</span><span class="sxs-lookup"><span data-stu-id="65d11-108">Properties</span></span>
<span data-ttu-id="65d11-109">无</span><span class="sxs-lookup"><span data-stu-id="65d11-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="65d11-110">关系</span><span class="sxs-lookup"><span data-stu-id="65d11-110">Relationships</span></span>
| <span data-ttu-id="65d11-111">关系</span><span class="sxs-lookup"><span data-stu-id="65d11-111">Relationship</span></span> | <span data-ttu-id="65d11-112">类型</span><span class="sxs-lookup"><span data-stu-id="65d11-112">Type</span></span>   |<span data-ttu-id="65d11-113">说明</span><span class="sxs-lookup"><span data-stu-id="65d11-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65d11-114">fill</span><span class="sxs-lookup"><span data-stu-id="65d11-114">fill</span></span>|[<span data-ttu-id="65d11-115">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="65d11-115">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="65d11-p101">表示图表系列的填充格式，包括背景格式信息。只读。</span><span class="sxs-lookup"><span data-stu-id="65d11-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="65d11-118">line</span><span class="sxs-lookup"><span data-stu-id="65d11-118">line</span></span>|[<span data-ttu-id="65d11-119">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="65d11-119">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="65d11-120">表示线条格式。</span><span class="sxs-lookup"><span data-stu-id="65d11-120">Represents line formatting.</span></span> <span data-ttu-id="65d11-121">只读。</span><span class="sxs-lookup"><span data-stu-id="65d11-121">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="65d11-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="65d11-122">JSON representation</span></span>

<span data-ttu-id="65d11-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65d11-123">Here is a JSON representation of the resource.</span></span>

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
