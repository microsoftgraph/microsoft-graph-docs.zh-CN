---
title: ChartAxisFormat 资源类型
description: 封装图表坐标轴的格式属性。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: a219122141da1f384279d0ff4c612f62226612c9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821264"
---
# <a name="chartaxisformat-resource-type"></a><span data-ttu-id="7639f-103">ChartAxisFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="7639f-103">ChartAxisFormat resource type</span></span>

<span data-ttu-id="7639f-104">封装图表坐标轴的格式属性。</span><span class="sxs-lookup"><span data-stu-id="7639f-104">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="7639f-105">方法</span><span class="sxs-lookup"><span data-stu-id="7639f-105">Methods</span></span>
<span data-ttu-id="7639f-106">无</span><span class="sxs-lookup"><span data-stu-id="7639f-106">None</span></span>
## <a name="properties"></a><span data-ttu-id="7639f-107">属性</span><span class="sxs-lookup"><span data-stu-id="7639f-107">Properties</span></span>
<span data-ttu-id="7639f-108">无</span><span class="sxs-lookup"><span data-stu-id="7639f-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="7639f-109">Relationships</span><span class="sxs-lookup"><span data-stu-id="7639f-109">Relationships</span></span>
| <span data-ttu-id="7639f-110">关系</span><span class="sxs-lookup"><span data-stu-id="7639f-110">Relationship</span></span> | <span data-ttu-id="7639f-111">类型</span><span class="sxs-lookup"><span data-stu-id="7639f-111">Type</span></span>   |<span data-ttu-id="7639f-112">说明</span><span class="sxs-lookup"><span data-stu-id="7639f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7639f-113">font</span><span class="sxs-lookup"><span data-stu-id="7639f-113">font</span></span>|[<span data-ttu-id="7639f-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="7639f-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="7639f-p101">表示图表坐标轴元素的字体属性（字体名称、字体大小、颜色等）。只读。</span><span class="sxs-lookup"><span data-stu-id="7639f-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="7639f-117">line</span><span class="sxs-lookup"><span data-stu-id="7639f-117">line</span></span>|[<span data-ttu-id="7639f-118">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="7639f-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="7639f-p102">表示图表线条格式。只读。</span><span class="sxs-lookup"><span data-stu-id="7639f-p102">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="7639f-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7639f-121">JSON representation</span></span>

<span data-ttu-id="7639f-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7639f-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"},
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
