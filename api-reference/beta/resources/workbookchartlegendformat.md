---
title: workbookChartLegendFormat 资源类型
description: 封装图表图例的格式属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 987753588beeec62ded346d2f2ff8611c0436e48
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007261"
---
# <a name="workbookchartlegendformat-resource-type"></a><span data-ttu-id="93e89-103">workbookChartLegendFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="93e89-103">workbookChartLegendFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93e89-104">封装图表图例的格式属性。</span><span class="sxs-lookup"><span data-stu-id="93e89-104">Encapsulates the format properties of a chart legend.</span></span>

## <a name="methods"></a><span data-ttu-id="93e89-105">方法</span><span class="sxs-lookup"><span data-stu-id="93e89-105">Methods</span></span>
<span data-ttu-id="93e89-106">无</span><span class="sxs-lookup"><span data-stu-id="93e89-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="93e89-107">属性</span><span class="sxs-lookup"><span data-stu-id="93e89-107">Properties</span></span>
<span data-ttu-id="93e89-108">无</span><span class="sxs-lookup"><span data-stu-id="93e89-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="93e89-109">关系</span><span class="sxs-lookup"><span data-stu-id="93e89-109">Relationships</span></span>
| <span data-ttu-id="93e89-110">关系</span><span class="sxs-lookup"><span data-stu-id="93e89-110">Relationship</span></span> | <span data-ttu-id="93e89-111">类型</span><span class="sxs-lookup"><span data-stu-id="93e89-111">Type</span></span>   |<span data-ttu-id="93e89-112">说明</span><span class="sxs-lookup"><span data-stu-id="93e89-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93e89-113">fill</span><span class="sxs-lookup"><span data-stu-id="93e89-113">fill</span></span>|[<span data-ttu-id="93e89-114">workbookChartFill</span><span class="sxs-lookup"><span data-stu-id="93e89-114">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="93e89-p101">表示对象的填充格式，包括背景格式信息。只读。</span><span class="sxs-lookup"><span data-stu-id="93e89-p101">Represents the fill format of an object, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="93e89-117">font</span><span class="sxs-lookup"><span data-stu-id="93e89-117">font</span></span>|[<span data-ttu-id="93e89-118">workbookChartFont</span><span class="sxs-lookup"><span data-stu-id="93e89-118">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="93e89-119">表示图表图例的字体属性，例如字体名称、字体大小、颜色等。</span><span class="sxs-lookup"><span data-stu-id="93e89-119">Represents the font attributes such as font name, font size, color, etc. of a chart legend.</span></span> <span data-ttu-id="93e89-120">只读。</span><span class="sxs-lookup"><span data-stu-id="93e89-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="93e89-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="93e89-121">JSON representation</span></span>

<span data-ttu-id="93e89-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="93e89-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "fill",
    "font"
    ],
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
<!--
{
  "type": "#page.annotation",
  "description": "workbookChartLegendFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
