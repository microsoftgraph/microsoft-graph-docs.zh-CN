---
title: accessReviewInstance 资源类型
description: 表示的定期 `accessReviewScheduleDefinition` 。
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 480774950e2257b7af099c02cbe7c6571c0ce4c6
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000844"
---
# <a name="accessreviewinstance-resource-type"></a><span data-ttu-id="8a1d4-103">accessReviewInstance 资源类型</span><span class="sxs-lookup"><span data-stu-id="8a1d4-103">accessReviewInstance resource type</span></span>

<span data-ttu-id="8a1d4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a1d4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a1d4-105">表示定期的 Azure AD [访问审核](accessreviewsv2-root.md) 。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-105">Represents an Azure AD [access review](accessreviewsv2-root.md) recurrence.</span></span> <span data-ttu-id="8a1d4-106">如果父 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 是定期访问审核，则实例表示每个重复周期。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-106">If the parent [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) is a recurring access review, instances represent each recurrence.</span></span> <span data-ttu-id="8a1d4-107">不重复的审阅将只有一个实例。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-107">A review that does not recur will have exactly one instance.</span></span> <span data-ttu-id="8a1d4-108">实例还表示在日程安排定义中审阅的每个唯一组。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-108">Instances also represent each unique group being reviewed in the schedule definition.</span></span> <span data-ttu-id="8a1d4-109">如果计划定义检查多个组，则每个组都将具有每个重复的唯一实例。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-109">If a schedule definition reviews multiple groups, each group will have a unique instance for each recurrence.</span></span>

<span data-ttu-id="8a1d4-110">每个 **accessReviewInstance** 都包含审阅者可对其执行操作的 [决策](accessreviewinstancedecisionitem.md) 列表。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-110">Every **accessReviewInstance** contains a list of [decisions](accessreviewinstancedecisionitem.md) that reviewers can take action on.</span></span> <span data-ttu-id="8a1d4-111">每个标识的检查都有一个决定。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-111">There is one decision per identity being reviewed.</span></span>

## <a name="methods"></a><span data-ttu-id="8a1d4-112">方法</span><span class="sxs-lookup"><span data-stu-id="8a1d4-112">Methods</span></span>

| <span data-ttu-id="8a1d4-113">方法</span><span class="sxs-lookup"><span data-stu-id="8a1d4-113">Method</span></span> | <span data-ttu-id="8a1d4-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="8a1d4-114">Return Type</span></span> | <span data-ttu-id="8a1d4-115">说明</span><span class="sxs-lookup"><span data-stu-id="8a1d4-115">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="8a1d4-116">列出 accessReviewInstances</span><span class="sxs-lookup"><span data-stu-id="8a1d4-116">List accessReviewInstances</span></span>](../api/accessreviewinstance-list.md) | <span data-ttu-id="8a1d4-117">[accessReviewInstance](accessreviewinstance.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8a1d4-117">[accessReviewInstance](accessreviewinstance.md) collection</span></span> | <span data-ttu-id="8a1d4-118">获取 [accessReviewInstance](../resources/accessreviewinstance.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-118">Get a list of the [accessReviewInstance](../resources/accessreviewinstance.md) objects and their properties.</span></span> |
|[<span data-ttu-id="8a1d4-119">获取 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="8a1d4-119">Get accessReviewInstance</span></span>](../api/accessreviewinstance-get.md) | [<span data-ttu-id="8a1d4-120">accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="8a1d4-120">accessReviewInstance</span></span>](accessreviewinstance.md) | <span data-ttu-id="8a1d4-121">返回 accessReviewScheduleDefinition 的 accessReviewInstance。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-121">Returns accessReviewInstance for an accessReviewScheduleDefinition.</span></span> <span data-ttu-id="8a1d4-122">不包括对象中关联的 accessReviewInstanceDecisionItem。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-122">Does not include associated accessReviewInstanceDecisionItem\`s in the object.</span></span> |
|[<span data-ttu-id="8a1d4-123">列出 pendingAccessReviewInstances</span><span class="sxs-lookup"><span data-stu-id="8a1d4-123">List pendingAccessReviewInstances</span></span>](../api/accessreviewinstance-pendingaccessreviewinstances.md) | <span data-ttu-id="8a1d4-124">[accessReviewInstance](accessreviewinstance.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-124">[accessReviewInstance](accessreviewinstance.md) collection.</span></span> | <span data-ttu-id="8a1d4-125">获取分配给呼叫用户的所有待处理的 accessReviewInstance 资源。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-125">Get all pending accessReviewInstance resources assigned to the calling user.</span></span> |
|[<span data-ttu-id="8a1d4-126">发送 accessReviewInstance 提醒</span><span class="sxs-lookup"><span data-stu-id="8a1d4-126">Send accessReviewInstance reminder</span></span>](../api/accessreviewinstance-sendreminder.md) | <span data-ttu-id="8a1d4-127">无。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-127">None.</span></span> | <span data-ttu-id="8a1d4-128">向 accessReviewInstance 的审阅者发送提醒。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-128">Send a reminder to the reviewers of an accessReviewInstance.</span></span> |
|[<span data-ttu-id="8a1d4-129">停止 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="8a1d4-129">Stop accessReviewInstance</span></span>](../api/accessreviewinstance-stop.md) | <span data-ttu-id="8a1d4-130">无。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-130">None.</span></span> | <span data-ttu-id="8a1d4-131">手动停止 accessReviewInstance。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-131">Manually stop an accessReviewInstance.</span></span> |
|[<span data-ttu-id="8a1d4-132">接受建议</span><span class="sxs-lookup"><span data-stu-id="8a1d4-132">Accept recommendations</span></span>](../api/accessreviewinstance-acceptrecommendations.md) | <span data-ttu-id="8a1d4-133">无。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-133">None.</span></span> | <span data-ttu-id="8a1d4-134">允许呼叫用户接受针对特定 accessReviewInstance 的审阅者的每个 NotReviewed accessReviewInstanceDecisionItem 的决策建议。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-134">Allows the calling user to accept the decision recommendation for each NotReviewed accessReviewInstanceDecisionItem that they are the reviewer on for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="8a1d4-135">应用决策</span><span class="sxs-lookup"><span data-stu-id="8a1d4-135">Apply decisions</span></span>](../api/accessreviewinstance-applydecisions.md) | <span data-ttu-id="8a1d4-136">无。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-136">None.</span></span> | <span data-ttu-id="8a1d4-137">手动对 accessReviewInstance 应用决策。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-137">Manually apply decision on an accessReviewInstance.</span></span> |



## <a name="properties"></a><span data-ttu-id="8a1d4-138">属性</span><span class="sxs-lookup"><span data-stu-id="8a1d4-138">Properties</span></span>
| <span data-ttu-id="8a1d4-139">属性</span><span class="sxs-lookup"><span data-stu-id="8a1d4-139">Property</span></span> | <span data-ttu-id="8a1d4-140">类型</span><span class="sxs-lookup"><span data-stu-id="8a1d4-140">Type</span></span> | <span data-ttu-id="8a1d4-141">说明</span><span class="sxs-lookup"><span data-stu-id="8a1d4-141">Description</span></span> |
| :-------------------------| :---------------------------------- | :---------- |
| <span data-ttu-id="8a1d4-142">id</span><span class="sxs-lookup"><span data-stu-id="8a1d4-142">id</span></span> | <span data-ttu-id="8a1d4-143">字符串</span><span class="sxs-lookup"><span data-stu-id="8a1d4-143">String</span></span> | <span data-ttu-id="8a1d4-144">实例的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-144">Unique identifier of the instance.</span></span> |
| <span data-ttu-id="8a1d4-145">displayName</span><span class="sxs-lookup"><span data-stu-id="8a1d4-145">displayName</span></span> | <span data-ttu-id="8a1d4-146">字符串</span><span class="sxs-lookup"><span data-stu-id="8a1d4-146">String</span></span> | <span data-ttu-id="8a1d4-147">父 accessReviewScheduleDefinition 的名称。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-147">Name of the parent accessReviewScheduleDefinition.</span></span> |
| <span data-ttu-id="8a1d4-148">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8a1d4-148">startDateTime</span></span> | <span data-ttu-id="8a1d4-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a1d4-149">DateTimeOffset</span></span> | <span data-ttu-id="8a1d4-150">将审阅实例安排为启动时的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-150">DateTime when review instance is scheduled to start.</span></span> <span data-ttu-id="8a1d4-151">可能是将来的。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-151">May be in the future.</span></span> |
| <span data-ttu-id="8a1d4-152">endDateTime</span><span class="sxs-lookup"><span data-stu-id="8a1d4-152">endDateTime</span></span> | <span data-ttu-id="8a1d4-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a1d4-153">DateTimeOffset</span></span> | <span data-ttu-id="8a1d4-154">将审阅实例安排结束时的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-154">DateTime when review instance is scheduled to end.</span></span> |
| <span data-ttu-id="8a1d4-155">状态</span><span class="sxs-lookup"><span data-stu-id="8a1d4-155">status</span></span> | <span data-ttu-id="8a1d4-156">string</span><span class="sxs-lookup"><span data-stu-id="8a1d4-156">string</span></span> | <span data-ttu-id="8a1d4-157">指定 accessReview 的状态。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-157">Specifies the status of an accessReview.</span></span> <span data-ttu-id="8a1d4-158">典型状态包括、、、、、、 `Initializing` `NotStarted` `Starting` `InProgress` `Completing` `Completed` `AutoReviewing` 和 `AutoReviewed` 。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-158">The typical states include `Initializing`, `NotStarted`, `Starting`, `InProgress`, `Completing`, `Completed`, `AutoReviewing`, and `AutoReviewed`.</span></span>  <span data-ttu-id="8a1d4-159">只读。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-159">Read-only.</span></span>|
| <span data-ttu-id="8a1d4-160">scope</span><span class="sxs-lookup"><span data-stu-id="8a1d4-160">scope</span></span> | [<span data-ttu-id="8a1d4-161">accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="8a1d4-161">accessReviewScope</span></span>](accessreviewscope.md) | <span data-ttu-id="8a1d4-162">根据 **作用域** 和 **instanceEnumerationScope** 在 accessReviewScheduleDefinition 级别创建。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-162">Created based on **scope** and **instanceEnumerationScope** at the accessReviewScheduleDefinition level.</span></span> <span data-ttu-id="8a1d4-163">定义在组中审阅的用户的范围。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-163">Defines the scope of users reviewed in a group.</span></span> <span data-ttu-id="8a1d4-164">在单组审阅的情况下，在该级别定义的作用域 `accessReviewScheduleDefinition` 适用于所有实例。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-164">In the case of a single-group review, the scope defined at the `accessReviewScheduleDefinition` level applies to all instances.</span></span> <span data-ttu-id="8a1d4-165">在所有组审阅的情况下，每个组的作用域可能会有所不同。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-165">In the case of all groups review, scope may be different for each group.</span></span> <span data-ttu-id="8a1d4-166">只读。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-166">Read-only.</span></span>  | 
| <span data-ttu-id="8a1d4-167">针对</span><span class="sxs-lookup"><span data-stu-id="8a1d4-167">decisions</span></span> | <span data-ttu-id="8a1d4-168">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8a1d4-168">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span></span> | <span data-ttu-id="8a1d4-169">在 accessReviewInstance 中审阅的每个用户都有一个决定其访问是已被批准、被拒绝还是尚未审阅的决议项目。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-169">Each user reviewed in an accessReviewInstance has a decision item representing if their access was approved, denied, or not yet reviewed.</span></span> |
| <span data-ttu-id="8a1d4-170">定义</span><span class="sxs-lookup"><span data-stu-id="8a1d4-170">definition</span></span> |[<span data-ttu-id="8a1d4-171">accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="8a1d4-171">accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition.md) | <span data-ttu-id="8a1d4-172">与每个实例关联的 accessReviewScheduleDefinition 正好有一个。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-172">There is exactly one accessReviewScheduleDefinition associated with each instance.</span></span> <span data-ttu-id="8a1d4-173">它是实例的父计划，其中实例是为每个评审定义的每个重复项创建的，每个组选择由定义评审。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-173">It is the parent schedule for the instance, where instances are created for each recurrence of a review definition and each group selected to review by the definition.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8a1d4-174">关系</span><span class="sxs-lookup"><span data-stu-id="8a1d4-174">Relationships</span></span>

| <span data-ttu-id="8a1d4-175">关系</span><span class="sxs-lookup"><span data-stu-id="8a1d4-175">Relationship</span></span> | <span data-ttu-id="8a1d4-176">类型</span><span class="sxs-lookup"><span data-stu-id="8a1d4-176">Type</span></span>   |<span data-ttu-id="8a1d4-177">说明</span><span class="sxs-lookup"><span data-stu-id="8a1d4-177">Description</span></span>|
|:---------------|:--------|:----------|
| `definition`               |[<span data-ttu-id="8a1d4-178">accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="8a1d4-178">accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition.md)          | <span data-ttu-id="8a1d4-179">`accessReviewScheduleDefinition`与每个实例关联的只有一个。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-179">There is exactly one `accessReviewScheduleDefinition` associated with each instance.</span></span> <span data-ttu-id="8a1d4-180">它是实例的父计划，其中实例是为每个评审定义的每个重复项创建的，每个组选择由定义评审。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-180">It is the parent schedule for the instance, where instances are created for each recurrence of a review definition and each group selected to review by the definition.</span></span> |
| `decisions`               |<span data-ttu-id="8a1d4-181">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8a1d4-181">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span></span>        | <span data-ttu-id="8a1d4-182">中审阅的每个用户 `accessReviewInstance` 都有一个决策项目，表示他们是已批准、已拒绝还是尚未审阅。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-182">Each user reviewed in an `accessReviewInstance` has a decision item representing if they were approved, denied, or not yet reviewed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8a1d4-183">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8a1d4-183">JSON representation</span></span>

<span data-ttu-id="8a1d4-184">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a1d4-184">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewInstance",
  "baseType": "",
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
