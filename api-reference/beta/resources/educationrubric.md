---
title: educationRubric 资源类型
description: 可附加到工作分配的评分 rubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b43b611465af4dabb62d9dd741eb9a8670f241b9
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173235"
---
# <a name="educationrubric-resource-type"></a><span data-ttu-id="1b055-103">educationRubric 资源类型</span><span class="sxs-lookup"><span data-stu-id="1b055-103">educationRubric resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b055-104">可附加到工作分配的评分 rubric。</span><span class="sxs-lookup"><span data-stu-id="1b055-104">A grading rubric that can be attached to an assignment.</span></span> <span data-ttu-id="1b055-105">Rubric 与**educationUser** (教师) 相关联, 并附加到一个或多个**educationAssignment**资源。</span><span class="sxs-lookup"><span data-stu-id="1b055-105">A rubric is associated with an **educationUser** (teacher), and attached to one or more **educationAssignment** resources.</span></span> 

<span data-ttu-id="1b055-106">有关详细信息, 请参阅[教育版 rubric 概述](https://developer.microsoft.com/graph/docs/concepts/education-rubric-overview)。</span><span class="sxs-lookup"><span data-stu-id="1b055-106">See [Education rubric overview](https://developer.microsoft.com/graph/docs/concepts/education-rubric-overview) for more information.</span></span>

## <a name="methods"></a><span data-ttu-id="1b055-107">方法</span><span class="sxs-lookup"><span data-stu-id="1b055-107">Methods</span></span>

| <span data-ttu-id="1b055-108">方法</span><span class="sxs-lookup"><span data-stu-id="1b055-108">Method</span></span>       | <span data-ttu-id="1b055-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="1b055-109">Return Type</span></span> | <span data-ttu-id="1b055-110">说明</span><span class="sxs-lookup"><span data-stu-id="1b055-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1b055-111">获取 educationRubric</span><span class="sxs-lookup"><span data-stu-id="1b055-111">Get educationRubric</span></span>](../api/educationrubric-get.md) | [<span data-ttu-id="1b055-112">educationRubric</span><span class="sxs-lookup"><span data-stu-id="1b055-112">educationRubric</span></span>](educationrubric.md) | <span data-ttu-id="1b055-113">读取 educationRubric 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1b055-113">Read properties and relationships of educationRubric object.</span></span> |
| [<span data-ttu-id="1b055-114">更新 educationRubric</span><span class="sxs-lookup"><span data-stu-id="1b055-114">Update educationRubric</span></span>](../api/educationrubric-update.md) | [<span data-ttu-id="1b055-115">educationRubric</span><span class="sxs-lookup"><span data-stu-id="1b055-115">educationRubric</span></span>](educationrubric.md) | <span data-ttu-id="1b055-116">更新 educationRubric 对象。</span><span class="sxs-lookup"><span data-stu-id="1b055-116">Update educationRubric object.</span></span> |
| [<span data-ttu-id="1b055-117">删除 educationRubric</span><span class="sxs-lookup"><span data-stu-id="1b055-117">Delete educationRubric</span></span>](../api/educationrubric-delete.md) | <span data-ttu-id="1b055-118">无</span><span class="sxs-lookup"><span data-stu-id="1b055-118">None</span></span> | <span data-ttu-id="1b055-119">删除 educationRubric 对象。</span><span class="sxs-lookup"><span data-stu-id="1b055-119">Delete educationRubric object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1b055-120">属性</span><span class="sxs-lookup"><span data-stu-id="1b055-120">Properties</span></span>

| <span data-ttu-id="1b055-121">属性</span><span class="sxs-lookup"><span data-stu-id="1b055-121">Property</span></span>     | <span data-ttu-id="1b055-122">类型</span><span class="sxs-lookup"><span data-stu-id="1b055-122">Type</span></span>        | <span data-ttu-id="1b055-123">说明</span><span class="sxs-lookup"><span data-stu-id="1b055-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1b055-124">createdBy</span><span class="sxs-lookup"><span data-stu-id="1b055-124">createdBy</span></span>|[<span data-ttu-id="1b055-125">identitySet</span><span class="sxs-lookup"><span data-stu-id="1b055-125">identitySet</span></span>](identityset.md)|<span data-ttu-id="1b055-126">创建此资源的用户。</span><span class="sxs-lookup"><span data-stu-id="1b055-126">The user who created this resource.</span></span>|
|<span data-ttu-id="1b055-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1b055-127">createdDateTime</span></span>|<span data-ttu-id="1b055-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b055-128">DateTimeOffset</span></span>|<span data-ttu-id="1b055-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="1b055-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="1b055-131">说明</span><span class="sxs-lookup"><span data-stu-id="1b055-131">description</span></span>|[<span data-ttu-id="1b055-132">itemBody</span><span class="sxs-lookup"><span data-stu-id="1b055-132">itemBody</span></span>](itembody.md)|<span data-ttu-id="1b055-133">此 rubric 的说明。</span><span class="sxs-lookup"><span data-stu-id="1b055-133">The description of this rubric.</span></span>|
|<span data-ttu-id="1b055-134">displayName</span><span class="sxs-lookup"><span data-stu-id="1b055-134">displayName</span></span>|<span data-ttu-id="1b055-135">String</span><span class="sxs-lookup"><span data-stu-id="1b055-135">String</span></span>|<span data-ttu-id="1b055-136">此 rubric 的名称。</span><span class="sxs-lookup"><span data-stu-id="1b055-136">The name of this rubric.</span></span>|
|<span data-ttu-id="1b055-137">评分</span><span class="sxs-lookup"><span data-stu-id="1b055-137">grading</span></span>|[<span data-ttu-id="1b055-138">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="1b055-138">educationAssignmentGradeType</span></span>](educationassignmentgradetype.md)|<span data-ttu-id="1b055-139">此 rubric 的评分类型--null 表示无点 rubric, 或[educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md)为点 rubric。</span><span class="sxs-lookup"><span data-stu-id="1b055-139">The grading type of this rubric -- null for a no-points rubric, or [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) for a points rubric.</span></span>|
|<span data-ttu-id="1b055-140">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="1b055-140">lastModifiedBy</span></span>|[<span data-ttu-id="1b055-141">identitySet</span><span class="sxs-lookup"><span data-stu-id="1b055-141">identitySet</span></span>](identityset.md)|<span data-ttu-id="1b055-142">修改资源的最后一个用户。</span><span class="sxs-lookup"><span data-stu-id="1b055-142">The last user to modify the resource.</span></span>|
|<span data-ttu-id="1b055-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b055-143">lastModifiedDateTime</span></span>|<span data-ttu-id="1b055-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b055-144">DateTimeOffset</span></span>|<span data-ttu-id="1b055-145">上次修改资源的时间点。</span><span class="sxs-lookup"><span data-stu-id="1b055-145">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="1b055-146">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="1b055-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1b055-147">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="1b055-147">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="1b055-148">等级</span><span class="sxs-lookup"><span data-stu-id="1b055-148">levels</span></span>|<span data-ttu-id="1b055-149">[rubricLevel](rubriclevel.md)集合</span><span class="sxs-lookup"><span data-stu-id="1b055-149">[rubricLevel](rubriclevel.md) collection</span></span>|<span data-ttu-id="1b055-150">构成此 rubric 的级别的集合。</span><span class="sxs-lookup"><span data-stu-id="1b055-150">The collection of levels making up this rubric.</span></span>|
|<span data-ttu-id="1b055-151">特质</span><span class="sxs-lookup"><span data-stu-id="1b055-151">qualities</span></span>|<span data-ttu-id="1b055-152">[rubricQuality](rubricquality.md)集合</span><span class="sxs-lookup"><span data-stu-id="1b055-152">[rubricQuality](rubricquality.md) collection</span></span>|<span data-ttu-id="1b055-153">构成此 rubric 的质量的集合。</span><span class="sxs-lookup"><span data-stu-id="1b055-153">The collection of qualities making up this rubric.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b055-154">关系</span><span class="sxs-lookup"><span data-stu-id="1b055-154">Relationships</span></span>

<span data-ttu-id="1b055-155">无</span><span class="sxs-lookup"><span data-stu-id="1b055-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1b055-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1b055-156">JSON representation</span></span>

<span data-ttu-id="1b055-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b055-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationRubric",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "description": {"@odata.type": "microsoft.graph.itemBody"},
  "displayName": "String",
  "grading": {"@odata.type": "microsoft.graph.educationAssignmentGradeType"},
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "levels": [{"@odata.type": "microsoft.graph.rubricLevel"}],
  "qualities": [{"@odata.type": "microsoft.graph.rubricQuality"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRubric resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->