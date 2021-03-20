---
title: accessReviewInstance 资源类型
description: 表示 重复发生 `accessReviewScheduleDefinition` 。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: af2f3b0512ead453413a4fd65aa3337c7d9b2cd0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952821"
---
# <a name="accessreviewinstance-resource-type"></a><span data-ttu-id="d8577-103">accessReviewInstance 资源类型</span><span class="sxs-lookup"><span data-stu-id="d8577-103">accessReviewInstance resource type</span></span>

<span data-ttu-id="d8577-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8577-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="d8577-105">表示 Azure AD [访问评审](accessreviewsv2-root.md) 定期。</span><span class="sxs-lookup"><span data-stu-id="d8577-105">Represents an Azure AD [access review](accessreviewsv2-root.md) recurrence.</span></span> <span data-ttu-id="d8577-106">如果父 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 是定期访问评审，则实例表示每个重复周期。</span><span class="sxs-lookup"><span data-stu-id="d8577-106">If the parent [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) is a recurring access review, instances represent each recurrence.</span></span> <span data-ttu-id="d8577-107">不重复的审阅将只具有一个实例。</span><span class="sxs-lookup"><span data-stu-id="d8577-107">A review that does not recur will have exactly one instance.</span></span> <span data-ttu-id="d8577-108">实例还表示计划定义中正在审阅的每个唯一组。</span><span class="sxs-lookup"><span data-stu-id="d8577-108">Instances also represent each unique group being reviewed in the schedule definition.</span></span> <span data-ttu-id="d8577-109">如果计划定义审阅多个组，则每个组将具有每个重复周期的唯一实例。</span><span class="sxs-lookup"><span data-stu-id="d8577-109">If a schedule definition reviews multiple groups, each group will have a unique instance for each recurrence.</span></span>

<span data-ttu-id="d8577-110">每个 **accessReviewInstance** 都包含审阅 [](accessreviewinstancedecisionitem.md)者可以采取措施的决策列表。</span><span class="sxs-lookup"><span data-stu-id="d8577-110">Every **accessReviewInstance** contains a list of [decisions](accessreviewinstancedecisionitem.md) that reviewers can take action on.</span></span> <span data-ttu-id="d8577-111">每个正在审阅的身份有一个决策。</span><span class="sxs-lookup"><span data-stu-id="d8577-111">There is one decision per identity being reviewed.</span></span>

## <a name="methods"></a><span data-ttu-id="d8577-112">Methods</span><span class="sxs-lookup"><span data-stu-id="d8577-112">Methods</span></span>

| <span data-ttu-id="d8577-113">方法</span><span class="sxs-lookup"><span data-stu-id="d8577-113">Method</span></span> | <span data-ttu-id="d8577-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="d8577-114">Return Type</span></span> | <span data-ttu-id="d8577-115">说明</span><span class="sxs-lookup"><span data-stu-id="d8577-115">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="d8577-116">列出 accessReviewInstances</span><span class="sxs-lookup"><span data-stu-id="d8577-116">List accessReviewInstances</span></span>](../api/accessreviewinstance-list.md) | <span data-ttu-id="d8577-117">[accessReviewInstance](accessreviewinstance.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d8577-117">[accessReviewInstance](accessreviewinstance.md) collection</span></span> | <span data-ttu-id="d8577-118">获取 [accessReviewInstance](../resources/accessreviewinstance.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="d8577-118">Get a list of the [accessReviewInstance](../resources/accessreviewinstance.md) objects and their properties.</span></span> |
|[<span data-ttu-id="d8577-119">获取 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="d8577-119">Get accessReviewInstance</span></span>](../api/accessreviewinstance-get.md) | [<span data-ttu-id="d8577-120">accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="d8577-120">accessReviewInstance</span></span>](accessreviewinstance.md) | <span data-ttu-id="d8577-121">返回 accessReviewScheduleDefinition 的 accessReviewInstance。</span><span class="sxs-lookup"><span data-stu-id="d8577-121">Returns accessReviewInstance for an accessReviewScheduleDefinition.</span></span> <span data-ttu-id="d8577-122">对象中不包括关联的 accessReviewInstanceDecisionItem。</span><span class="sxs-lookup"><span data-stu-id="d8577-122">Does not include associated accessReviewInstanceDecisionItem\`s in the object.</span></span> |
|[<span data-ttu-id="d8577-123">列出 pendingAccessReviewInstances</span><span class="sxs-lookup"><span data-stu-id="d8577-123">List pendingAccessReviewInstances</span></span>](../api/accessreviewinstance-pendingaccessreviewinstances.md) | <span data-ttu-id="d8577-124">[accessReviewInstance](accessreviewinstance.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="d8577-124">[accessReviewInstance](accessreviewinstance.md) collection.</span></span> | <span data-ttu-id="d8577-125">获取分配给调用用户的所有待定 accessReviewInstance 资源。</span><span class="sxs-lookup"><span data-stu-id="d8577-125">Get all pending accessReviewInstance resources assigned to the calling user.</span></span> |
|[<span data-ttu-id="d8577-126">发送 accessReviewInstance 提醒</span><span class="sxs-lookup"><span data-stu-id="d8577-126">Send accessReviewInstance reminder</span></span>](../api/accessreviewinstance-sendreminder.md) | <span data-ttu-id="d8577-127">无。</span><span class="sxs-lookup"><span data-stu-id="d8577-127">None.</span></span> | <span data-ttu-id="d8577-128">向 accessReviewInstance 的审阅者发送提醒。</span><span class="sxs-lookup"><span data-stu-id="d8577-128">Send a reminder to the reviewers of an accessReviewInstance.</span></span> |
|[<span data-ttu-id="d8577-129">停止访问ReviewInstance</span><span class="sxs-lookup"><span data-stu-id="d8577-129">Stop accessReviewInstance</span></span>](../api/accessreviewinstance-stop.md) | <span data-ttu-id="d8577-130">无。</span><span class="sxs-lookup"><span data-stu-id="d8577-130">None.</span></span> | <span data-ttu-id="d8577-131">手动停止 accessReviewInstance。</span><span class="sxs-lookup"><span data-stu-id="d8577-131">Manually stop an accessReviewInstance.</span></span> |
|[<span data-ttu-id="d8577-132">接受建议</span><span class="sxs-lookup"><span data-stu-id="d8577-132">Accept recommendations</span></span>](../api/accessreviewinstance-acceptrecommendations.md) | <span data-ttu-id="d8577-133">无。</span><span class="sxs-lookup"><span data-stu-id="d8577-133">None.</span></span> | <span data-ttu-id="d8577-134">允许调用用户接受他们作为特定 accessReviewInstance 审阅者的每个 NotReviewed accessReviewInstanceDecisionItem 的决策建议。</span><span class="sxs-lookup"><span data-stu-id="d8577-134">Allows the calling user to accept the decision recommendation for each NotReviewed accessReviewInstanceDecisionItem that they are the reviewer on for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="d8577-135">应用决策</span><span class="sxs-lookup"><span data-stu-id="d8577-135">Apply decisions</span></span>](../api/accessreviewinstance-applydecisions.md) | <span data-ttu-id="d8577-136">无。</span><span class="sxs-lookup"><span data-stu-id="d8577-136">None.</span></span> | <span data-ttu-id="d8577-137">手动对 accessReviewInstance 应用决策。</span><span class="sxs-lookup"><span data-stu-id="d8577-137">Manually apply decision on an accessReviewInstance.</span></span> |



## <a name="properties"></a><span data-ttu-id="d8577-138">属性</span><span class="sxs-lookup"><span data-stu-id="d8577-138">Properties</span></span>
| <span data-ttu-id="d8577-139">属性</span><span class="sxs-lookup"><span data-stu-id="d8577-139">Property</span></span> | <span data-ttu-id="d8577-140">类型</span><span class="sxs-lookup"><span data-stu-id="d8577-140">Type</span></span> | <span data-ttu-id="d8577-141">说明</span><span class="sxs-lookup"><span data-stu-id="d8577-141">Description</span></span> |
| :-------------------------| :---------------------------------- | :---------- |
| <span data-ttu-id="d8577-142">id</span><span class="sxs-lookup"><span data-stu-id="d8577-142">id</span></span> | <span data-ttu-id="d8577-143">String</span><span class="sxs-lookup"><span data-stu-id="d8577-143">String</span></span> | <span data-ttu-id="d8577-144">实例的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d8577-144">Unique identifier of the instance.</span></span> |
| <span data-ttu-id="d8577-145">displayName</span><span class="sxs-lookup"><span data-stu-id="d8577-145">displayName</span></span> | <span data-ttu-id="d8577-146">String</span><span class="sxs-lookup"><span data-stu-id="d8577-146">String</span></span> | <span data-ttu-id="d8577-147">父 [accessReviewScheduleDefinition 的名称](accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="d8577-147">Name of the parent [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> |
| <span data-ttu-id="d8577-148">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d8577-148">startDateTime</span></span> | <span data-ttu-id="d8577-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8577-149">DateTimeOffset</span></span> | <span data-ttu-id="d8577-150">计划启动审阅实例的 DateTime。</span><span class="sxs-lookup"><span data-stu-id="d8577-150">DateTime when review instance is scheduled to start.</span></span> <span data-ttu-id="d8577-151">可能在将来。</span><span class="sxs-lookup"><span data-stu-id="d8577-151">May be in the future.</span></span> <span data-ttu-id="d8577-152">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="d8577-152">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d8577-153">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="d8577-153">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="d8577-154">endDateTime</span><span class="sxs-lookup"><span data-stu-id="d8577-154">endDateTime</span></span> | <span data-ttu-id="d8577-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8577-155">DateTimeOffset</span></span> | <span data-ttu-id="d8577-156">将审阅实例计划结束的 DateTime。DatetimeOffset 类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="d8577-156">DateTime when review instance is scheduled to end.The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d8577-157">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="d8577-157">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="d8577-158">状态</span><span class="sxs-lookup"><span data-stu-id="d8577-158">status</span></span> | <span data-ttu-id="d8577-159">String</span><span class="sxs-lookup"><span data-stu-id="d8577-159">String</span></span> | <span data-ttu-id="d8577-160">指定 accessReview 的状态。</span><span class="sxs-lookup"><span data-stu-id="d8577-160">Specifies the status of an accessReview.</span></span> <span data-ttu-id="d8577-161">典型状态包括 `Initializing` `NotStarted` `Starting` `InProgress` 、、、、、、 `Completing` `Completed` `AutoReviewing` 和 `AutoReviewed` 。</span><span class="sxs-lookup"><span data-stu-id="d8577-161">The typical states include `Initializing`, `NotStarted`, `Starting`, `InProgress`, `Completing`, `Completed`, `AutoReviewing`, and `AutoReviewed`.</span></span>  <span data-ttu-id="d8577-162">只读。</span><span class="sxs-lookup"><span data-stu-id="d8577-162">Read-only.</span></span>|
| <span data-ttu-id="d8577-163">scope</span><span class="sxs-lookup"><span data-stu-id="d8577-163">scope</span></span> | [<span data-ttu-id="d8577-164">accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="d8577-164">accessReviewScope</span></span>](accessreviewscope.md) | <span data-ttu-id="d8577-165">基于级别的 **scope 和** **instanceEnumerationScope** `accessReviewScheduleDefinition` 创建。</span><span class="sxs-lookup"><span data-stu-id="d8577-165">Created based on **scope** and **instanceEnumerationScope** at the `accessReviewScheduleDefinition` level.</span></span> <span data-ttu-id="d8577-166">定义在组中查看的用户范围。</span><span class="sxs-lookup"><span data-stu-id="d8577-166">Defines the scope of users reviewed in a group.</span></span> <span data-ttu-id="d8577-167">对于单组评审，在级别定义的范围 `accessReviewScheduleDefinition` 适用于所有实例。</span><span class="sxs-lookup"><span data-stu-id="d8577-167">In the case of a single-group review, the scope defined at the `accessReviewScheduleDefinition` level applies to all instances.</span></span> <span data-ttu-id="d8577-168">在查看所有组的情况下，每个组的范围可能不同。</span><span class="sxs-lookup"><span data-stu-id="d8577-168">In the case of all groups review, scope may be different for each group.</span></span> <span data-ttu-id="d8577-169">只读。</span><span class="sxs-lookup"><span data-stu-id="d8577-169">Read-only.</span></span>  | 
| <span data-ttu-id="d8577-170">决策</span><span class="sxs-lookup"><span data-stu-id="d8577-170">decisions</span></span> | <span data-ttu-id="d8577-171">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d8577-171">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span></span> | <span data-ttu-id="d8577-172">在 [accessReviewInstance](#accessreviewinstance-resource-type) 中查看的每个用户都有一个决定项，该项目表示其访问是经过批准、拒绝还是尚未被审阅。</span><span class="sxs-lookup"><span data-stu-id="d8577-172">Each user reviewed in an [accessReviewInstance](#accessreviewinstance-resource-type) has a decision item representing if their access was approved, denied, or not yet reviewed.</span></span> |
| <span data-ttu-id="d8577-173">definition</span><span class="sxs-lookup"><span data-stu-id="d8577-173">definition</span></span> |[<span data-ttu-id="d8577-174">accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="d8577-174">accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition.md) | <span data-ttu-id="d8577-175">每个实例只关联一 **个 accessReviewScheduleDefinition。**</span><span class="sxs-lookup"><span data-stu-id="d8577-175">There is exactly one **accessReviewScheduleDefinition** associated with each instance.</span></span> <span data-ttu-id="d8577-176">它是实例的父计划，其中为审阅定义的每个重复周期创建实例，并按定义选择查看每个组。</span><span class="sxs-lookup"><span data-stu-id="d8577-176">It is the parent schedule for the instance, where instances are created for each recurrence of a review definition and each group selected to review by the definition.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d8577-177">关系</span><span class="sxs-lookup"><span data-stu-id="d8577-177">Relationships</span></span>

| <span data-ttu-id="d8577-178">关系</span><span class="sxs-lookup"><span data-stu-id="d8577-178">Relationship</span></span> | <span data-ttu-id="d8577-179">类型</span><span class="sxs-lookup"><span data-stu-id="d8577-179">Type</span></span>   |<span data-ttu-id="d8577-180">说明</span><span class="sxs-lookup"><span data-stu-id="d8577-180">Description</span></span>|
|:---------------|:--------|:----------|
| `definition`               |[<span data-ttu-id="d8577-181">accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="d8577-181">accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition.md)          | <span data-ttu-id="d8577-182">每个实例只 `accessReviewScheduleDefinition` 关联一个。</span><span class="sxs-lookup"><span data-stu-id="d8577-182">There is exactly one `accessReviewScheduleDefinition` associated with each instance.</span></span> <span data-ttu-id="d8577-183">它是实例的父计划，其中为审阅定义的每个重复周期创建实例，并按定义选择查看每个组。</span><span class="sxs-lookup"><span data-stu-id="d8577-183">It is the parent schedule for the instance, where instances are created for each recurrence of a review definition and each group selected to review by the definition.</span></span> |
| `decisions`               |<span data-ttu-id="d8577-184">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d8577-184">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span></span>        | <span data-ttu-id="d8577-185">在 中审阅的 `accessReviewInstance` 每个用户都有一个决策项，代表他们被批准、拒绝还是尚未被审阅。</span><span class="sxs-lookup"><span data-stu-id="d8577-185">Each user reviewed in an `accessReviewInstance` has a decision item representing if they were approved, denied, or not yet reviewed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d8577-186">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d8577-186">JSON representation</span></span>

<span data-ttu-id="d8577-187">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8577-187">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewInstance",
  "openType": false
}
-->

```json
{
 "@odata.type": "#microsoft.graph.accessReviewInstance",
 "id": "string (identifier)",
 "displayName": "string",
 "startDateTime": "string (timestamp)",
 "endDateTime": "string (timestamp)",
 "status": "string",
 "scope": {
    "@odata.type": "microsoft.graph.accessReviewScope"
  }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewInstance resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
