---
title: ChartPointFormat 资源类型
description: 表示图表点的格式化对象。
ms.openlocfilehash: f06b31ad030dd587128f35667145f19d5cbd2e7e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009631"
---
# <a name="chartpointformat-resource-type"></a><span data-ttu-id="99269-103">ChartPointFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="99269-103">ChartPointFormat resource type</span></span>

<span data-ttu-id="99269-104">表示图表点的格式化对象。</span><span class="sxs-lookup"><span data-stu-id="99269-104">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="99269-105">方法</span><span class="sxs-lookup"><span data-stu-id="99269-105">Methods</span></span>
<span data-ttu-id="99269-106">无</span><span class="sxs-lookup"><span data-stu-id="99269-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="99269-107">属性</span><span class="sxs-lookup"><span data-stu-id="99269-107">Properties</span></span>
<span data-ttu-id="99269-108">无</span><span class="sxs-lookup"><span data-stu-id="99269-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="99269-109">Relationships</span><span class="sxs-lookup"><span data-stu-id="99269-109">Relationships</span></span>
| <span data-ttu-id="99269-110">关系</span><span class="sxs-lookup"><span data-stu-id="99269-110">Relationship</span></span> | <span data-ttu-id="99269-111">类型</span><span class="sxs-lookup"><span data-stu-id="99269-111">Type</span></span>   |<span data-ttu-id="99269-112">说明</span><span class="sxs-lookup"><span data-stu-id="99269-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99269-113">fill</span><span class="sxs-lookup"><span data-stu-id="99269-113">fill</span></span>|[<span data-ttu-id="99269-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="99269-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="99269-p101">表示图表的填充格式，包括背景格式信息。只读。</span><span class="sxs-lookup"><span data-stu-id="99269-p101">Represents the fill format of a chart, which includes background formating information. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="99269-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="99269-117">JSON representation</span></span>

<span data-ttu-id="99269-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99269-118">Here is a JSON representation of the resource.</span></span>

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