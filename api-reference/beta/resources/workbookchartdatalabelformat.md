---
title: workbookChartDataLabelFormat 资源类型
description: 封装图表数据表的格式属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 883f2ff1ce1c0b89f1525ea39e0adb558a1870cc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979292"
---
# <a name="workbookchartdatalabelformat-resource-type"></a><span data-ttu-id="89393-103">workbookChartDataLabelFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="89393-103">workbookChartDataLabelFormat resource type</span></span>

<span data-ttu-id="89393-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89393-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89393-105">封装图表数据表的格式属性。</span><span class="sxs-lookup"><span data-stu-id="89393-105">Encapsulates the format properties for the chart data labels.</span></span>


## <a name="methods"></a><span data-ttu-id="89393-106">方法</span><span class="sxs-lookup"><span data-stu-id="89393-106">Methods</span></span>
<span data-ttu-id="89393-107">无</span><span class="sxs-lookup"><span data-stu-id="89393-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="89393-108">属性</span><span class="sxs-lookup"><span data-stu-id="89393-108">Properties</span></span>
<span data-ttu-id="89393-109">无</span><span class="sxs-lookup"><span data-stu-id="89393-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="89393-110">关系</span><span class="sxs-lookup"><span data-stu-id="89393-110">Relationships</span></span>
| <span data-ttu-id="89393-111">关系</span><span class="sxs-lookup"><span data-stu-id="89393-111">Relationship</span></span> | <span data-ttu-id="89393-112">类型</span><span class="sxs-lookup"><span data-stu-id="89393-112">Type</span></span>   |<span data-ttu-id="89393-113">说明</span><span class="sxs-lookup"><span data-stu-id="89393-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89393-114">fill</span><span class="sxs-lookup"><span data-stu-id="89393-114">fill</span></span>|[<span data-ttu-id="89393-115">workbookChartFill</span><span class="sxs-lookup"><span data-stu-id="89393-115">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="89393-p101">表示当前图表数据标签的填充格式。只读。</span><span class="sxs-lookup"><span data-stu-id="89393-p101">Represents the fill format of the current chart data label. Read-only.</span></span>|
|<span data-ttu-id="89393-118">font</span><span class="sxs-lookup"><span data-stu-id="89393-118">font</span></span>|[<span data-ttu-id="89393-119">workbookChartFont</span><span class="sxs-lookup"><span data-stu-id="89393-119">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="89393-120">表示图表数据标签的字体属性（字体名称、字体大小、颜色等）。</span><span class="sxs-lookup"><span data-stu-id="89393-120">Represents the font attributes (font name, font size, color, etc.) for a chart data label.</span></span> <span data-ttu-id="89393-121">只读。</span><span class="sxs-lookup"><span data-stu-id="89393-121">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="89393-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="89393-122">JSON representation</span></span>

<span data-ttu-id="89393-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89393-123">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "fill",
    "font"
    ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartDataLabelFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartDataLabelFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


