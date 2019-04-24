---
title: ChartTitleFormat 资源类型
description: 封装图表标题的格式属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3a2c16d37d2ca86d7cafbb4047ee0bcea1ee4bde
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585046"
---
# <a name="charttitleformat-resource-type"></a><span data-ttu-id="5069e-103">ChartTitleFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="5069e-103">ChartTitleFormat resource type</span></span>

<span data-ttu-id="5069e-104">封装图表标题的格式属性。</span><span class="sxs-lookup"><span data-stu-id="5069e-104">Encapsulates the format properties for the chart title.</span></span>


## <a name="methods"></a><span data-ttu-id="5069e-105">方法</span><span class="sxs-lookup"><span data-stu-id="5069e-105">Methods</span></span>
<span data-ttu-id="5069e-106">无</span><span class="sxs-lookup"><span data-stu-id="5069e-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="5069e-107">属性</span><span class="sxs-lookup"><span data-stu-id="5069e-107">Properties</span></span>
<span data-ttu-id="5069e-108">无</span><span class="sxs-lookup"><span data-stu-id="5069e-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="5069e-109">关系</span><span class="sxs-lookup"><span data-stu-id="5069e-109">Relationships</span></span>
| <span data-ttu-id="5069e-110">关系</span><span class="sxs-lookup"><span data-stu-id="5069e-110">Relationship</span></span> | <span data-ttu-id="5069e-111">类型</span><span class="sxs-lookup"><span data-stu-id="5069e-111">Type</span></span>   |<span data-ttu-id="5069e-112">说明</span><span class="sxs-lookup"><span data-stu-id="5069e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5069e-113">fill</span><span class="sxs-lookup"><span data-stu-id="5069e-113">fill</span></span>|[<span data-ttu-id="5069e-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="5069e-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="5069e-p101">表示对象的填充格式，包括背景格式信息。只读。</span><span class="sxs-lookup"><span data-stu-id="5069e-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="5069e-117">font</span><span class="sxs-lookup"><span data-stu-id="5069e-117">font</span></span>|[<span data-ttu-id="5069e-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="5069e-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="5069e-119">表示当前对象的字体属性（字体名称、字体大小、颜色等）。</span><span class="sxs-lookup"><span data-stu-id="5069e-119">Represents the font attributes (font name, font size, color, etc.) for the current object.</span></span> <span data-ttu-id="5069e-120">只读。</span><span class="sxs-lookup"><span data-stu-id="5069e-120">Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="5069e-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5069e-121">JSON representation</span></span>

<span data-ttu-id="5069e-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5069e-122">Here is a JSON representation of the resource.</span></span>

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
