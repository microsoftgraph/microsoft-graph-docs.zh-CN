---
title: ChartGridlinesFormat 资源类型
description: 封装图表网格线的格式属性。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 8fde51cc220b20c533c3af122375047dd3276a9c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826458"
---
# <a name="chartgridlinesformat-resource-type"></a><span data-ttu-id="afd8f-103">ChartGridlinesFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="afd8f-103">ChartGridlinesFormat resource type</span></span>

<span data-ttu-id="afd8f-104">封装图表网格线的格式属性。</span><span class="sxs-lookup"><span data-stu-id="afd8f-104">Encapsulates the format properties for chart gridlines.</span></span>


## <a name="methods"></a><span data-ttu-id="afd8f-105">方法</span><span class="sxs-lookup"><span data-stu-id="afd8f-105">Methods</span></span>
<span data-ttu-id="afd8f-106">无</span><span class="sxs-lookup"><span data-stu-id="afd8f-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="afd8f-107">属性</span><span class="sxs-lookup"><span data-stu-id="afd8f-107">Properties</span></span>
<span data-ttu-id="afd8f-108">无</span><span class="sxs-lookup"><span data-stu-id="afd8f-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="afd8f-109">Relationships</span><span class="sxs-lookup"><span data-stu-id="afd8f-109">Relationships</span></span>
| <span data-ttu-id="afd8f-110">关系</span><span class="sxs-lookup"><span data-stu-id="afd8f-110">Relationship</span></span> | <span data-ttu-id="afd8f-111">类型</span><span class="sxs-lookup"><span data-stu-id="afd8f-111">Type</span></span>   |<span data-ttu-id="afd8f-112">说明</span><span class="sxs-lookup"><span data-stu-id="afd8f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="afd8f-113">line</span><span class="sxs-lookup"><span data-stu-id="afd8f-113">line</span></span>|[<span data-ttu-id="afd8f-114">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="afd8f-114">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="afd8f-p101">表示图表线条格式。只读。</span><span class="sxs-lookup"><span data-stu-id="afd8f-p101">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="afd8f-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="afd8f-117">JSON representation</span></span>

<span data-ttu-id="afd8f-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="afd8f-118">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartGridlinesFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
