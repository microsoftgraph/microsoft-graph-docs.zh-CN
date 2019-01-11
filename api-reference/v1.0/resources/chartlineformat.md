---
title: ChartLineFormat 资源类型
description: 封装线条元素的格式选项。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 70e4e3d5c88fccd2a34c3fa17d5fe4bf5dcf1e5b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805738"
---
# <a name="chartlineformat-resource-type"></a><span data-ttu-id="162ef-103">ChartLineFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="162ef-103">ChartLineFormat resource type</span></span>

<span data-ttu-id="162ef-104">封装线条元素的格式选项。</span><span class="sxs-lookup"><span data-stu-id="162ef-104">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="162ef-105">方法</span><span class="sxs-lookup"><span data-stu-id="162ef-105">Methods</span></span>

| <span data-ttu-id="162ef-106">方法</span><span class="sxs-lookup"><span data-stu-id="162ef-106">Method</span></span>           | <span data-ttu-id="162ef-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="162ef-107">Return Type</span></span>    |<span data-ttu-id="162ef-108">说明</span><span class="sxs-lookup"><span data-stu-id="162ef-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="162ef-109">获取 ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="162ef-109">Get ChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="162ef-110">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="162ef-110">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="162ef-111">读取 chartLineFormat 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="162ef-111">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="162ef-112">Update</span><span class="sxs-lookup"><span data-stu-id="162ef-112">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="162ef-113">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="162ef-113">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="162ef-114">更新 ChartLineFormat 对象。</span><span class="sxs-lookup"><span data-stu-id="162ef-114">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="162ef-115">Clear</span><span class="sxs-lookup"><span data-stu-id="162ef-115">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="162ef-116">无</span><span class="sxs-lookup"><span data-stu-id="162ef-116">None</span></span>|<span data-ttu-id="162ef-117">清除图表元素的线条格式。</span><span class="sxs-lookup"><span data-stu-id="162ef-117">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="162ef-118">属性</span><span class="sxs-lookup"><span data-stu-id="162ef-118">Properties</span></span>
| <span data-ttu-id="162ef-119">属性</span><span class="sxs-lookup"><span data-stu-id="162ef-119">Property</span></span>     | <span data-ttu-id="162ef-120">类型</span><span class="sxs-lookup"><span data-stu-id="162ef-120">Type</span></span>   |<span data-ttu-id="162ef-121">说明</span><span class="sxs-lookup"><span data-stu-id="162ef-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="162ef-122">color</span><span class="sxs-lookup"><span data-stu-id="162ef-122">color</span></span>|<span data-ttu-id="162ef-123">string</span><span class="sxs-lookup"><span data-stu-id="162ef-123">string</span></span>|<span data-ttu-id="162ef-124">表示图表中的线条颜色的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="162ef-124">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="162ef-125">Relationships</span><span class="sxs-lookup"><span data-stu-id="162ef-125">Relationships</span></span>
<span data-ttu-id="162ef-126">无</span><span class="sxs-lookup"><span data-stu-id="162ef-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="162ef-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="162ef-127">JSON representation</span></span>

<span data-ttu-id="162ef-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="162ef-128">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartLineFormat"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
