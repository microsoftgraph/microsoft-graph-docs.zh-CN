---
title: ChartDataLabelFormat 资源类型
description: 封装图表数据表的格式属性。
author: lumine2008
ms.openlocfilehash: 4c8961eb884a5ab603feda368934795cb73915d0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356474"
---
# <a name="chartdatalabelformat-resource-type"></a><span data-ttu-id="de537-103">ChartDataLabelFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="de537-103">ChartDataLabelFormat resource type</span></span>

<span data-ttu-id="de537-104">封装图表数据表的格式属性。</span><span class="sxs-lookup"><span data-stu-id="de537-104">Encapsulates the format properties for the chart data labels.</span></span>


## <a name="methods"></a><span data-ttu-id="de537-105">方法</span><span class="sxs-lookup"><span data-stu-id="de537-105">Methods</span></span>
<span data-ttu-id="de537-106">无</span><span class="sxs-lookup"><span data-stu-id="de537-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="de537-107">属性</span><span class="sxs-lookup"><span data-stu-id="de537-107">Properties</span></span>
<span data-ttu-id="de537-108">无</span><span class="sxs-lookup"><span data-stu-id="de537-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="de537-109">Relationships</span><span class="sxs-lookup"><span data-stu-id="de537-109">Relationships</span></span>
| <span data-ttu-id="de537-110">关系</span><span class="sxs-lookup"><span data-stu-id="de537-110">Relationship</span></span> | <span data-ttu-id="de537-111">类型</span><span class="sxs-lookup"><span data-stu-id="de537-111">Type</span></span>   |<span data-ttu-id="de537-112">说明</span><span class="sxs-lookup"><span data-stu-id="de537-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de537-113">fill</span><span class="sxs-lookup"><span data-stu-id="de537-113">fill</span></span>|[<span data-ttu-id="de537-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="de537-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="de537-p101">表示当前图表数据标签的填充格式。只读。</span><span class="sxs-lookup"><span data-stu-id="de537-p101">Represents the fill format of the current chart data label. Read-only.</span></span>|
|<span data-ttu-id="de537-117">font</span><span class="sxs-lookup"><span data-stu-id="de537-117">font</span></span>|[<span data-ttu-id="de537-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="de537-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="de537-p102">表示图表数据标签的字体属性（字体名称、字体大小、颜色等）。只读。</span><span class="sxs-lookup"><span data-stu-id="de537-p102">Represents the font attributes (font name, font size, color, etc.) for a chart data label. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="de537-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="de537-121">JSON representation</span></span>

<span data-ttu-id="de537-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de537-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
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
<!-- {
  "type": "#page.annotation",
  "description": "ChartDataLabelFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->