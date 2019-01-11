---
title: 图标资源类型
description: 表示单元格图标。
localization_priority: Normal
ms.openlocfilehash: 833fa4cb4061a96b01077c3adeb7dcaed49e0a02
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872567"
---
# <a name="icon-resource-type"></a><span data-ttu-id="a591c-103">图标资源类型</span><span class="sxs-lookup"><span data-stu-id="a591c-103">Icon resource type</span></span>

<span data-ttu-id="a591c-104">表示单元格图标。</span><span class="sxs-lookup"><span data-stu-id="a591c-104">Represents a cell icon.</span></span>


## <a name="methods"></a><span data-ttu-id="a591c-105">方法</span><span class="sxs-lookup"><span data-stu-id="a591c-105">Methods</span></span>

| <span data-ttu-id="a591c-106">方法</span><span class="sxs-lookup"><span data-stu-id="a591c-106">Method</span></span>           | <span data-ttu-id="a591c-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="a591c-107">Return Type</span></span>    |<span data-ttu-id="a591c-108">说明</span><span class="sxs-lookup"><span data-stu-id="a591c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a591c-109">获取图标</span><span class="sxs-lookup"><span data-stu-id="a591c-109">Get Icon</span></span>](../api/icon-get.md) | [<span data-ttu-id="a591c-110">Icon</span><span class="sxs-lookup"><span data-stu-id="a591c-110">Icon</span></span>](icon.md) |<span data-ttu-id="a591c-111">读取 icon 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a591c-111">Read properties and relationships of icon object.</span></span>|
|[<span data-ttu-id="a591c-112">Update</span><span class="sxs-lookup"><span data-stu-id="a591c-112">Update</span></span>](../api/icon-update.md) | [<span data-ttu-id="a591c-113">Icon</span><span class="sxs-lookup"><span data-stu-id="a591c-113">Icon</span></span>](icon.md)  |<span data-ttu-id="a591c-114">更新 icon 对象。</span><span class="sxs-lookup"><span data-stu-id="a591c-114">Update Icon object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a591c-115">属性</span><span class="sxs-lookup"><span data-stu-id="a591c-115">Properties</span></span>
| <span data-ttu-id="a591c-116">属性</span><span class="sxs-lookup"><span data-stu-id="a591c-116">Property</span></span>     | <span data-ttu-id="a591c-117">类型</span><span class="sxs-lookup"><span data-stu-id="a591c-117">Type</span></span>   |<span data-ttu-id="a591c-118">说明</span><span class="sxs-lookup"><span data-stu-id="a591c-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a591c-119">index</span><span class="sxs-lookup"><span data-stu-id="a591c-119">index</span></span>|<span data-ttu-id="a591c-120">int</span><span class="sxs-lookup"><span data-stu-id="a591c-120">int</span></span>|<span data-ttu-id="a591c-121">表示给定集合中图标的索引。</span><span class="sxs-lookup"><span data-stu-id="a591c-121">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="a591c-122">set</span><span class="sxs-lookup"><span data-stu-id="a591c-122">set</span></span>|<span data-ttu-id="a591c-123">string</span><span class="sxs-lookup"><span data-stu-id="a591c-123">string</span></span>|<span data-ttu-id="a591c-124">表示的图标集。</span><span class="sxs-lookup"><span data-stu-id="a591c-124">Represents the set that the icon is part of.</span></span> <span data-ttu-id="a591c-125">可能的值为： `Invalid`， `ThreeArrows`， `ThreeArrowsGray`， `ThreeFlags`， `ThreeTrafficLights1`， `ThreeTrafficLights2`， `ThreeSigns`， `ThreeSymbols`， `ThreeSymbols2`， `FourArrows`， `FourArrowsGray`， `FourRedToBlack`， `FourRating`， `FourTrafficLights`， `FiveArrows`， `FiveArrowsGray`， `FiveRating`， `FiveQuarters`， `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span><span class="sxs-lookup"><span data-stu-id="a591c-125">The possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a591c-126">Relationships</span><span class="sxs-lookup"><span data-stu-id="a591c-126">Relationships</span></span>
<span data-ttu-id="a591c-127">无</span><span class="sxs-lookup"><span data-stu-id="a591c-127">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a591c-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a591c-128">JSON representation</span></span>

<span data-ttu-id="a591c-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a591c-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookIcon"
}-->

```json
{
  "index": 1024,
  "set": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Icon resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
