---
title: ChartLegendFormat 资源类型
description: 封装图表图例的格式属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: f4d018fd01a9ad9899eefcb663b0860096567c84
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988391"
---
# <a name="chartlegendformat-resource-type"></a><span data-ttu-id="9eb78-103">ChartLegendFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="9eb78-103">ChartLegendFormat resource type</span></span>

<span data-ttu-id="9eb78-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9eb78-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9eb78-105">封装图表图例的格式属性。</span><span class="sxs-lookup"><span data-stu-id="9eb78-105">Encapsulates the format properties of a chart legend.</span></span>


## <a name="methods"></a><span data-ttu-id="9eb78-106">方法</span><span class="sxs-lookup"><span data-stu-id="9eb78-106">Methods</span></span>
<span data-ttu-id="9eb78-107">无</span><span class="sxs-lookup"><span data-stu-id="9eb78-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="9eb78-108">属性</span><span class="sxs-lookup"><span data-stu-id="9eb78-108">Properties</span></span>
<span data-ttu-id="9eb78-109">无</span><span class="sxs-lookup"><span data-stu-id="9eb78-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="9eb78-110">关系</span><span class="sxs-lookup"><span data-stu-id="9eb78-110">Relationships</span></span>
| <span data-ttu-id="9eb78-111">关系</span><span class="sxs-lookup"><span data-stu-id="9eb78-111">Relationship</span></span> | <span data-ttu-id="9eb78-112">类型</span><span class="sxs-lookup"><span data-stu-id="9eb78-112">Type</span></span>   |<span data-ttu-id="9eb78-113">说明</span><span class="sxs-lookup"><span data-stu-id="9eb78-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9eb78-114">fill</span><span class="sxs-lookup"><span data-stu-id="9eb78-114">fill</span></span>|[<span data-ttu-id="9eb78-115">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="9eb78-115">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="9eb78-p101">表示对象的填充格式，包括背景格式信息。只读。</span><span class="sxs-lookup"><span data-stu-id="9eb78-p101">Represents the fill format of an object, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="9eb78-118">font</span><span class="sxs-lookup"><span data-stu-id="9eb78-118">font</span></span>|[<span data-ttu-id="9eb78-119">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="9eb78-119">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="9eb78-120">表示图表图例的字体属性，例如字体名称、字体大小、颜色等。</span><span class="sxs-lookup"><span data-stu-id="9eb78-120">Represents the font attributes such as font name, font size, color, etc. of a chart legend.</span></span> <span data-ttu-id="9eb78-121">只读。</span><span class="sxs-lookup"><span data-stu-id="9eb78-121">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="9eb78-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9eb78-122">JSON representation</span></span>

<span data-ttu-id="9eb78-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9eb78-123">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartLegendFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLegendFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

