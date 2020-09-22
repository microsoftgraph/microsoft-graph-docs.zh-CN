---
title: workbookChartAxisFormat 资源类型
description: 封装图表坐标轴的格式属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: d04f885f135eadf2a8404b7e17b3b2ed32554e14
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039053"
---
# <a name="workbookchartaxisformat-resource-type"></a><span data-ttu-id="8960c-103">workbookChartAxisFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="8960c-103">workbookChartAxisFormat resource type</span></span>

<span data-ttu-id="8960c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8960c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8960c-105">封装图表坐标轴的格式属性。</span><span class="sxs-lookup"><span data-stu-id="8960c-105">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="8960c-106">方法</span><span class="sxs-lookup"><span data-stu-id="8960c-106">Methods</span></span>
<span data-ttu-id="8960c-107">无</span><span class="sxs-lookup"><span data-stu-id="8960c-107">None</span></span>
## <a name="properties"></a><span data-ttu-id="8960c-108">属性</span><span class="sxs-lookup"><span data-stu-id="8960c-108">Properties</span></span>
<span data-ttu-id="8960c-109">无</span><span class="sxs-lookup"><span data-stu-id="8960c-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="8960c-110">关系</span><span class="sxs-lookup"><span data-stu-id="8960c-110">Relationships</span></span>
| <span data-ttu-id="8960c-111">关系</span><span class="sxs-lookup"><span data-stu-id="8960c-111">Relationship</span></span> | <span data-ttu-id="8960c-112">类型</span><span class="sxs-lookup"><span data-stu-id="8960c-112">Type</span></span>   |<span data-ttu-id="8960c-113">说明</span><span class="sxs-lookup"><span data-stu-id="8960c-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8960c-114">font</span><span class="sxs-lookup"><span data-stu-id="8960c-114">font</span></span>|[<span data-ttu-id="8960c-115">workbookChartFont</span><span class="sxs-lookup"><span data-stu-id="8960c-115">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="8960c-p101">表示图表坐标轴元素的字体属性（字体名称、字体大小、颜色等）。只读。</span><span class="sxs-lookup"><span data-stu-id="8960c-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="8960c-118">line</span><span class="sxs-lookup"><span data-stu-id="8960c-118">line</span></span>|[<span data-ttu-id="8960c-119">workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="8960c-119">workbookChartLineFormat</span></span>](workbookchartlineformat.md)|<span data-ttu-id="8960c-120">表示图表线条格式。</span><span class="sxs-lookup"><span data-stu-id="8960c-120">Represents chart line formatting.</span></span> <span data-ttu-id="8960c-121">只读。</span><span class="sxs-lookup"><span data-stu-id="8960c-121">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="8960c-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8960c-122">JSON representation</span></span>

<span data-ttu-id="8960c-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8960c-123">Here is a JSON representation of the resource.</span></span>

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


