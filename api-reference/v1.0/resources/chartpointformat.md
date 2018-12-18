---
title: ChartPointFormat 资源类型
description: 表示图表点的格式化对象。
author: lumine2008
ms.openlocfilehash: 94ba58eb60f80cf704de3d8a44e6e96f010429a7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311310"
---
# <a name="chartpointformat-resource-type"></a><span data-ttu-id="dd622-103">ChartPointFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="dd622-103">ChartPointFormat resource type</span></span>

<span data-ttu-id="dd622-104">表示图表点的格式化对象。</span><span class="sxs-lookup"><span data-stu-id="dd622-104">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="dd622-105">方法</span><span class="sxs-lookup"><span data-stu-id="dd622-105">Methods</span></span>
<span data-ttu-id="dd622-106">无</span><span class="sxs-lookup"><span data-stu-id="dd622-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="dd622-107">属性</span><span class="sxs-lookup"><span data-stu-id="dd622-107">Properties</span></span>
<span data-ttu-id="dd622-108">无</span><span class="sxs-lookup"><span data-stu-id="dd622-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="dd622-109">Relationships</span><span class="sxs-lookup"><span data-stu-id="dd622-109">Relationships</span></span>
| <span data-ttu-id="dd622-110">关系</span><span class="sxs-lookup"><span data-stu-id="dd622-110">Relationship</span></span> | <span data-ttu-id="dd622-111">类型</span><span class="sxs-lookup"><span data-stu-id="dd622-111">Type</span></span>   |<span data-ttu-id="dd622-112">说明</span><span class="sxs-lookup"><span data-stu-id="dd622-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd622-113">fill</span><span class="sxs-lookup"><span data-stu-id="dd622-113">fill</span></span>|[<span data-ttu-id="dd622-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="dd622-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="dd622-p101">表示图表的填充格式，包括背景格式信息。只读。</span><span class="sxs-lookup"><span data-stu-id="dd622-p101">Represents the fill format of a chart, which includes background formating information. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="dd622-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dd622-117">JSON representation</span></span>

<span data-ttu-id="dd622-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd622-118">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartPointFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->