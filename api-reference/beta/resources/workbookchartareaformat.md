---
title: workbookChartAreaFormat 资源类型
description: 封装整个图表区域的格式属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 02e176887053654c103bf2aedaf86f48831d9d08
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039137"
---
# <a name="workbookchartareaformat-resource-type"></a><span data-ttu-id="d273f-103">workbookChartAreaFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="d273f-103">workbookChartAreaFormat resource type</span></span>

<span data-ttu-id="d273f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d273f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d273f-105">封装整个图表区域的格式属性。</span><span class="sxs-lookup"><span data-stu-id="d273f-105">Encapsulates the format properties for the overall chart area.</span></span>


## <a name="methods"></a><span data-ttu-id="d273f-106">方法</span><span class="sxs-lookup"><span data-stu-id="d273f-106">Methods</span></span>
<span data-ttu-id="d273f-107">无</span><span class="sxs-lookup"><span data-stu-id="d273f-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="d273f-108">属性</span><span class="sxs-lookup"><span data-stu-id="d273f-108">Properties</span></span>
<span data-ttu-id="d273f-109">无</span><span class="sxs-lookup"><span data-stu-id="d273f-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="d273f-110">关系</span><span class="sxs-lookup"><span data-stu-id="d273f-110">Relationships</span></span>
| <span data-ttu-id="d273f-111">关系</span><span class="sxs-lookup"><span data-stu-id="d273f-111">Relationship</span></span> | <span data-ttu-id="d273f-112">类型</span><span class="sxs-lookup"><span data-stu-id="d273f-112">Type</span></span>   |<span data-ttu-id="d273f-113">说明</span><span class="sxs-lookup"><span data-stu-id="d273f-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d273f-114">fill</span><span class="sxs-lookup"><span data-stu-id="d273f-114">fill</span></span>|[<span data-ttu-id="d273f-115">workbookChartFill</span><span class="sxs-lookup"><span data-stu-id="d273f-115">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="d273f-p101">表示对象的填充格式，包括背景格式信息。只读。</span><span class="sxs-lookup"><span data-stu-id="d273f-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="d273f-118">font</span><span class="sxs-lookup"><span data-stu-id="d273f-118">font</span></span>|[<span data-ttu-id="d273f-119">workbookChartFont</span><span class="sxs-lookup"><span data-stu-id="d273f-119">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="d273f-120">表示当前对象的字体属性（字体名称、字体大小、颜色等）。</span><span class="sxs-lookup"><span data-stu-id="d273f-120">Represents the font attributes (font name, font size, color, etc.) for the current object.</span></span> <span data-ttu-id="d273f-121">只读。</span><span class="sxs-lookup"><span data-stu-id="d273f-121">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d273f-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d273f-122">JSON representation</span></span>

<span data-ttu-id="d273f-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d273f-123">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "fill",
    "font"
    ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAreaFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartAreaFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


