---
title: rubricLevel 资源类型
description: 标准级别。
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b4cbd952d8c5bed366d6cfbbda5920d7eddba97d
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911406"
---
# <a name="rubriclevel-resource-type"></a><span data-ttu-id="7ff12-103">rubricLevel 资源类型</span><span class="sxs-lookup"><span data-stu-id="7ff12-103">rubricLevel resource type</span></span>

<span data-ttu-id="7ff12-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ff12-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7ff12-105">标准级别。</span><span class="sxs-lookup"><span data-stu-id="7ff12-105">A level of a rubric.</span></span> 

<span data-ttu-id="7ff12-106">有关标准质量、级别和条件之间的关系的说明，请参阅[educationRubric。](educationrubric.md) </span><span class="sxs-lookup"><span data-stu-id="7ff12-106">See [educationRubric](educationrubric.md) for a description of the relationship between rubric *qualities*, *levels*, and *criteria*.</span></span>

## <a name="properties"></a><span data-ttu-id="7ff12-107">属性</span><span class="sxs-lookup"><span data-stu-id="7ff12-107">Properties</span></span>

| <span data-ttu-id="7ff12-108">属性</span><span class="sxs-lookup"><span data-stu-id="7ff12-108">Property</span></span>     | <span data-ttu-id="7ff12-109">类型</span><span class="sxs-lookup"><span data-stu-id="7ff12-109">Type</span></span>        | <span data-ttu-id="7ff12-110">说明</span><span class="sxs-lookup"><span data-stu-id="7ff12-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7ff12-111">说明</span><span class="sxs-lookup"><span data-stu-id="7ff12-111">description</span></span>|[<span data-ttu-id="7ff12-112">itemBody</span><span class="sxs-lookup"><span data-stu-id="7ff12-112">itemBody</span></span>](itembody.md)|<span data-ttu-id="7ff12-113">此标准级别的说明。</span><span class="sxs-lookup"><span data-stu-id="7ff12-113">The description of this rubric level.</span></span>|
|<span data-ttu-id="7ff12-114">displayName</span><span class="sxs-lookup"><span data-stu-id="7ff12-114">displayName</span></span>|<span data-ttu-id="7ff12-115">String</span><span class="sxs-lookup"><span data-stu-id="7ff12-115">String</span></span>|<span data-ttu-id="7ff12-116">此标准级别的名称。</span><span class="sxs-lookup"><span data-stu-id="7ff12-116">The name of this rubric level.</span></span>|
|<span data-ttu-id="7ff12-117">一个</span><span class="sxs-lookup"><span data-stu-id="7ff12-117">grading</span></span>|[<span data-ttu-id="7ff12-118">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="7ff12-118">educationAssignmentGradeType</span></span>](educationassignmentgradetype.md)|<span data-ttu-id="7ff12-119">如果这是无点数的分值，则其为 Null; [educationAssignmentPointsGradeType（](educationassignmentpointsgradetype.md) 如果为分数）。</span><span class="sxs-lookup"><span data-stu-id="7ff12-119">Null if this is a no-points rubric; [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) if it is a points rubric.</span></span>|
|<span data-ttu-id="7ff12-120">levelId</span><span class="sxs-lookup"><span data-stu-id="7ff12-120">levelId</span></span>|<span data-ttu-id="7ff12-121">String</span><span class="sxs-lookup"><span data-stu-id="7ff12-121">String</span></span>|<span data-ttu-id="7ff12-122">此资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="7ff12-122">The ID of this resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7ff12-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ff12-123">JSON representation</span></span>

<span data-ttu-id="7ff12-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ff12-124">The following is a JSON representation of the resource.</span></span>

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

