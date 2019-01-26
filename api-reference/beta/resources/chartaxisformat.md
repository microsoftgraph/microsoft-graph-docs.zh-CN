---
title: ChartAxisFormat 资源类型
description: 封装图表坐标轴的格式属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 587c35f0bf28d695f67e61a8eefa1593317a8d5d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577107"
---
# <a name="chartaxisformat-resource-type"></a><span data-ttu-id="77f53-103">ChartAxisFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="77f53-103">ChartAxisFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77f53-104">封装图表坐标轴的格式属性。</span><span class="sxs-lookup"><span data-stu-id="77f53-104">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="77f53-105">方法</span><span class="sxs-lookup"><span data-stu-id="77f53-105">Methods</span></span>
<span data-ttu-id="77f53-106">无</span><span class="sxs-lookup"><span data-stu-id="77f53-106">None</span></span>
## <a name="properties"></a><span data-ttu-id="77f53-107">属性</span><span class="sxs-lookup"><span data-stu-id="77f53-107">Properties</span></span>
<span data-ttu-id="77f53-108">无</span><span class="sxs-lookup"><span data-stu-id="77f53-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="77f53-109">关系</span><span class="sxs-lookup"><span data-stu-id="77f53-109">Relationships</span></span>
| <span data-ttu-id="77f53-110">关系</span><span class="sxs-lookup"><span data-stu-id="77f53-110">Relationship</span></span> | <span data-ttu-id="77f53-111">类型</span><span class="sxs-lookup"><span data-stu-id="77f53-111">Type</span></span>   |<span data-ttu-id="77f53-112">说明</span><span class="sxs-lookup"><span data-stu-id="77f53-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77f53-113">font</span><span class="sxs-lookup"><span data-stu-id="77f53-113">font</span></span>|[<span data-ttu-id="77f53-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="77f53-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="77f53-p101">表示图表坐标轴元素的字体属性（字体名称、字体大小、颜色等）。只读。</span><span class="sxs-lookup"><span data-stu-id="77f53-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="77f53-117">line</span><span class="sxs-lookup"><span data-stu-id="77f53-117">line</span></span>|[<span data-ttu-id="77f53-118">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="77f53-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="77f53-p102">表示图表线条格式。只读。</span><span class="sxs-lookup"><span data-stu-id="77f53-p102">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="77f53-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="77f53-121">JSON representation</span></span>

<span data-ttu-id="77f53-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="77f53-122">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxisFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartaxisformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
