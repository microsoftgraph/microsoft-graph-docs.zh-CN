---
title: ChartGridlinesFormat 资源类型
description: 封装图表网格线的格式属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: c34a9e640589a0df537d5f13652552551ac00372
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029776"
---
# <a name="chartgridlinesformat-resource-type"></a><span data-ttu-id="5d897-103">ChartGridlinesFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="5d897-103">ChartGridlinesFormat resource type</span></span>

<span data-ttu-id="5d897-104">封装图表网格线的格式属性。</span><span class="sxs-lookup"><span data-stu-id="5d897-104">Encapsulates the format properties for chart gridlines.</span></span>


## <a name="methods"></a><span data-ttu-id="5d897-105">方法</span><span class="sxs-lookup"><span data-stu-id="5d897-105">Methods</span></span>
<span data-ttu-id="5d897-106">无</span><span class="sxs-lookup"><span data-stu-id="5d897-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="5d897-107">属性</span><span class="sxs-lookup"><span data-stu-id="5d897-107">Properties</span></span>
<span data-ttu-id="5d897-108">无</span><span class="sxs-lookup"><span data-stu-id="5d897-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="5d897-109">关系</span><span class="sxs-lookup"><span data-stu-id="5d897-109">Relationships</span></span>
| <span data-ttu-id="5d897-110">关系</span><span class="sxs-lookup"><span data-stu-id="5d897-110">Relationship</span></span> | <span data-ttu-id="5d897-111">类型</span><span class="sxs-lookup"><span data-stu-id="5d897-111">Type</span></span>   |<span data-ttu-id="5d897-112">说明</span><span class="sxs-lookup"><span data-stu-id="5d897-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5d897-113">line</span><span class="sxs-lookup"><span data-stu-id="5d897-113">line</span></span>|[<span data-ttu-id="5d897-114">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="5d897-114">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="5d897-115">表示图表线条格式。</span><span class="sxs-lookup"><span data-stu-id="5d897-115">Represents chart line formatting.</span></span> <span data-ttu-id="5d897-116">只读。</span><span class="sxs-lookup"><span data-stu-id="5d897-116">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="5d897-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5d897-117">JSON representation</span></span>

<span data-ttu-id="5d897-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5d897-118">Here is a JSON representation of the resource.</span></span>

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
