---
title: workbookChartGridlinesFormat 资源类型
description: 封装图表网格线的格式属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 53c6561ef9d7695a0096b928b7be4c7a72432960
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348603"
---
# <a name="workbookchartgridlinesformat-resource-type"></a><span data-ttu-id="e5ae4-103">workbookChartGridlinesFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="e5ae4-103">workbookChartGridlinesFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5ae4-104">封装图表网格线的格式属性。</span><span class="sxs-lookup"><span data-stu-id="e5ae4-104">Encapsulates the format properties for chart gridlines.</span></span>

## <a name="methods"></a><span data-ttu-id="e5ae4-105">方法</span><span class="sxs-lookup"><span data-stu-id="e5ae4-105">Methods</span></span>
<span data-ttu-id="e5ae4-106">无</span><span class="sxs-lookup"><span data-stu-id="e5ae4-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="e5ae4-107">属性</span><span class="sxs-lookup"><span data-stu-id="e5ae4-107">Properties</span></span>
<span data-ttu-id="e5ae4-108">无</span><span class="sxs-lookup"><span data-stu-id="e5ae4-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="e5ae4-109">关系</span><span class="sxs-lookup"><span data-stu-id="e5ae4-109">Relationships</span></span>
| <span data-ttu-id="e5ae4-110">关系</span><span class="sxs-lookup"><span data-stu-id="e5ae4-110">Relationship</span></span> | <span data-ttu-id="e5ae4-111">类型</span><span class="sxs-lookup"><span data-stu-id="e5ae4-111">Type</span></span>   |<span data-ttu-id="e5ae4-112">说明</span><span class="sxs-lookup"><span data-stu-id="e5ae4-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5ae4-113">line</span><span class="sxs-lookup"><span data-stu-id="e5ae4-113">line</span></span>|[<span data-ttu-id="e5ae4-114">workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="e5ae4-114">workbookChartLineFormat</span></span>](workbookchartlineformat.md)|<span data-ttu-id="e5ae4-115">表示图表线条格式。</span><span class="sxs-lookup"><span data-stu-id="e5ae4-115">Represents chart line formatting.</span></span> <span data-ttu-id="e5ae4-116">只读。</span><span class="sxs-lookup"><span data-stu-id="e5ae4-116">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e5ae4-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e5ae4-117">JSON representation</span></span>

<span data-ttu-id="e5ae4-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5ae4-118">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "line"
    ],
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
  "suppressions": []
}
-->
