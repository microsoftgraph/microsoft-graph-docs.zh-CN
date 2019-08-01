---
title: ChartAreaFormat 资源类型
description: 封装整个图表区域的格式属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ee39e1fc58fe604ff24433dcb540b44e22bb3ee9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033003"
---
# <a name="chartareaformat-resource-type"></a><span data-ttu-id="0554a-103">ChartAreaFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="0554a-103">ChartAreaFormat resource type</span></span>

<span data-ttu-id="0554a-104">封装整个图表区域的格式属性。</span><span class="sxs-lookup"><span data-stu-id="0554a-104">Encapsulates the format properties for the overall chart area.</span></span>


## <a name="methods"></a><span data-ttu-id="0554a-105">方法</span><span class="sxs-lookup"><span data-stu-id="0554a-105">Methods</span></span>
<span data-ttu-id="0554a-106">无</span><span class="sxs-lookup"><span data-stu-id="0554a-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="0554a-107">属性</span><span class="sxs-lookup"><span data-stu-id="0554a-107">Properties</span></span>
<span data-ttu-id="0554a-108">无</span><span class="sxs-lookup"><span data-stu-id="0554a-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="0554a-109">关系</span><span class="sxs-lookup"><span data-stu-id="0554a-109">Relationships</span></span>
| <span data-ttu-id="0554a-110">关系</span><span class="sxs-lookup"><span data-stu-id="0554a-110">Relationship</span></span> | <span data-ttu-id="0554a-111">类型</span><span class="sxs-lookup"><span data-stu-id="0554a-111">Type</span></span>   |<span data-ttu-id="0554a-112">说明</span><span class="sxs-lookup"><span data-stu-id="0554a-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0554a-113">fill</span><span class="sxs-lookup"><span data-stu-id="0554a-113">fill</span></span>|[<span data-ttu-id="0554a-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="0554a-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="0554a-p101">表示对象的填充格式，包括背景格式信息。只读。</span><span class="sxs-lookup"><span data-stu-id="0554a-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="0554a-117">font</span><span class="sxs-lookup"><span data-stu-id="0554a-117">font</span></span>|[<span data-ttu-id="0554a-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="0554a-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="0554a-119">表示当前对象的字体属性（字体名称、字体大小、颜色等）。</span><span class="sxs-lookup"><span data-stu-id="0554a-119">Represents the font attributes (font name, font size, color, etc.) for the current object.</span></span> <span data-ttu-id="0554a-120">只读。</span><span class="sxs-lookup"><span data-stu-id="0554a-120">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0554a-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0554a-121">JSON representation</span></span>

<span data-ttu-id="0554a-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0554a-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
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
<!-- {
  "type": "#page.annotation",
  "description": "ChartAreaFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
