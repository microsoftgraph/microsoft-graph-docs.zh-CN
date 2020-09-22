---
title: ChartTitleFormat 资源类型
description: 封装图表标题的格式属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 632b3a165a5f2f3a4216868bf440099610cdc800
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059213"
---
# <a name="charttitleformat-resource-type"></a><span data-ttu-id="225f7-103">ChartTitleFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="225f7-103">ChartTitleFormat resource type</span></span>

<span data-ttu-id="225f7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="225f7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="225f7-105">封装图表标题的格式属性。</span><span class="sxs-lookup"><span data-stu-id="225f7-105">Encapsulates the format properties for the chart title.</span></span>


## <a name="methods"></a><span data-ttu-id="225f7-106">方法</span><span class="sxs-lookup"><span data-stu-id="225f7-106">Methods</span></span>
<span data-ttu-id="225f7-107">无</span><span class="sxs-lookup"><span data-stu-id="225f7-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="225f7-108">属性</span><span class="sxs-lookup"><span data-stu-id="225f7-108">Properties</span></span>
<span data-ttu-id="225f7-109">无</span><span class="sxs-lookup"><span data-stu-id="225f7-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="225f7-110">关系</span><span class="sxs-lookup"><span data-stu-id="225f7-110">Relationships</span></span>
| <span data-ttu-id="225f7-111">关系</span><span class="sxs-lookup"><span data-stu-id="225f7-111">Relationship</span></span> | <span data-ttu-id="225f7-112">类型</span><span class="sxs-lookup"><span data-stu-id="225f7-112">Type</span></span>   |<span data-ttu-id="225f7-113">说明</span><span class="sxs-lookup"><span data-stu-id="225f7-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="225f7-114">fill</span><span class="sxs-lookup"><span data-stu-id="225f7-114">fill</span></span>|[<span data-ttu-id="225f7-115">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="225f7-115">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="225f7-p101">表示对象的填充格式，包括背景格式信息。只读。</span><span class="sxs-lookup"><span data-stu-id="225f7-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="225f7-118">font</span><span class="sxs-lookup"><span data-stu-id="225f7-118">font</span></span>|[<span data-ttu-id="225f7-119">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="225f7-119">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="225f7-120">表示当前对象的字体属性（字体名称、字体大小、颜色等）。</span><span class="sxs-lookup"><span data-stu-id="225f7-120">Represents the font attributes (font name, font size, color, etc.) for the current object.</span></span> <span data-ttu-id="225f7-121">只读。</span><span class="sxs-lookup"><span data-stu-id="225f7-121">Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="225f7-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="225f7-122">JSON representation</span></span>

<span data-ttu-id="225f7-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="225f7-123">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartTitleFormat"
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
  "description": "ChartAreaFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

