---
title: accessReviewInstanceDecisionItem 资源类型
description: 表示有关用户访问 accessReviewInstance 的决定。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 228fbe473fe65fe84c9dfa7c62f3689681d47e39
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443186"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a><span data-ttu-id="f42f4-103">accessReviewInstanceDecisionItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="f42f4-103">accessReviewInstanceDecisionItem resource type</span></span>

<span data-ttu-id="f42f4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f42f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="f42f4-105">表示有关评价 [实例的](accessreviewsv2-root.md) Azure AD 访问评审决定。</span><span class="sxs-lookup"><span data-stu-id="f42f4-105">Represents an Azure AD [access review](accessreviewsv2-root.md) decision on an instance of a review.</span></span> <span data-ttu-id="f42f4-106">此决定表示确定用户或服务主体对给定访问评审实例 [的访问权限](accessreviewinstance.md)。</span><span class="sxs-lookup"><span data-stu-id="f42f4-106">This decision represents the determination of a user or service principal's access for a given [access review instance](accessreviewinstance.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f42f4-107">Methods</span><span class="sxs-lookup"><span data-stu-id="f42f4-107">Methods</span></span>

| <span data-ttu-id="f42f4-108">方法</span><span class="sxs-lookup"><span data-stu-id="f42f4-108">Method</span></span> | <span data-ttu-id="f42f4-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="f42f4-109">Return Type</span></span> | <span data-ttu-id="f42f4-110">说明</span><span class="sxs-lookup"><span data-stu-id="f42f4-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="f42f4-111">列出 accessReviewInstanceDecisionItems</span><span class="sxs-lookup"><span data-stu-id="f42f4-111">List accessReviewInstanceDecisionItems</span></span>](../api/accessreviewinstancedecisionitem-list.md) | <span data-ttu-id="f42f4-112">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f42f4-112">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span></span> | <span data-ttu-id="f42f4-113">列出特定 accessReviewInstance 的每个 accessReviewInstanceDecisionItem。</span><span class="sxs-lookup"><span data-stu-id="f42f4-113">Lists every accessReviewInstanceDecisionItem for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="f42f4-114">列出待审批的 accessReviewInstanceDecisionItems</span><span class="sxs-lookup"><span data-stu-id="f42f4-114">List accessReviewInstanceDecisionItems pending approval</span></span>](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | <span data-ttu-id="f42f4-115">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="f42f4-115">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection.</span></span> | <span data-ttu-id="f42f4-116">获取分配给调用用户的所有 accessReviewInstanceDecisionItems，用于特定 accessReviewInstance。</span><span class="sxs-lookup"><span data-stu-id="f42f4-116">Get all accessReviewInstanceDecisionItems assigned to the calling user, for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="f42f4-117">更新 accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="f42f4-117">Update accessReviewInstanceDecisionItem</span></span>](../api/accessreviewinstancedecisionitem-update.md) | <span data-ttu-id="f42f4-118">无。</span><span class="sxs-lookup"><span data-stu-id="f42f4-118">None.</span></span> | <span data-ttu-id="f42f4-119">对于分配了呼叫用户审阅者的任何 accessReviewInstanceDecisionItems，调用用户可以通过修补决策对象来记录决策。</span><span class="sxs-lookup"><span data-stu-id="f42f4-119">For any accessReviewInstanceDecisionItems that the calling user is assigned a reviewer on, calling user can record a decision by patching the decision object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f42f4-120">属性</span><span class="sxs-lookup"><span data-stu-id="f42f4-120">Properties</span></span>
| <span data-ttu-id="f42f4-121">属性</span><span class="sxs-lookup"><span data-stu-id="f42f4-121">Property</span></span> | <span data-ttu-id="f42f4-122">类型</span><span class="sxs-lookup"><span data-stu-id="f42f4-122">Type</span></span> |  <span data-ttu-id="f42f4-123">说明</span><span class="sxs-lookup"><span data-stu-id="f42f4-123">Description</span></span> |
| :---------------| :---- | :---------- |
| <span data-ttu-id="f42f4-124">id</span><span class="sxs-lookup"><span data-stu-id="f42f4-124">id</span></span> | <span data-ttu-id="f42f4-125">String</span><span class="sxs-lookup"><span data-stu-id="f42f4-125">String</span></span> | <span data-ttu-id="f42f4-126">决策的标识符。</span><span class="sxs-lookup"><span data-stu-id="f42f4-126">The identifier of the decision.</span></span> |
| <span data-ttu-id="f42f4-127">accessReviewId</span><span class="sxs-lookup"><span data-stu-id="f42f4-127">accessReviewId</span></span> | <span data-ttu-id="f42f4-128">String</span><span class="sxs-lookup"><span data-stu-id="f42f4-128">String</span></span> | <span data-ttu-id="f42f4-129">accessReviewInstance 父项的标识符。</span><span class="sxs-lookup"><span data-stu-id="f42f4-129">The identifier of the accessReviewInstance parent.</span></span> |
| <span data-ttu-id="f42f4-130">reviewedBy</span><span class="sxs-lookup"><span data-stu-id="f42f4-130">reviewedBy</span></span> | [<span data-ttu-id="f42f4-131">userIdentity</span><span class="sxs-lookup"><span data-stu-id="f42f4-131">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="f42f4-132">审阅者的标识符。</span><span class="sxs-lookup"><span data-stu-id="f42f4-132">The identifier of the reviewer.</span></span> |
| <span data-ttu-id="f42f4-133">reviewedDateTime</span><span class="sxs-lookup"><span data-stu-id="f42f4-133">reviewedDateTime</span></span> | <span data-ttu-id="f42f4-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f42f4-134">DateTimeOffset</span></span> | <span data-ttu-id="f42f4-135">审阅发生的 DateTime。</span><span class="sxs-lookup"><span data-stu-id="f42f4-135">The DateTime when the review occurred.</span></span> |
| <span data-ttu-id="f42f4-136">决策</span><span class="sxs-lookup"><span data-stu-id="f42f4-136">decision</span></span> | <span data-ttu-id="f42f4-137">String</span><span class="sxs-lookup"><span data-stu-id="f42f4-137">String</span></span> | <span data-ttu-id="f42f4-138">评价结果。</span><span class="sxs-lookup"><span data-stu-id="f42f4-138">Result of the review.</span></span> <span data-ttu-id="f42f4-139">可能的值 `Approve` `Deny` ：、、 `NotReviewed` 或 `DontKnow` 。</span><span class="sxs-lookup"><span data-stu-id="f42f4-139">Possible values: `Approve`, `Deny`, `NotReviewed`, or `DontKnow`.</span></span> |
| <span data-ttu-id="f42f4-140">justification</span><span class="sxs-lookup"><span data-stu-id="f42f4-140">justification</span></span> | <span data-ttu-id="f42f4-141">String</span><span class="sxs-lookup"><span data-stu-id="f42f4-141">String</span></span> | <span data-ttu-id="f42f4-142">审阅决策理由。</span><span class="sxs-lookup"><span data-stu-id="f42f4-142">The review decision justification.</span></span> |
| <span data-ttu-id="f42f4-143">appliedBy</span><span class="sxs-lookup"><span data-stu-id="f42f4-143">appliedBy</span></span> | [<span data-ttu-id="f42f4-144">userIdentity</span><span class="sxs-lookup"><span data-stu-id="f42f4-144">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="f42f4-145">应用决策的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="f42f4-145">The identifier of the user who applied the decision.</span></span> |
| <span data-ttu-id="f42f4-146">appliedDateTime</span><span class="sxs-lookup"><span data-stu-id="f42f4-146">appliedDateTime</span></span> | <span data-ttu-id="f42f4-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f42f4-147">DateTimeOffset</span></span> | <span data-ttu-id="f42f4-148">应用审批决定的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f42f4-148">The DateTime when the approval decision was applied.</span></span> |
| <span data-ttu-id="f42f4-149">applyResult</span><span class="sxs-lookup"><span data-stu-id="f42f4-149">applyResult</span></span> | <span data-ttu-id="f42f4-150">String</span><span class="sxs-lookup"><span data-stu-id="f42f4-150">String</span></span> | <span data-ttu-id="f42f4-151">应用决策的结果。</span><span class="sxs-lookup"><span data-stu-id="f42f4-151">The result of applying the decision.</span></span> <span data-ttu-id="f42f4-152">可能的值 `NotApplied` `Success` `Failed` ：、、、 `NotFound` 或 `NotSupported` 。</span><span class="sxs-lookup"><span data-stu-id="f42f4-152">Possible values: `NotApplied`, `Success`, `Failed`, `NotFound`, or `NotSupported`.</span></span> |
| <span data-ttu-id="f42f4-153">recommendation</span><span class="sxs-lookup"><span data-stu-id="f42f4-153">recommendation</span></span> | <span data-ttu-id="f42f4-154">String</span><span class="sxs-lookup"><span data-stu-id="f42f4-154">String</span></span> | <span data-ttu-id="f42f4-155">针对审批决策的系统生成的建议。</span><span class="sxs-lookup"><span data-stu-id="f42f4-155">A system-generated recommendation for the approval decision.</span></span> <span data-ttu-id="f42f4-156">可能的值： `Approve` ， `Deny` 或 `NotAvailable` 。</span><span class="sxs-lookup"><span data-stu-id="f42f4-156">Possible values: `Approve`, `Deny`, or `NotAvailable`.</span></span>  |
| <span data-ttu-id="f42f4-157">target</span><span class="sxs-lookup"><span data-stu-id="f42f4-157">target</span></span> | [<span data-ttu-id="f42f4-158">accessReviewInstanceDecisionItemTarget</span><span class="sxs-lookup"><span data-stu-id="f42f4-158">accessReviewInstanceDecisionItemTarget</span></span>](accessreviewinstancedecisionitemtarget.md)  | <span data-ttu-id="f42f4-159">此特定决策的目标。</span><span class="sxs-lookup"><span data-stu-id="f42f4-159">The target of this specific decision.</span></span> <span data-ttu-id="f42f4-160">决策目标可以是不同类型的 ， 每个类型都有其自己的特定属性。</span><span class="sxs-lookup"><span data-stu-id="f42f4-160">Decision targets can be of different types – each one with its own specific properties.</span></span> <span data-ttu-id="f42f4-161">请参阅 [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md)。</span><span class="sxs-lookup"><span data-stu-id="f42f4-161">See [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="f42f4-162">关系</span><span class="sxs-lookup"><span data-stu-id="f42f4-162">Relationships</span></span>

| <span data-ttu-id="f42f4-163">关系</span><span class="sxs-lookup"><span data-stu-id="f42f4-163">Relationship</span></span> | <span data-ttu-id="f42f4-164">类型</span><span class="sxs-lookup"><span data-stu-id="f42f4-164">Type</span></span>   |<span data-ttu-id="f42f4-165">说明</span><span class="sxs-lookup"><span data-stu-id="f42f4-165">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f42f4-166">实例</span><span class="sxs-lookup"><span data-stu-id="f42f4-166">instance</span></span> |[<span data-ttu-id="f42f4-167">accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="f42f4-167">accessReviewInstance</span></span>](accessreviewinstance.md) | <span data-ttu-id="f42f4-168">每个决策只关联一个 accessReviewInstance。</span><span class="sxs-lookup"><span data-stu-id="f42f4-168">There is exactly one accessReviewInstance associated with each decision.</span></span> <span data-ttu-id="f42f4-169">该实例是决策项的父项，表示做出该决策的访问评审的定期发生。</span><span class="sxs-lookup"><span data-stu-id="f42f4-169">The instance is the parent of the decision item, representing the recurrence of the access review the decision is made on.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="f42f4-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f42f4-170">JSON representation</span></span>

<span data-ttu-id="f42f4-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f42f4-171">Here is a JSON representation of the resource.</span></span>

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
