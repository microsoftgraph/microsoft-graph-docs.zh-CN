---
title: educationRubricOutcome 资源类型
description: 提供评分的 rubric 的 educationOutcome
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4640daa1bb93945463cffc9dcf54d4db23b84da1
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173256"
---
# <a name="educationrubricoutcome-resource-type"></a><span data-ttu-id="cb9ba-103">educationRubricOutcome 资源类型</span><span class="sxs-lookup"><span data-stu-id="cb9ba-103">educationRubricOutcome resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb9ba-104">提供评分的 rubric 的[educationOutcome](educationoutcome.md) 。</span><span class="sxs-lookup"><span data-stu-id="cb9ba-104">An [educationOutcome](educationoutcome.md) that provides a graded rubric.</span></span>

## <a name="methods"></a><span data-ttu-id="cb9ba-105">方法</span><span class="sxs-lookup"><span data-stu-id="cb9ba-105">Methods</span></span>

| <span data-ttu-id="cb9ba-106">方法</span><span class="sxs-lookup"><span data-stu-id="cb9ba-106">Method</span></span>       | <span data-ttu-id="cb9ba-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="cb9ba-107">Return Type</span></span> | <span data-ttu-id="cb9ba-108">说明</span><span class="sxs-lookup"><span data-stu-id="cb9ba-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="cb9ba-109">更新 educationOutcome</span><span class="sxs-lookup"><span data-stu-id="cb9ba-109">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="cb9ba-110">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="cb9ba-110">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="cb9ba-111">更新 educationOutcome 对象。</span><span class="sxs-lookup"><span data-stu-id="cb9ba-111">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="cb9ba-112">属性</span><span class="sxs-lookup"><span data-stu-id="cb9ba-112">Properties</span></span>

| <span data-ttu-id="cb9ba-113">属性</span><span class="sxs-lookup"><span data-stu-id="cb9ba-113">Property</span></span>     | <span data-ttu-id="cb9ba-114">类型</span><span class="sxs-lookup"><span data-stu-id="cb9ba-114">Type</span></span>        | <span data-ttu-id="cb9ba-115">说明</span><span class="sxs-lookup"><span data-stu-id="cb9ba-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cb9ba-116">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="cb9ba-116">lastModifiedBy</span></span>|[<span data-ttu-id="cb9ba-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="cb9ba-117">identitySet</span></span>](identityset.md)|<span data-ttu-id="cb9ba-118">修改资源的最后一个用户。</span><span class="sxs-lookup"><span data-stu-id="cb9ba-118">The last user to modify the resource.</span></span>|
|<span data-ttu-id="cb9ba-119">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cb9ba-119">lastModifiedDateTime</span></span>|<span data-ttu-id="cb9ba-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb9ba-120">DateTimeOffset</span></span>|<span data-ttu-id="cb9ba-121">上次修改资源的时间点。</span><span class="sxs-lookup"><span data-stu-id="cb9ba-121">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="cb9ba-122">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="cb9ba-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="cb9ba-123">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="cb9ba-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="cb9ba-124">publishedRubricQualityFeedback</span><span class="sxs-lookup"><span data-stu-id="cb9ba-124">publishedRubricQualityFeedback</span></span>|<span data-ttu-id="cb9ba-125">[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md)集合</span><span class="sxs-lookup"><span data-stu-id="cb9ba-125">[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md) collection</span></span>|<span data-ttu-id="cb9ba-126">在向学生发布评分时所做的 rubricQualityFeedback 属性的副本。</span><span class="sxs-lookup"><span data-stu-id="cb9ba-126">A copy of the rubricQualityFeedback property that is made when the grade is released to the student.</span></span>|
|<span data-ttu-id="cb9ba-127">publishedRubricQualitySelectedLevels</span><span class="sxs-lookup"><span data-stu-id="cb9ba-127">publishedRubricQualitySelectedLevels</span></span>|<span data-ttu-id="cb9ba-128">[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md)集合</span><span class="sxs-lookup"><span data-stu-id="cb9ba-128">[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md) collection</span></span>|<span data-ttu-id="cb9ba-129">在向学生发布评分时所做的 rubricQualitySelectedLevels 属性的副本。</span><span class="sxs-lookup"><span data-stu-id="cb9ba-129">A copy of the rubricQualitySelectedLevels property that is made when the grade is released to the student.</span></span>|
|<span data-ttu-id="cb9ba-130">rubricQualityFeedback</span><span class="sxs-lookup"><span data-stu-id="cb9ba-130">rubricQualityFeedback</span></span>|<span data-ttu-id="cb9ba-131">[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md)集合</span><span class="sxs-lookup"><span data-stu-id="cb9ba-131">[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md) collection</span></span>|<span data-ttu-id="cb9ba-132">针对此 rubric 的每种质量的特定反馈的集合。</span><span class="sxs-lookup"><span data-stu-id="cb9ba-132">A collection of specific feedback for each quality of this rubric.</span></span>|
|<span data-ttu-id="cb9ba-133">rubricQualitySelectedLevels</span><span class="sxs-lookup"><span data-stu-id="cb9ba-133">rubricQualitySelectedLevels</span></span>|<span data-ttu-id="cb9ba-134">[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md)集合</span><span class="sxs-lookup"><span data-stu-id="cb9ba-134">[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md) collection</span></span>|<span data-ttu-id="cb9ba-135">为此工作分配评分的同时, 教师为每种质量选择的级别。</span><span class="sxs-lookup"><span data-stu-id="cb9ba-135">The level that the teacher has selected for each quality while grading this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb9ba-136">关系</span><span class="sxs-lookup"><span data-stu-id="cb9ba-136">Relationships</span></span>

<span data-ttu-id="cb9ba-137">无</span><span class="sxs-lookup"><span data-stu-id="cb9ba-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cb9ba-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cb9ba-138">JSON representation</span></span>

<span data-ttu-id="cb9ba-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cb9ba-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationRubricOutcome",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "publishedRubricQualityFeedback": [{"@odata.type": "microsoft.graph.rubricQualityFeedbackModel"}],
  "publishedRubricQualitySelectedLevels": [{"@odata.type": "microsoft.graph.rubricQualitySelectedColumnModel"}],
  "rubricQualityFeedback": [{"@odata.type": "microsoft.graph.rubricQualityFeedbackModel"}],
  "rubricQualitySelectedLevels": [{"@odata.type": "microsoft.graph.rubricQualitySelectedColumnModel"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRubricOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->