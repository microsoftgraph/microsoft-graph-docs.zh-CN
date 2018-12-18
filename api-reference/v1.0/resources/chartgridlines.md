---
title: ChartGridlines 资源类型
description: 代表图表坐标轴的主要或次要网格线。
author: lumine2008
ms.openlocfilehash: 2aaf044b09d061af4853e76e0f2ba118bd1b2321
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353030"
---
# <a name="chartgridlines-resource-type"></a><span data-ttu-id="402ab-103">ChartGridlines 资源类型</span><span class="sxs-lookup"><span data-stu-id="402ab-103">ChartGridlines resource type</span></span>

<span data-ttu-id="402ab-104">代表图表坐标轴的主要或次要网格线。</span><span class="sxs-lookup"><span data-stu-id="402ab-104">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="402ab-105">方法</span><span class="sxs-lookup"><span data-stu-id="402ab-105">Methods</span></span>

| <span data-ttu-id="402ab-106">方法</span><span class="sxs-lookup"><span data-stu-id="402ab-106">Method</span></span>           | <span data-ttu-id="402ab-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="402ab-107">Return Type</span></span>    |<span data-ttu-id="402ab-108">说明</span><span class="sxs-lookup"><span data-stu-id="402ab-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="402ab-109">获取 ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="402ab-109">Get ChartGridlines</span></span>](../api/chartgridlines-get.md) | [<span data-ttu-id="402ab-110">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="402ab-110">WorkbookChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="402ab-111">读取 chartGridlines 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="402ab-111">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="402ab-112">Update</span><span class="sxs-lookup"><span data-stu-id="402ab-112">Update</span></span>](../api/chartgridlines-update.md) | [<span data-ttu-id="402ab-113">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="402ab-113">WorkbookChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="402ab-114">更新 ChartGridlines 对象。</span><span class="sxs-lookup"><span data-stu-id="402ab-114">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="402ab-115">属性</span><span class="sxs-lookup"><span data-stu-id="402ab-115">Properties</span></span>
| <span data-ttu-id="402ab-116">属性</span><span class="sxs-lookup"><span data-stu-id="402ab-116">Property</span></span>     | <span data-ttu-id="402ab-117">类型</span><span class="sxs-lookup"><span data-stu-id="402ab-117">Type</span></span>   |<span data-ttu-id="402ab-118">说明</span><span class="sxs-lookup"><span data-stu-id="402ab-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="402ab-119">visible</span><span class="sxs-lookup"><span data-stu-id="402ab-119">visible</span></span>|<span data-ttu-id="402ab-120">boolean</span><span class="sxs-lookup"><span data-stu-id="402ab-120">boolean</span></span>|<span data-ttu-id="402ab-121">表示坐标轴网格线是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="402ab-121">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="402ab-122">Relationships</span><span class="sxs-lookup"><span data-stu-id="402ab-122">Relationships</span></span>
| <span data-ttu-id="402ab-123">关系</span><span class="sxs-lookup"><span data-stu-id="402ab-123">Relationship</span></span> | <span data-ttu-id="402ab-124">类型</span><span class="sxs-lookup"><span data-stu-id="402ab-124">Type</span></span>   |<span data-ttu-id="402ab-125">说明</span><span class="sxs-lookup"><span data-stu-id="402ab-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="402ab-126">format</span><span class="sxs-lookup"><span data-stu-id="402ab-126">format</span></span>|[<span data-ttu-id="402ab-127">WorkbookChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="402ab-127">WorkbookChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="402ab-p101">表示图表网格线的格式。只读。</span><span class="sxs-lookup"><span data-stu-id="402ab-p101">Represents the formatting of chart gridlines. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="402ab-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="402ab-130">JSON representation</span></span>

<span data-ttu-id="402ab-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="402ab-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartGridlines"
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