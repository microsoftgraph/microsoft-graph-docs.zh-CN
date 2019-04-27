---
title: workbookChartPointFormat 资源类型
description: 表示图表点的格式化对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f0896001fda140ff1d2693b3463c472568f1d28e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348596"
---
# <a name="workbookchartpointformat-resource-type"></a><span data-ttu-id="ae31c-103">workbookChartPointFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="ae31c-103">workbookChartPointFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae31c-104">表示图表点的格式化对象。</span><span class="sxs-lookup"><span data-stu-id="ae31c-104">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="ae31c-105">方法</span><span class="sxs-lookup"><span data-stu-id="ae31c-105">Methods</span></span>
<span data-ttu-id="ae31c-106">无</span><span class="sxs-lookup"><span data-stu-id="ae31c-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="ae31c-107">属性</span><span class="sxs-lookup"><span data-stu-id="ae31c-107">Properties</span></span>
<span data-ttu-id="ae31c-108">无</span><span class="sxs-lookup"><span data-stu-id="ae31c-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="ae31c-109">关系</span><span class="sxs-lookup"><span data-stu-id="ae31c-109">Relationships</span></span>
| <span data-ttu-id="ae31c-110">关系</span><span class="sxs-lookup"><span data-stu-id="ae31c-110">Relationship</span></span> | <span data-ttu-id="ae31c-111">类型</span><span class="sxs-lookup"><span data-stu-id="ae31c-111">Type</span></span>   |<span data-ttu-id="ae31c-112">说明</span><span class="sxs-lookup"><span data-stu-id="ae31c-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae31c-113">fill</span><span class="sxs-lookup"><span data-stu-id="ae31c-113">fill</span></span>|[<span data-ttu-id="ae31c-114">workbookChartFill</span><span class="sxs-lookup"><span data-stu-id="ae31c-114">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="ae31c-115">表示图表的填充格式，包括背景格式信息。</span><span class="sxs-lookup"><span data-stu-id="ae31c-115">Represents the fill format of a chart, which includes background formating information.</span></span> <span data-ttu-id="ae31c-116">只读。</span><span class="sxs-lookup"><span data-stu-id="ae31c-116">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="ae31c-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ae31c-117">JSON representation</span></span>

<span data-ttu-id="ae31c-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ae31c-118">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "fill"
    ],
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
  "suppressions": []
}
-->
