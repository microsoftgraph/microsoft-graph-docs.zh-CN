---
title: ChartAxisTitleFormat 资源类型
description: 表示图表坐标轴标题格式。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: aeb39c46b349bda9f71385d13ef8e9ab17320823
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575917"
---
# <a name="chartaxistitleformat-resource-type"></a><span data-ttu-id="97dd8-103">ChartAxisTitleFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="97dd8-103">ChartAxisTitleFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97dd8-104">表示图表坐标轴标题格式。</span><span class="sxs-lookup"><span data-stu-id="97dd8-104">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="97dd8-105">方法</span><span class="sxs-lookup"><span data-stu-id="97dd8-105">Methods</span></span>
<span data-ttu-id="97dd8-106">无</span><span class="sxs-lookup"><span data-stu-id="97dd8-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="97dd8-107">属性</span><span class="sxs-lookup"><span data-stu-id="97dd8-107">Properties</span></span>
<span data-ttu-id="97dd8-108">无</span><span class="sxs-lookup"><span data-stu-id="97dd8-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="97dd8-109">关系</span><span class="sxs-lookup"><span data-stu-id="97dd8-109">Relationships</span></span>
| <span data-ttu-id="97dd8-110">关系</span><span class="sxs-lookup"><span data-stu-id="97dd8-110">Relationship</span></span> | <span data-ttu-id="97dd8-111">类型</span><span class="sxs-lookup"><span data-stu-id="97dd8-111">Type</span></span>   |<span data-ttu-id="97dd8-112">说明</span><span class="sxs-lookup"><span data-stu-id="97dd8-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97dd8-113">font</span><span class="sxs-lookup"><span data-stu-id="97dd8-113">font</span></span>|[<span data-ttu-id="97dd8-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="97dd8-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="97dd8-p101">表示图表坐标轴标题对象的字体属性，例如字体名称、字体大小、颜色等。只读。</span><span class="sxs-lookup"><span data-stu-id="97dd8-p101">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="97dd8-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="97dd8-117">JSON representation</span></span>

<span data-ttu-id="97dd8-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97dd8-118">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisTitleFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxisTitleFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartaxistitleformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
