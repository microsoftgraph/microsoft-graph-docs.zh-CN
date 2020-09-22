---
title: workbookRangeBorder 资源类型
description: 代表对象的边框。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 054b2db2b1292136c5044a158f3aaa6072d68e51
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046232"
---
# <a name="workbookrangeborder-resource-type"></a><span data-ttu-id="aa5ae-103">workbookRangeBorder 资源类型</span><span class="sxs-lookup"><span data-stu-id="aa5ae-103">workbookRangeBorder resource type</span></span>

<span data-ttu-id="aa5ae-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa5ae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa5ae-105">代表对象的边框。</span><span class="sxs-lookup"><span data-stu-id="aa5ae-105">Represents the border of an object.</span></span>


## <a name="methods"></a><span data-ttu-id="aa5ae-106">方法</span><span class="sxs-lookup"><span data-stu-id="aa5ae-106">Methods</span></span>

| <span data-ttu-id="aa5ae-107">方法</span><span class="sxs-lookup"><span data-stu-id="aa5ae-107">Method</span></span>           | <span data-ttu-id="aa5ae-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="aa5ae-108">Return Type</span></span>    |<span data-ttu-id="aa5ae-109">说明</span><span class="sxs-lookup"><span data-stu-id="aa5ae-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aa5ae-110">获取 workbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="aa5ae-110">Get workbookRangeBorder</span></span>](../api/rangeborder-get.md) | [<span data-ttu-id="aa5ae-111">workbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="aa5ae-111">workbookRangeBorder</span></span>](workbookrangeborder.md) |<span data-ttu-id="aa5ae-112">读取 rangeborder 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="aa5ae-112">Read properties and relationships of rangeBorder object.</span></span>|
|[<span data-ttu-id="aa5ae-113">更新</span><span class="sxs-lookup"><span data-stu-id="aa5ae-113">Update</span></span>](../api/rangeborder-update.md) | [<span data-ttu-id="aa5ae-114">workbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="aa5ae-114">workbookRangeBorder</span></span>](workbookrangeborder.md) |<span data-ttu-id="aa5ae-115">更新 RangeBorder 对象。</span><span class="sxs-lookup"><span data-stu-id="aa5ae-115">Update RangeBorder object.</span></span> |
|[<span data-ttu-id="aa5ae-116">列出</span><span class="sxs-lookup"><span data-stu-id="aa5ae-116">List</span></span>](../api/rangeborder-list.md) | <span data-ttu-id="aa5ae-117">[workbookRangeBorder](workbookrangeborder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aa5ae-117">[workbookRangeBorder](workbookrangeborder.md) collection</span></span> |<span data-ttu-id="aa5ae-118">获取 rangeBorder 对象集合。</span><span class="sxs-lookup"><span data-stu-id="aa5ae-118">Get rangeBorder object collection.</span></span> |
|[<span data-ttu-id="aa5ae-119">Itemat</span><span class="sxs-lookup"><span data-stu-id="aa5ae-119">Itemat</span></span>](../api/rangebordercollection-itemat.md)|[<span data-ttu-id="aa5ae-120">workbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="aa5ae-120">workbookRangeBorder</span></span>](workbookrangeborder.md)|<span data-ttu-id="aa5ae-121">使用其索引获取 border 对象</span><span class="sxs-lookup"><span data-stu-id="aa5ae-121">Gets a border object using its index</span></span>|

## <a name="properties"></a><span data-ttu-id="aa5ae-122">属性</span><span class="sxs-lookup"><span data-stu-id="aa5ae-122">Properties</span></span>
| <span data-ttu-id="aa5ae-123">属性</span><span class="sxs-lookup"><span data-stu-id="aa5ae-123">Property</span></span>     | <span data-ttu-id="aa5ae-124">类型</span><span class="sxs-lookup"><span data-stu-id="aa5ae-124">Type</span></span>   |<span data-ttu-id="aa5ae-125">说明</span><span class="sxs-lookup"><span data-stu-id="aa5ae-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa5ae-126">color</span><span class="sxs-lookup"><span data-stu-id="aa5ae-126">color</span></span>|<span data-ttu-id="aa5ae-127">string</span><span class="sxs-lookup"><span data-stu-id="aa5ae-127">string</span></span>|<span data-ttu-id="aa5ae-128">表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="aa5ae-128">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="aa5ae-129">id</span><span class="sxs-lookup"><span data-stu-id="aa5ae-129">id</span></span>|<span data-ttu-id="aa5ae-130">string</span><span class="sxs-lookup"><span data-stu-id="aa5ae-130">string</span></span>|<span data-ttu-id="aa5ae-p101">表示边框标识符。可能的值是：`EdgeTop`、`EdgeBottom`、`EdgeLeft`、`EdgeRight`、`InsideVertical`、`InsideHorizontal`、`DiagonalDown`、`DiagonalUp`。只读。</span><span class="sxs-lookup"><span data-stu-id="aa5ae-p101">Represents border identifier. Possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Read-only.</span></span>|
|<span data-ttu-id="aa5ae-134">sideIndex</span><span class="sxs-lookup"><span data-stu-id="aa5ae-134">sideIndex</span></span>|<span data-ttu-id="aa5ae-135">string</span><span class="sxs-lookup"><span data-stu-id="aa5ae-135">string</span></span>|<span data-ttu-id="aa5ae-p102">指示边框的特定边的常量值。可能的值是：`EdgeTop`、`EdgeBottom`、`EdgeLeft`、`EdgeRight`、`InsideVertical`、`InsideHorizontal`、`DiagonalDown`、`DiagonalUp`。只读。</span><span class="sxs-lookup"><span data-stu-id="aa5ae-p102">Constant value that indicates the specific side of the border. Possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Read-only.</span></span>|
|<span data-ttu-id="aa5ae-139">style</span><span class="sxs-lookup"><span data-stu-id="aa5ae-139">style</span></span>|<span data-ttu-id="aa5ae-140">string</span><span class="sxs-lookup"><span data-stu-id="aa5ae-140">string</span></span>|<span data-ttu-id="aa5ae-p103">线条样式的常量之一，指定边框的线条样式。可能的值是：`None`、`Continuous`、`Dash`、`DashDot`、`DashDotDot`、`Dot`、`Double`、`SlantDashDot`。</span><span class="sxs-lookup"><span data-stu-id="aa5ae-p103">One of the constants of line style specifying the line style for the border. Possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="aa5ae-143">weight</span><span class="sxs-lookup"><span data-stu-id="aa5ae-143">weight</span></span>|<span data-ttu-id="aa5ae-144">string</span><span class="sxs-lookup"><span data-stu-id="aa5ae-144">string</span></span>|<span data-ttu-id="aa5ae-p104">指定区域周围边框的权重。可能的值是：`Hairline`、`Thin`、`Medium`、`Thick`。</span><span class="sxs-lookup"><span data-stu-id="aa5ae-p104">Specifies the weight of the border around a range. Possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa5ae-147">关系</span><span class="sxs-lookup"><span data-stu-id="aa5ae-147">Relationships</span></span>
<span data-ttu-id="aa5ae-148">无</span><span class="sxs-lookup"><span data-stu-id="aa5ae-148">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="aa5ae-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aa5ae-149">JSON representation</span></span>

<span data-ttu-id="aa5ae-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa5ae-150">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "RangeBorder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


