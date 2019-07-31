---
title: workbookChartAxisFormat 资源类型
description: 封装图表坐标轴的格式属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 91e749fd0f1449883eca261f5ef27c0f2a7ba5dc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964084"
---
# <a name="workbookchartaxisformat-resource-type"></a><span data-ttu-id="ab462-103">workbookChartAxisFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="ab462-103">workbookChartAxisFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab462-104">封装图表坐标轴的格式属性。</span><span class="sxs-lookup"><span data-stu-id="ab462-104">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="ab462-105">方法</span><span class="sxs-lookup"><span data-stu-id="ab462-105">Methods</span></span>
<span data-ttu-id="ab462-106">无</span><span class="sxs-lookup"><span data-stu-id="ab462-106">None</span></span>
## <a name="properties"></a><span data-ttu-id="ab462-107">属性</span><span class="sxs-lookup"><span data-stu-id="ab462-107">Properties</span></span>
<span data-ttu-id="ab462-108">无</span><span class="sxs-lookup"><span data-stu-id="ab462-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="ab462-109">关系</span><span class="sxs-lookup"><span data-stu-id="ab462-109">Relationships</span></span>
| <span data-ttu-id="ab462-110">关系</span><span class="sxs-lookup"><span data-stu-id="ab462-110">Relationship</span></span> | <span data-ttu-id="ab462-111">类型</span><span class="sxs-lookup"><span data-stu-id="ab462-111">Type</span></span>   |<span data-ttu-id="ab462-112">说明</span><span class="sxs-lookup"><span data-stu-id="ab462-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ab462-113">font</span><span class="sxs-lookup"><span data-stu-id="ab462-113">font</span></span>|[<span data-ttu-id="ab462-114">workbookChartFont</span><span class="sxs-lookup"><span data-stu-id="ab462-114">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="ab462-p101">表示图表坐标轴元素的字体属性（字体名称、字体大小、颜色等）。只读。</span><span class="sxs-lookup"><span data-stu-id="ab462-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="ab462-117">line</span><span class="sxs-lookup"><span data-stu-id="ab462-117">line</span></span>|[<span data-ttu-id="ab462-118">workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="ab462-118">workbookChartLineFormat</span></span>](workbookchartlineformat.md)|<span data-ttu-id="ab462-119">表示图表线条格式。</span><span class="sxs-lookup"><span data-stu-id="ab462-119">Represents chart line formatting.</span></span> <span data-ttu-id="ab462-120">只读。</span><span class="sxs-lookup"><span data-stu-id="ab462-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="ab462-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ab462-121">JSON representation</span></span>

<span data-ttu-id="ab462-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab462-122">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
