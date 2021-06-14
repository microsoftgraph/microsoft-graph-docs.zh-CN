---
title: educationRubric 资源类型
description: 可附加到工作分配的评分标准。
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f70fded2c35576d31f3c5b17edf0342d97a88302
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912325"
---
# <a name="educationrubric-resource-type"></a><span data-ttu-id="b8dd2-103">educationRubric 资源类型</span><span class="sxs-lookup"><span data-stu-id="b8dd2-103">educationRubric resource type</span></span>

<span data-ttu-id="b8dd2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8dd2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b8dd2-105">可附加到工作分配的评分标准。</span><span class="sxs-lookup"><span data-stu-id="b8dd2-105">A grading rubric that can be attached to an assignment.</span></span> <span data-ttu-id="b8dd2-106">一个分卡与 **educationUser** (教师) ，并附加到一个或多个 **education分配** 资源。</span><span class="sxs-lookup"><span data-stu-id="b8dd2-106">A rubric is associated with an **educationUser** (teacher), and attached to one or more **educationAssignment** resources.</span></span> 

<span data-ttu-id="b8dd2-107">有关详细信息 [，请参阅教育](/graph/education-rubric-overview) 程度概述。</span><span class="sxs-lookup"><span data-stu-id="b8dd2-107">See [Education rubric overview](/graph/education-rubric-overview) for more information.</span></span>

## <a name="methods"></a><span data-ttu-id="b8dd2-108">方法</span><span class="sxs-lookup"><span data-stu-id="b8dd2-108">Methods</span></span>

| <span data-ttu-id="b8dd2-109">方法</span><span class="sxs-lookup"><span data-stu-id="b8dd2-109">Method</span></span>       | <span data-ttu-id="b8dd2-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="b8dd2-110">Return Type</span></span> | <span data-ttu-id="b8dd2-111">说明</span><span class="sxs-lookup"><span data-stu-id="b8dd2-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b8dd2-112">创建 educationRubric</span><span class="sxs-lookup"><span data-stu-id="b8dd2-112">Create educationRubric</span></span>](../api/educationuser-post-rubrics.md) | [<span data-ttu-id="b8dd2-113">educationRubric</span><span class="sxs-lookup"><span data-stu-id="b8dd2-113">educationRubric</span></span>](educationrubric.md) | <span data-ttu-id="b8dd2-114">创建新的 educationRubric 对象。</span><span class="sxs-lookup"><span data-stu-id="b8dd2-114">Create a new educationRubric object.</span></span> |
| [<span data-ttu-id="b8dd2-115">获取 educationRubric</span><span class="sxs-lookup"><span data-stu-id="b8dd2-115">Get educationRubric</span></span>](../api/educationrubric-get.md) | [<span data-ttu-id="b8dd2-116">educationRubric</span><span class="sxs-lookup"><span data-stu-id="b8dd2-116">educationRubric</span></span>](educationrubric.md) | <span data-ttu-id="b8dd2-117">读取 educationRubric 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b8dd2-117">Read properties and relationships of educationRubric object.</span></span> |
| [<span data-ttu-id="b8dd2-118">更新 educationRubric</span><span class="sxs-lookup"><span data-stu-id="b8dd2-118">Update educationRubric</span></span>](../api/educationrubric-update.md) | [<span data-ttu-id="b8dd2-119">educationRubric</span><span class="sxs-lookup"><span data-stu-id="b8dd2-119">educationRubric</span></span>](educationrubric.md) | <span data-ttu-id="b8dd2-120">更新 educationRubric 对象。</span><span class="sxs-lookup"><span data-stu-id="b8dd2-120">Update educationRubric object.</span></span> |
| [<span data-ttu-id="b8dd2-121">删除 educationRubric</span><span class="sxs-lookup"><span data-stu-id="b8dd2-121">Delete educationRubric</span></span>](../api/educationrubric-delete.md) | <span data-ttu-id="b8dd2-122">无</span><span class="sxs-lookup"><span data-stu-id="b8dd2-122">None</span></span> | <span data-ttu-id="b8dd2-123">删除 educationRubric 对象。</span><span class="sxs-lookup"><span data-stu-id="b8dd2-123">Delete educationRubric object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b8dd2-124">属性</span><span class="sxs-lookup"><span data-stu-id="b8dd2-124">Properties</span></span>

| <span data-ttu-id="b8dd2-125">属性</span><span class="sxs-lookup"><span data-stu-id="b8dd2-125">Property</span></span>     | <span data-ttu-id="b8dd2-126">类型</span><span class="sxs-lookup"><span data-stu-id="b8dd2-126">Type</span></span>        | <span data-ttu-id="b8dd2-127">说明</span><span class="sxs-lookup"><span data-stu-id="b8dd2-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b8dd2-128">createdBy</span><span class="sxs-lookup"><span data-stu-id="b8dd2-128">createdBy</span></span>|[<span data-ttu-id="b8dd2-129">identitySet</span><span class="sxs-lookup"><span data-stu-id="b8dd2-129">identitySet</span></span>](identityset.md)|<span data-ttu-id="b8dd2-130">创建此资源的用户。</span><span class="sxs-lookup"><span data-stu-id="b8dd2-130">The user who created this resource.</span></span>|
|<span data-ttu-id="b8dd2-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b8dd2-131">createdDateTime</span></span>|<span data-ttu-id="b8dd2-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8dd2-132">DateTimeOffset</span></span>|<span data-ttu-id="b8dd2-133">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="b8dd2-133">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b8dd2-134">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="b8dd2-134">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="b8dd2-135">说明</span><span class="sxs-lookup"><span data-stu-id="b8dd2-135">description</span></span>|[<span data-ttu-id="b8dd2-136">itemBody</span><span class="sxs-lookup"><span data-stu-id="b8dd2-136">itemBody</span></span>](itembody.md)|<span data-ttu-id="b8dd2-137">此分卡的说明。</span><span class="sxs-lookup"><span data-stu-id="b8dd2-137">The description of this rubric.</span></span>|
|<span data-ttu-id="b8dd2-138">displayName</span><span class="sxs-lookup"><span data-stu-id="b8dd2-138">displayName</span></span>|<span data-ttu-id="b8dd2-139">String</span><span class="sxs-lookup"><span data-stu-id="b8dd2-139">String</span></span>|<span data-ttu-id="b8dd2-140">此分号的名称。</span><span class="sxs-lookup"><span data-stu-id="b8dd2-140">The name of this rubric.</span></span>|
|<span data-ttu-id="b8dd2-141">一个</span><span class="sxs-lookup"><span data-stu-id="b8dd2-141">grading</span></span>|[<span data-ttu-id="b8dd2-142">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="b8dd2-142">educationAssignmentGradeType</span></span>](educationassignmentgradetype.md)|<span data-ttu-id="b8dd2-143">此评分标准评分类型 -- 无评分标准为 [null，educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) 为评分标准。</span><span class="sxs-lookup"><span data-stu-id="b8dd2-143">The grading type of this rubric -- null for a no-points rubric, or [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) for a points rubric.</span></span>|
|<span data-ttu-id="b8dd2-144">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="b8dd2-144">lastModifiedBy</span></span>|[<span data-ttu-id="b8dd2-145">identitySet</span><span class="sxs-lookup"><span data-stu-id="b8dd2-145">identitySet</span></span>](identityset.md)|<span data-ttu-id="b8dd2-146">最后一个修改资源的用户。</span><span class="sxs-lookup"><span data-stu-id="b8dd2-146">The last user to modify the resource.</span></span>|
|<span data-ttu-id="b8dd2-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8dd2-147">lastModifiedDateTime</span></span>|<span data-ttu-id="b8dd2-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8dd2-148">DateTimeOffset</span></span>|<span data-ttu-id="b8dd2-149">上次修改资源的时间。</span><span class="sxs-lookup"><span data-stu-id="b8dd2-149">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="b8dd2-150">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="b8dd2-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b8dd2-151">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="b8dd2-151">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="b8dd2-152">levels</span><span class="sxs-lookup"><span data-stu-id="b8dd2-152">levels</span></span>|<span data-ttu-id="b8dd2-153">[rubricLevel](rubriclevel.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b8dd2-153">[rubricLevel](rubriclevel.md) collection</span></span>|<span data-ttu-id="b8dd2-154">此标准中的级别集合。</span><span class="sxs-lookup"><span data-stu-id="b8dd2-154">The collection of levels making up this rubric.</span></span>|
|<span data-ttu-id="b8dd2-155">一些</span><span class="sxs-lookup"><span data-stu-id="b8dd2-155">qualities</span></span>|<span data-ttu-id="b8dd2-156">[rubricQuality](rubricquality.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b8dd2-156">[rubricQuality](rubricquality.md) collection</span></span>|<span data-ttu-id="b8dd2-157">此分项由质量集合决定。</span><span class="sxs-lookup"><span data-stu-id="b8dd2-157">The collection of qualities making up this rubric.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8dd2-158">关系</span><span class="sxs-lookup"><span data-stu-id="b8dd2-158">Relationships</span></span>

<span data-ttu-id="b8dd2-159">无</span><span class="sxs-lookup"><span data-stu-id="b8dd2-159">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8dd2-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b8dd2-160">JSON representation</span></span>

<span data-ttu-id="b8dd2-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8dd2-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationRubric",
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