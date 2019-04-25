---
title: ChartPointFormat 资源类型
description: 表示图表点的格式化对象。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1c1b0a4a7d9076771da11061723f275079d429cb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569065"
---
# <a name="chartpointformat-resource-type"></a><span data-ttu-id="21b63-103">ChartPointFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="21b63-103">ChartPointFormat resource type</span></span>

<span data-ttu-id="21b63-104">表示图表点的格式化对象。</span><span class="sxs-lookup"><span data-stu-id="21b63-104">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="21b63-105">方法</span><span class="sxs-lookup"><span data-stu-id="21b63-105">Methods</span></span>
<span data-ttu-id="21b63-106">无</span><span class="sxs-lookup"><span data-stu-id="21b63-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="21b63-107">属性</span><span class="sxs-lookup"><span data-stu-id="21b63-107">Properties</span></span>
<span data-ttu-id="21b63-108">无</span><span class="sxs-lookup"><span data-stu-id="21b63-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="21b63-109">关系</span><span class="sxs-lookup"><span data-stu-id="21b63-109">Relationships</span></span>
| <span data-ttu-id="21b63-110">关系</span><span class="sxs-lookup"><span data-stu-id="21b63-110">Relationship</span></span> | <span data-ttu-id="21b63-111">类型</span><span class="sxs-lookup"><span data-stu-id="21b63-111">Type</span></span>   |<span data-ttu-id="21b63-112">说明</span><span class="sxs-lookup"><span data-stu-id="21b63-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21b63-113">fill</span><span class="sxs-lookup"><span data-stu-id="21b63-113">fill</span></span>|[<span data-ttu-id="21b63-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="21b63-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="21b63-115">表示图表的填充格式，包括背景格式信息。</span><span class="sxs-lookup"><span data-stu-id="21b63-115">Represents the fill format of a chart, which includes background formating information.</span></span> <span data-ttu-id="21b63-116">只读。</span><span class="sxs-lookup"><span data-stu-id="21b63-116">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="21b63-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="21b63-117">JSON representation</span></span>

<span data-ttu-id="21b63-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="21b63-118">Here is a JSON representation of the resource.</span></span>

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
