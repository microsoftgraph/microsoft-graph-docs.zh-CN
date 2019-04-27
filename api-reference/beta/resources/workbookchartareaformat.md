---
title: workbookChartAreaFormat 资源类型
description: 封装整个图表区域的格式属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6554604e2bb4c49d7e14546f1c5079690f99637f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348555"
---
# <a name="workbookchartareaformat-resource-type"></a><span data-ttu-id="99117-103">workbookChartAreaFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="99117-103">workbookChartAreaFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99117-104">封装整个图表区域的格式属性。</span><span class="sxs-lookup"><span data-stu-id="99117-104">Encapsulates the format properties for the overall chart area.</span></span>


## <a name="methods"></a><span data-ttu-id="99117-105">方法</span><span class="sxs-lookup"><span data-stu-id="99117-105">Methods</span></span>
<span data-ttu-id="99117-106">无</span><span class="sxs-lookup"><span data-stu-id="99117-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="99117-107">属性</span><span class="sxs-lookup"><span data-stu-id="99117-107">Properties</span></span>
<span data-ttu-id="99117-108">无</span><span class="sxs-lookup"><span data-stu-id="99117-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="99117-109">关系</span><span class="sxs-lookup"><span data-stu-id="99117-109">Relationships</span></span>
| <span data-ttu-id="99117-110">关系</span><span class="sxs-lookup"><span data-stu-id="99117-110">Relationship</span></span> | <span data-ttu-id="99117-111">类型</span><span class="sxs-lookup"><span data-stu-id="99117-111">Type</span></span>   |<span data-ttu-id="99117-112">说明</span><span class="sxs-lookup"><span data-stu-id="99117-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99117-113">fill</span><span class="sxs-lookup"><span data-stu-id="99117-113">fill</span></span>|[<span data-ttu-id="99117-114">workbookChartFill</span><span class="sxs-lookup"><span data-stu-id="99117-114">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="99117-p101">表示对象的填充格式，包括背景格式信息。只读。</span><span class="sxs-lookup"><span data-stu-id="99117-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="99117-117">font</span><span class="sxs-lookup"><span data-stu-id="99117-117">font</span></span>|[<span data-ttu-id="99117-118">workbookChartFont</span><span class="sxs-lookup"><span data-stu-id="99117-118">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="99117-119">表示当前对象的字体属性（字体名称、字体大小、颜色等）。</span><span class="sxs-lookup"><span data-stu-id="99117-119">Represents the font attributes (font name, font size, color, etc.) for the current object.</span></span> <span data-ttu-id="99117-120">只读。</span><span class="sxs-lookup"><span data-stu-id="99117-120">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="99117-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="99117-121">JSON representation</span></span>

<span data-ttu-id="99117-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99117-122">Here is a JSON representation of the resource.</span></span>

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
