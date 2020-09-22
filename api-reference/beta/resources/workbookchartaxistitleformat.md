---
title: workbookChartAxisTitleFormat 资源类型
description: 表示图表坐标轴标题格式。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: c585fc426474fe0a7790874331a2ae53227fc1a7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039048"
---
# <a name="workbookchartaxistitleformat-resource-type"></a><span data-ttu-id="a2a0d-103">workbookChartAxisTitleFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="a2a0d-103">workbookChartAxisTitleFormat resource type</span></span>

<span data-ttu-id="a2a0d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2a0d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2a0d-105">表示图表坐标轴标题格式。</span><span class="sxs-lookup"><span data-stu-id="a2a0d-105">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="a2a0d-106">方法</span><span class="sxs-lookup"><span data-stu-id="a2a0d-106">Methods</span></span>
<span data-ttu-id="a2a0d-107">无</span><span class="sxs-lookup"><span data-stu-id="a2a0d-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="a2a0d-108">属性</span><span class="sxs-lookup"><span data-stu-id="a2a0d-108">Properties</span></span>
<span data-ttu-id="a2a0d-109">无</span><span class="sxs-lookup"><span data-stu-id="a2a0d-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="a2a0d-110">关系</span><span class="sxs-lookup"><span data-stu-id="a2a0d-110">Relationships</span></span>
| <span data-ttu-id="a2a0d-111">关系</span><span class="sxs-lookup"><span data-stu-id="a2a0d-111">Relationship</span></span> | <span data-ttu-id="a2a0d-112">类型</span><span class="sxs-lookup"><span data-stu-id="a2a0d-112">Type</span></span>   |<span data-ttu-id="a2a0d-113">说明</span><span class="sxs-lookup"><span data-stu-id="a2a0d-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2a0d-114">font</span><span class="sxs-lookup"><span data-stu-id="a2a0d-114">font</span></span>|[<span data-ttu-id="a2a0d-115">workbookChartFont</span><span class="sxs-lookup"><span data-stu-id="a2a0d-115">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="a2a0d-116">表示图表坐标轴标题对象的字体属性，例如字体名称、字体大小、颜色等。</span><span class="sxs-lookup"><span data-stu-id="a2a0d-116">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object.</span></span> <span data-ttu-id="a2a0d-117">只读。</span><span class="sxs-lookup"><span data-stu-id="a2a0d-117">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a2a0d-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a2a0d-118">JSON representation</span></span>

<span data-ttu-id="a2a0d-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2a0d-119">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "font"
    ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisTitleFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxisTitleFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


