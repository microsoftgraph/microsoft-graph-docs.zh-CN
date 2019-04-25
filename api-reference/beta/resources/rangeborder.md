---
title: RangeBorder 资源类型
description: 代表对象的边框。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5b3b814da53013d1daca686d549596a7ab656027
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563229"
---
# <a name="rangeborder-resource-type"></a><span data-ttu-id="393be-103">RangeBorder 资源类型</span><span class="sxs-lookup"><span data-stu-id="393be-103">RangeBorder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="393be-104">代表对象的边框。</span><span class="sxs-lookup"><span data-stu-id="393be-104">Represents the border of an object.</span></span>


## <a name="methods"></a><span data-ttu-id="393be-105">方法</span><span class="sxs-lookup"><span data-stu-id="393be-105">Methods</span></span>

| <span data-ttu-id="393be-106">方法</span><span class="sxs-lookup"><span data-stu-id="393be-106">Method</span></span>           | <span data-ttu-id="393be-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="393be-107">Return Type</span></span>    |<span data-ttu-id="393be-108">说明</span><span class="sxs-lookup"><span data-stu-id="393be-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="393be-109">获取 RangeBorder</span><span class="sxs-lookup"><span data-stu-id="393be-109">Get RangeBorder</span></span>](../api/rangeborder-get.md) | [<span data-ttu-id="393be-110">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="393be-110">RangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="393be-111">读取 rangeborder 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="393be-111">Read properties and relationships of rangeBorder object.</span></span>|
|[<span data-ttu-id="393be-112">更新</span><span class="sxs-lookup"><span data-stu-id="393be-112">Update</span></span>](../api/rangeborder-update.md) | [<span data-ttu-id="393be-113">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="393be-113">RangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="393be-114">更新 RangeBorder 对象。</span><span class="sxs-lookup"><span data-stu-id="393be-114">Update RangeBorder object.</span></span> |
|[<span data-ttu-id="393be-115">列出</span><span class="sxs-lookup"><span data-stu-id="393be-115">List</span></span>](../api/rangeborder-list.md) | <span data-ttu-id="393be-116">[RangeBorder](rangeborder.md) 集合</span><span class="sxs-lookup"><span data-stu-id="393be-116">[RangeBorder](rangeborder.md) collection</span></span> |<span data-ttu-id="393be-117">获取 rangeBorder 对象集合。</span><span class="sxs-lookup"><span data-stu-id="393be-117">Get rangeBorder object collection.</span></span> |
|[<span data-ttu-id="393be-118">Itemat</span><span class="sxs-lookup"><span data-stu-id="393be-118">Itemat</span></span>](../api/rangebordercollection-itemat.md)|[<span data-ttu-id="393be-119">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="393be-119">RangeBorder</span></span>](rangeborder.md)|<span data-ttu-id="393be-120">使用其索引获取 border 对象</span><span class="sxs-lookup"><span data-stu-id="393be-120">Gets a border object using its index</span></span>|

## <a name="properties"></a><span data-ttu-id="393be-121">属性</span><span class="sxs-lookup"><span data-stu-id="393be-121">Properties</span></span>
| <span data-ttu-id="393be-122">属性</span><span class="sxs-lookup"><span data-stu-id="393be-122">Property</span></span>     | <span data-ttu-id="393be-123">类型</span><span class="sxs-lookup"><span data-stu-id="393be-123">Type</span></span>   |<span data-ttu-id="393be-124">说明</span><span class="sxs-lookup"><span data-stu-id="393be-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="393be-125">color</span><span class="sxs-lookup"><span data-stu-id="393be-125">color</span></span>|<span data-ttu-id="393be-126">字符串</span><span class="sxs-lookup"><span data-stu-id="393be-126">string</span></span>|<span data-ttu-id="393be-127">表示窗体 #RRGGBB（例如“FFA500”）的边框线条颜色或作为已命名的 HTML 颜色（例如“orange”）的 HTML 颜色代码。</span><span class="sxs-lookup"><span data-stu-id="393be-127">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="393be-128">id</span><span class="sxs-lookup"><span data-stu-id="393be-128">id</span></span>|<span data-ttu-id="393be-129">string</span><span class="sxs-lookup"><span data-stu-id="393be-129">string</span></span>|<span data-ttu-id="393be-p101">表示边框标识符。可能的值是：`EdgeTop`、`EdgeBottom`、`EdgeLeft`、`EdgeRight`、`InsideVertical`、`InsideHorizontal`、`DiagonalDown`、`DiagonalUp`。只读。</span><span class="sxs-lookup"><span data-stu-id="393be-p101">Represents border identifier. Possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Read-only.</span></span>|
|<span data-ttu-id="393be-133">sideIndex</span><span class="sxs-lookup"><span data-stu-id="393be-133">sideIndex</span></span>|<span data-ttu-id="393be-134">string</span><span class="sxs-lookup"><span data-stu-id="393be-134">string</span></span>|<span data-ttu-id="393be-p102">指示边框的特定边的常量值。可能的值是：`EdgeTop`、`EdgeBottom`、`EdgeLeft`、`EdgeRight`、`InsideVertical`、`InsideHorizontal`、`DiagonalDown`、`DiagonalUp`。只读。</span><span class="sxs-lookup"><span data-stu-id="393be-p102">Constant value that indicates the specific side of the border. Possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Read-only.</span></span>|
|<span data-ttu-id="393be-138">样式</span><span class="sxs-lookup"><span data-stu-id="393be-138">style</span></span>|<span data-ttu-id="393be-139">string</span><span class="sxs-lookup"><span data-stu-id="393be-139">string</span></span>|<span data-ttu-id="393be-p103">线条样式的常量之一，指定边框的线条样式。可能的值是：`None`、`Continuous`、`Dash`、`DashDot`、`DashDotDot`、`Dot`、`Double`、`SlantDashDot`。</span><span class="sxs-lookup"><span data-stu-id="393be-p103">One of the constants of line style specifying the line style for the border. Possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="393be-142">weight</span><span class="sxs-lookup"><span data-stu-id="393be-142">weight</span></span>|<span data-ttu-id="393be-143">string</span><span class="sxs-lookup"><span data-stu-id="393be-143">string</span></span>|<span data-ttu-id="393be-p104">指定区域周围边框的权重。可能的值是：`Hairline`、`Thin`、`Medium`、`Thick`。</span><span class="sxs-lookup"><span data-stu-id="393be-p104">Specifies the weight of the border around a range. Possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="393be-146">关系</span><span class="sxs-lookup"><span data-stu-id="393be-146">Relationships</span></span>
<span data-ttu-id="393be-147">无</span><span class="sxs-lookup"><span data-stu-id="393be-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="393be-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="393be-148">JSON representation</span></span>

<span data-ttu-id="393be-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="393be-149">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "RangeBorder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/rangeborder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
