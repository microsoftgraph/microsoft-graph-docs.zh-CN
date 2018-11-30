---
title: 图标资源类型
description: 表示单元格图标。
ms.openlocfilehash: fd3e0682a7eb73dd4e3286e11d9f9680755db265
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043502"
---
# <a name="icon-resource-type"></a><span data-ttu-id="e32a8-103">图标资源类型</span><span class="sxs-lookup"><span data-stu-id="e32a8-103">Icon resource type</span></span>

> <span data-ttu-id="e32a8-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e32a8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e32a8-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e32a8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e32a8-106">表示单元格图标。</span><span class="sxs-lookup"><span data-stu-id="e32a8-106">Represents a cell icon.</span></span>


## <a name="methods"></a><span data-ttu-id="e32a8-107">方法</span><span class="sxs-lookup"><span data-stu-id="e32a8-107">Methods</span></span>

| <span data-ttu-id="e32a8-108">方法</span><span class="sxs-lookup"><span data-stu-id="e32a8-108">Method</span></span>           | <span data-ttu-id="e32a8-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e32a8-109">Return Type</span></span>    |<span data-ttu-id="e32a8-110">说明</span><span class="sxs-lookup"><span data-stu-id="e32a8-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e32a8-111">获取图标</span><span class="sxs-lookup"><span data-stu-id="e32a8-111">Get Icon</span></span>](../api/icon-get.md) | [<span data-ttu-id="e32a8-112">Icon</span><span class="sxs-lookup"><span data-stu-id="e32a8-112">Icon</span></span>](icon.md) |<span data-ttu-id="e32a8-113">读取 icon 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e32a8-113">Read properties and relationships of icon object.</span></span>|
|[<span data-ttu-id="e32a8-114">Update</span><span class="sxs-lookup"><span data-stu-id="e32a8-114">Update</span></span>](../api/icon-update.md) | [<span data-ttu-id="e32a8-115">Icon</span><span class="sxs-lookup"><span data-stu-id="e32a8-115">Icon</span></span>](icon.md)  |<span data-ttu-id="e32a8-116">更新 icon 对象。</span><span class="sxs-lookup"><span data-stu-id="e32a8-116">Update Icon object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e32a8-117">属性</span><span class="sxs-lookup"><span data-stu-id="e32a8-117">Properties</span></span>
| <span data-ttu-id="e32a8-118">属性</span><span class="sxs-lookup"><span data-stu-id="e32a8-118">Property</span></span>     | <span data-ttu-id="e32a8-119">类型</span><span class="sxs-lookup"><span data-stu-id="e32a8-119">Type</span></span>   |<span data-ttu-id="e32a8-120">说明</span><span class="sxs-lookup"><span data-stu-id="e32a8-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e32a8-121">index</span><span class="sxs-lookup"><span data-stu-id="e32a8-121">index</span></span>|<span data-ttu-id="e32a8-122">整数</span><span class="sxs-lookup"><span data-stu-id="e32a8-122">int</span></span>|<span data-ttu-id="e32a8-123">表示给定集合中图标的索引。</span><span class="sxs-lookup"><span data-stu-id="e32a8-123">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="e32a8-124">set</span><span class="sxs-lookup"><span data-stu-id="e32a8-124">set</span></span>|<span data-ttu-id="e32a8-125">string</span><span class="sxs-lookup"><span data-stu-id="e32a8-125">string</span></span>|<span data-ttu-id="e32a8-p102">表示图标所属的集合。可能的值是：`Invalid`、`ThreeArrows`、`ThreeArrowsGray`、`ThreeFlags`、`ThreeTrafficLights1`、`ThreeTrafficLights2`、`ThreeSigns`、`ThreeSymbols`、`ThreeSymbols2`、`FourArrows`、`FourArrowsGray`、`FourRedToBlack`、`FourRating`、`FourTrafficLights`、`FiveArrows`、`FiveArrowsGray`、`FiveRating`、`FiveQuarters`、`ThreeStars`、`ThreeTriangles``FiveBoxes`。</span><span class="sxs-lookup"><span data-stu-id="e32a8-p102">Represents the set that the icon is part of. Possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e32a8-128">Relationships</span><span class="sxs-lookup"><span data-stu-id="e32a8-128">Relationships</span></span>
<span data-ttu-id="e32a8-129">无</span><span class="sxs-lookup"><span data-stu-id="e32a8-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e32a8-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e32a8-130">JSON representation</span></span>

<span data-ttu-id="e32a8-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e32a8-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.icon"
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