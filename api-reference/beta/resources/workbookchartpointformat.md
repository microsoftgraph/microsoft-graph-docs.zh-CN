---
title: workbookChartPointFormat 资源类型
description: 表示图表点的格式化对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 9c3d968c4d36b8220d505edb6b7503a2b1206416
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007233"
---
# <a name="workbookchartpointformat-resource-type"></a><span data-ttu-id="adec1-103">workbookChartPointFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="adec1-103">workbookChartPointFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adec1-104">表示图表点的格式化对象。</span><span class="sxs-lookup"><span data-stu-id="adec1-104">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="adec1-105">方法</span><span class="sxs-lookup"><span data-stu-id="adec1-105">Methods</span></span>
<span data-ttu-id="adec1-106">无</span><span class="sxs-lookup"><span data-stu-id="adec1-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="adec1-107">属性</span><span class="sxs-lookup"><span data-stu-id="adec1-107">Properties</span></span>
<span data-ttu-id="adec1-108">无</span><span class="sxs-lookup"><span data-stu-id="adec1-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="adec1-109">关系</span><span class="sxs-lookup"><span data-stu-id="adec1-109">Relationships</span></span>
| <span data-ttu-id="adec1-110">关系</span><span class="sxs-lookup"><span data-stu-id="adec1-110">Relationship</span></span> | <span data-ttu-id="adec1-111">类型</span><span class="sxs-lookup"><span data-stu-id="adec1-111">Type</span></span>   |<span data-ttu-id="adec1-112">说明</span><span class="sxs-lookup"><span data-stu-id="adec1-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="adec1-113">fill</span><span class="sxs-lookup"><span data-stu-id="adec1-113">fill</span></span>|[<span data-ttu-id="adec1-114">workbookChartFill</span><span class="sxs-lookup"><span data-stu-id="adec1-114">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="adec1-115">表示图表的填充格式，包括背景格式信息。</span><span class="sxs-lookup"><span data-stu-id="adec1-115">Represents the fill format of a chart, which includes background formating information.</span></span> <span data-ttu-id="adec1-116">只读。</span><span class="sxs-lookup"><span data-stu-id="adec1-116">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="adec1-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="adec1-117">JSON representation</span></span>

<span data-ttu-id="adec1-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="adec1-118">Here is a JSON representation of the resource.</span></span>

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
