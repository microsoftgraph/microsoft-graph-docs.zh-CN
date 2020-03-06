---
title: ChartTitleFormat 资源类型
description: 封装图表标题的格式属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: da702a7718765af464525c3ae2fafc8376296d25
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533088"
---
# <a name="charttitleformat-resource-type"></a><span data-ttu-id="db5a3-103">ChartTitleFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="db5a3-103">ChartTitleFormat resource type</span></span>

<span data-ttu-id="db5a3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db5a3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="db5a3-105">封装图表标题的格式属性。</span><span class="sxs-lookup"><span data-stu-id="db5a3-105">Encapsulates the format properties for the chart title.</span></span>


## <a name="methods"></a><span data-ttu-id="db5a3-106">Methods</span><span class="sxs-lookup"><span data-stu-id="db5a3-106">Methods</span></span>
<span data-ttu-id="db5a3-107">无</span><span class="sxs-lookup"><span data-stu-id="db5a3-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="db5a3-108">属性</span><span class="sxs-lookup"><span data-stu-id="db5a3-108">Properties</span></span>
<span data-ttu-id="db5a3-109">无</span><span class="sxs-lookup"><span data-stu-id="db5a3-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="db5a3-110">关系</span><span class="sxs-lookup"><span data-stu-id="db5a3-110">Relationships</span></span>
| <span data-ttu-id="db5a3-111">关系</span><span class="sxs-lookup"><span data-stu-id="db5a3-111">Relationship</span></span> | <span data-ttu-id="db5a3-112">类型</span><span class="sxs-lookup"><span data-stu-id="db5a3-112">Type</span></span>   |<span data-ttu-id="db5a3-113">说明</span><span class="sxs-lookup"><span data-stu-id="db5a3-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db5a3-114">fill</span><span class="sxs-lookup"><span data-stu-id="db5a3-114">fill</span></span>|[<span data-ttu-id="db5a3-115">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="db5a3-115">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="db5a3-p101">表示对象的填充格式，包括背景格式信息。只读。</span><span class="sxs-lookup"><span data-stu-id="db5a3-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="db5a3-118">font</span><span class="sxs-lookup"><span data-stu-id="db5a3-118">font</span></span>|[<span data-ttu-id="db5a3-119">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="db5a3-119">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="db5a3-120">表示当前对象的字体属性（字体名称、字体大小、颜色等）。</span><span class="sxs-lookup"><span data-stu-id="db5a3-120">Represents the font attributes (font name, font size, color, etc.) for the current object.</span></span> <span data-ttu-id="db5a3-121">只读。</span><span class="sxs-lookup"><span data-stu-id="db5a3-121">Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="db5a3-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="db5a3-122">JSON representation</span></span>

<span data-ttu-id="db5a3-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db5a3-123">Here is a JSON representation of the resource.</span></span>

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
