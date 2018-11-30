---
title: ChartGridlinesFormat 资源类型
description: 封装图表网格线的格式属性。
ms.openlocfilehash: 8286cd1a03188e9f6267b0e4731689c18b868083
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010625"
---
# <a name="chartgridlinesformat-resource-type"></a><span data-ttu-id="6905c-103">ChartGridlinesFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="6905c-103">ChartGridlinesFormat resource type</span></span>

<span data-ttu-id="6905c-104">封装图表网格线的格式属性。</span><span class="sxs-lookup"><span data-stu-id="6905c-104">Encapsulates the format properties for chart gridlines.</span></span>


## <a name="methods"></a><span data-ttu-id="6905c-105">方法</span><span class="sxs-lookup"><span data-stu-id="6905c-105">Methods</span></span>
<span data-ttu-id="6905c-106">无</span><span class="sxs-lookup"><span data-stu-id="6905c-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="6905c-107">属性</span><span class="sxs-lookup"><span data-stu-id="6905c-107">Properties</span></span>
<span data-ttu-id="6905c-108">无</span><span class="sxs-lookup"><span data-stu-id="6905c-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="6905c-109">Relationships</span><span class="sxs-lookup"><span data-stu-id="6905c-109">Relationships</span></span>
| <span data-ttu-id="6905c-110">关系</span><span class="sxs-lookup"><span data-stu-id="6905c-110">Relationship</span></span> | <span data-ttu-id="6905c-111">类型</span><span class="sxs-lookup"><span data-stu-id="6905c-111">Type</span></span>   |<span data-ttu-id="6905c-112">说明</span><span class="sxs-lookup"><span data-stu-id="6905c-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6905c-113">line</span><span class="sxs-lookup"><span data-stu-id="6905c-113">line</span></span>|[<span data-ttu-id="6905c-114">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="6905c-114">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="6905c-p101">表示图表线条格式。只读。</span><span class="sxs-lookup"><span data-stu-id="6905c-p101">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="6905c-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6905c-117">JSON representation</span></span>

<span data-ttu-id="6905c-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6905c-118">Here is a JSON representation of the resource.</span></span>

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