---
title: rubricQuality 资源类型
description: Rubric 的质量
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1773bfb40e7857b65272cbf611cb7394b019197e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016092"
---
# <a name="rubricquality-resource-type"></a><span data-ttu-id="ee7c3-103">rubricQuality 资源类型</span><span class="sxs-lookup"><span data-stu-id="ee7c3-103">rubricQuality resource type</span></span>

<span data-ttu-id="ee7c3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee7c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee7c3-105">Rubric 的质量。</span><span class="sxs-lookup"><span data-stu-id="ee7c3-105">A quality of a rubric.</span></span> <span data-ttu-id="ee7c3-106">有关 rubric*质量*、*级别*和*条件*之间的关系的说明，请参阅[educationRubric](educationrubric.md) 。</span><span class="sxs-lookup"><span data-stu-id="ee7c3-106">See [educationRubric](educationrubric.md) for a description of the relationship between rubric *qualities*, *levels*, and *criteria*.</span></span>

## <a name="properties"></a><span data-ttu-id="ee7c3-107">属性</span><span class="sxs-lookup"><span data-stu-id="ee7c3-107">Properties</span></span>

| <span data-ttu-id="ee7c3-108">属性</span><span class="sxs-lookup"><span data-stu-id="ee7c3-108">Property</span></span>     | <span data-ttu-id="ee7c3-109">类型</span><span class="sxs-lookup"><span data-stu-id="ee7c3-109">Type</span></span>        | <span data-ttu-id="ee7c3-110">说明</span><span class="sxs-lookup"><span data-stu-id="ee7c3-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ee7c3-111">条件</span><span class="sxs-lookup"><span data-stu-id="ee7c3-111">criteria</span></span>|<span data-ttu-id="ee7c3-112">[rubricCriterion](rubriccriterion.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ee7c3-112">[rubricCriterion](rubriccriterion.md) collection</span></span>|<span data-ttu-id="ee7c3-113">此 rubric 质量的条件集合。</span><span class="sxs-lookup"><span data-stu-id="ee7c3-113">The collection of criteria for this rubric quality.</span></span>|
|<span data-ttu-id="ee7c3-114">description</span><span class="sxs-lookup"><span data-stu-id="ee7c3-114">description</span></span>|[<span data-ttu-id="ee7c3-115">itemBody</span><span class="sxs-lookup"><span data-stu-id="ee7c3-115">itemBody</span></span>](itembody.md)|<span data-ttu-id="ee7c3-116">此 rubric 质量的说明。</span><span class="sxs-lookup"><span data-stu-id="ee7c3-116">The description of this rubric quality.</span></span>|
|<span data-ttu-id="ee7c3-117">displayName</span><span class="sxs-lookup"><span data-stu-id="ee7c3-117">displayName</span></span>|<span data-ttu-id="ee7c3-118">String</span><span class="sxs-lookup"><span data-stu-id="ee7c3-118">String</span></span>|<span data-ttu-id="ee7c3-119">此 rubric 质量的名称。</span><span class="sxs-lookup"><span data-stu-id="ee7c3-119">The name of this rubric quality.</span></span>|
|<span data-ttu-id="ee7c3-120">qualityId</span><span class="sxs-lookup"><span data-stu-id="ee7c3-120">qualityId</span></span>|<span data-ttu-id="ee7c3-121">String</span><span class="sxs-lookup"><span data-stu-id="ee7c3-121">String</span></span>|<span data-ttu-id="ee7c3-122">此资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="ee7c3-122">The ID of this resource.</span></span>|
|<span data-ttu-id="ee7c3-123">weight</span><span class="sxs-lookup"><span data-stu-id="ee7c3-123">weight</span></span>|<span data-ttu-id="ee7c3-124">单一</span><span class="sxs-lookup"><span data-stu-id="ee7c3-124">Single</span></span>|<span data-ttu-id="ee7c3-125">如果有，则为此质量的数字权重。</span><span class="sxs-lookup"><span data-stu-id="ee7c3-125">If present, a numerical weight for this quality.</span></span>  <span data-ttu-id="ee7c3-126">权重必须添加到100。</span><span class="sxs-lookup"><span data-stu-id="ee7c3-126">Weights must add up to 100.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ee7c3-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ee7c3-127">JSON representation</span></span>

<span data-ttu-id="ee7c3-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ee7c3-128">The following is a JSON representation of the resource.</span></span>

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

