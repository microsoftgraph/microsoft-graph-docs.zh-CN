---
title: ChartLineFormat 资源类型
description: 封装线条元素的格式选项。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: b2b7e8bd5c0b489ed42baaa3939f7a839c74c3e7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871132"
---
# <a name="chartlineformat-resource-type"></a><span data-ttu-id="a1d73-103">ChartLineFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="a1d73-103">ChartLineFormat resource type</span></span>

> <span data-ttu-id="a1d73-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a1d73-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1d73-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a1d73-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a1d73-106">封装线条元素的格式选项。</span><span class="sxs-lookup"><span data-stu-id="a1d73-106">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="a1d73-107">方法</span><span class="sxs-lookup"><span data-stu-id="a1d73-107">Methods</span></span>

| <span data-ttu-id="a1d73-108">方法</span><span class="sxs-lookup"><span data-stu-id="a1d73-108">Method</span></span>           | <span data-ttu-id="a1d73-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a1d73-109">Return Type</span></span>    |<span data-ttu-id="a1d73-110">说明</span><span class="sxs-lookup"><span data-stu-id="a1d73-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a1d73-111">获取 ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="a1d73-111">Get ChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="a1d73-112">ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="a1d73-112">ChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="a1d73-113">读取 chartLineFormat 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a1d73-113">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="a1d73-114">Update</span><span class="sxs-lookup"><span data-stu-id="a1d73-114">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="a1d73-115">ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="a1d73-115">ChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="a1d73-116">更新 ChartLineFormat 对象。</span><span class="sxs-lookup"><span data-stu-id="a1d73-116">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="a1d73-117">Clear</span><span class="sxs-lookup"><span data-stu-id="a1d73-117">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="a1d73-118">无</span><span class="sxs-lookup"><span data-stu-id="a1d73-118">None</span></span>|<span data-ttu-id="a1d73-119">清除图表元素的线条格式。</span><span class="sxs-lookup"><span data-stu-id="a1d73-119">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="a1d73-120">属性</span><span class="sxs-lookup"><span data-stu-id="a1d73-120">Properties</span></span>
| <span data-ttu-id="a1d73-121">属性</span><span class="sxs-lookup"><span data-stu-id="a1d73-121">Property</span></span>     | <span data-ttu-id="a1d73-122">类型</span><span class="sxs-lookup"><span data-stu-id="a1d73-122">Type</span></span>   |<span data-ttu-id="a1d73-123">说明</span><span class="sxs-lookup"><span data-stu-id="a1d73-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1d73-124">color</span><span class="sxs-lookup"><span data-stu-id="a1d73-124">color</span></span>|<span data-ttu-id="a1d73-125">string</span><span class="sxs-lookup"><span data-stu-id="a1d73-125">string</span></span>|<span data-ttu-id="a1d73-126">表示图表中的线条颜色的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="a1d73-126">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a1d73-127">Relationships</span><span class="sxs-lookup"><span data-stu-id="a1d73-127">Relationships</span></span>
<span data-ttu-id="a1d73-128">无</span><span class="sxs-lookup"><span data-stu-id="a1d73-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a1d73-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a1d73-129">JSON representation</span></span>

<span data-ttu-id="a1d73-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1d73-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartLineFormat"
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
