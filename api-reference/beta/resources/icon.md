---
title: 图标资源类型
description: 表示单元格图标。
localization_priority: Normal
ms.openlocfilehash: c15ee02d1c6830cbb5246826665d0353b7e999b9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506399"
---
# <a name="icon-resource-type"></a><span data-ttu-id="d6299-103">图标资源类型</span><span class="sxs-lookup"><span data-stu-id="d6299-103">Icon resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6299-104">表示单元格图标。</span><span class="sxs-lookup"><span data-stu-id="d6299-104">Represents a cell icon.</span></span>


## <a name="methods"></a><span data-ttu-id="d6299-105">方法</span><span class="sxs-lookup"><span data-stu-id="d6299-105">Methods</span></span>

| <span data-ttu-id="d6299-106">方法</span><span class="sxs-lookup"><span data-stu-id="d6299-106">Method</span></span>           | <span data-ttu-id="d6299-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="d6299-107">Return Type</span></span>    |<span data-ttu-id="d6299-108">说明</span><span class="sxs-lookup"><span data-stu-id="d6299-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d6299-109">获取图标</span><span class="sxs-lookup"><span data-stu-id="d6299-109">Get Icon</span></span>](../api/icon-get.md) | [<span data-ttu-id="d6299-110">Icon</span><span class="sxs-lookup"><span data-stu-id="d6299-110">Icon</span></span>](icon.md) |<span data-ttu-id="d6299-111">读取 icon 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d6299-111">Read properties and relationships of icon object.</span></span>|
|[<span data-ttu-id="d6299-112">更新</span><span class="sxs-lookup"><span data-stu-id="d6299-112">Update</span></span>](../api/icon-update.md) | [<span data-ttu-id="d6299-113">图标</span><span class="sxs-lookup"><span data-stu-id="d6299-113">Icon</span></span>](icon.md)  |<span data-ttu-id="d6299-114">更新 icon 对象。</span><span class="sxs-lookup"><span data-stu-id="d6299-114">Update Icon object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d6299-115">属性</span><span class="sxs-lookup"><span data-stu-id="d6299-115">Properties</span></span>
| <span data-ttu-id="d6299-116">属性</span><span class="sxs-lookup"><span data-stu-id="d6299-116">Property</span></span>     | <span data-ttu-id="d6299-117">类型</span><span class="sxs-lookup"><span data-stu-id="d6299-117">Type</span></span>   |<span data-ttu-id="d6299-118">说明</span><span class="sxs-lookup"><span data-stu-id="d6299-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d6299-119">index</span><span class="sxs-lookup"><span data-stu-id="d6299-119">index</span></span>|<span data-ttu-id="d6299-120">int</span><span class="sxs-lookup"><span data-stu-id="d6299-120">int</span></span>|<span data-ttu-id="d6299-121">表示给定集合中图标的索引。</span><span class="sxs-lookup"><span data-stu-id="d6299-121">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="d6299-122">set</span><span class="sxs-lookup"><span data-stu-id="d6299-122">set</span></span>|<span data-ttu-id="d6299-123">string</span><span class="sxs-lookup"><span data-stu-id="d6299-123">string</span></span>|<span data-ttu-id="d6299-124">表示图标所属的集合。</span><span class="sxs-lookup"><span data-stu-id="d6299-124">Represents the set that the icon is part of.</span></span> <span data-ttu-id="d6299-125">可取值为：`Invalid`、`ThreeArrows`、`ThreeArrowsGray`、`ThreeFlags`、`ThreeTrafficLights1`、`ThreeTrafficLights2`、`ThreeSigns`、`ThreeSymbols`、`ThreeSymbols2`、`FourArrows`、`FourArrowsGray`、`FourRedToBlack`、`FourRating`、`FourTrafficLights`、`FiveArrows`、`FiveArrowsGray`、`FiveRating`、`FiveQuarters`、`ThreeStars`、`ThreeTriangles`、`FiveBoxes`。</span><span class="sxs-lookup"><span data-stu-id="d6299-125">Possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6299-126">关系</span><span class="sxs-lookup"><span data-stu-id="d6299-126">Relationships</span></span>
<span data-ttu-id="d6299-127">无</span><span class="sxs-lookup"><span data-stu-id="d6299-127">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d6299-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d6299-128">JSON representation</span></span>

<span data-ttu-id="d6299-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d6299-129">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Icon resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/icon.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
