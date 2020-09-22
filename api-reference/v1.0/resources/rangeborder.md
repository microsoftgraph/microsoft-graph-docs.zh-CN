---
title: RangeBorder 资源类型
description: 代表对象的边框。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: a4536607c4723a9e16d77e045e17bd151da50d36
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090926"
---
# <a name="rangeborder-resource-type"></a><span data-ttu-id="58f23-103">RangeBorder 资源类型</span><span class="sxs-lookup"><span data-stu-id="58f23-103">RangeBorder resource type</span></span>

<span data-ttu-id="58f23-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58f23-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="58f23-105">代表对象的边框。</span><span class="sxs-lookup"><span data-stu-id="58f23-105">Represents the border of an object.</span></span>


## <a name="methods"></a><span data-ttu-id="58f23-106">方法</span><span class="sxs-lookup"><span data-stu-id="58f23-106">Methods</span></span>

| <span data-ttu-id="58f23-107">方法</span><span class="sxs-lookup"><span data-stu-id="58f23-107">Method</span></span>           | <span data-ttu-id="58f23-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="58f23-108">Return Type</span></span>    |<span data-ttu-id="58f23-109">说明</span><span class="sxs-lookup"><span data-stu-id="58f23-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="58f23-110">获取 RangeBorder</span><span class="sxs-lookup"><span data-stu-id="58f23-110">Get RangeBorder</span></span>](../api/rangeborder-get.md) | [<span data-ttu-id="58f23-111">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="58f23-111">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="58f23-112">读取 rangeborder 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="58f23-112">Read properties and relationships of rangeBorder object.</span></span>|
|[<span data-ttu-id="58f23-113">更新</span><span class="sxs-lookup"><span data-stu-id="58f23-113">Update</span></span>](../api/rangeborder-update.md) | [<span data-ttu-id="58f23-114">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="58f23-114">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="58f23-115">更新 RangeBorder 对象。</span><span class="sxs-lookup"><span data-stu-id="58f23-115">Update RangeBorder object.</span></span> |
|[<span data-ttu-id="58f23-116">列出</span><span class="sxs-lookup"><span data-stu-id="58f23-116">List</span></span>](../api/rangeborder-list.md) | <span data-ttu-id="58f23-117">[WorkbookRangeBorder](rangeborder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="58f23-117">[WorkbookRangeBorder](rangeborder.md) collection</span></span> |<span data-ttu-id="58f23-118">获取 rangeBorder 对象集合。</span><span class="sxs-lookup"><span data-stu-id="58f23-118">Get rangeBorder object collection.</span></span> |
|[<span data-ttu-id="58f23-119">Itemat</span><span class="sxs-lookup"><span data-stu-id="58f23-119">Itemat</span></span>](../api/rangebordercollection-itemat.md)|[<span data-ttu-id="58f23-120">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="58f23-120">WorkbookRangeBorder</span></span>](rangeborder.md)|<span data-ttu-id="58f23-121">使用其索引获取 border 对象</span><span class="sxs-lookup"><span data-stu-id="58f23-121">Gets a border object using its index</span></span>|

## <a name="properties"></a><span data-ttu-id="58f23-122">属性</span><span class="sxs-lookup"><span data-stu-id="58f23-122">Properties</span></span>
| <span data-ttu-id="58f23-123">属性</span><span class="sxs-lookup"><span data-stu-id="58f23-123">Property</span></span>     | <span data-ttu-id="58f23-124">类型</span><span class="sxs-lookup"><span data-stu-id="58f23-124">Type</span></span>   |<span data-ttu-id="58f23-125">说明</span><span class="sxs-lookup"><span data-stu-id="58f23-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58f23-126">color</span><span class="sxs-lookup"><span data-stu-id="58f23-126">color</span></span>|<span data-ttu-id="58f23-127">string</span><span class="sxs-lookup"><span data-stu-id="58f23-127">string</span></span>|<span data-ttu-id="58f23-128">表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="58f23-128">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="58f23-129">id</span><span class="sxs-lookup"><span data-stu-id="58f23-129">id</span></span>|<span data-ttu-id="58f23-130">string</span><span class="sxs-lookup"><span data-stu-id="58f23-130">string</span></span>|<span data-ttu-id="58f23-131">表示边框标识符。</span><span class="sxs-lookup"><span data-stu-id="58f23-131">Represents border identifier.</span></span> <span data-ttu-id="58f23-132">可能的值为：、、、、、、 `EdgeTop` `EdgeBottom` `EdgeLeft` `EdgeRight` `InsideVertical` `InsideHorizontal` `DiagonalDown` `DiagonalUp` 。</span><span class="sxs-lookup"><span data-stu-id="58f23-132">The possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span></span> <span data-ttu-id="58f23-133">只读。</span><span class="sxs-lookup"><span data-stu-id="58f23-133">Read-only.</span></span>|
|<span data-ttu-id="58f23-134">sideIndex</span><span class="sxs-lookup"><span data-stu-id="58f23-134">sideIndex</span></span>|<span data-ttu-id="58f23-135">string</span><span class="sxs-lookup"><span data-stu-id="58f23-135">string</span></span>|<span data-ttu-id="58f23-136">指示边框的特定边的常量值。</span><span class="sxs-lookup"><span data-stu-id="58f23-136">Constant value that indicates the specific side of the border.</span></span> <span data-ttu-id="58f23-137">可能的值为：、、、、、、 `EdgeTop` `EdgeBottom` `EdgeLeft` `EdgeRight` `InsideVertical` `InsideHorizontal` `DiagonalDown` `DiagonalUp` 。</span><span class="sxs-lookup"><span data-stu-id="58f23-137">The possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span></span> <span data-ttu-id="58f23-138">只读。</span><span class="sxs-lookup"><span data-stu-id="58f23-138">Read-only.</span></span>|
|<span data-ttu-id="58f23-139">style</span><span class="sxs-lookup"><span data-stu-id="58f23-139">style</span></span>|<span data-ttu-id="58f23-140">string</span><span class="sxs-lookup"><span data-stu-id="58f23-140">string</span></span>|<span data-ttu-id="58f23-141">线条样式的常量之一，指定边框的线条样式。</span><span class="sxs-lookup"><span data-stu-id="58f23-141">One of the constants of line style specifying the line style for the border.</span></span> <span data-ttu-id="58f23-142">可能的值为：、、、、、、 `None` `Continuous` `Dash` `DashDot` `DashDotDot` `Dot` `Double` `SlantDashDot` 。</span><span class="sxs-lookup"><span data-stu-id="58f23-142">The possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="58f23-143">weight</span><span class="sxs-lookup"><span data-stu-id="58f23-143">weight</span></span>|<span data-ttu-id="58f23-144">string</span><span class="sxs-lookup"><span data-stu-id="58f23-144">string</span></span>|<span data-ttu-id="58f23-145">指定区域周围的边框的粗细。</span><span class="sxs-lookup"><span data-stu-id="58f23-145">Specifies the weight of the border around a range.</span></span> <span data-ttu-id="58f23-146">可能的值包括 `Hairline`、`Thin`、`Medium`、`Thick`。</span><span class="sxs-lookup"><span data-stu-id="58f23-146">The possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="58f23-147">关系</span><span class="sxs-lookup"><span data-stu-id="58f23-147">Relationships</span></span>
<span data-ttu-id="58f23-148">无</span><span class="sxs-lookup"><span data-stu-id="58f23-148">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="58f23-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="58f23-149">JSON representation</span></span>

<span data-ttu-id="58f23-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="58f23-150">Here is a JSON representation of the resource.</span></span>

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

