---
title: ChartAxisFormat 资源类型
description: 封装图表坐标轴的格式属性。
author: lumine2008
ms.openlocfilehash: e503b4e62ef7907943f10a395f12eb5d86c1928f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359456"
---
# <a name="chartaxisformat-resource-type"></a><span data-ttu-id="c2c69-103">ChartAxisFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="c2c69-103">ChartAxisFormat resource type</span></span>

<span data-ttu-id="c2c69-104">封装图表坐标轴的格式属性。</span><span class="sxs-lookup"><span data-stu-id="c2c69-104">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="c2c69-105">方法</span><span class="sxs-lookup"><span data-stu-id="c2c69-105">Methods</span></span>
<span data-ttu-id="c2c69-106">无</span><span class="sxs-lookup"><span data-stu-id="c2c69-106">None</span></span>
## <a name="properties"></a><span data-ttu-id="c2c69-107">属性</span><span class="sxs-lookup"><span data-stu-id="c2c69-107">Properties</span></span>
<span data-ttu-id="c2c69-108">无</span><span class="sxs-lookup"><span data-stu-id="c2c69-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="c2c69-109">Relationships</span><span class="sxs-lookup"><span data-stu-id="c2c69-109">Relationships</span></span>
| <span data-ttu-id="c2c69-110">关系</span><span class="sxs-lookup"><span data-stu-id="c2c69-110">Relationship</span></span> | <span data-ttu-id="c2c69-111">类型</span><span class="sxs-lookup"><span data-stu-id="c2c69-111">Type</span></span>   |<span data-ttu-id="c2c69-112">说明</span><span class="sxs-lookup"><span data-stu-id="c2c69-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2c69-113">font</span><span class="sxs-lookup"><span data-stu-id="c2c69-113">font</span></span>|[<span data-ttu-id="c2c69-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="c2c69-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="c2c69-p101">表示图表坐标轴元素的字体属性（字体名称、字体大小、颜色等）。只读。</span><span class="sxs-lookup"><span data-stu-id="c2c69-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="c2c69-117">line</span><span class="sxs-lookup"><span data-stu-id="c2c69-117">line</span></span>|[<span data-ttu-id="c2c69-118">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="c2c69-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="c2c69-p102">表示图表线条格式。只读。</span><span class="sxs-lookup"><span data-stu-id="c2c69-p102">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="c2c69-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c2c69-121">JSON representation</span></span>

<span data-ttu-id="c2c69-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c2c69-122">Here is a JSON representation of the resource.</span></span>

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