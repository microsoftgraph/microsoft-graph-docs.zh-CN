---
title: workbookChartLineFormat 资源类型
description: 封装线条元素的格式选项。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 24afbf388def4c1132e312ce41b1c8307ce18661
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971410"
---
# <a name="workbookchartlineformat-resource-type"></a><span data-ttu-id="04d67-103">workbookChartLineFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="04d67-103">workbookChartLineFormat resource type</span></span>

<span data-ttu-id="04d67-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04d67-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04d67-105">封装线条元素的格式选项。</span><span class="sxs-lookup"><span data-stu-id="04d67-105">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="04d67-106">方法</span><span class="sxs-lookup"><span data-stu-id="04d67-106">Methods</span></span>

| <span data-ttu-id="04d67-107">方法</span><span class="sxs-lookup"><span data-stu-id="04d67-107">Method</span></span>           | <span data-ttu-id="04d67-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="04d67-108">Return Type</span></span>    |<span data-ttu-id="04d67-109">说明</span><span class="sxs-lookup"><span data-stu-id="04d67-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="04d67-110">获取 workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="04d67-110">Get workbookChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="04d67-111">workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="04d67-111">workbookChartLineFormat</span></span>](workbookchartlineformat.md) |<span data-ttu-id="04d67-112">读取 chartLineFormat 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="04d67-112">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="04d67-113">更新</span><span class="sxs-lookup"><span data-stu-id="04d67-113">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="04d67-114">workbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="04d67-114">workbookChartLineFormat</span></span>](workbookchartlineformat.md) |<span data-ttu-id="04d67-115">更新 ChartLineFormat 对象。</span><span class="sxs-lookup"><span data-stu-id="04d67-115">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="04d67-116">清除</span><span class="sxs-lookup"><span data-stu-id="04d67-116">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="04d67-117">None</span><span class="sxs-lookup"><span data-stu-id="04d67-117">None</span></span>|<span data-ttu-id="04d67-118">清除图表元素的线条格式。</span><span class="sxs-lookup"><span data-stu-id="04d67-118">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="04d67-119">属性</span><span class="sxs-lookup"><span data-stu-id="04d67-119">Properties</span></span>
| <span data-ttu-id="04d67-120">属性</span><span class="sxs-lookup"><span data-stu-id="04d67-120">Property</span></span>     | <span data-ttu-id="04d67-121">类型</span><span class="sxs-lookup"><span data-stu-id="04d67-121">Type</span></span>   |<span data-ttu-id="04d67-122">说明</span><span class="sxs-lookup"><span data-stu-id="04d67-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04d67-123">color</span><span class="sxs-lookup"><span data-stu-id="04d67-123">color</span></span>|<span data-ttu-id="04d67-124">string</span><span class="sxs-lookup"><span data-stu-id="04d67-124">string</span></span>|<span data-ttu-id="04d67-125">表示图表中的线条颜色的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="04d67-125">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="04d67-126">关系</span><span class="sxs-lookup"><span data-stu-id="04d67-126">Relationships</span></span>
<span data-ttu-id="04d67-127">无</span><span class="sxs-lookup"><span data-stu-id="04d67-127">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="04d67-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="04d67-128">JSON representation</span></span>

<span data-ttu-id="04d67-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="04d67-129">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "workbookChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


