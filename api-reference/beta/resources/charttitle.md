---
title: ChartTitle 资源类型
description: 表示图表的 chart title 对象。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: fc470e01ca6c312429422f871edbc7868c3d209d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864874"
---
# <a name="charttitle-resource-type"></a><span data-ttu-id="8056e-103">ChartTitle 资源类型</span><span class="sxs-lookup"><span data-stu-id="8056e-103">ChartTitle resource type</span></span>

> <span data-ttu-id="8056e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8056e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8056e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8056e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8056e-106">表示图表的 chart title 对象。</span><span class="sxs-lookup"><span data-stu-id="8056e-106">Represents a chart title object of a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="8056e-107">方法</span><span class="sxs-lookup"><span data-stu-id="8056e-107">Methods</span></span>

| <span data-ttu-id="8056e-108">方法</span><span class="sxs-lookup"><span data-stu-id="8056e-108">Method</span></span>           | <span data-ttu-id="8056e-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="8056e-109">Return Type</span></span>    |<span data-ttu-id="8056e-110">说明</span><span class="sxs-lookup"><span data-stu-id="8056e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8056e-111">获取 ChartTitle</span><span class="sxs-lookup"><span data-stu-id="8056e-111">Get ChartTitle</span></span>](../api/charttitle-get.md) | [<span data-ttu-id="8056e-112">ChartTitle</span><span class="sxs-lookup"><span data-stu-id="8056e-112">ChartTitle</span></span>](charttitle.md) |<span data-ttu-id="8056e-113">读取 chartTitle 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8056e-113">Read properties and relationships of chartTitle object.</span></span>|
|[<span data-ttu-id="8056e-114">Update</span><span class="sxs-lookup"><span data-stu-id="8056e-114">Update</span></span>](../api/charttitle-update.md) | [<span data-ttu-id="8056e-115">ChartTitle</span><span class="sxs-lookup"><span data-stu-id="8056e-115">ChartTitle</span></span>](charttitle.md)    |<span data-ttu-id="8056e-116">更新 ChartTitle 对象。</span><span class="sxs-lookup"><span data-stu-id="8056e-116">Update ChartTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8056e-117">属性</span><span class="sxs-lookup"><span data-stu-id="8056e-117">Properties</span></span>
| <span data-ttu-id="8056e-118">属性</span><span class="sxs-lookup"><span data-stu-id="8056e-118">Property</span></span>     | <span data-ttu-id="8056e-119">类型</span><span class="sxs-lookup"><span data-stu-id="8056e-119">Type</span></span>   |<span data-ttu-id="8056e-120">说明</span><span class="sxs-lookup"><span data-stu-id="8056e-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8056e-121">overlay</span><span class="sxs-lookup"><span data-stu-id="8056e-121">overlay</span></span>|<span data-ttu-id="8056e-122">boolean</span><span class="sxs-lookup"><span data-stu-id="8056e-122">boolean</span></span>|<span data-ttu-id="8056e-123">表示图表标题是否将叠加在图表上的布尔值。</span><span class="sxs-lookup"><span data-stu-id="8056e-123">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="8056e-124">text</span><span class="sxs-lookup"><span data-stu-id="8056e-124">text</span></span>|<span data-ttu-id="8056e-125">string</span><span class="sxs-lookup"><span data-stu-id="8056e-125">string</span></span>|<span data-ttu-id="8056e-126">表示图表的标题文本。</span><span class="sxs-lookup"><span data-stu-id="8056e-126">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="8056e-127">visible</span><span class="sxs-lookup"><span data-stu-id="8056e-127">visible</span></span>|<span data-ttu-id="8056e-128">boolean</span><span class="sxs-lookup"><span data-stu-id="8056e-128">boolean</span></span>|<span data-ttu-id="8056e-129">表示 chart title 对象的可见性的布尔值。</span><span class="sxs-lookup"><span data-stu-id="8056e-129">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8056e-130">Relationships</span><span class="sxs-lookup"><span data-stu-id="8056e-130">Relationships</span></span>
| <span data-ttu-id="8056e-131">关系</span><span class="sxs-lookup"><span data-stu-id="8056e-131">Relationship</span></span> | <span data-ttu-id="8056e-132">类型</span><span class="sxs-lookup"><span data-stu-id="8056e-132">Type</span></span>   |<span data-ttu-id="8056e-133">说明</span><span class="sxs-lookup"><span data-stu-id="8056e-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8056e-134">format</span><span class="sxs-lookup"><span data-stu-id="8056e-134">format</span></span>|[<span data-ttu-id="8056e-135">ChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="8056e-135">ChartTitleFormat</span></span>](charttitleformat.md)|<span data-ttu-id="8056e-p102">表示图表标题的格式，包括填充和字体格式。只读。</span><span class="sxs-lookup"><span data-stu-id="8056e-p102">Represents the formatting of a chart title, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8056e-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8056e-138">JSON representation</span></span>

<span data-ttu-id="8056e-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8056e-139">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartTitle"
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
