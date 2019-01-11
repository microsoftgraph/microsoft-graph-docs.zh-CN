---
title: ChartTitle 资源类型
description: 表示图表的 chart title 对象。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 6cf6a2e6355fc4bc8955899dde48f9cc843e920c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879413"
---
# <a name="charttitle-resource-type"></a><span data-ttu-id="e36fd-103">ChartTitle 资源类型</span><span class="sxs-lookup"><span data-stu-id="e36fd-103">ChartTitle resource type</span></span>

<span data-ttu-id="e36fd-104">表示图表的 chart title 对象。</span><span class="sxs-lookup"><span data-stu-id="e36fd-104">Represents a chart title object of a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="e36fd-105">方法</span><span class="sxs-lookup"><span data-stu-id="e36fd-105">Methods</span></span>

| <span data-ttu-id="e36fd-106">方法</span><span class="sxs-lookup"><span data-stu-id="e36fd-106">Method</span></span>           | <span data-ttu-id="e36fd-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="e36fd-107">Return Type</span></span>    |<span data-ttu-id="e36fd-108">说明</span><span class="sxs-lookup"><span data-stu-id="e36fd-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e36fd-109">获取 ChartTitle</span><span class="sxs-lookup"><span data-stu-id="e36fd-109">Get ChartTitle</span></span>](../api/charttitle-get.md) | [<span data-ttu-id="e36fd-110">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="e36fd-110">WorkbookChartTitle</span></span>](charttitle.md) |<span data-ttu-id="e36fd-111">读取 chartTitle 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e36fd-111">Read properties and relationships of chartTitle object.</span></span>|
|[<span data-ttu-id="e36fd-112">Update</span><span class="sxs-lookup"><span data-stu-id="e36fd-112">Update</span></span>](../api/charttitle-update.md) | [<span data-ttu-id="e36fd-113">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="e36fd-113">WorkbookChartTitle</span></span>](charttitle.md)    |<span data-ttu-id="e36fd-114">更新 ChartTitle 对象。</span><span class="sxs-lookup"><span data-stu-id="e36fd-114">Update ChartTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e36fd-115">属性</span><span class="sxs-lookup"><span data-stu-id="e36fd-115">Properties</span></span>
| <span data-ttu-id="e36fd-116">属性</span><span class="sxs-lookup"><span data-stu-id="e36fd-116">Property</span></span>     | <span data-ttu-id="e36fd-117">类型</span><span class="sxs-lookup"><span data-stu-id="e36fd-117">Type</span></span>   |<span data-ttu-id="e36fd-118">说明</span><span class="sxs-lookup"><span data-stu-id="e36fd-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e36fd-119">overlay</span><span class="sxs-lookup"><span data-stu-id="e36fd-119">overlay</span></span>|<span data-ttu-id="e36fd-120">boolean</span><span class="sxs-lookup"><span data-stu-id="e36fd-120">boolean</span></span>|<span data-ttu-id="e36fd-121">表示图表标题是否将叠加在图表上的布尔值。</span><span class="sxs-lookup"><span data-stu-id="e36fd-121">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="e36fd-122">text</span><span class="sxs-lookup"><span data-stu-id="e36fd-122">text</span></span>|<span data-ttu-id="e36fd-123">string</span><span class="sxs-lookup"><span data-stu-id="e36fd-123">string</span></span>|<span data-ttu-id="e36fd-124">表示图表的标题文本。</span><span class="sxs-lookup"><span data-stu-id="e36fd-124">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="e36fd-125">visible</span><span class="sxs-lookup"><span data-stu-id="e36fd-125">visible</span></span>|<span data-ttu-id="e36fd-126">boolean</span><span class="sxs-lookup"><span data-stu-id="e36fd-126">boolean</span></span>|<span data-ttu-id="e36fd-127">表示 chart title 对象的可见性的布尔值。</span><span class="sxs-lookup"><span data-stu-id="e36fd-127">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e36fd-128">Relationships</span><span class="sxs-lookup"><span data-stu-id="e36fd-128">Relationships</span></span>
| <span data-ttu-id="e36fd-129">关系</span><span class="sxs-lookup"><span data-stu-id="e36fd-129">Relationship</span></span> | <span data-ttu-id="e36fd-130">类型</span><span class="sxs-lookup"><span data-stu-id="e36fd-130">Type</span></span>   |<span data-ttu-id="e36fd-131">说明</span><span class="sxs-lookup"><span data-stu-id="e36fd-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e36fd-132">format</span><span class="sxs-lookup"><span data-stu-id="e36fd-132">format</span></span>|[<span data-ttu-id="e36fd-133">WorkbookChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="e36fd-133">WorkbookChartTitleFormat</span></span>](charttitleformat.md)|<span data-ttu-id="e36fd-p101">表示图表标题的格式，包括填充和字体格式。只读。</span><span class="sxs-lookup"><span data-stu-id="e36fd-p101">Represents the formatting of a chart title, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e36fd-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e36fd-136">JSON representation</span></span>

<span data-ttu-id="e36fd-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e36fd-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartTitle"
}-->

```json
{
  "overlay": true,
  "text": "string",
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
