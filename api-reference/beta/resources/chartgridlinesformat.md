---
title: ChartGridlinesFormat 资源类型
description: 封装图表网格线的格式属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: cf2e9f1202774cc971cc09a2ce1904df2e1fb5a2
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573282"
---
# <a name="chartgridlinesformat-resource-type"></a><span data-ttu-id="6a907-103">ChartGridlinesFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="6a907-103">ChartGridlinesFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a907-104">封装图表网格线的格式属性。</span><span class="sxs-lookup"><span data-stu-id="6a907-104">Encapsulates the format properties for chart gridlines.</span></span>


## <a name="methods"></a><span data-ttu-id="6a907-105">方法</span><span class="sxs-lookup"><span data-stu-id="6a907-105">Methods</span></span>
<span data-ttu-id="6a907-106">无</span><span class="sxs-lookup"><span data-stu-id="6a907-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="6a907-107">属性</span><span class="sxs-lookup"><span data-stu-id="6a907-107">Properties</span></span>
<span data-ttu-id="6a907-108">无</span><span class="sxs-lookup"><span data-stu-id="6a907-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="6a907-109">关系</span><span class="sxs-lookup"><span data-stu-id="6a907-109">Relationships</span></span>
| <span data-ttu-id="6a907-110">关系</span><span class="sxs-lookup"><span data-stu-id="6a907-110">Relationship</span></span> | <span data-ttu-id="6a907-111">类型</span><span class="sxs-lookup"><span data-stu-id="6a907-111">Type</span></span>   |<span data-ttu-id="6a907-112">说明</span><span class="sxs-lookup"><span data-stu-id="6a907-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a907-113">line</span><span class="sxs-lookup"><span data-stu-id="6a907-113">line</span></span>|[<span data-ttu-id="6a907-114">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="6a907-114">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="6a907-p101">表示图表线条格式。只读。</span><span class="sxs-lookup"><span data-stu-id="6a907-p101">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="6a907-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6a907-117">JSON representation</span></span>

<span data-ttu-id="6a907-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a907-118">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartGridlinesFormat"
}-->

```json
{
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartGridlinesFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartgridlinesformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
