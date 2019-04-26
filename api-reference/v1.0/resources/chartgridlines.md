---
title: ChartGridlines 资源类型
description: 代表图表坐标轴的主要或次要网格线。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7347ac1b7ff251b12764534df217cd883ba730b3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569023"
---
# <a name="chartgridlines-resource-type"></a><span data-ttu-id="7d0e1-103">ChartGridlines 资源类型</span><span class="sxs-lookup"><span data-stu-id="7d0e1-103">ChartGridlines resource type</span></span>

<span data-ttu-id="7d0e1-104">代表图表坐标轴的主要或次要网格线。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-104">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="7d0e1-105">方法</span><span class="sxs-lookup"><span data-stu-id="7d0e1-105">Methods</span></span>

| <span data-ttu-id="7d0e1-106">方法</span><span class="sxs-lookup"><span data-stu-id="7d0e1-106">Method</span></span>           | <span data-ttu-id="7d0e1-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="7d0e1-107">Return Type</span></span>    |<span data-ttu-id="7d0e1-108">说明</span><span class="sxs-lookup"><span data-stu-id="7d0e1-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7d0e1-109">获取 ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="7d0e1-109">Get ChartGridlines</span></span>](../api/chartgridlines-get.md) | [<span data-ttu-id="7d0e1-110">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="7d0e1-110">WorkbookChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="7d0e1-111">读取 chartGridlines 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-111">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="7d0e1-112">更新</span><span class="sxs-lookup"><span data-stu-id="7d0e1-112">Update</span></span>](../api/chartgridlines-update.md) | [<span data-ttu-id="7d0e1-113">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="7d0e1-113">WorkbookChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="7d0e1-114">更新 ChartGridlines 对象。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-114">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7d0e1-115">属性</span><span class="sxs-lookup"><span data-stu-id="7d0e1-115">Properties</span></span>
| <span data-ttu-id="7d0e1-116">属性</span><span class="sxs-lookup"><span data-stu-id="7d0e1-116">Property</span></span>     | <span data-ttu-id="7d0e1-117">类型</span><span class="sxs-lookup"><span data-stu-id="7d0e1-117">Type</span></span>   |<span data-ttu-id="7d0e1-118">说明</span><span class="sxs-lookup"><span data-stu-id="7d0e1-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d0e1-119">visible</span><span class="sxs-lookup"><span data-stu-id="7d0e1-119">visible</span></span>|<span data-ttu-id="7d0e1-120">布尔</span><span class="sxs-lookup"><span data-stu-id="7d0e1-120">boolean</span></span>|<span data-ttu-id="7d0e1-121">表示坐标轴网格线是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-121">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d0e1-122">关系</span><span class="sxs-lookup"><span data-stu-id="7d0e1-122">Relationships</span></span>
| <span data-ttu-id="7d0e1-123">关系</span><span class="sxs-lookup"><span data-stu-id="7d0e1-123">Relationship</span></span> | <span data-ttu-id="7d0e1-124">类型</span><span class="sxs-lookup"><span data-stu-id="7d0e1-124">Type</span></span>   |<span data-ttu-id="7d0e1-125">说明</span><span class="sxs-lookup"><span data-stu-id="7d0e1-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d0e1-126">format</span><span class="sxs-lookup"><span data-stu-id="7d0e1-126">format</span></span>|[<span data-ttu-id="7d0e1-127">WorkbookChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="7d0e1-127">WorkbookChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="7d0e1-128">表示图表网格线的格式。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-128">Represents the formatting of chart gridlines.</span></span> <span data-ttu-id="7d0e1-129">只读。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-129">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7d0e1-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7d0e1-130">JSON representation</span></span>

<span data-ttu-id="7d0e1-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-131">Here is a JSON representation of the resource.</span></span>

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
