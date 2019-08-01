---
title: ChartLegendFormat 资源类型
description: 封装图表图例的格式属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 2148b6b5baf8bb680f85954d000da097bcf8f0b9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032954"
---
# <a name="chartlegendformat-resource-type"></a><span data-ttu-id="1b184-103">ChartLegendFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="1b184-103">ChartLegendFormat resource type</span></span>

<span data-ttu-id="1b184-104">封装图表图例的格式属性。</span><span class="sxs-lookup"><span data-stu-id="1b184-104">Encapsulates the format properties of a chart legend.</span></span>


## <a name="methods"></a><span data-ttu-id="1b184-105">方法</span><span class="sxs-lookup"><span data-stu-id="1b184-105">Methods</span></span>
<span data-ttu-id="1b184-106">无</span><span class="sxs-lookup"><span data-stu-id="1b184-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="1b184-107">属性</span><span class="sxs-lookup"><span data-stu-id="1b184-107">Properties</span></span>
<span data-ttu-id="1b184-108">无</span><span class="sxs-lookup"><span data-stu-id="1b184-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="1b184-109">关系</span><span class="sxs-lookup"><span data-stu-id="1b184-109">Relationships</span></span>
| <span data-ttu-id="1b184-110">关系</span><span class="sxs-lookup"><span data-stu-id="1b184-110">Relationship</span></span> | <span data-ttu-id="1b184-111">类型</span><span class="sxs-lookup"><span data-stu-id="1b184-111">Type</span></span>   |<span data-ttu-id="1b184-112">说明</span><span class="sxs-lookup"><span data-stu-id="1b184-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b184-113">fill</span><span class="sxs-lookup"><span data-stu-id="1b184-113">fill</span></span>|[<span data-ttu-id="1b184-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="1b184-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="1b184-p101">表示对象的填充格式，包括背景格式信息。只读。</span><span class="sxs-lookup"><span data-stu-id="1b184-p101">Represents the fill format of an object, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="1b184-117">font</span><span class="sxs-lookup"><span data-stu-id="1b184-117">font</span></span>|[<span data-ttu-id="1b184-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="1b184-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="1b184-119">表示图表图例的字体属性，例如字体名称、字体大小、颜色等。</span><span class="sxs-lookup"><span data-stu-id="1b184-119">Represents the font attributes such as font name, font size, color, etc. of a chart legend.</span></span> <span data-ttu-id="1b184-120">只读。</span><span class="sxs-lookup"><span data-stu-id="1b184-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="1b184-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1b184-121">JSON representation</span></span>

<span data-ttu-id="1b184-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b184-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartLegendFormat"
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
  "description": "ChartLegendFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
