---
title: rubricLevel 资源类型
description: Rubric 的级别
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: dd8e67cbf4ba8994e03d683665928f9e62608d8e
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173333"
---
# <a name="rubriclevel-resource-type"></a><span data-ttu-id="5ee99-103">rubricLevel 资源类型</span><span class="sxs-lookup"><span data-stu-id="5ee99-103">rubricLevel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ee99-104">Rubric 的级别。</span><span class="sxs-lookup"><span data-stu-id="5ee99-104">A level of a rubric.</span></span> <span data-ttu-id="5ee99-105">有关 rubric*质量*、*级别*和*条件*之间的关系的说明, 请参阅[educationRubric](educationrubric.md) 。</span><span class="sxs-lookup"><span data-stu-id="5ee99-105">See [educationRubric](educationrubric.md) for a description of the relationship between rubric *qualities*, *levels*, and *criteria*.</span></span>

## <a name="properties"></a><span data-ttu-id="5ee99-106">属性</span><span class="sxs-lookup"><span data-stu-id="5ee99-106">Properties</span></span>

| <span data-ttu-id="5ee99-107">属性</span><span class="sxs-lookup"><span data-stu-id="5ee99-107">Property</span></span>     | <span data-ttu-id="5ee99-108">类型</span><span class="sxs-lookup"><span data-stu-id="5ee99-108">Type</span></span>        | <span data-ttu-id="5ee99-109">说明</span><span class="sxs-lookup"><span data-stu-id="5ee99-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5ee99-110">说明</span><span class="sxs-lookup"><span data-stu-id="5ee99-110">description</span></span>|[<span data-ttu-id="5ee99-111">itemBody</span><span class="sxs-lookup"><span data-stu-id="5ee99-111">itemBody</span></span>](itembody.md)|<span data-ttu-id="5ee99-112">此 rubric 级别的说明。</span><span class="sxs-lookup"><span data-stu-id="5ee99-112">The description of this rubric level.</span></span>|
|<span data-ttu-id="5ee99-113">displayName</span><span class="sxs-lookup"><span data-stu-id="5ee99-113">displayName</span></span>|<span data-ttu-id="5ee99-114">String</span><span class="sxs-lookup"><span data-stu-id="5ee99-114">String</span></span>|<span data-ttu-id="5ee99-115">此 rubric 级别的名称。</span><span class="sxs-lookup"><span data-stu-id="5ee99-115">The name of this rubric level.</span></span>|
|<span data-ttu-id="5ee99-116">评分</span><span class="sxs-lookup"><span data-stu-id="5ee99-116">grading</span></span>|[<span data-ttu-id="5ee99-117">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="5ee99-117">educationAssignmentGradeType</span></span>](educationassignmentgradetype.md)|<span data-ttu-id="5ee99-118">如果这是一个无点的 rubric, 则为 Null;[educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md)如果是点 rubric。</span><span class="sxs-lookup"><span data-stu-id="5ee99-118">Null if this is a no-points rubric; [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) if it is a points rubric.</span></span>|
|<span data-ttu-id="5ee99-119">levelId</span><span class="sxs-lookup"><span data-stu-id="5ee99-119">levelId</span></span>|<span data-ttu-id="5ee99-120">String</span><span class="sxs-lookup"><span data-stu-id="5ee99-120">String</span></span>|<span data-ttu-id="5ee99-121">此资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="5ee99-121">The ID of this resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5ee99-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5ee99-122">JSON representation</span></span>

<span data-ttu-id="5ee99-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5ee99-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricLevel",
  "baseType": null
}-->

```json
{
  "description": {"@odata.type": "microsoft.graph.itemBody"},
  "displayName": "String",
  "grading": {"@odata.type": "microsoft.graph.educationAssignmentGradeType"},
  "levelId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->