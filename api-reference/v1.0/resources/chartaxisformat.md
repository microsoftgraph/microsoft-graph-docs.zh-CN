---
title: ChartAxisFormat 资源类型
description: 封装图表坐标轴的格式属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 1d52063e63e179540bcbd5c3b4ec0cd09fb620d7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029853"
---
# <a name="chartaxisformat-resource-type"></a><span data-ttu-id="a1118-103">ChartAxisFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="a1118-103">ChartAxisFormat resource type</span></span>

<span data-ttu-id="a1118-104">封装图表坐标轴的格式属性。</span><span class="sxs-lookup"><span data-stu-id="a1118-104">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="a1118-105">方法</span><span class="sxs-lookup"><span data-stu-id="a1118-105">Methods</span></span>
<span data-ttu-id="a1118-106">无</span><span class="sxs-lookup"><span data-stu-id="a1118-106">None</span></span>
## <a name="properties"></a><span data-ttu-id="a1118-107">属性</span><span class="sxs-lookup"><span data-stu-id="a1118-107">Properties</span></span>
<span data-ttu-id="a1118-108">无</span><span class="sxs-lookup"><span data-stu-id="a1118-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="a1118-109">关系</span><span class="sxs-lookup"><span data-stu-id="a1118-109">Relationships</span></span>
| <span data-ttu-id="a1118-110">关系</span><span class="sxs-lookup"><span data-stu-id="a1118-110">Relationship</span></span> | <span data-ttu-id="a1118-111">类型</span><span class="sxs-lookup"><span data-stu-id="a1118-111">Type</span></span>   |<span data-ttu-id="a1118-112">说明</span><span class="sxs-lookup"><span data-stu-id="a1118-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1118-113">font</span><span class="sxs-lookup"><span data-stu-id="a1118-113">font</span></span>|[<span data-ttu-id="a1118-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="a1118-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="a1118-p101">表示图表坐标轴元素的字体属性（字体名称、字体大小、颜色等）。只读。</span><span class="sxs-lookup"><span data-stu-id="a1118-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="a1118-117">line</span><span class="sxs-lookup"><span data-stu-id="a1118-117">line</span></span>|[<span data-ttu-id="a1118-118">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="a1118-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="a1118-119">表示图表线条格式。</span><span class="sxs-lookup"><span data-stu-id="a1118-119">Represents chart line formatting.</span></span> <span data-ttu-id="a1118-120">只读。</span><span class="sxs-lookup"><span data-stu-id="a1118-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="a1118-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a1118-121">JSON representation</span></span>

<span data-ttu-id="a1118-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1118-122">Here is a JSON representation of the resource.</span></span>

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
