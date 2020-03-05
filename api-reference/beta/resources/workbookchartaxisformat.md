---
title: workbookChartAxisFormat 资源类型
description: 封装图表坐标轴的格式属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 0bb5375edc2a2e504b602d6b66720ac9aee9bc55
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519370"
---
# <a name="workbookchartaxisformat-resource-type"></a><span data-ttu-id="b5759-103">workbookChartAxisFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="b5759-103">workbookChartAxisFormat resource type</span></span>

<span data-ttu-id="b5759-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b5759-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5759-105">封装图表坐标轴的格式属性。</span><span class="sxs-lookup"><span data-stu-id="b5759-105">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="b5759-106">方法</span><span class="sxs-lookup"><span data-stu-id="b5759-106">Methods</span></span>
<span data-ttu-id="b5759-107">无</span><span class="sxs-lookup"><span data-stu-id="b5759-107">None</span></span>
## <a name="properties"></a><span data-ttu-id="b5759-108">属性</span><span class="sxs-lookup"><span data-stu-id="b5759-108">Properties</span></span>
<span data-ttu-id="b5759-109">无</span><span class="sxs-lookup"><span data-stu-id="b5759-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="b5759-110">关系</span><span class="sxs-lookup"><span data-stu-id="b5759-110">Relationships</span></span>
| <span data-ttu-id="b5759-111">关系</span><span class="sxs-lookup"><span data-stu-id="b5759-111">Relationship</span></span> | <span data-ttu-id="b5759-112">类型</span><span class="sxs-lookup"><span data-stu-id="b5759-112">Type</span></span>   |<span data-ttu-id="b5759-113">说明</span><span class="sxs-lookup"><span data-stu-id="b5759-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5759-114">font</span><span class="sxs-lookup"><span data-stu-id="b5759-114">font</span></span>|[<span data-ttu-id="b5759-115">workbookChartFont</span><span class="sxs-lookup"><span data-stu-id="b5759-115">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="b5759-p101">表示图表坐标轴元素的字体属性（字体名称、字体大小、颜色等）。只读。</span><span class="sxs-lookup"><span data-stu-id="b5759-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="b5759-118">line</span><span class="sxs-lookup"><span data-stu-id="b5759-118">line</span></span>|[<span data-ttu-id="b5759-119">workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="b5759-119">workbookChartLineFormat</span></span>](workbookchartlineformat.md)|<span data-ttu-id="b5759-120">表示图表线条格式。</span><span class="sxs-lookup"><span data-stu-id="b5759-120">Represents chart line formatting.</span></span> <span data-ttu-id="b5759-121">只读。</span><span class="sxs-lookup"><span data-stu-id="b5759-121">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b5759-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b5759-122">JSON representation</span></span>

<span data-ttu-id="b5759-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5759-123">Here is a JSON representation of the resource.</span></span>

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
