---
title: RangeBorder 资源类型
description: 代表对象的边框。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9c32264311400951152f892e6f88d70645f47064
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579485"
---
# <a name="rangeborder-resource-type"></a><span data-ttu-id="884d0-103">RangeBorder 资源类型</span><span class="sxs-lookup"><span data-stu-id="884d0-103">RangeBorder resource type</span></span>

<span data-ttu-id="884d0-104">代表对象的边框。</span><span class="sxs-lookup"><span data-stu-id="884d0-104">Represents the border of an object.</span></span>


## <a name="methods"></a><span data-ttu-id="884d0-105">方法</span><span class="sxs-lookup"><span data-stu-id="884d0-105">Methods</span></span>

| <span data-ttu-id="884d0-106">方法</span><span class="sxs-lookup"><span data-stu-id="884d0-106">Method</span></span>           | <span data-ttu-id="884d0-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="884d0-107">Return Type</span></span>    |<span data-ttu-id="884d0-108">说明</span><span class="sxs-lookup"><span data-stu-id="884d0-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="884d0-109">获取 RangeBorder</span><span class="sxs-lookup"><span data-stu-id="884d0-109">Get RangeBorder</span></span>](../api/rangeborder-get.md) | [<span data-ttu-id="884d0-110">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="884d0-110">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="884d0-111">读取 rangeborder 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="884d0-111">Read properties and relationships of rangeBorder object.</span></span>|
|[<span data-ttu-id="884d0-112">更新</span><span class="sxs-lookup"><span data-stu-id="884d0-112">Update</span></span>](../api/rangeborder-update.md) | [<span data-ttu-id="884d0-113">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="884d0-113">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="884d0-114">更新 RangeBorder 对象。</span><span class="sxs-lookup"><span data-stu-id="884d0-114">Update RangeBorder object.</span></span> |
|[<span data-ttu-id="884d0-115">列出</span><span class="sxs-lookup"><span data-stu-id="884d0-115">List</span></span>](../api/rangeborder-list.md) | <span data-ttu-id="884d0-116">[WorkbookRangeBorder](rangeborder.md)集合</span><span class="sxs-lookup"><span data-stu-id="884d0-116">[WorkbookRangeBorder](rangeborder.md) collection</span></span> |<span data-ttu-id="884d0-117">获取 rangeBorder 对象集合。</span><span class="sxs-lookup"><span data-stu-id="884d0-117">Get rangeBorder object collection.</span></span> |
|[<span data-ttu-id="884d0-118">Itemat</span><span class="sxs-lookup"><span data-stu-id="884d0-118">Itemat</span></span>](../api/rangebordercollection-itemat.md)|[<span data-ttu-id="884d0-119">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="884d0-119">WorkbookRangeBorder</span></span>](rangeborder.md)|<span data-ttu-id="884d0-120">使用其索引获取 border 对象</span><span class="sxs-lookup"><span data-stu-id="884d0-120">Gets a border object using its index</span></span>|

## <a name="properties"></a><span data-ttu-id="884d0-121">属性</span><span class="sxs-lookup"><span data-stu-id="884d0-121">Properties</span></span>
| <span data-ttu-id="884d0-122">属性</span><span class="sxs-lookup"><span data-stu-id="884d0-122">Property</span></span>     | <span data-ttu-id="884d0-123">类型</span><span class="sxs-lookup"><span data-stu-id="884d0-123">Type</span></span>   |<span data-ttu-id="884d0-124">说明</span><span class="sxs-lookup"><span data-stu-id="884d0-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="884d0-125">color</span><span class="sxs-lookup"><span data-stu-id="884d0-125">color</span></span>|<span data-ttu-id="884d0-126">字符串</span><span class="sxs-lookup"><span data-stu-id="884d0-126">string</span></span>|<span data-ttu-id="884d0-127">表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="884d0-127">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="884d0-128">id</span><span class="sxs-lookup"><span data-stu-id="884d0-128">id</span></span>|<span data-ttu-id="884d0-129">string</span><span class="sxs-lookup"><span data-stu-id="884d0-129">string</span></span>|<span data-ttu-id="884d0-130">表示边框标识符。</span><span class="sxs-lookup"><span data-stu-id="884d0-130">Represents border identifier.</span></span> <span data-ttu-id="884d0-131">可能的值为: `EdgeTop`、 `EdgeBottom`、 `EdgeLeft` `EdgeRight` `InsideVertical` `InsideHorizontal` `DiagonalDown`、、、、 `DiagonalUp`。</span><span class="sxs-lookup"><span data-stu-id="884d0-131">The possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span></span> <span data-ttu-id="884d0-132">只读。</span><span class="sxs-lookup"><span data-stu-id="884d0-132">Read-only.</span></span>|
|<span data-ttu-id="884d0-133">sideIndex</span><span class="sxs-lookup"><span data-stu-id="884d0-133">sideIndex</span></span>|<span data-ttu-id="884d0-134">string</span><span class="sxs-lookup"><span data-stu-id="884d0-134">string</span></span>|<span data-ttu-id="884d0-135">指示边框的特定边的常量值。</span><span class="sxs-lookup"><span data-stu-id="884d0-135">Constant value that indicates the specific side of the border.</span></span> <span data-ttu-id="884d0-136">可能的值为: `EdgeTop`、 `EdgeBottom`、 `EdgeLeft` `EdgeRight` `InsideVertical` `InsideHorizontal` `DiagonalDown`、、、、 `DiagonalUp`。</span><span class="sxs-lookup"><span data-stu-id="884d0-136">The possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span></span> <span data-ttu-id="884d0-137">只读。</span><span class="sxs-lookup"><span data-stu-id="884d0-137">Read-only.</span></span>|
|<span data-ttu-id="884d0-138">样式</span><span class="sxs-lookup"><span data-stu-id="884d0-138">style</span></span>|<span data-ttu-id="884d0-139">string</span><span class="sxs-lookup"><span data-stu-id="884d0-139">string</span></span>|<span data-ttu-id="884d0-140">线条样式的常量之一，指定边框的线条样式。</span><span class="sxs-lookup"><span data-stu-id="884d0-140">One of the constants of line style specifying the line style for the border.</span></span> <span data-ttu-id="884d0-141">可能的值为: `None`、 `Continuous`、 `Dash` `DashDot` `DashDotDot` `Dot` `Double`、、、、 `SlantDashDot`。</span><span class="sxs-lookup"><span data-stu-id="884d0-141">The possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="884d0-142">weight</span><span class="sxs-lookup"><span data-stu-id="884d0-142">weight</span></span>|<span data-ttu-id="884d0-143">string</span><span class="sxs-lookup"><span data-stu-id="884d0-143">string</span></span>|<span data-ttu-id="884d0-144">指定区域周围的边框的粗细。</span><span class="sxs-lookup"><span data-stu-id="884d0-144">Specifies the weight of the border around a range.</span></span> <span data-ttu-id="884d0-145">可能的值为: `Hairline`、 `Thin`、 `Medium`、 `Thick`。</span><span class="sxs-lookup"><span data-stu-id="884d0-145">The possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="884d0-146">关系</span><span class="sxs-lookup"><span data-stu-id="884d0-146">Relationships</span></span>
<span data-ttu-id="884d0-147">无</span><span class="sxs-lookup"><span data-stu-id="884d0-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="884d0-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="884d0-148">JSON representation</span></span>

<span data-ttu-id="884d0-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="884d0-149">Here is a JSON representation of the resource.</span></span>

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
