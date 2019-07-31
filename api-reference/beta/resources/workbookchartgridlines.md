---
title: workbookChartGridlines 资源类型
description: 代表图表坐标轴的主要或次要网格线。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: bf2b481b3b60b7cf5893a1c7ab6e2f168c7cc1ca
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964013"
---
# <a name="workbookchartgridlines-resource-type"></a><span data-ttu-id="99bc0-103">workbookChartGridlines 资源类型</span><span class="sxs-lookup"><span data-stu-id="99bc0-103">workbookChartGridlines resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99bc0-104">代表图表坐标轴的主要或次要网格线。</span><span class="sxs-lookup"><span data-stu-id="99bc0-104">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="99bc0-105">方法</span><span class="sxs-lookup"><span data-stu-id="99bc0-105">Methods</span></span>

| <span data-ttu-id="99bc0-106">方法</span><span class="sxs-lookup"><span data-stu-id="99bc0-106">Method</span></span>           | <span data-ttu-id="99bc0-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="99bc0-107">Return Type</span></span>    |<span data-ttu-id="99bc0-108">说明</span><span class="sxs-lookup"><span data-stu-id="99bc0-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="99bc0-109">获取 workbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="99bc0-109">Get workbookChartGridlines</span></span>](../api/chartgridlines-get.md) | [<span data-ttu-id="99bc0-110">workbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="99bc0-110">workbookChartGridlines</span></span>](workbookchartgridlines.md) |<span data-ttu-id="99bc0-111">读取 chartGridlines 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="99bc0-111">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="99bc0-112">更新</span><span class="sxs-lookup"><span data-stu-id="99bc0-112">Update</span></span>](../api/chartgridlines-update.md) | [<span data-ttu-id="99bc0-113">workbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="99bc0-113">workbookChartGridlines</span></span>](workbookchartgridlines.md)    |<span data-ttu-id="99bc0-114">更新 ChartGridlines 对象。</span><span class="sxs-lookup"><span data-stu-id="99bc0-114">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="99bc0-115">属性</span><span class="sxs-lookup"><span data-stu-id="99bc0-115">Properties</span></span>
| <span data-ttu-id="99bc0-116">属性</span><span class="sxs-lookup"><span data-stu-id="99bc0-116">Property</span></span>     | <span data-ttu-id="99bc0-117">类型</span><span class="sxs-lookup"><span data-stu-id="99bc0-117">Type</span></span>   |<span data-ttu-id="99bc0-118">说明</span><span class="sxs-lookup"><span data-stu-id="99bc0-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99bc0-119">visible</span><span class="sxs-lookup"><span data-stu-id="99bc0-119">visible</span></span>|<span data-ttu-id="99bc0-120">布尔</span><span class="sxs-lookup"><span data-stu-id="99bc0-120">boolean</span></span>|<span data-ttu-id="99bc0-121">表示坐标轴网格线是否可见的布尔值。</span><span class="sxs-lookup"><span data-stu-id="99bc0-121">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99bc0-122">关系</span><span class="sxs-lookup"><span data-stu-id="99bc0-122">Relationships</span></span>
| <span data-ttu-id="99bc0-123">关系</span><span class="sxs-lookup"><span data-stu-id="99bc0-123">Relationship</span></span> | <span data-ttu-id="99bc0-124">类型</span><span class="sxs-lookup"><span data-stu-id="99bc0-124">Type</span></span>   |<span data-ttu-id="99bc0-125">说明</span><span class="sxs-lookup"><span data-stu-id="99bc0-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99bc0-126">format</span><span class="sxs-lookup"><span data-stu-id="99bc0-126">format</span></span>|[<span data-ttu-id="99bc0-127">workbookChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="99bc0-127">workbookChartGridlinesFormat</span></span>](workbookchartgridlinesformat.md)|<span data-ttu-id="99bc0-128">表示图表网格线的格式。</span><span class="sxs-lookup"><span data-stu-id="99bc0-128">Represents the formatting of chart gridlines.</span></span> <span data-ttu-id="99bc0-129">只读。</span><span class="sxs-lookup"><span data-stu-id="99bc0-129">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="99bc0-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="99bc0-130">JSON representation</span></span>

<span data-ttu-id="99bc0-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99bc0-131">Here is a JSON representation of the resource.</span></span>

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
