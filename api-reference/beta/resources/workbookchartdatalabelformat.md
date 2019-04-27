---
title: workbookChartDataLabelFormat 资源类型
description: 封装图表数据表的格式属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a4bf03bb2c40ce0dc78c24d76e859d040526cf17
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348356"
---
# <a name="workbookchartdatalabelformat-resource-type"></a><span data-ttu-id="d0984-103">workbookChartDataLabelFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="d0984-103">workbookChartDataLabelFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0984-104">封装图表数据表的格式属性。</span><span class="sxs-lookup"><span data-stu-id="d0984-104">Encapsulates the format properties for the chart data labels.</span></span>


## <a name="methods"></a><span data-ttu-id="d0984-105">方法</span><span class="sxs-lookup"><span data-stu-id="d0984-105">Methods</span></span>
<span data-ttu-id="d0984-106">无</span><span class="sxs-lookup"><span data-stu-id="d0984-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="d0984-107">属性</span><span class="sxs-lookup"><span data-stu-id="d0984-107">Properties</span></span>
<span data-ttu-id="d0984-108">无</span><span class="sxs-lookup"><span data-stu-id="d0984-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="d0984-109">关系</span><span class="sxs-lookup"><span data-stu-id="d0984-109">Relationships</span></span>
| <span data-ttu-id="d0984-110">关系</span><span class="sxs-lookup"><span data-stu-id="d0984-110">Relationship</span></span> | <span data-ttu-id="d0984-111">类型</span><span class="sxs-lookup"><span data-stu-id="d0984-111">Type</span></span>   |<span data-ttu-id="d0984-112">说明</span><span class="sxs-lookup"><span data-stu-id="d0984-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0984-113">fill</span><span class="sxs-lookup"><span data-stu-id="d0984-113">fill</span></span>|[<span data-ttu-id="d0984-114">workbookChartFill</span><span class="sxs-lookup"><span data-stu-id="d0984-114">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="d0984-p101">表示当前图表数据标签的填充格式。只读。</span><span class="sxs-lookup"><span data-stu-id="d0984-p101">Represents the fill format of the current chart data label. Read-only.</span></span>|
|<span data-ttu-id="d0984-117">font</span><span class="sxs-lookup"><span data-stu-id="d0984-117">font</span></span>|[<span data-ttu-id="d0984-118">workbookChartFont</span><span class="sxs-lookup"><span data-stu-id="d0984-118">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="d0984-119">表示图表数据标签的字体属性（字体名称、字体大小、颜色等）。</span><span class="sxs-lookup"><span data-stu-id="d0984-119">Represents the font attributes (font name, font size, color, etc.) for a chart data label.</span></span> <span data-ttu-id="d0984-120">只读。</span><span class="sxs-lookup"><span data-stu-id="d0984-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="d0984-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d0984-121">JSON representation</span></span>

<span data-ttu-id="d0984-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d0984-122">Here is a JSON representation of the resource.</span></span>

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
