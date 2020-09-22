---
title: workbookChartGridlines 资源类型
description: 代表图表坐标轴的主要或次要网格线。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ae89fb8714cfa1c9fba90961fafa3b74f679113b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979257"
---
# <a name="workbookchartgridlines-resource-type"></a><span data-ttu-id="19d47-103">workbookChartGridlines 资源类型</span><span class="sxs-lookup"><span data-stu-id="19d47-103">workbookChartGridlines resource type</span></span>

<span data-ttu-id="19d47-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19d47-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19d47-105">代表图表坐标轴的主要或次要网格线。</span><span class="sxs-lookup"><span data-stu-id="19d47-105">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="19d47-106">方法</span><span class="sxs-lookup"><span data-stu-id="19d47-106">Methods</span></span>

| <span data-ttu-id="19d47-107">方法</span><span class="sxs-lookup"><span data-stu-id="19d47-107">Method</span></span>           | <span data-ttu-id="19d47-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="19d47-108">Return Type</span></span>    |<span data-ttu-id="19d47-109">说明</span><span class="sxs-lookup"><span data-stu-id="19d47-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="19d47-110">获取 workbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="19d47-110">Get workbookChartGridlines</span></span>](../api/chartgridlines-get.md) | [<span data-ttu-id="19d47-111">workbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="19d47-111">workbookChartGridlines</span></span>](workbookchartgridlines.md) |<span data-ttu-id="19d47-112">读取 chartGridlines 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="19d47-112">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="19d47-113">更新</span><span class="sxs-lookup"><span data-stu-id="19d47-113">Update</span></span>](../api/chartgridlines-update.md) | [<span data-ttu-id="19d47-114">workbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="19d47-114">workbookChartGridlines</span></span>](workbookchartgridlines.md)    |<span data-ttu-id="19d47-115">更新 ChartGridlines 对象。</span><span class="sxs-lookup"><span data-stu-id="19d47-115">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="19d47-116">属性</span><span class="sxs-lookup"><span data-stu-id="19d47-116">Properties</span></span>
| <span data-ttu-id="19d47-117">属性</span><span class="sxs-lookup"><span data-stu-id="19d47-117">Property</span></span>     | <span data-ttu-id="19d47-118">类型</span><span class="sxs-lookup"><span data-stu-id="19d47-118">Type</span></span>   |<span data-ttu-id="19d47-119">说明</span><span class="sxs-lookup"><span data-stu-id="19d47-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19d47-120">visible</span><span class="sxs-lookup"><span data-stu-id="19d47-120">visible</span></span>|<span data-ttu-id="19d47-121">布尔</span><span class="sxs-lookup"><span data-stu-id="19d47-121">boolean</span></span>|<span data-ttu-id="19d47-122">表示坐标轴网格线是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="19d47-122">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="19d47-123">关系</span><span class="sxs-lookup"><span data-stu-id="19d47-123">Relationships</span></span>
| <span data-ttu-id="19d47-124">关系</span><span class="sxs-lookup"><span data-stu-id="19d47-124">Relationship</span></span> | <span data-ttu-id="19d47-125">类型</span><span class="sxs-lookup"><span data-stu-id="19d47-125">Type</span></span>   |<span data-ttu-id="19d47-126">说明</span><span class="sxs-lookup"><span data-stu-id="19d47-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19d47-127">format</span><span class="sxs-lookup"><span data-stu-id="19d47-127">format</span></span>|[<span data-ttu-id="19d47-128">workbookChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="19d47-128">workbookChartGridlinesFormat</span></span>](workbookchartgridlinesformat.md)|<span data-ttu-id="19d47-129">表示图表网格线的格式。</span><span class="sxs-lookup"><span data-stu-id="19d47-129">Represents the formatting of chart gridlines.</span></span> <span data-ttu-id="19d47-130">只读。</span><span class="sxs-lookup"><span data-stu-id="19d47-130">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="19d47-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="19d47-131">JSON representation</span></span>

<span data-ttu-id="19d47-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="19d47-132">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartGridlines resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


