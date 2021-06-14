---
title: rubricQuality 资源类型
description: 标准的质量。
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 82fdb8fa226ab6eb2c38b1e49e12904ff26b6491
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911405"
---
# <a name="rubricquality-resource-type"></a><span data-ttu-id="ae2a0-103">rubricQuality 资源类型</span><span class="sxs-lookup"><span data-stu-id="ae2a0-103">rubricQuality resource type</span></span>

<span data-ttu-id="ae2a0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae2a0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ae2a0-105">标准的质量。</span><span class="sxs-lookup"><span data-stu-id="ae2a0-105">A quality of a rubric.</span></span> 

<span data-ttu-id="ae2a0-106">有关标准质量、级别和条件之间的关系的说明，请参阅[educationRubric。](educationrubric.md) </span><span class="sxs-lookup"><span data-stu-id="ae2a0-106">See [educationRubric](educationrubric.md) for a description of the relationship between rubric *qualities*, *levels*, and *criteria*.</span></span>

## <a name="properties"></a><span data-ttu-id="ae2a0-107">属性</span><span class="sxs-lookup"><span data-stu-id="ae2a0-107">Properties</span></span>

| <span data-ttu-id="ae2a0-108">属性</span><span class="sxs-lookup"><span data-stu-id="ae2a0-108">Property</span></span>     | <span data-ttu-id="ae2a0-109">类型</span><span class="sxs-lookup"><span data-stu-id="ae2a0-109">Type</span></span>        | <span data-ttu-id="ae2a0-110">说明</span><span class="sxs-lookup"><span data-stu-id="ae2a0-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ae2a0-111">条件</span><span class="sxs-lookup"><span data-stu-id="ae2a0-111">criteria</span></span>|<span data-ttu-id="ae2a0-112">[rubricCriterion](rubriccriterion.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ae2a0-112">[rubricCriterion](rubriccriterion.md) collection</span></span>|<span data-ttu-id="ae2a0-113">此标准质量标准的集合。</span><span class="sxs-lookup"><span data-stu-id="ae2a0-113">The collection of criteria for this rubric quality.</span></span>|
|<span data-ttu-id="ae2a0-114">说明</span><span class="sxs-lookup"><span data-stu-id="ae2a0-114">description</span></span>|[<span data-ttu-id="ae2a0-115">itemBody</span><span class="sxs-lookup"><span data-stu-id="ae2a0-115">itemBody</span></span>](itembody.md)|<span data-ttu-id="ae2a0-116">此标准质量的说明。</span><span class="sxs-lookup"><span data-stu-id="ae2a0-116">The description of this rubric quality.</span></span>|
|<span data-ttu-id="ae2a0-117">displayName</span><span class="sxs-lookup"><span data-stu-id="ae2a0-117">displayName</span></span>|<span data-ttu-id="ae2a0-118">String</span><span class="sxs-lookup"><span data-stu-id="ae2a0-118">String</span></span>|<span data-ttu-id="ae2a0-119">此标准质量的名称。</span><span class="sxs-lookup"><span data-stu-id="ae2a0-119">The name of this rubric quality.</span></span>|
|<span data-ttu-id="ae2a0-120">qualityId</span><span class="sxs-lookup"><span data-stu-id="ae2a0-120">qualityId</span></span>|<span data-ttu-id="ae2a0-121">String</span><span class="sxs-lookup"><span data-stu-id="ae2a0-121">String</span></span>|<span data-ttu-id="ae2a0-122">此资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="ae2a0-122">The ID of this resource.</span></span>|
|<span data-ttu-id="ae2a0-123">weight</span><span class="sxs-lookup"><span data-stu-id="ae2a0-123">weight</span></span>|<span data-ttu-id="ae2a0-124">单一</span><span class="sxs-lookup"><span data-stu-id="ae2a0-124">Single</span></span>|<span data-ttu-id="ae2a0-125">如果存在，则此质量的数字权重。</span><span class="sxs-lookup"><span data-stu-id="ae2a0-125">If present, a numerical weight for this quality.</span></span>  <span data-ttu-id="ae2a0-126">权重必须最多增加 100。</span><span class="sxs-lookup"><span data-stu-id="ae2a0-126">Weights must add up to 100.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ae2a0-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ae2a0-127">JSON representation</span></span>

<span data-ttu-id="ae2a0-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ae2a0-128">The following is a JSON representation of the resource.</span></span>

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

