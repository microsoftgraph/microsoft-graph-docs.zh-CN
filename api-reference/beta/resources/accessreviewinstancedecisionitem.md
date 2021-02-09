---
title: accessReviewInstanceDecisionItem 资源类型
description: 表示有关用户访问 accessReviewInstance 的决定。
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 10166dc9da512bf74a0b4e5ad97f4797cdf6c317
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159197"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a><span data-ttu-id="df3be-103">accessReviewInstanceDecisionItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="df3be-103">accessReviewInstanceDecisionItem resource type</span></span>

<span data-ttu-id="df3be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df3be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df3be-105">表示有关评价 [实例的](accessreviewsv2-root.md) Azure AD 访问评审决定。</span><span class="sxs-lookup"><span data-stu-id="df3be-105">Represents an Azure AD [access review](accessreviewsv2-root.md) decision on an instance of a review.</span></span> <span data-ttu-id="df3be-106">此决定表示确定用户或服务主体对给定访问评审 [实例的访问权限](accessreviewinstance.md)。</span><span class="sxs-lookup"><span data-stu-id="df3be-106">This decision represents the determination of a user or service principal's access for a given [access review instance](accessreviewinstance.md).</span></span>

## <a name="methods"></a><span data-ttu-id="df3be-107">方法</span><span class="sxs-lookup"><span data-stu-id="df3be-107">Methods</span></span>

| <span data-ttu-id="df3be-108">方法</span><span class="sxs-lookup"><span data-stu-id="df3be-108">Method</span></span> | <span data-ttu-id="df3be-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="df3be-109">Return Type</span></span> | <span data-ttu-id="df3be-110">说明</span><span class="sxs-lookup"><span data-stu-id="df3be-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="df3be-111">列出 accessReviewInstanceDecisionItems</span><span class="sxs-lookup"><span data-stu-id="df3be-111">List accessReviewInstanceDecisionItems</span></span>](../api/accessreviewinstancedecisionitem-list.md) | <span data-ttu-id="df3be-112">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="df3be-112">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span></span> | <span data-ttu-id="df3be-113">列出特定 accessReviewInstance 的每一个 accessReviewInstanceDecisionItem。</span><span class="sxs-lookup"><span data-stu-id="df3be-113">Lists every accessReviewInstanceDecisionItem for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="df3be-114">列出 accessReviewInstanceDecisionItems 挂起审批</span><span class="sxs-lookup"><span data-stu-id="df3be-114">List accessReviewInstanceDecisionItems pending approval</span></span>](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | <span data-ttu-id="df3be-115">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="df3be-115">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection.</span></span> | <span data-ttu-id="df3be-116">获取分配给特定 accessReviewInstance 的调用用户的所有 accessReviewInstanceDecisionItems。</span><span class="sxs-lookup"><span data-stu-id="df3be-116">Get all accessReviewInstanceDecisionItems assigned to the calling user, for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="df3be-117">更新 accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="df3be-117">Update accessReviewInstanceDecisionItem</span></span>](../api/accessreviewinstancedecisionitem-update.md) | <span data-ttu-id="df3be-118">无。</span><span class="sxs-lookup"><span data-stu-id="df3be-118">None.</span></span> | <span data-ttu-id="df3be-119">对于分配了呼叫用户审阅者的任何 accessReviewInstanceDecisionItems，调用用户可以通过修补决策对象来记录决策。</span><span class="sxs-lookup"><span data-stu-id="df3be-119">For any accessReviewInstanceDecisionItems that the calling user is assigned a reviewer on, calling user can record a decision by patching the decision object.</span></span> |

## <a name="properties"></a><span data-ttu-id="df3be-120">属性</span><span class="sxs-lookup"><span data-stu-id="df3be-120">Properties</span></span>
| <span data-ttu-id="df3be-121">属性</span><span class="sxs-lookup"><span data-stu-id="df3be-121">Property</span></span> | <span data-ttu-id="df3be-122">类型</span><span class="sxs-lookup"><span data-stu-id="df3be-122">Type</span></span> |  <span data-ttu-id="df3be-123">说明</span><span class="sxs-lookup"><span data-stu-id="df3be-123">Description</span></span> |
| :---------------| :---- | :---------- |
| <span data-ttu-id="df3be-124">id</span><span class="sxs-lookup"><span data-stu-id="df3be-124">id</span></span> | <span data-ttu-id="df3be-125">String</span><span class="sxs-lookup"><span data-stu-id="df3be-125">String</span></span> | <span data-ttu-id="df3be-126">决策的标识符。</span><span class="sxs-lookup"><span data-stu-id="df3be-126">The identifier of the decision.</span></span> |
| <span data-ttu-id="df3be-127">accessReviewId</span><span class="sxs-lookup"><span data-stu-id="df3be-127">accessReviewId</span></span> | <span data-ttu-id="df3be-128">String</span><span class="sxs-lookup"><span data-stu-id="df3be-128">String</span></span> | <span data-ttu-id="df3be-129">accessReviewInstance 父项的标识符。</span><span class="sxs-lookup"><span data-stu-id="df3be-129">The identifier of the accessReviewInstance parent.</span></span> |
| <span data-ttu-id="df3be-130">reviewedBy</span><span class="sxs-lookup"><span data-stu-id="df3be-130">reviewedBy</span></span> | [<span data-ttu-id="df3be-131">userIdentity</span><span class="sxs-lookup"><span data-stu-id="df3be-131">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="df3be-132">审阅者的标识符。</span><span class="sxs-lookup"><span data-stu-id="df3be-132">The identifier of the reviewer.</span></span> |
| <span data-ttu-id="df3be-133">reviewedDateTime</span><span class="sxs-lookup"><span data-stu-id="df3be-133">reviewedDateTime</span></span> | <span data-ttu-id="df3be-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df3be-134">DateTimeOffset</span></span> | <span data-ttu-id="df3be-135">评价发生的 DateTime。</span><span class="sxs-lookup"><span data-stu-id="df3be-135">The DateTime when the review occurred.</span></span> |
| <span data-ttu-id="df3be-136">decision</span><span class="sxs-lookup"><span data-stu-id="df3be-136">decision</span></span> | <span data-ttu-id="df3be-137">String</span><span class="sxs-lookup"><span data-stu-id="df3be-137">String</span></span> | <span data-ttu-id="df3be-138">评价结果。</span><span class="sxs-lookup"><span data-stu-id="df3be-138">Result of the review.</span></span> <span data-ttu-id="df3be-139">可能的值 `Approve` `Deny` ：、、 `NotReviewed` 或 `DontKnow` 。</span><span class="sxs-lookup"><span data-stu-id="df3be-139">Possible values: `Approve`, `Deny`, `NotReviewed`, or `DontKnow`.</span></span> |
| <span data-ttu-id="df3be-140">justification</span><span class="sxs-lookup"><span data-stu-id="df3be-140">justification</span></span> | <span data-ttu-id="df3be-141">String</span><span class="sxs-lookup"><span data-stu-id="df3be-141">String</span></span> | <span data-ttu-id="df3be-142">审阅决策理由。</span><span class="sxs-lookup"><span data-stu-id="df3be-142">The review decision justification.</span></span> |
| <span data-ttu-id="df3be-143">appliedBy</span><span class="sxs-lookup"><span data-stu-id="df3be-143">appliedBy</span></span> | [<span data-ttu-id="df3be-144">userIdentity</span><span class="sxs-lookup"><span data-stu-id="df3be-144">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="df3be-145">应用决策的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="df3be-145">The identifier of the user who applied the decision.</span></span> |
| <span data-ttu-id="df3be-146">appliedDateTime</span><span class="sxs-lookup"><span data-stu-id="df3be-146">appliedDateTime</span></span> | <span data-ttu-id="df3be-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df3be-147">DateTimeOffset</span></span> | <span data-ttu-id="df3be-148">应用审批决定的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="df3be-148">The DateTime when the approval decision was applied.</span></span> |
| <span data-ttu-id="df3be-149">applyResult</span><span class="sxs-lookup"><span data-stu-id="df3be-149">applyResult</span></span> | <span data-ttu-id="df3be-150">String</span><span class="sxs-lookup"><span data-stu-id="df3be-150">String</span></span> | <span data-ttu-id="df3be-151">应用决策的结果。</span><span class="sxs-lookup"><span data-stu-id="df3be-151">The result of applying the decision.</span></span> <span data-ttu-id="df3be-152">可能的值 `NotApplied` `Success` `Failed` ：、、、 `NotFound` 或 `NotSupported` 。</span><span class="sxs-lookup"><span data-stu-id="df3be-152">Possible values: `NotApplied`, `Success`, `Failed`, `NotFound`, or `NotSupported`.</span></span> |
| <span data-ttu-id="df3be-153">建议</span><span class="sxs-lookup"><span data-stu-id="df3be-153">recommendation</span></span> | <span data-ttu-id="df3be-154">String</span><span class="sxs-lookup"><span data-stu-id="df3be-154">String</span></span> | <span data-ttu-id="df3be-155">针对审批决策的系统生成的建议。</span><span class="sxs-lookup"><span data-stu-id="df3be-155">A system-generated recommendation for the approval decision.</span></span> <span data-ttu-id="df3be-156">可能的值： `Approve` ， `Deny` 或 `NotAvailable` 。</span><span class="sxs-lookup"><span data-stu-id="df3be-156">Possible values: `Approve`, `Deny`, or `NotAvailable`.</span></span>  |
| <span data-ttu-id="df3be-157">target</span><span class="sxs-lookup"><span data-stu-id="df3be-157">target</span></span> | [<span data-ttu-id="df3be-158">accessReviewInstanceDecisionItemTarget</span><span class="sxs-lookup"><span data-stu-id="df3be-158">accessReviewInstanceDecisionItemTarget</span></span>](accessreviewinstancedecisionitemtarget.md)  | <span data-ttu-id="df3be-159">此特定决策的目标。</span><span class="sxs-lookup"><span data-stu-id="df3be-159">The target of this specific decision.</span></span> <span data-ttu-id="df3be-160">决策目标可以是不同类型的 - 每个目标都有其自己的特定属性。</span><span class="sxs-lookup"><span data-stu-id="df3be-160">Decision targets can be of different types – each one with its own specific properties.</span></span> <span data-ttu-id="df3be-161">请参阅 [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md)。</span><span class="sxs-lookup"><span data-stu-id="df3be-161">See [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="df3be-162">关系</span><span class="sxs-lookup"><span data-stu-id="df3be-162">Relationships</span></span>

| <span data-ttu-id="df3be-163">关系</span><span class="sxs-lookup"><span data-stu-id="df3be-163">Relationship</span></span> | <span data-ttu-id="df3be-164">类型</span><span class="sxs-lookup"><span data-stu-id="df3be-164">Type</span></span>   |<span data-ttu-id="df3be-165">说明</span><span class="sxs-lookup"><span data-stu-id="df3be-165">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="df3be-166">实例</span><span class="sxs-lookup"><span data-stu-id="df3be-166">instance</span></span> |[<span data-ttu-id="df3be-167">accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="df3be-167">accessReviewInstance</span></span>](accessreviewinstance.md) | <span data-ttu-id="df3be-168">每个决策只关联一个 accessReviewInstance。</span><span class="sxs-lookup"><span data-stu-id="df3be-168">There is exactly one accessReviewInstance associated with each decision.</span></span> <span data-ttu-id="df3be-169">该实例是决策项的父项，表示做出该决策的访问评审的定期发生。</span><span class="sxs-lookup"><span data-stu-id="df3be-169">The instance is the parent of the decision item, representing the recurrence of the access review the decision is made on.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="df3be-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="df3be-170">JSON representation</span></span>

<span data-ttu-id="df3be-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df3be-171">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem",
  "openType": true
}
-->

```json
{
 "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItem",
 "id": "string (identifier)",
 "accessReviewId": "string",
 "reviewedBy": {
    "@odata.type": "microsoft.graph.userIdentity"
 },
 "reviewedDateTime": "string (timestamp)",
 "decision": "string",
 "justification": "string",
 "appliedBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
 "appliedDateTime": "DateTimeOffset",
 "applyResult": "string",
 "recommendation": "string",
 "target": {
    "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemTarget"
  }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewInstanceDecisionItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
