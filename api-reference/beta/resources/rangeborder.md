---
title: RangeBorder 资源类型
description: 表示对象的边框。
author: lumine2008
ms.openlocfilehash: 2aa8807949724766930c5938d1ee6e06db98212a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301216"
---
# <a name="rangeborder-resource-type"></a><span data-ttu-id="770d5-103">RangeBorder 资源类型</span><span class="sxs-lookup"><span data-stu-id="770d5-103">RangeBorder resource type</span></span>

> <span data-ttu-id="770d5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="770d5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="770d5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="770d5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="770d5-106">表示对象的边框。</span><span class="sxs-lookup"><span data-stu-id="770d5-106">Represents the border of an object.</span></span>


## <a name="methods"></a><span data-ttu-id="770d5-107">方法</span><span class="sxs-lookup"><span data-stu-id="770d5-107">Methods</span></span>

| <span data-ttu-id="770d5-108">方法</span><span class="sxs-lookup"><span data-stu-id="770d5-108">Method</span></span>           | <span data-ttu-id="770d5-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="770d5-109">Return Type</span></span>    |<span data-ttu-id="770d5-110">说明</span><span class="sxs-lookup"><span data-stu-id="770d5-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="770d5-111">获取 RangeBorder</span><span class="sxs-lookup"><span data-stu-id="770d5-111">Get RangeBorder</span></span>](../api/rangeborder-get.md) | [<span data-ttu-id="770d5-112">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="770d5-112">RangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="770d5-113">读取 rangeborder 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="770d5-113">Read properties and relationships of rangeBorder object.</span></span>|
|[<span data-ttu-id="770d5-114">Update</span><span class="sxs-lookup"><span data-stu-id="770d5-114">Update</span></span>](../api/rangeborder-update.md) | [<span data-ttu-id="770d5-115">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="770d5-115">RangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="770d5-116">更新 RangeBorder 对象。</span><span class="sxs-lookup"><span data-stu-id="770d5-116">Update RangeBorder object.</span></span> |
|[<span data-ttu-id="770d5-117">List</span><span class="sxs-lookup"><span data-stu-id="770d5-117">List</span></span>](../api/rangeborder-list.md) | <span data-ttu-id="770d5-118">[RangeBorder](rangeborder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="770d5-118">[RangeBorder](rangeborder.md) collection</span></span> |<span data-ttu-id="770d5-119">获取 rangeBorder 对象集合。</span><span class="sxs-lookup"><span data-stu-id="770d5-119">Get rangeBorder object collection.</span></span> |
|[<span data-ttu-id="770d5-120">Itemat</span><span class="sxs-lookup"><span data-stu-id="770d5-120">Itemat</span></span>](../api/rangebordercollection-itemat.md)|[<span data-ttu-id="770d5-121">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="770d5-121">RangeBorder</span></span>](rangeborder.md)|<span data-ttu-id="770d5-122">使用其索引获取 border 对象</span><span class="sxs-lookup"><span data-stu-id="770d5-122">Gets a border object using its index</span></span>|

## <a name="properties"></a><span data-ttu-id="770d5-123">属性</span><span class="sxs-lookup"><span data-stu-id="770d5-123">Properties</span></span>
| <span data-ttu-id="770d5-124">属性</span><span class="sxs-lookup"><span data-stu-id="770d5-124">Property</span></span>     | <span data-ttu-id="770d5-125">类型</span><span class="sxs-lookup"><span data-stu-id="770d5-125">Type</span></span>   |<span data-ttu-id="770d5-126">说明</span><span class="sxs-lookup"><span data-stu-id="770d5-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="770d5-127">color</span><span class="sxs-lookup"><span data-stu-id="770d5-127">color</span></span>|<span data-ttu-id="770d5-128">string</span><span class="sxs-lookup"><span data-stu-id="770d5-128">string</span></span>|<span data-ttu-id="770d5-129">表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="770d5-129">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="770d5-130">id</span><span class="sxs-lookup"><span data-stu-id="770d5-130">id</span></span>|<span data-ttu-id="770d5-131">string</span><span class="sxs-lookup"><span data-stu-id="770d5-131">string</span></span>|<span data-ttu-id="770d5-p102">表示边框标识符。可能的值是：`EdgeTop`、`EdgeBottom`、`EdgeLeft`、`EdgeRight`、`InsideVertical`、`InsideHorizontal`、`DiagonalDown`、`DiagonalUp`。只读。</span><span class="sxs-lookup"><span data-stu-id="770d5-p102">Represents border identifier. Possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Read-only.</span></span>|
|<span data-ttu-id="770d5-135">sideIndex</span><span class="sxs-lookup"><span data-stu-id="770d5-135">sideIndex</span></span>|<span data-ttu-id="770d5-136">string</span><span class="sxs-lookup"><span data-stu-id="770d5-136">string</span></span>|<span data-ttu-id="770d5-p103">指示边框的特定边的常量值。可能的值是：`EdgeTop`、`EdgeBottom`、`EdgeLeft`、`EdgeRight`、`InsideVertical`、`InsideHorizontal`、`DiagonalDown`、`DiagonalUp`。只读。</span><span class="sxs-lookup"><span data-stu-id="770d5-p103">Constant value that indicates the specific side of the border. Possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Read-only.</span></span>|
|<span data-ttu-id="770d5-140">style</span><span class="sxs-lookup"><span data-stu-id="770d5-140">style</span></span>|<span data-ttu-id="770d5-141">string</span><span class="sxs-lookup"><span data-stu-id="770d5-141">string</span></span>|<span data-ttu-id="770d5-p104">线条样式的常量之一，指定边框的线条样式。可能的值是：`None`、`Continuous`、`Dash`、`DashDot`、`DashDotDot`、`Dot`、`Double`、`SlantDashDot`。</span><span class="sxs-lookup"><span data-stu-id="770d5-p104">One of the constants of line style specifying the line style for the border. Possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="770d5-144">weight</span><span class="sxs-lookup"><span data-stu-id="770d5-144">weight</span></span>|<span data-ttu-id="770d5-145">string</span><span class="sxs-lookup"><span data-stu-id="770d5-145">string</span></span>|<span data-ttu-id="770d5-p105">指定区域周围边框的权重。可能的值是：`Hairline`、`Thin`、`Medium`、`Thick`。</span><span class="sxs-lookup"><span data-stu-id="770d5-p105">Specifies the weight of the border around a range. Possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="770d5-148">Relationships</span><span class="sxs-lookup"><span data-stu-id="770d5-148">Relationships</span></span>
<span data-ttu-id="770d5-149">无</span><span class="sxs-lookup"><span data-stu-id="770d5-149">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="770d5-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="770d5-150">JSON representation</span></span>

<span data-ttu-id="770d5-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="770d5-151">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeBorder"
}-->

```json
{
  "color": "string",
  "id": "string",
  "sideIndex": "string",
  "style": "string",
  "weight": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->