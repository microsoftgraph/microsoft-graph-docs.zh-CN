---
title: ChartTitleFormat 资源类型
description: 封装图表标题的格式属性。
ms.openlocfilehash: 7e84412adb46981a0a2b8570ed28c62d36936e36
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008487"
---
# <a name="charttitleformat-resource-type"></a><span data-ttu-id="50ca9-103">ChartTitleFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="50ca9-103">ChartTitleFormat resource type</span></span>

<span data-ttu-id="50ca9-104">封装图表标题的格式属性。</span><span class="sxs-lookup"><span data-stu-id="50ca9-104">Encapsulates the format properties for the chart title.</span></span>


## <a name="methods"></a><span data-ttu-id="50ca9-105">方法</span><span class="sxs-lookup"><span data-stu-id="50ca9-105">Methods</span></span>
<span data-ttu-id="50ca9-106">无</span><span class="sxs-lookup"><span data-stu-id="50ca9-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="50ca9-107">属性</span><span class="sxs-lookup"><span data-stu-id="50ca9-107">Properties</span></span>
<span data-ttu-id="50ca9-108">无</span><span class="sxs-lookup"><span data-stu-id="50ca9-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="50ca9-109">Relationships</span><span class="sxs-lookup"><span data-stu-id="50ca9-109">Relationships</span></span>
| <span data-ttu-id="50ca9-110">关系</span><span class="sxs-lookup"><span data-stu-id="50ca9-110">Relationship</span></span> | <span data-ttu-id="50ca9-111">类型</span><span class="sxs-lookup"><span data-stu-id="50ca9-111">Type</span></span>   |<span data-ttu-id="50ca9-112">说明</span><span class="sxs-lookup"><span data-stu-id="50ca9-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50ca9-113">fill</span><span class="sxs-lookup"><span data-stu-id="50ca9-113">fill</span></span>|[<span data-ttu-id="50ca9-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="50ca9-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="50ca9-p101">表示对象的填充格式，包括背景格式信息。只读。</span><span class="sxs-lookup"><span data-stu-id="50ca9-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="50ca9-117">font</span><span class="sxs-lookup"><span data-stu-id="50ca9-117">font</span></span>|[<span data-ttu-id="50ca9-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="50ca9-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="50ca9-p102">表示当前对象的字体属性（字体名称、字体大小、颜色等）。只读。</span><span class="sxs-lookup"><span data-stu-id="50ca9-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="50ca9-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="50ca9-121">JSON representation</span></span>

<span data-ttu-id="50ca9-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50ca9-122">Here is a JSON representation of the resource.</span></span>

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
