---
title: educationRubricOutcome 资源类型
description: 提供评分分数的 educationOutcome
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 10863f6ce1271f132ad23fb3e0c62a625e012058
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721024"
---
# <a name="educationrubricoutcome-resource-type"></a><span data-ttu-id="4d2ad-103">educationRubricOutcome 资源类型</span><span class="sxs-lookup"><span data-stu-id="4d2ad-103">educationRubricOutcome resource type</span></span>

<span data-ttu-id="4d2ad-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d2ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d2ad-105">提供[评分分数的 educationOutcome。](educationoutcome.md)</span><span class="sxs-lookup"><span data-stu-id="4d2ad-105">An [educationOutcome](educationoutcome.md) that provides a graded rubric.</span></span>

## <a name="methods"></a><span data-ttu-id="4d2ad-106">方法</span><span class="sxs-lookup"><span data-stu-id="4d2ad-106">Methods</span></span>

| <span data-ttu-id="4d2ad-107">方法</span><span class="sxs-lookup"><span data-stu-id="4d2ad-107">Method</span></span>       | <span data-ttu-id="4d2ad-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="4d2ad-108">Return Type</span></span> | <span data-ttu-id="4d2ad-109">说明</span><span class="sxs-lookup"><span data-stu-id="4d2ad-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4d2ad-110">更新 educationOutcome</span><span class="sxs-lookup"><span data-stu-id="4d2ad-110">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="4d2ad-111">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="4d2ad-111">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="4d2ad-112">更新 educationOutcome 对象。</span><span class="sxs-lookup"><span data-stu-id="4d2ad-112">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4d2ad-113">属性</span><span class="sxs-lookup"><span data-stu-id="4d2ad-113">Properties</span></span>

| <span data-ttu-id="4d2ad-114">属性</span><span class="sxs-lookup"><span data-stu-id="4d2ad-114">Property</span></span>     | <span data-ttu-id="4d2ad-115">类型</span><span class="sxs-lookup"><span data-stu-id="4d2ad-115">Type</span></span>        | <span data-ttu-id="4d2ad-116">说明</span><span class="sxs-lookup"><span data-stu-id="4d2ad-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4d2ad-117">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="4d2ad-117">lastModifiedBy</span></span>|[<span data-ttu-id="4d2ad-118">identitySet</span><span class="sxs-lookup"><span data-stu-id="4d2ad-118">identitySet</span></span>](identityset.md)|<span data-ttu-id="4d2ad-119">最后一个修改资源的用户。</span><span class="sxs-lookup"><span data-stu-id="4d2ad-119">The last user to modify the resource.</span></span>|
|<span data-ttu-id="4d2ad-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4d2ad-120">lastModifiedDateTime</span></span>|<span data-ttu-id="4d2ad-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d2ad-121">DateTimeOffset</span></span>|<span data-ttu-id="4d2ad-122">上次修改资源的时间。</span><span class="sxs-lookup"><span data-stu-id="4d2ad-122">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="4d2ad-123">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="4d2ad-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4d2ad-124">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="4d2ad-124">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="4d2ad-125">publishedRubricQualityFeedback</span><span class="sxs-lookup"><span data-stu-id="4d2ad-125">publishedRubricQualityFeedback</span></span>|<span data-ttu-id="4d2ad-126">[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4d2ad-126">[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md) collection</span></span>|<span data-ttu-id="4d2ad-127">在将成绩释放给学生时所创建 rubricQualityFeedback 属性的副本。</span><span class="sxs-lookup"><span data-stu-id="4d2ad-127">A copy of the rubricQualityFeedback property that is made when the grade is released to the student.</span></span>|
|<span data-ttu-id="4d2ad-128">publishedRubricQualitySelectedLevels</span><span class="sxs-lookup"><span data-stu-id="4d2ad-128">publishedRubricQualitySelectedLevels</span></span>|<span data-ttu-id="4d2ad-129">[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4d2ad-129">[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md) collection</span></span>|<span data-ttu-id="4d2ad-130">在将成绩释放给学生时所创建 rubricQualitySelectedLevels 属性的副本。</span><span class="sxs-lookup"><span data-stu-id="4d2ad-130">A copy of the rubricQualitySelectedLevels property that is made when the grade is released to the student.</span></span>|
|<span data-ttu-id="4d2ad-131">rubricQualityFeedback</span><span class="sxs-lookup"><span data-stu-id="4d2ad-131">rubricQualityFeedback</span></span>|<span data-ttu-id="4d2ad-132">[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4d2ad-132">[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md) collection</span></span>|<span data-ttu-id="4d2ad-133">此标准的每个质量的特定反馈的集合。</span><span class="sxs-lookup"><span data-stu-id="4d2ad-133">A collection of specific feedback for each quality of this rubric.</span></span>|
|<span data-ttu-id="4d2ad-134">rubricQualitySelectedLevels</span><span class="sxs-lookup"><span data-stu-id="4d2ad-134">rubricQualitySelectedLevels</span></span>|<span data-ttu-id="4d2ad-135">[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4d2ad-135">[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md) collection</span></span>|<span data-ttu-id="4d2ad-136">教师为此作业评分时针对每个质量选择的级别。</span><span class="sxs-lookup"><span data-stu-id="4d2ad-136">The level that the teacher has selected for each quality while grading this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d2ad-137">关系</span><span class="sxs-lookup"><span data-stu-id="4d2ad-137">Relationships</span></span>

<span data-ttu-id="4d2ad-138">无</span><span class="sxs-lookup"><span data-stu-id="4d2ad-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4d2ad-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4d2ad-139">JSON representation</span></span>

<span data-ttu-id="4d2ad-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4d2ad-140">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationRubricOutcome",
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

