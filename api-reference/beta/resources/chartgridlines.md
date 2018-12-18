---
title: ChartGridlines 资源类型
description: 代表图表坐标轴的主要或次要网格线。
author: lumine2008
ms.openlocfilehash: 263bbefad519fef8b12080cb7b2bfd74ce1a331f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319556"
---
# <a name="chartgridlines-resource-type"></a><span data-ttu-id="7df35-103">ChartGridlines 资源类型</span><span class="sxs-lookup"><span data-stu-id="7df35-103">ChartGridlines resource type</span></span>

> <span data-ttu-id="7df35-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7df35-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7df35-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7df35-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7df35-106">代表图表坐标轴的主要或次要网格线。</span><span class="sxs-lookup"><span data-stu-id="7df35-106">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="7df35-107">方法</span><span class="sxs-lookup"><span data-stu-id="7df35-107">Methods</span></span>

| <span data-ttu-id="7df35-108">方法</span><span class="sxs-lookup"><span data-stu-id="7df35-108">Method</span></span>           | <span data-ttu-id="7df35-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="7df35-109">Return Type</span></span>    |<span data-ttu-id="7df35-110">说明</span><span class="sxs-lookup"><span data-stu-id="7df35-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7df35-111">获取 ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="7df35-111">Get ChartGridlines</span></span>](../api/chartgridlines-get.md) | [<span data-ttu-id="7df35-112">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="7df35-112">ChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="7df35-113">读取 chartGridlines 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7df35-113">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="7df35-114">Update</span><span class="sxs-lookup"><span data-stu-id="7df35-114">Update</span></span>](../api/chartgridlines-update.md) | [<span data-ttu-id="7df35-115">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="7df35-115">ChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="7df35-116">更新 ChartGridlines 对象。</span><span class="sxs-lookup"><span data-stu-id="7df35-116">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7df35-117">属性</span><span class="sxs-lookup"><span data-stu-id="7df35-117">Properties</span></span>
| <span data-ttu-id="7df35-118">属性</span><span class="sxs-lookup"><span data-stu-id="7df35-118">Property</span></span>     | <span data-ttu-id="7df35-119">类型</span><span class="sxs-lookup"><span data-stu-id="7df35-119">Type</span></span>   |<span data-ttu-id="7df35-120">说明</span><span class="sxs-lookup"><span data-stu-id="7df35-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7df35-121">visible</span><span class="sxs-lookup"><span data-stu-id="7df35-121">visible</span></span>|<span data-ttu-id="7df35-122">boolean</span><span class="sxs-lookup"><span data-stu-id="7df35-122">boolean</span></span>|<span data-ttu-id="7df35-123">表示坐标轴网格线是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="7df35-123">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7df35-124">Relationships</span><span class="sxs-lookup"><span data-stu-id="7df35-124">Relationships</span></span>
| <span data-ttu-id="7df35-125">关系</span><span class="sxs-lookup"><span data-stu-id="7df35-125">Relationship</span></span> | <span data-ttu-id="7df35-126">类型</span><span class="sxs-lookup"><span data-stu-id="7df35-126">Type</span></span>   |<span data-ttu-id="7df35-127">说明</span><span class="sxs-lookup"><span data-stu-id="7df35-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7df35-128">format</span><span class="sxs-lookup"><span data-stu-id="7df35-128">format</span></span>|[<span data-ttu-id="7df35-129">ChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="7df35-129">ChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="7df35-p102">表示图表网格线的格式。只读。</span><span class="sxs-lookup"><span data-stu-id="7df35-p102">Represents the formatting of chart gridlines. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7df35-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7df35-132">JSON representation</span></span>

<span data-ttu-id="7df35-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7df35-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartGridLines"
}-->

```json
{
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartGridlines resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->