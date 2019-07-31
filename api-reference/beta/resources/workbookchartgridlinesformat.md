---
title: workbookChartGridlinesFormat 资源类型
description: 封装图表网格线的格式属性。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 6d32e916b3156082b45cbcaa105fd55e1c377b2e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007275"
---
# <a name="workbookchartgridlinesformat-resource-type"></a><span data-ttu-id="c8216-103">workbookChartGridlinesFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="c8216-103">workbookChartGridlinesFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8216-104">封装图表网格线的格式属性。</span><span class="sxs-lookup"><span data-stu-id="c8216-104">Encapsulates the format properties for chart gridlines.</span></span>

## <a name="methods"></a><span data-ttu-id="c8216-105">方法</span><span class="sxs-lookup"><span data-stu-id="c8216-105">Methods</span></span>
<span data-ttu-id="c8216-106">无</span><span class="sxs-lookup"><span data-stu-id="c8216-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="c8216-107">属性</span><span class="sxs-lookup"><span data-stu-id="c8216-107">Properties</span></span>
<span data-ttu-id="c8216-108">无</span><span class="sxs-lookup"><span data-stu-id="c8216-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="c8216-109">关系</span><span class="sxs-lookup"><span data-stu-id="c8216-109">Relationships</span></span>
| <span data-ttu-id="c8216-110">关系</span><span class="sxs-lookup"><span data-stu-id="c8216-110">Relationship</span></span> | <span data-ttu-id="c8216-111">类型</span><span class="sxs-lookup"><span data-stu-id="c8216-111">Type</span></span>   |<span data-ttu-id="c8216-112">说明</span><span class="sxs-lookup"><span data-stu-id="c8216-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c8216-113">line</span><span class="sxs-lookup"><span data-stu-id="c8216-113">line</span></span>|[<span data-ttu-id="c8216-114">workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="c8216-114">workbookChartLineFormat</span></span>](workbookchartlineformat.md)|<span data-ttu-id="c8216-115">表示图表线条格式。</span><span class="sxs-lookup"><span data-stu-id="c8216-115">Represents chart line formatting.</span></span> <span data-ttu-id="c8216-116">只读。</span><span class="sxs-lookup"><span data-stu-id="c8216-116">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="c8216-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c8216-117">JSON representation</span></span>

<span data-ttu-id="c8216-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c8216-118">Here is a JSON representation of the resource.</span></span>

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
