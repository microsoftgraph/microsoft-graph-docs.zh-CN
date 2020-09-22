---
title: ChartAxisFormat 资源类型
description: 封装图表坐标轴的格式属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 18021b2776ccd749538ba5a94e7af9b1518a9bb6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988441"
---
# <a name="chartaxisformat-resource-type"></a><span data-ttu-id="edc23-103">ChartAxisFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="edc23-103">ChartAxisFormat resource type</span></span>

<span data-ttu-id="edc23-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edc23-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="edc23-105">封装图表坐标轴的格式属性。</span><span class="sxs-lookup"><span data-stu-id="edc23-105">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="edc23-106">方法</span><span class="sxs-lookup"><span data-stu-id="edc23-106">Methods</span></span>
<span data-ttu-id="edc23-107">无</span><span class="sxs-lookup"><span data-stu-id="edc23-107">None</span></span>
## <a name="properties"></a><span data-ttu-id="edc23-108">属性</span><span class="sxs-lookup"><span data-stu-id="edc23-108">Properties</span></span>
<span data-ttu-id="edc23-109">无</span><span class="sxs-lookup"><span data-stu-id="edc23-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="edc23-110">关系</span><span class="sxs-lookup"><span data-stu-id="edc23-110">Relationships</span></span>
| <span data-ttu-id="edc23-111">关系</span><span class="sxs-lookup"><span data-stu-id="edc23-111">Relationship</span></span> | <span data-ttu-id="edc23-112">类型</span><span class="sxs-lookup"><span data-stu-id="edc23-112">Type</span></span>   |<span data-ttu-id="edc23-113">说明</span><span class="sxs-lookup"><span data-stu-id="edc23-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="edc23-114">font</span><span class="sxs-lookup"><span data-stu-id="edc23-114">font</span></span>|[<span data-ttu-id="edc23-115">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="edc23-115">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="edc23-p101">表示图表坐标轴元素的字体属性（字体名称、字体大小、颜色等）。只读。</span><span class="sxs-lookup"><span data-stu-id="edc23-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="edc23-118">line</span><span class="sxs-lookup"><span data-stu-id="edc23-118">line</span></span>|[<span data-ttu-id="edc23-119">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="edc23-119">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="edc23-120">表示图表线条格式。</span><span class="sxs-lookup"><span data-stu-id="edc23-120">Represents chart line formatting.</span></span> <span data-ttu-id="edc23-121">只读。</span><span class="sxs-lookup"><span data-stu-id="edc23-121">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="edc23-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="edc23-122">JSON representation</span></span>

<span data-ttu-id="edc23-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="edc23-123">Here is a JSON representation of the resource.</span></span>

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

