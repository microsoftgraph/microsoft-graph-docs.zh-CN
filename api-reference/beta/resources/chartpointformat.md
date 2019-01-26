---
title: ChartPointFormat 资源类型
description: 表示图表点的格式化对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3004577a5ca9687b4bef85f59cfcc8eb528c4a66
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573303"
---
# <a name="chartpointformat-resource-type"></a><span data-ttu-id="48c0a-103">ChartPointFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="48c0a-103">ChartPointFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48c0a-104">表示图表点的格式化对象。</span><span class="sxs-lookup"><span data-stu-id="48c0a-104">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="48c0a-105">方法</span><span class="sxs-lookup"><span data-stu-id="48c0a-105">Methods</span></span>
<span data-ttu-id="48c0a-106">无</span><span class="sxs-lookup"><span data-stu-id="48c0a-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="48c0a-107">属性</span><span class="sxs-lookup"><span data-stu-id="48c0a-107">Properties</span></span>
<span data-ttu-id="48c0a-108">无</span><span class="sxs-lookup"><span data-stu-id="48c0a-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="48c0a-109">关系</span><span class="sxs-lookup"><span data-stu-id="48c0a-109">Relationships</span></span>
| <span data-ttu-id="48c0a-110">关系</span><span class="sxs-lookup"><span data-stu-id="48c0a-110">Relationship</span></span> | <span data-ttu-id="48c0a-111">类型</span><span class="sxs-lookup"><span data-stu-id="48c0a-111">Type</span></span>   |<span data-ttu-id="48c0a-112">说明</span><span class="sxs-lookup"><span data-stu-id="48c0a-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48c0a-113">fill</span><span class="sxs-lookup"><span data-stu-id="48c0a-113">fill</span></span>|[<span data-ttu-id="48c0a-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="48c0a-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="48c0a-p101">表示图表的填充格式，包括背景格式信息。只读。</span><span class="sxs-lookup"><span data-stu-id="48c0a-p101">Represents the fill format of a chart, which includes background formating information. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="48c0a-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="48c0a-117">JSON representation</span></span>

<span data-ttu-id="48c0a-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="48c0a-118">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPointFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartPointFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartpointformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
