---
title: ChartLineFormat 资源类型
description: 封装线条元素的格式选项。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9da0c29acf49d0e183a2ded4652fe0972f21bf76
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925915"
---
# <a name="chartlineformat-resource-type"></a><span data-ttu-id="6dfb4-103">ChartLineFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="6dfb4-103">ChartLineFormat resource type</span></span>

<span data-ttu-id="6dfb4-104">封装线条元素的格式选项。</span><span class="sxs-lookup"><span data-stu-id="6dfb4-104">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="6dfb4-105">方法</span><span class="sxs-lookup"><span data-stu-id="6dfb4-105">Methods</span></span>

| <span data-ttu-id="6dfb4-106">方法</span><span class="sxs-lookup"><span data-stu-id="6dfb4-106">Method</span></span>           | <span data-ttu-id="6dfb4-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="6dfb4-107">Return Type</span></span>    |<span data-ttu-id="6dfb4-108">说明</span><span class="sxs-lookup"><span data-stu-id="6dfb4-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6dfb4-109">获取 ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="6dfb4-109">Get ChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="6dfb4-110">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="6dfb4-110">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="6dfb4-111">读取 chartLineFormat 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6dfb4-111">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="6dfb4-112">更新</span><span class="sxs-lookup"><span data-stu-id="6dfb4-112">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="6dfb4-113">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="6dfb4-113">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="6dfb4-114">更新 ChartLineFormat 对象。</span><span class="sxs-lookup"><span data-stu-id="6dfb4-114">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="6dfb4-115">Clear</span><span class="sxs-lookup"><span data-stu-id="6dfb4-115">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="6dfb4-116">无</span><span class="sxs-lookup"><span data-stu-id="6dfb4-116">None</span></span>|<span data-ttu-id="6dfb4-117">清除图表元素的线条格式。</span><span class="sxs-lookup"><span data-stu-id="6dfb4-117">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="6dfb4-118">属性</span><span class="sxs-lookup"><span data-stu-id="6dfb4-118">Properties</span></span>
| <span data-ttu-id="6dfb4-119">属性</span><span class="sxs-lookup"><span data-stu-id="6dfb4-119">Property</span></span>     | <span data-ttu-id="6dfb4-120">类型</span><span class="sxs-lookup"><span data-stu-id="6dfb4-120">Type</span></span>   |<span data-ttu-id="6dfb4-121">说明</span><span class="sxs-lookup"><span data-stu-id="6dfb4-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6dfb4-122">color</span><span class="sxs-lookup"><span data-stu-id="6dfb4-122">color</span></span>|<span data-ttu-id="6dfb4-123">string</span><span class="sxs-lookup"><span data-stu-id="6dfb4-123">string</span></span>|<span data-ttu-id="6dfb4-124">表示图表中的线条颜色的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="6dfb4-124">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6dfb4-125">Relationships</span><span class="sxs-lookup"><span data-stu-id="6dfb4-125">Relationships</span></span>
<span data-ttu-id="6dfb4-126">无</span><span class="sxs-lookup"><span data-stu-id="6dfb4-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6dfb4-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6dfb4-127">JSON representation</span></span>

<span data-ttu-id="6dfb4-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6dfb4-128">Here is a JSON representation of the resource.</span></span>

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
