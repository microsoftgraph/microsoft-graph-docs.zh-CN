---
title: rubricLevel 资源类型
description: Rubric 的级别
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 14a7c084aad907ce2e5f90b06f17b64aca9c331e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016102"
---
# <a name="rubriclevel-resource-type"></a><span data-ttu-id="42877-103">rubricLevel 资源类型</span><span class="sxs-lookup"><span data-stu-id="42877-103">rubricLevel resource type</span></span>

<span data-ttu-id="42877-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42877-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42877-105">Rubric 的级别。</span><span class="sxs-lookup"><span data-stu-id="42877-105">A level of a rubric.</span></span> <span data-ttu-id="42877-106">有关 rubric*质量*、*级别*和*条件*之间的关系的说明，请参阅[educationRubric](educationrubric.md) 。</span><span class="sxs-lookup"><span data-stu-id="42877-106">See [educationRubric](educationrubric.md) for a description of the relationship between rubric *qualities*, *levels*, and *criteria*.</span></span>

## <a name="properties"></a><span data-ttu-id="42877-107">属性</span><span class="sxs-lookup"><span data-stu-id="42877-107">Properties</span></span>

| <span data-ttu-id="42877-108">属性</span><span class="sxs-lookup"><span data-stu-id="42877-108">Property</span></span>     | <span data-ttu-id="42877-109">类型</span><span class="sxs-lookup"><span data-stu-id="42877-109">Type</span></span>        | <span data-ttu-id="42877-110">说明</span><span class="sxs-lookup"><span data-stu-id="42877-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="42877-111">说明</span><span class="sxs-lookup"><span data-stu-id="42877-111">description</span></span>|[<span data-ttu-id="42877-112">itemBody</span><span class="sxs-lookup"><span data-stu-id="42877-112">itemBody</span></span>](itembody.md)|<span data-ttu-id="42877-113">此 rubric 级别的说明。</span><span class="sxs-lookup"><span data-stu-id="42877-113">The description of this rubric level.</span></span>|
|<span data-ttu-id="42877-114">displayName</span><span class="sxs-lookup"><span data-stu-id="42877-114">displayName</span></span>|<span data-ttu-id="42877-115">String</span><span class="sxs-lookup"><span data-stu-id="42877-115">String</span></span>|<span data-ttu-id="42877-116">此 rubric 级别的名称。</span><span class="sxs-lookup"><span data-stu-id="42877-116">The name of this rubric level.</span></span>|
|<span data-ttu-id="42877-117">评分</span><span class="sxs-lookup"><span data-stu-id="42877-117">grading</span></span>|[<span data-ttu-id="42877-118">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="42877-118">educationAssignmentGradeType</span></span>](educationassignmentgradetype.md)|<span data-ttu-id="42877-119">如果这是一个无点的 rubric，则为 Null; [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) 如果是点 rubric。</span><span class="sxs-lookup"><span data-stu-id="42877-119">Null if this is a no-points rubric; [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) if it is a points rubric.</span></span>|
|<span data-ttu-id="42877-120">levelId</span><span class="sxs-lookup"><span data-stu-id="42877-120">levelId</span></span>|<span data-ttu-id="42877-121">String</span><span class="sxs-lookup"><span data-stu-id="42877-121">String</span></span>|<span data-ttu-id="42877-122">此资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="42877-122">The ID of this resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="42877-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="42877-123">JSON representation</span></span>

<span data-ttu-id="42877-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="42877-124">The following is a JSON representation of the resource.</span></span>

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

