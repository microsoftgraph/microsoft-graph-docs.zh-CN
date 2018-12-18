---
title: RangeBorder 资源类型
description: 表示对象的边框。
author: lumine2008
ms.openlocfilehash: c6166e1cfebc0759ad25fda5c0e8ec471af07b11
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359148"
---
# <a name="rangeborder-resource-type"></a><span data-ttu-id="0700c-103">RangeBorder 资源类型</span><span class="sxs-lookup"><span data-stu-id="0700c-103">RangeBorder resource type</span></span>

<span data-ttu-id="0700c-104">表示对象的边框。</span><span class="sxs-lookup"><span data-stu-id="0700c-104">Represents the border of an object.</span></span>


## <a name="methods"></a><span data-ttu-id="0700c-105">方法</span><span class="sxs-lookup"><span data-stu-id="0700c-105">Methods</span></span>

| <span data-ttu-id="0700c-106">方法</span><span class="sxs-lookup"><span data-stu-id="0700c-106">Method</span></span>           | <span data-ttu-id="0700c-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="0700c-107">Return Type</span></span>    |<span data-ttu-id="0700c-108">说明</span><span class="sxs-lookup"><span data-stu-id="0700c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0700c-109">获取 RangeBorder</span><span class="sxs-lookup"><span data-stu-id="0700c-109">Get RangeBorder</span></span>](../api/rangeborder-get.md) | [<span data-ttu-id="0700c-110">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="0700c-110">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="0700c-111">读取 rangeborder 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0700c-111">Read properties and relationships of rangeBorder object.</span></span>|
|[<span data-ttu-id="0700c-112">Update</span><span class="sxs-lookup"><span data-stu-id="0700c-112">Update</span></span>](../api/rangeborder-update.md) | [<span data-ttu-id="0700c-113">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="0700c-113">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="0700c-114">更新 RangeBorder 对象。</span><span class="sxs-lookup"><span data-stu-id="0700c-114">Update RangeBorder object.</span></span> |
|[<span data-ttu-id="0700c-115">List</span><span class="sxs-lookup"><span data-stu-id="0700c-115">List</span></span>](../api/rangeborder-list.md) | <span data-ttu-id="0700c-116">[WorkbookRangeBorder](rangeborder.md)集合</span><span class="sxs-lookup"><span data-stu-id="0700c-116">[WorkbookRangeBorder](rangeborder.md) collection</span></span> |<span data-ttu-id="0700c-117">获取 rangeBorder 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0700c-117">Get rangeBorder object collection.</span></span> |
|[<span data-ttu-id="0700c-118">Itemat</span><span class="sxs-lookup"><span data-stu-id="0700c-118">Itemat</span></span>](../api/rangebordercollection-itemat.md)|[<span data-ttu-id="0700c-119">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="0700c-119">WorkbookRangeBorder</span></span>](rangeborder.md)|<span data-ttu-id="0700c-120">使用其索引获取 border 对象</span><span class="sxs-lookup"><span data-stu-id="0700c-120">Gets a border object using its index</span></span>|

## <a name="properties"></a><span data-ttu-id="0700c-121">属性</span><span class="sxs-lookup"><span data-stu-id="0700c-121">Properties</span></span>
| <span data-ttu-id="0700c-122">属性</span><span class="sxs-lookup"><span data-stu-id="0700c-122">Property</span></span>     | <span data-ttu-id="0700c-123">类型</span><span class="sxs-lookup"><span data-stu-id="0700c-123">Type</span></span>   |<span data-ttu-id="0700c-124">说明</span><span class="sxs-lookup"><span data-stu-id="0700c-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0700c-125">color</span><span class="sxs-lookup"><span data-stu-id="0700c-125">color</span></span>|<span data-ttu-id="0700c-126">string</span><span class="sxs-lookup"><span data-stu-id="0700c-126">string</span></span>|<span data-ttu-id="0700c-127">表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="0700c-127">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="0700c-128">id</span><span class="sxs-lookup"><span data-stu-id="0700c-128">id</span></span>|<span data-ttu-id="0700c-129">string</span><span class="sxs-lookup"><span data-stu-id="0700c-129">string</span></span>|<span data-ttu-id="0700c-130">代表边框标识符。</span><span class="sxs-lookup"><span data-stu-id="0700c-130">Represents border identifier.</span></span> <span data-ttu-id="0700c-131">可能的值为： `EdgeTop`， `EdgeBottom`， `EdgeLeft`， `EdgeRight`， `InsideVertical`， `InsideHorizontal`， `DiagonalDown`， `DiagonalUp`。</span><span class="sxs-lookup"><span data-stu-id="0700c-131">The possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span></span> <span data-ttu-id="0700c-132">只读。</span><span class="sxs-lookup"><span data-stu-id="0700c-132">Read-only.</span></span>|
|<span data-ttu-id="0700c-133">sideIndex</span><span class="sxs-lookup"><span data-stu-id="0700c-133">sideIndex</span></span>|<span data-ttu-id="0700c-134">string</span><span class="sxs-lookup"><span data-stu-id="0700c-134">string</span></span>|<span data-ttu-id="0700c-135">常量值，该值指示的特定的一侧边框。</span><span class="sxs-lookup"><span data-stu-id="0700c-135">Constant value that indicates the specific side of the border.</span></span> <span data-ttu-id="0700c-136">可能的值为： `EdgeTop`， `EdgeBottom`， `EdgeLeft`， `EdgeRight`， `InsideVertical`， `InsideHorizontal`， `DiagonalDown`， `DiagonalUp`。</span><span class="sxs-lookup"><span data-stu-id="0700c-136">The possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span></span> <span data-ttu-id="0700c-137">只读。</span><span class="sxs-lookup"><span data-stu-id="0700c-137">Read-only.</span></span>|
|<span data-ttu-id="0700c-138">style</span><span class="sxs-lookup"><span data-stu-id="0700c-138">style</span></span>|<span data-ttu-id="0700c-139">string</span><span class="sxs-lookup"><span data-stu-id="0700c-139">string</span></span>|<span data-ttu-id="0700c-140">指定边框线型的线条样式的常量之一。</span><span class="sxs-lookup"><span data-stu-id="0700c-140">One of the constants of line style specifying the line style for the border.</span></span> <span data-ttu-id="0700c-141">可能的值为： `None`， `Continuous`， `Dash`， `DashDot`， `DashDotDot`， `Dot`， `Double`， `SlantDashDot`。</span><span class="sxs-lookup"><span data-stu-id="0700c-141">The possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="0700c-142">weight</span><span class="sxs-lookup"><span data-stu-id="0700c-142">weight</span></span>|<span data-ttu-id="0700c-143">string</span><span class="sxs-lookup"><span data-stu-id="0700c-143">string</span></span>|<span data-ttu-id="0700c-144">指定某一区域周围的边框的粗细。</span><span class="sxs-lookup"><span data-stu-id="0700c-144">Specifies the weight of the border around a range.</span></span> <span data-ttu-id="0700c-145">可能的值为： `Hairline`， `Thin`， `Medium`， `Thick`。</span><span class="sxs-lookup"><span data-stu-id="0700c-145">The possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0700c-146">Relationships</span><span class="sxs-lookup"><span data-stu-id="0700c-146">Relationships</span></span>
<span data-ttu-id="0700c-147">无</span><span class="sxs-lookup"><span data-stu-id="0700c-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0700c-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0700c-148">JSON representation</span></span>

<span data-ttu-id="0700c-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0700c-149">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeBorder"
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