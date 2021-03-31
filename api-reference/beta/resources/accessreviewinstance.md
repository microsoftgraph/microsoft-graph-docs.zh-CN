---
title: accessReviewInstance 资源类型
description: 表示 重复发生 `accessReviewScheduleDefinition` 。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8ef2e48900484c32669a56c15b88de87dc4710d3
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469051"
---
# <a name="accessreviewinstance-resource-type"></a><span data-ttu-id="31ae4-103">accessReviewInstance 资源类型</span><span class="sxs-lookup"><span data-stu-id="31ae4-103">accessReviewInstance resource type</span></span>

<span data-ttu-id="31ae4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31ae4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="31ae4-105">表示 Azure AD [访问评审](accessreviewsv2-root.md) 定期。</span><span class="sxs-lookup"><span data-stu-id="31ae4-105">Represents an Azure AD [access review](accessreviewsv2-root.md) recurrence.</span></span> <span data-ttu-id="31ae4-106">如果父 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 是定期访问评审，则实例表示每个重复周期。</span><span class="sxs-lookup"><span data-stu-id="31ae4-106">If the parent [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) is a recurring access review, instances represent each recurrence.</span></span> <span data-ttu-id="31ae4-107">不重复的审阅将只具有一个实例。</span><span class="sxs-lookup"><span data-stu-id="31ae4-107">A review that does not recur will have exactly one instance.</span></span> <span data-ttu-id="31ae4-108">实例还表示计划定义中正在审阅的每个唯一组。</span><span class="sxs-lookup"><span data-stu-id="31ae4-108">Instances also represent each unique group being reviewed in the schedule definition.</span></span> <span data-ttu-id="31ae4-109">如果计划定义审阅多个组，则每个组将具有每个重复周期的唯一实例。</span><span class="sxs-lookup"><span data-stu-id="31ae4-109">If a schedule definition reviews multiple groups, each group will have a unique instance for each recurrence.</span></span>

<span data-ttu-id="31ae4-110">每个 **accessReviewInstance** 都包含审阅 [](accessreviewinstancedecisionitem.md)者可以采取措施的决策列表。</span><span class="sxs-lookup"><span data-stu-id="31ae4-110">Every **accessReviewInstance** contains a list of [decisions](accessreviewinstancedecisionitem.md) that reviewers can take action on.</span></span> <span data-ttu-id="31ae4-111">每个正在审阅的身份有一个决策。</span><span class="sxs-lookup"><span data-stu-id="31ae4-111">There is one decision per identity being reviewed.</span></span>

## <a name="methods"></a><span data-ttu-id="31ae4-112">方法</span><span class="sxs-lookup"><span data-stu-id="31ae4-112">Methods</span></span>

| <span data-ttu-id="31ae4-113">方法</span><span class="sxs-lookup"><span data-stu-id="31ae4-113">Method</span></span> | <span data-ttu-id="31ae4-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="31ae4-114">Return Type</span></span> | <span data-ttu-id="31ae4-115">说明</span><span class="sxs-lookup"><span data-stu-id="31ae4-115">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="31ae4-116">列出 accessReviewInstances</span><span class="sxs-lookup"><span data-stu-id="31ae4-116">List accessReviewInstances</span></span>](../api/accessreviewinstance-list.md) | <span data-ttu-id="31ae4-117">[accessReviewInstance](accessreviewinstance.md) 集合</span><span class="sxs-lookup"><span data-stu-id="31ae4-117">[accessReviewInstance](accessreviewinstance.md) collection</span></span> | <span data-ttu-id="31ae4-118">获取 [accessReviewInstance](../resources/accessreviewinstance.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="31ae4-118">Get a list of the [accessReviewInstance](../resources/accessreviewinstance.md) objects and their properties.</span></span> |
|[<span data-ttu-id="31ae4-119">获取 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="31ae4-119">Get accessReviewInstance</span></span>](../api/accessreviewinstance-get.md) | [<span data-ttu-id="31ae4-120">accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="31ae4-120">accessReviewInstance</span></span>](accessreviewinstance.md) | <span data-ttu-id="31ae4-121">返回 accessReviewScheduleDefinition 的 accessReviewInstance。</span><span class="sxs-lookup"><span data-stu-id="31ae4-121">Returns accessReviewInstance for an accessReviewScheduleDefinition.</span></span> <span data-ttu-id="31ae4-122">对象中不包括关联的 accessReviewInstanceDecisionItem。</span><span class="sxs-lookup"><span data-stu-id="31ae4-122">Does not include associated accessReviewInstanceDecisionItem\`s in the object.</span></span> |
|[<span data-ttu-id="31ae4-123">列出 pendingAccessReviewInstances</span><span class="sxs-lookup"><span data-stu-id="31ae4-123">List pendingAccessReviewInstances</span></span>](../api/accessreviewinstance-pendingaccessreviewinstances.md) | <span data-ttu-id="31ae4-124">[accessReviewInstance](accessreviewinstance.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="31ae4-124">[accessReviewInstance](accessreviewinstance.md) collection.</span></span> | <span data-ttu-id="31ae4-125">获取分配给调用用户的所有待定 accessReviewInstance 资源。</span><span class="sxs-lookup"><span data-stu-id="31ae4-125">Get all pending accessReviewInstance resources assigned to the calling user.</span></span> |
|[<span data-ttu-id="31ae4-126">发送 accessReviewInstance 提醒</span><span class="sxs-lookup"><span data-stu-id="31ae4-126">Send accessReviewInstance reminder</span></span>](../api/accessreviewinstance-sendreminder.md) | <span data-ttu-id="31ae4-127">无。</span><span class="sxs-lookup"><span data-stu-id="31ae4-127">None.</span></span> | <span data-ttu-id="31ae4-128">向 accessReviewInstance 的审阅者发送提醒。</span><span class="sxs-lookup"><span data-stu-id="31ae4-128">Send a reminder to the reviewers of an accessReviewInstance.</span></span> |
|[<span data-ttu-id="31ae4-129">停止访问ReviewInstance</span><span class="sxs-lookup"><span data-stu-id="31ae4-129">Stop accessReviewInstance</span></span>](../api/accessreviewinstance-stop.md) | <span data-ttu-id="31ae4-130">无。</span><span class="sxs-lookup"><span data-stu-id="31ae4-130">None.</span></span> | <span data-ttu-id="31ae4-131">手动停止 accessReviewInstance。</span><span class="sxs-lookup"><span data-stu-id="31ae4-131">Manually stop an accessReviewInstance.</span></span> |
|[<span data-ttu-id="31ae4-132">接受建议</span><span class="sxs-lookup"><span data-stu-id="31ae4-132">Accept recommendations</span></span>](../api/accessreviewinstance-acceptrecommendations.md) | <span data-ttu-id="31ae4-133">无。</span><span class="sxs-lookup"><span data-stu-id="31ae4-133">None.</span></span> | <span data-ttu-id="31ae4-134">允许调用用户接受他们作为特定 accessReviewInstance 审阅者的每个 NotReviewed accessReviewInstanceDecisionItem 的决策建议。</span><span class="sxs-lookup"><span data-stu-id="31ae4-134">Allows the calling user to accept the decision recommendation for each NotReviewed accessReviewInstanceDecisionItem that they are the reviewer on for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="31ae4-135">应用决策</span><span class="sxs-lookup"><span data-stu-id="31ae4-135">Apply decisions</span></span>](../api/accessreviewinstance-applydecisions.md) | <span data-ttu-id="31ae4-136">无。</span><span class="sxs-lookup"><span data-stu-id="31ae4-136">None.</span></span> | <span data-ttu-id="31ae4-137">手动对 accessReviewInstance 应用决策。</span><span class="sxs-lookup"><span data-stu-id="31ae4-137">Manually apply decision on an accessReviewInstance.</span></span> |
|[<span data-ttu-id="31ae4-138">批处理记录决策</span><span class="sxs-lookup"><span data-stu-id="31ae4-138">Batch record decisions</span></span>](../api/accessreviewinstance-batchrecorddecisions.md)|<span data-ttu-id="31ae4-139">无</span><span class="sxs-lookup"><span data-stu-id="31ae4-139">None</span></span>|<span data-ttu-id="31ae4-140">在一次调用中查看主体或资源的批次。</span><span class="sxs-lookup"><span data-stu-id="31ae4-140">Review batches of principals or resources in one call.</span></span>|

## <a name="properties"></a><span data-ttu-id="31ae4-141">属性</span><span class="sxs-lookup"><span data-stu-id="31ae4-141">Properties</span></span>
| <span data-ttu-id="31ae4-142">属性</span><span class="sxs-lookup"><span data-stu-id="31ae4-142">Property</span></span> | <span data-ttu-id="31ae4-143">类型</span><span class="sxs-lookup"><span data-stu-id="31ae4-143">Type</span></span> | <span data-ttu-id="31ae4-144">说明</span><span class="sxs-lookup"><span data-stu-id="31ae4-144">Description</span></span> |
| :-------------------------| :---------------------------------- | :---------- |
| <span data-ttu-id="31ae4-145">id</span><span class="sxs-lookup"><span data-stu-id="31ae4-145">id</span></span> | <span data-ttu-id="31ae4-146">String</span><span class="sxs-lookup"><span data-stu-id="31ae4-146">String</span></span> | <span data-ttu-id="31ae4-147">实例的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="31ae4-147">Unique identifier of the instance.</span></span> |
| <span data-ttu-id="31ae4-148">displayName</span><span class="sxs-lookup"><span data-stu-id="31ae4-148">displayName</span></span> | <span data-ttu-id="31ae4-149">String</span><span class="sxs-lookup"><span data-stu-id="31ae4-149">String</span></span> | <span data-ttu-id="31ae4-150">父 [accessReviewScheduleDefinition 的名称](accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="31ae4-150">Name of the parent [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> |
| <span data-ttu-id="31ae4-151">startDateTime</span><span class="sxs-lookup"><span data-stu-id="31ae4-151">startDateTime</span></span> | <span data-ttu-id="31ae4-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31ae4-152">DateTimeOffset</span></span> | <span data-ttu-id="31ae4-153">计划启动审阅实例的 DateTime。</span><span class="sxs-lookup"><span data-stu-id="31ae4-153">DateTime when review instance is scheduled to start.</span></span> <span data-ttu-id="31ae4-154">可能在将来。</span><span class="sxs-lookup"><span data-stu-id="31ae4-154">May be in the future.</span></span> <span data-ttu-id="31ae4-155">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="31ae4-155">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="31ae4-156">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="31ae4-156">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="31ae4-157">endDateTime</span><span class="sxs-lookup"><span data-stu-id="31ae4-157">endDateTime</span></span> | <span data-ttu-id="31ae4-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31ae4-158">DateTimeOffset</span></span> | <span data-ttu-id="31ae4-159">将审阅实例计划结束的 DateTime。DatetimeOffset 类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="31ae4-159">DateTime when review instance is scheduled to end.The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="31ae4-160">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="31ae4-160">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="31ae4-161">状态</span><span class="sxs-lookup"><span data-stu-id="31ae4-161">status</span></span> | <span data-ttu-id="31ae4-162">String</span><span class="sxs-lookup"><span data-stu-id="31ae4-162">String</span></span> | <span data-ttu-id="31ae4-163">指定 accessReview 的状态。</span><span class="sxs-lookup"><span data-stu-id="31ae4-163">Specifies the status of an accessReview.</span></span> <span data-ttu-id="31ae4-164">典型状态包括 `Initializing` `NotStarted` `Starting` `InProgress` 、、、、、、 `Completing` `Completed` `AutoReviewing` 和 `AutoReviewed` 。</span><span class="sxs-lookup"><span data-stu-id="31ae4-164">The typical states include `Initializing`, `NotStarted`, `Starting`, `InProgress`, `Completing`, `Completed`, `AutoReviewing`, and `AutoReviewed`.</span></span>  <span data-ttu-id="31ae4-165">只读。</span><span class="sxs-lookup"><span data-stu-id="31ae4-165">Read-only.</span></span>|
| <span data-ttu-id="31ae4-166">scope</span><span class="sxs-lookup"><span data-stu-id="31ae4-166">scope</span></span> | [<span data-ttu-id="31ae4-167">accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="31ae4-167">accessReviewScope</span></span>](accessreviewscope.md) | <span data-ttu-id="31ae4-168">基于级别的 **scope 和** **instanceEnumerationScope** `accessReviewScheduleDefinition` 创建。</span><span class="sxs-lookup"><span data-stu-id="31ae4-168">Created based on **scope** and **instanceEnumerationScope** at the `accessReviewScheduleDefinition` level.</span></span> <span data-ttu-id="31ae4-169">定义在组中查看的用户范围。</span><span class="sxs-lookup"><span data-stu-id="31ae4-169">Defines the scope of users reviewed in a group.</span></span> <span data-ttu-id="31ae4-170">对于单组评审，在级别定义的范围 `accessReviewScheduleDefinition` 适用于所有实例。</span><span class="sxs-lookup"><span data-stu-id="31ae4-170">In the case of a single-group review, the scope defined at the `accessReviewScheduleDefinition` level applies to all instances.</span></span> <span data-ttu-id="31ae4-171">在查看所有组的情况下，每个组的范围可能不同。</span><span class="sxs-lookup"><span data-stu-id="31ae4-171">In the case of all groups review, scope may be different for each group.</span></span> <span data-ttu-id="31ae4-172">只读。</span><span class="sxs-lookup"><span data-stu-id="31ae4-172">Read-only.</span></span>  | 
| <span data-ttu-id="31ae4-173">决策</span><span class="sxs-lookup"><span data-stu-id="31ae4-173">decisions</span></span> | <span data-ttu-id="31ae4-174">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="31ae4-174">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span></span> | <span data-ttu-id="31ae4-175">在 [accessReviewInstance](#accessreviewinstance-resource-type) 中查看的每个用户都有一个决定项，该项目表示其访问是经过批准、拒绝还是尚未被审阅。</span><span class="sxs-lookup"><span data-stu-id="31ae4-175">Each user reviewed in an [accessReviewInstance](#accessreviewinstance-resource-type) has a decision item representing if their access was approved, denied, or not yet reviewed.</span></span> |
| <span data-ttu-id="31ae4-176">definition</span><span class="sxs-lookup"><span data-stu-id="31ae4-176">definition</span></span> |[<span data-ttu-id="31ae4-177">accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="31ae4-177">accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition.md) | <span data-ttu-id="31ae4-178">每个实例只关联一 **个 accessReviewScheduleDefinition。**</span><span class="sxs-lookup"><span data-stu-id="31ae4-178">There is exactly one **accessReviewScheduleDefinition** associated with each instance.</span></span> <span data-ttu-id="31ae4-179">它是实例的父计划，其中为审阅定义的每个重复周期创建实例，并按定义选择查看每个组。</span><span class="sxs-lookup"><span data-stu-id="31ae4-179">It is the parent schedule for the instance, where instances are created for each recurrence of a review definition and each group selected to review by the definition.</span></span> |

## <a name="relationships"></a><span data-ttu-id="31ae4-180">关系</span><span class="sxs-lookup"><span data-stu-id="31ae4-180">Relationships</span></span>

| <span data-ttu-id="31ae4-181">关系</span><span class="sxs-lookup"><span data-stu-id="31ae4-181">Relationship</span></span> | <span data-ttu-id="31ae4-182">类型</span><span class="sxs-lookup"><span data-stu-id="31ae4-182">Type</span></span>   |<span data-ttu-id="31ae4-183">说明</span><span class="sxs-lookup"><span data-stu-id="31ae4-183">Description</span></span>|
|:---------------|:--------|:----------|
| `definition`               |[<span data-ttu-id="31ae4-184">accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="31ae4-184">accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition.md)          | <span data-ttu-id="31ae4-185">每个实例只 `accessReviewScheduleDefinition` 关联一个。</span><span class="sxs-lookup"><span data-stu-id="31ae4-185">There is exactly one `accessReviewScheduleDefinition` associated with each instance.</span></span> <span data-ttu-id="31ae4-186">它是实例的父计划，其中为审阅定义的每个重复周期创建实例，并按定义选择查看每个组。</span><span class="sxs-lookup"><span data-stu-id="31ae4-186">It is the parent schedule for the instance, where instances are created for each recurrence of a review definition and each group selected to review by the definition.</span></span> |
| `decisions`               |<span data-ttu-id="31ae4-187">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="31ae4-187">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span></span>        | <span data-ttu-id="31ae4-188">在 中审阅的 `accessReviewInstance` 每个用户都有一个决策项，代表他们被批准、拒绝还是尚未被审阅。</span><span class="sxs-lookup"><span data-stu-id="31ae4-188">Each user reviewed in an `accessReviewInstance` has a decision item representing if they were approved, denied, or not yet reviewed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="31ae4-189">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="31ae4-189">JSON representation</span></span>

<span data-ttu-id="31ae4-190">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="31ae4-190">Here is a JSON representation of the resource.</span></span>

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
