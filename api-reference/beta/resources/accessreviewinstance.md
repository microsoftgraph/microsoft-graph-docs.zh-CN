---
title: accessReviewInstance 资源类型
description: 表示重复的 `accessReviewScheduleDefinition` 。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a0003ab8a79372a4dfefea1a62120ea8e40fa2c1
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443193"
---
# <a name="accessreviewinstance-resource-type"></a><span data-ttu-id="9405d-103">accessReviewInstance 资源类型</span><span class="sxs-lookup"><span data-stu-id="9405d-103">accessReviewInstance resource type</span></span>

<span data-ttu-id="9405d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9405d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="9405d-105">表示 Azure AD [访问评审定期](accessreviewsv2-root.md) 。</span><span class="sxs-lookup"><span data-stu-id="9405d-105">Represents an Azure AD [access review](accessreviewsv2-root.md) recurrence.</span></span> <span data-ttu-id="9405d-106">如果父 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 是定期访问评审，则实例表示每个重复周期。</span><span class="sxs-lookup"><span data-stu-id="9405d-106">If the parent [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) is a recurring access review, instances represent each recurrence.</span></span> <span data-ttu-id="9405d-107">不重复的审阅将只具有一个实例。</span><span class="sxs-lookup"><span data-stu-id="9405d-107">A review that does not recur will have exactly one instance.</span></span> <span data-ttu-id="9405d-108">实例还表示计划定义中正在审阅的每个唯一组。</span><span class="sxs-lookup"><span data-stu-id="9405d-108">Instances also represent each unique group being reviewed in the schedule definition.</span></span> <span data-ttu-id="9405d-109">如果计划定义检查多个组，则每个组将具有每个重复周期的唯一实例。</span><span class="sxs-lookup"><span data-stu-id="9405d-109">If a schedule definition reviews multiple groups, each group will have a unique instance for each recurrence.</span></span>

<span data-ttu-id="9405d-110">每个 **accessReviewInstance** 都包含审阅 [](accessreviewinstancedecisionitem.md)者可以采取措施的决策列表。</span><span class="sxs-lookup"><span data-stu-id="9405d-110">Every **accessReviewInstance** contains a list of [decisions](accessreviewinstancedecisionitem.md) that reviewers can take action on.</span></span> <span data-ttu-id="9405d-111">检查每个标识有一个决策。</span><span class="sxs-lookup"><span data-stu-id="9405d-111">There is one decision per identity being reviewed.</span></span>

## <a name="methods"></a><span data-ttu-id="9405d-112">Methods</span><span class="sxs-lookup"><span data-stu-id="9405d-112">Methods</span></span>

| <span data-ttu-id="9405d-113">方法</span><span class="sxs-lookup"><span data-stu-id="9405d-113">Method</span></span> | <span data-ttu-id="9405d-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="9405d-114">Return Type</span></span> | <span data-ttu-id="9405d-115">说明</span><span class="sxs-lookup"><span data-stu-id="9405d-115">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="9405d-116">列出 accessReviewInstances</span><span class="sxs-lookup"><span data-stu-id="9405d-116">List accessReviewInstances</span></span>](../api/accessreviewinstance-list.md) | <span data-ttu-id="9405d-117">[accessReviewInstance](accessreviewinstance.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9405d-117">[accessReviewInstance](accessreviewinstance.md) collection</span></span> | <span data-ttu-id="9405d-118">获取 [accessReviewInstance](../resources/accessreviewinstance.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="9405d-118">Get a list of the [accessReviewInstance](../resources/accessreviewinstance.md) objects and their properties.</span></span> |
|[<span data-ttu-id="9405d-119">获取 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="9405d-119">Get accessReviewInstance</span></span>](../api/accessreviewinstance-get.md) | [<span data-ttu-id="9405d-120">accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="9405d-120">accessReviewInstance</span></span>](accessreviewinstance.md) | <span data-ttu-id="9405d-121">返回 accessReviewScheduleDefinition 的 accessReviewInstance。</span><span class="sxs-lookup"><span data-stu-id="9405d-121">Returns accessReviewInstance for an accessReviewScheduleDefinition.</span></span> <span data-ttu-id="9405d-122">对象中不包括关联的 accessReviewInstanceDecisionItem。</span><span class="sxs-lookup"><span data-stu-id="9405d-122">Does not include associated accessReviewInstanceDecisionItem\`s in the object.</span></span> |
|[<span data-ttu-id="9405d-123">列出 pendingAccessReviewInstances</span><span class="sxs-lookup"><span data-stu-id="9405d-123">List pendingAccessReviewInstances</span></span>](../api/accessreviewinstance-pendingaccessreviewinstances.md) | <span data-ttu-id="9405d-124">[accessReviewInstance](accessreviewinstance.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="9405d-124">[accessReviewInstance](accessreviewinstance.md) collection.</span></span> | <span data-ttu-id="9405d-125">获取分配给调用用户的所有待定 accessReviewInstance 资源。</span><span class="sxs-lookup"><span data-stu-id="9405d-125">Get all pending accessReviewInstance resources assigned to the calling user.</span></span> |
|[<span data-ttu-id="9405d-126">发送 accessReviewInstance 提醒</span><span class="sxs-lookup"><span data-stu-id="9405d-126">Send accessReviewInstance reminder</span></span>](../api/accessreviewinstance-sendreminder.md) | <span data-ttu-id="9405d-127">无。</span><span class="sxs-lookup"><span data-stu-id="9405d-127">None.</span></span> | <span data-ttu-id="9405d-128">向 accessReviewInstance 的审阅者发送提醒。</span><span class="sxs-lookup"><span data-stu-id="9405d-128">Send a reminder to the reviewers of an accessReviewInstance.</span></span> |
|[<span data-ttu-id="9405d-129">停止 accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="9405d-129">Stop accessReviewInstance</span></span>](../api/accessreviewinstance-stop.md) | <span data-ttu-id="9405d-130">无。</span><span class="sxs-lookup"><span data-stu-id="9405d-130">None.</span></span> | <span data-ttu-id="9405d-131">手动停止 accessReviewInstance。</span><span class="sxs-lookup"><span data-stu-id="9405d-131">Manually stop an accessReviewInstance.</span></span> |
|[<span data-ttu-id="9405d-132">接受建议</span><span class="sxs-lookup"><span data-stu-id="9405d-132">Accept recommendations</span></span>](../api/accessreviewinstance-acceptrecommendations.md) | <span data-ttu-id="9405d-133">无。</span><span class="sxs-lookup"><span data-stu-id="9405d-133">None.</span></span> | <span data-ttu-id="9405d-134">允许调用用户接受他们作为特定 accessReviewInstance 审阅者的每个 NotReviewed accessReviewInstanceDecisionItem 的决策建议。</span><span class="sxs-lookup"><span data-stu-id="9405d-134">Allows the calling user to accept the decision recommendation for each NotReviewed accessReviewInstanceDecisionItem that they are the reviewer on for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="9405d-135">应用决策</span><span class="sxs-lookup"><span data-stu-id="9405d-135">Apply decisions</span></span>](../api/accessreviewinstance-applydecisions.md) | <span data-ttu-id="9405d-136">无。</span><span class="sxs-lookup"><span data-stu-id="9405d-136">None.</span></span> | <span data-ttu-id="9405d-137">手动对 accessReviewInstance 应用决策。</span><span class="sxs-lookup"><span data-stu-id="9405d-137">Manually apply decision on an accessReviewInstance.</span></span> |



## <a name="properties"></a><span data-ttu-id="9405d-138">属性</span><span class="sxs-lookup"><span data-stu-id="9405d-138">Properties</span></span>
| <span data-ttu-id="9405d-139">属性</span><span class="sxs-lookup"><span data-stu-id="9405d-139">Property</span></span> | <span data-ttu-id="9405d-140">类型</span><span class="sxs-lookup"><span data-stu-id="9405d-140">Type</span></span> | <span data-ttu-id="9405d-141">说明</span><span class="sxs-lookup"><span data-stu-id="9405d-141">Description</span></span> |
| :-------------------------| :---------------------------------- | :---------- |
| <span data-ttu-id="9405d-142">id</span><span class="sxs-lookup"><span data-stu-id="9405d-142">id</span></span> | <span data-ttu-id="9405d-143">String</span><span class="sxs-lookup"><span data-stu-id="9405d-143">String</span></span> | <span data-ttu-id="9405d-144">实例的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9405d-144">Unique identifier of the instance.</span></span> |
| <span data-ttu-id="9405d-145">displayName</span><span class="sxs-lookup"><span data-stu-id="9405d-145">displayName</span></span> | <span data-ttu-id="9405d-146">String</span><span class="sxs-lookup"><span data-stu-id="9405d-146">String</span></span> | <span data-ttu-id="9405d-147">父 accessReviewScheduleDefinition 的名称。</span><span class="sxs-lookup"><span data-stu-id="9405d-147">Name of the parent accessReviewScheduleDefinition.</span></span> |
| <span data-ttu-id="9405d-148">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9405d-148">startDateTime</span></span> | <span data-ttu-id="9405d-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9405d-149">DateTimeOffset</span></span> | <span data-ttu-id="9405d-150">计划启动审阅实例的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9405d-150">DateTime when review instance is scheduled to start.</span></span> <span data-ttu-id="9405d-151">可能在将来。</span><span class="sxs-lookup"><span data-stu-id="9405d-151">May be in the future.</span></span> |
| <span data-ttu-id="9405d-152">endDateTime</span><span class="sxs-lookup"><span data-stu-id="9405d-152">endDateTime</span></span> | <span data-ttu-id="9405d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9405d-153">DateTimeOffset</span></span> | <span data-ttu-id="9405d-154">计划结束审阅实例的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9405d-154">DateTime when review instance is scheduled to end.</span></span> |
| <span data-ttu-id="9405d-155">状态</span><span class="sxs-lookup"><span data-stu-id="9405d-155">status</span></span> | <span data-ttu-id="9405d-156">string</span><span class="sxs-lookup"><span data-stu-id="9405d-156">string</span></span> | <span data-ttu-id="9405d-157">指定 accessReview 的状态。</span><span class="sxs-lookup"><span data-stu-id="9405d-157">Specifies the status of an accessReview.</span></span> <span data-ttu-id="9405d-158">典型状态包括 `Initializing` 、 `NotStarted` `Starting` 、 、 、 `InProgress` `Completing` 和 `Completed` `AutoReviewing` `AutoReviewed` 。</span><span class="sxs-lookup"><span data-stu-id="9405d-158">The typical states include `Initializing`, `NotStarted`, `Starting`, `InProgress`, `Completing`, `Completed`, `AutoReviewing`, and `AutoReviewed`.</span></span>  <span data-ttu-id="9405d-159">只读。</span><span class="sxs-lookup"><span data-stu-id="9405d-159">Read-only.</span></span>|
| <span data-ttu-id="9405d-160">scope</span><span class="sxs-lookup"><span data-stu-id="9405d-160">scope</span></span> | [<span data-ttu-id="9405d-161">accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="9405d-161">accessReviewScope</span></span>](accessreviewscope.md) | <span data-ttu-id="9405d-162">基于范围 **和** **instanceEnumerationScope** 在 accessReviewScheduleDefinition 级别创建。</span><span class="sxs-lookup"><span data-stu-id="9405d-162">Created based on **scope** and **instanceEnumerationScope** at the accessReviewScheduleDefinition level.</span></span> <span data-ttu-id="9405d-163">定义在组中审阅的用户范围。</span><span class="sxs-lookup"><span data-stu-id="9405d-163">Defines the scope of users reviewed in a group.</span></span> <span data-ttu-id="9405d-164">对于单组审阅，级别定义的范围 `accessReviewScheduleDefinition` 适用于所有实例。</span><span class="sxs-lookup"><span data-stu-id="9405d-164">In the case of a single-group review, the scope defined at the `accessReviewScheduleDefinition` level applies to all instances.</span></span> <span data-ttu-id="9405d-165">对于所有组审阅，每个组的范围可能不同。</span><span class="sxs-lookup"><span data-stu-id="9405d-165">In the case of all groups review, scope may be different for each group.</span></span> <span data-ttu-id="9405d-166">只读。</span><span class="sxs-lookup"><span data-stu-id="9405d-166">Read-only.</span></span>  | 
| <span data-ttu-id="9405d-167">决策</span><span class="sxs-lookup"><span data-stu-id="9405d-167">decisions</span></span> | <span data-ttu-id="9405d-168">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9405d-168">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span></span> | <span data-ttu-id="9405d-169">在 accessReviewInstance 中审阅的每个用户都有一个决策项，它表示其访问是否得到批准、拒绝或尚未审查。</span><span class="sxs-lookup"><span data-stu-id="9405d-169">Each user reviewed in an accessReviewInstance has a decision item representing if their access was approved, denied, or not yet reviewed.</span></span> |
| <span data-ttu-id="9405d-170">definition</span><span class="sxs-lookup"><span data-stu-id="9405d-170">definition</span></span> |[<span data-ttu-id="9405d-171">accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="9405d-171">accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition.md) | <span data-ttu-id="9405d-172">每个实例只关联一个 accessReviewScheduleDefinition。</span><span class="sxs-lookup"><span data-stu-id="9405d-172">There is exactly one accessReviewScheduleDefinition associated with each instance.</span></span> <span data-ttu-id="9405d-173">它是实例的父计划，其中会针对每次重复的审阅定义创建实例，并且每个组都由定义选择审阅。</span><span class="sxs-lookup"><span data-stu-id="9405d-173">It is the parent schedule for the instance, where instances are created for each recurrence of a review definition and each group selected to review by the definition.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9405d-174">关系</span><span class="sxs-lookup"><span data-stu-id="9405d-174">Relationships</span></span>

| <span data-ttu-id="9405d-175">关系</span><span class="sxs-lookup"><span data-stu-id="9405d-175">Relationship</span></span> | <span data-ttu-id="9405d-176">类型</span><span class="sxs-lookup"><span data-stu-id="9405d-176">Type</span></span>   |<span data-ttu-id="9405d-177">说明</span><span class="sxs-lookup"><span data-stu-id="9405d-177">Description</span></span>|
|:---------------|:--------|:----------|
| `definition`               |[<span data-ttu-id="9405d-178">accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="9405d-178">accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition.md)          | <span data-ttu-id="9405d-179">每个实例只关联 `accessReviewScheduleDefinition` 一个。</span><span class="sxs-lookup"><span data-stu-id="9405d-179">There is exactly one `accessReviewScheduleDefinition` associated with each instance.</span></span> <span data-ttu-id="9405d-180">它是实例的父计划，其中会为每次重复的审阅定义创建实例，并按定义选择要审阅的每个组。</span><span class="sxs-lookup"><span data-stu-id="9405d-180">It is the parent schedule for the instance, where instances are created for each recurrence of a review definition and each group selected to review by the definition.</span></span> |
| `decisions`               |<span data-ttu-id="9405d-181">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9405d-181">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span></span>        | <span data-ttu-id="9405d-182">在一个已审阅的每个用户都有一个决策项，它表示他们被批准、拒绝还是 `accessReviewInstance` 尚未被审阅。</span><span class="sxs-lookup"><span data-stu-id="9405d-182">Each user reviewed in an `accessReviewInstance` has a decision item representing if they were approved, denied, or not yet reviewed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9405d-183">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9405d-183">JSON representation</span></span>

<span data-ttu-id="9405d-184">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9405d-184">Here is a JSON representation of the resource.</span></span>

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
