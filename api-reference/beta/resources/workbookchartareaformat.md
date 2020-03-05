---
title: workbookChartAreaFormat 资源类型
description: 封装整个图表区域的格式属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 69183153f066ba2b3521ec1519babb991491431e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519398"
---
# <a name="workbookchartareaformat-resource-type"></a><span data-ttu-id="1d1cf-103">workbookChartAreaFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="1d1cf-103">workbookChartAreaFormat resource type</span></span>

<span data-ttu-id="1d1cf-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="1d1cf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d1cf-105">封装整个图表区域的格式属性。</span><span class="sxs-lookup"><span data-stu-id="1d1cf-105">Encapsulates the format properties for the overall chart area.</span></span>


## <a name="methods"></a><span data-ttu-id="1d1cf-106">方法</span><span class="sxs-lookup"><span data-stu-id="1d1cf-106">Methods</span></span>
<span data-ttu-id="1d1cf-107">无</span><span class="sxs-lookup"><span data-stu-id="1d1cf-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="1d1cf-108">属性</span><span class="sxs-lookup"><span data-stu-id="1d1cf-108">Properties</span></span>
<span data-ttu-id="1d1cf-109">无</span><span class="sxs-lookup"><span data-stu-id="1d1cf-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="1d1cf-110">关系</span><span class="sxs-lookup"><span data-stu-id="1d1cf-110">Relationships</span></span>
| <span data-ttu-id="1d1cf-111">关系</span><span class="sxs-lookup"><span data-stu-id="1d1cf-111">Relationship</span></span> | <span data-ttu-id="1d1cf-112">类型</span><span class="sxs-lookup"><span data-stu-id="1d1cf-112">Type</span></span>   |<span data-ttu-id="1d1cf-113">说明</span><span class="sxs-lookup"><span data-stu-id="1d1cf-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d1cf-114">fill</span><span class="sxs-lookup"><span data-stu-id="1d1cf-114">fill</span></span>|[<span data-ttu-id="1d1cf-115">workbookChartFill</span><span class="sxs-lookup"><span data-stu-id="1d1cf-115">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="1d1cf-p101">表示对象的填充格式，包括背景格式信息。只读。</span><span class="sxs-lookup"><span data-stu-id="1d1cf-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="1d1cf-118">font</span><span class="sxs-lookup"><span data-stu-id="1d1cf-118">font</span></span>|[<span data-ttu-id="1d1cf-119">workbookChartFont</span><span class="sxs-lookup"><span data-stu-id="1d1cf-119">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="1d1cf-120">表示当前对象的字体属性（字体名称、字体大小、颜色等）。</span><span class="sxs-lookup"><span data-stu-id="1d1cf-120">Represents the font attributes (font name, font size, color, etc.) for the current object.</span></span> <span data-ttu-id="1d1cf-121">只读。</span><span class="sxs-lookup"><span data-stu-id="1d1cf-121">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1d1cf-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1d1cf-122">JSON representation</span></span>

<span data-ttu-id="1d1cf-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d1cf-123">Here is a JSON representation of the resource.</span></span>

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
