---
title: rubricQuality 资源类型
description: Rubric 的质量
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e63fd8ad7aa7d0a19fe1774e18bba5d59af52140
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173305"
---
# <a name="rubricquality-resource-type"></a><span data-ttu-id="b1b48-103">rubricQuality 资源类型</span><span class="sxs-lookup"><span data-stu-id="b1b48-103">rubricQuality resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1b48-104">Rubric 的质量。</span><span class="sxs-lookup"><span data-stu-id="b1b48-104">A quality of a rubric.</span></span> <span data-ttu-id="b1b48-105">有关 rubric*质量*、*级别*和*条件*之间的关系的说明, 请参阅[educationRubric](educationrubric.md) 。</span><span class="sxs-lookup"><span data-stu-id="b1b48-105">See [educationRubric](educationrubric.md) for a description of the relationship between rubric *qualities*, *levels*, and *criteria*.</span></span>

## <a name="properties"></a><span data-ttu-id="b1b48-106">属性</span><span class="sxs-lookup"><span data-stu-id="b1b48-106">Properties</span></span>

| <span data-ttu-id="b1b48-107">属性</span><span class="sxs-lookup"><span data-stu-id="b1b48-107">Property</span></span>     | <span data-ttu-id="b1b48-108">类型</span><span class="sxs-lookup"><span data-stu-id="b1b48-108">Type</span></span>        | <span data-ttu-id="b1b48-109">说明</span><span class="sxs-lookup"><span data-stu-id="b1b48-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b1b48-110">条件</span><span class="sxs-lookup"><span data-stu-id="b1b48-110">criteria</span></span>|<span data-ttu-id="b1b48-111">[rubricCriterion](rubriccriterion.md)集合</span><span class="sxs-lookup"><span data-stu-id="b1b48-111">[rubricCriterion](rubriccriterion.md) collection</span></span>|<span data-ttu-id="b1b48-112">此 rubric 质量的条件集合。</span><span class="sxs-lookup"><span data-stu-id="b1b48-112">The collection of criteria for this rubric quality.</span></span>|
|<span data-ttu-id="b1b48-113">说明</span><span class="sxs-lookup"><span data-stu-id="b1b48-113">description</span></span>|[<span data-ttu-id="b1b48-114">itemBody</span><span class="sxs-lookup"><span data-stu-id="b1b48-114">itemBody</span></span>](itembody.md)|<span data-ttu-id="b1b48-115">此 rubric 质量的说明。</span><span class="sxs-lookup"><span data-stu-id="b1b48-115">The description of this rubric quality.</span></span>|
|<span data-ttu-id="b1b48-116">displayName</span><span class="sxs-lookup"><span data-stu-id="b1b48-116">displayName</span></span>|<span data-ttu-id="b1b48-117">String</span><span class="sxs-lookup"><span data-stu-id="b1b48-117">String</span></span>|<span data-ttu-id="b1b48-118">此 rubric 质量的名称。</span><span class="sxs-lookup"><span data-stu-id="b1b48-118">The name of this rubric quality.</span></span>|
|<span data-ttu-id="b1b48-119">qualityId</span><span class="sxs-lookup"><span data-stu-id="b1b48-119">qualityId</span></span>|<span data-ttu-id="b1b48-120">String</span><span class="sxs-lookup"><span data-stu-id="b1b48-120">String</span></span>|<span data-ttu-id="b1b48-121">此资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="b1b48-121">The ID of this resource.</span></span>|
|<span data-ttu-id="b1b48-122">weight</span><span class="sxs-lookup"><span data-stu-id="b1b48-122">weight</span></span>|<span data-ttu-id="b1b48-123">单精度</span><span class="sxs-lookup"><span data-stu-id="b1b48-123">Single</span></span>|<span data-ttu-id="b1b48-124">如果有, 则为此质量的数字权重。</span><span class="sxs-lookup"><span data-stu-id="b1b48-124">If present, a numerical weight for this quality.</span></span>  <span data-ttu-id="b1b48-125">权重必须添加到100。</span><span class="sxs-lookup"><span data-stu-id="b1b48-125">Weights must add up to 100.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b1b48-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b1b48-126">JSON representation</span></span>

<span data-ttu-id="b1b48-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1b48-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricQuality",
  "baseType": null
}-->

```json
{
  "criteria": [{"@odata.type": "microsoft.graph.rubricCriterion"}],
  "description": {"@odata.type": "microsoft.graph.itemBody"},
  "displayName": "String",
  "qualityId": "String",
  "weight": "Double"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricQuality resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->