---
title: ChartLegendFormat 资源类型
description: 封装图表图例的格式属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 0ce9ac757f255bbee0334f5c6a3f397736a81884
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570944"
---
# <a name="chartlegendformat-resource-type"></a><span data-ttu-id="b38b2-103">ChartLegendFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="b38b2-103">ChartLegendFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b38b2-104">封装图表图例的格式属性。</span><span class="sxs-lookup"><span data-stu-id="b38b2-104">Encapsulates the format properties of a chart legend.</span></span>


## <a name="methods"></a><span data-ttu-id="b38b2-105">方法</span><span class="sxs-lookup"><span data-stu-id="b38b2-105">Methods</span></span>
<span data-ttu-id="b38b2-106">无</span><span class="sxs-lookup"><span data-stu-id="b38b2-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="b38b2-107">属性</span><span class="sxs-lookup"><span data-stu-id="b38b2-107">Properties</span></span>
<span data-ttu-id="b38b2-108">无</span><span class="sxs-lookup"><span data-stu-id="b38b2-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="b38b2-109">关系</span><span class="sxs-lookup"><span data-stu-id="b38b2-109">Relationships</span></span>
| <span data-ttu-id="b38b2-110">关系</span><span class="sxs-lookup"><span data-stu-id="b38b2-110">Relationship</span></span> | <span data-ttu-id="b38b2-111">类型</span><span class="sxs-lookup"><span data-stu-id="b38b2-111">Type</span></span>   |<span data-ttu-id="b38b2-112">说明</span><span class="sxs-lookup"><span data-stu-id="b38b2-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b38b2-113">fill</span><span class="sxs-lookup"><span data-stu-id="b38b2-113">fill</span></span>|[<span data-ttu-id="b38b2-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="b38b2-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="b38b2-p101">表示对象的填充格式，包括背景格式信息。只读。</span><span class="sxs-lookup"><span data-stu-id="b38b2-p101">Represents the fill format of an object, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="b38b2-117">font</span><span class="sxs-lookup"><span data-stu-id="b38b2-117">font</span></span>|[<span data-ttu-id="b38b2-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="b38b2-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="b38b2-p102">表示图表图例的字体属性，例如字体名称、字体大小、颜色等。只读。</span><span class="sxs-lookup"><span data-stu-id="b38b2-p102">Represents the font attributes such as font name, font size, color, etc. of a chart legend. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b38b2-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b38b2-121">JSON representation</span></span>

<span data-ttu-id="b38b2-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b38b2-122">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartLegendFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartlegendformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
