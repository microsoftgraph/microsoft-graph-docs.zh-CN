---
title: ChartTitleFormat 资源类型
description: 封装图表标题的格式属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7dd9400873234fd73ebe506a49caf6583d05b75b
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574010"
---
# <a name="charttitleformat-resource-type"></a><span data-ttu-id="ad0ec-103">ChartTitleFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="ad0ec-103">ChartTitleFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="methods"></a><span data-ttu-id="ad0ec-104">方法</span><span class="sxs-lookup"><span data-stu-id="ad0ec-104">Methods</span></span>
<span data-ttu-id="ad0ec-105">无</span><span class="sxs-lookup"><span data-stu-id="ad0ec-105">None</span></span>

## <a name="properties"></a><span data-ttu-id="ad0ec-106">属性</span><span class="sxs-lookup"><span data-stu-id="ad0ec-106">Properties</span></span>
<span data-ttu-id="ad0ec-107">无</span><span class="sxs-lookup"><span data-stu-id="ad0ec-107">None</span></span>

## <a name="relationships"></a><span data-ttu-id="ad0ec-108">关系</span><span class="sxs-lookup"><span data-stu-id="ad0ec-108">Relationships</span></span>
| <span data-ttu-id="ad0ec-109">关系</span><span class="sxs-lookup"><span data-stu-id="ad0ec-109">Relationship</span></span> | <span data-ttu-id="ad0ec-110">类型</span><span class="sxs-lookup"><span data-stu-id="ad0ec-110">Type</span></span>   |<span data-ttu-id="ad0ec-111">说明</span><span class="sxs-lookup"><span data-stu-id="ad0ec-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad0ec-112">fill</span><span class="sxs-lookup"><span data-stu-id="ad0ec-112">fill</span></span>|[<span data-ttu-id="ad0ec-113">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="ad0ec-113">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="ad0ec-p101">表示对象的填充格式，包括背景格式信息。只读。</span><span class="sxs-lookup"><span data-stu-id="ad0ec-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="ad0ec-116">font</span><span class="sxs-lookup"><span data-stu-id="ad0ec-116">font</span></span>|[<span data-ttu-id="ad0ec-117">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="ad0ec-117">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="ad0ec-p102">表示当前对象的字体属性（字体名称、字体大小、颜色等）。只读。</span><span class="sxs-lookup"><span data-stu-id="ad0ec-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="ad0ec-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ad0ec-120">JSON representation</span></span>

<span data-ttu-id="ad0ec-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ad0ec-121">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartAreaFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/charttitleformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
