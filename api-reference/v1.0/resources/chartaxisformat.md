---
title: ChartAxisFormat 资源类型
description: 封装图表坐标轴的格式属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 92258887c9646890ee63d14aebcd32ada7a8aaa6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569247"
---
# <a name="chartaxisformat-resource-type"></a><span data-ttu-id="26e00-103">ChartAxisFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="26e00-103">ChartAxisFormat resource type</span></span>

<span data-ttu-id="26e00-104">封装图表坐标轴的格式属性。</span><span class="sxs-lookup"><span data-stu-id="26e00-104">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="26e00-105">方法</span><span class="sxs-lookup"><span data-stu-id="26e00-105">Methods</span></span>
<span data-ttu-id="26e00-106">无</span><span class="sxs-lookup"><span data-stu-id="26e00-106">None</span></span>
## <a name="properties"></a><span data-ttu-id="26e00-107">属性</span><span class="sxs-lookup"><span data-stu-id="26e00-107">Properties</span></span>
<span data-ttu-id="26e00-108">无</span><span class="sxs-lookup"><span data-stu-id="26e00-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="26e00-109">关系</span><span class="sxs-lookup"><span data-stu-id="26e00-109">Relationships</span></span>
| <span data-ttu-id="26e00-110">关系</span><span class="sxs-lookup"><span data-stu-id="26e00-110">Relationship</span></span> | <span data-ttu-id="26e00-111">类型</span><span class="sxs-lookup"><span data-stu-id="26e00-111">Type</span></span>   |<span data-ttu-id="26e00-112">说明</span><span class="sxs-lookup"><span data-stu-id="26e00-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26e00-113">font</span><span class="sxs-lookup"><span data-stu-id="26e00-113">font</span></span>|[<span data-ttu-id="26e00-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="26e00-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="26e00-p101">表示图表坐标轴元素的字体属性（字体名称、字体大小、颜色等）。只读。</span><span class="sxs-lookup"><span data-stu-id="26e00-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="26e00-117">line</span><span class="sxs-lookup"><span data-stu-id="26e00-117">line</span></span>|[<span data-ttu-id="26e00-118">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="26e00-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="26e00-119">表示图表线条格式。</span><span class="sxs-lookup"><span data-stu-id="26e00-119">Represents chart line formatting.</span></span> <span data-ttu-id="26e00-120">只读。</span><span class="sxs-lookup"><span data-stu-id="26e00-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="26e00-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="26e00-121">JSON representation</span></span>

<span data-ttu-id="26e00-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26e00-122">Here is a JSON representation of the resource.</span></span>

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
