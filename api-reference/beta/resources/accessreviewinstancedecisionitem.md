---
title: accessReviewInstanceDecisionItem 资源类型
description: 代表用户对 accessReviewInstance 的访问的决定。
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d9ad5f8a49d44c82f1a43a1666f08f2b49853395
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000843"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a><span data-ttu-id="c92ea-103">accessReviewInstanceDecisionItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="c92ea-103">accessReviewInstanceDecisionItem resource type</span></span>

<span data-ttu-id="c92ea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c92ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c92ea-105">表示对评审实例的 Azure AD [访问审核](accessreviewsv2-root.md) 决定。</span><span class="sxs-lookup"><span data-stu-id="c92ea-105">Represents an Azure AD [access review](accessreviewsv2-root.md) decision on an instance of a review.</span></span> <span data-ttu-id="c92ea-106">此决定表示确定用户或服务主体对给定的 [访问评审实例](accessreviewinstance.md)的访问权限。</span><span class="sxs-lookup"><span data-stu-id="c92ea-106">This decision represents the determination of a user or service principal's access for a given [access review instance](accessreviewinstance.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c92ea-107">方法</span><span class="sxs-lookup"><span data-stu-id="c92ea-107">Methods</span></span>

| <span data-ttu-id="c92ea-108">方法</span><span class="sxs-lookup"><span data-stu-id="c92ea-108">Method</span></span> | <span data-ttu-id="c92ea-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="c92ea-109">Return Type</span></span> | <span data-ttu-id="c92ea-110">说明</span><span class="sxs-lookup"><span data-stu-id="c92ea-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="c92ea-111">列出 accessReviewInstanceDecisionItems</span><span class="sxs-lookup"><span data-stu-id="c92ea-111">List accessReviewInstanceDecisionItems</span></span>](../api/accessreviewinstancedecisionitem-list.md) | <span data-ttu-id="c92ea-112">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c92ea-112">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span></span> | <span data-ttu-id="c92ea-113">列出特定 accessReviewInstance 的每个 accessReviewInstanceDecisionItem。</span><span class="sxs-lookup"><span data-stu-id="c92ea-113">Lists every accessReviewInstanceDecisionItem for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="c92ea-114">列出 accessReviewInstanceDecisionItems 待审批</span><span class="sxs-lookup"><span data-stu-id="c92ea-114">List accessReviewInstanceDecisionItems pending approval</span></span>](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | <span data-ttu-id="c92ea-115">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="c92ea-115">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection.</span></span> | <span data-ttu-id="c92ea-116">获取特定 accessReviewInstance 的所有分配给呼叫用户的 accessReviewInstanceDecisionItems。</span><span class="sxs-lookup"><span data-stu-id="c92ea-116">Get all accessReviewInstanceDecisionItems assigned to the calling user, for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="c92ea-117">更新 accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="c92ea-117">Update accessReviewInstanceDecisionItem</span></span>](../api/accessreviewinstancedecisionitem-update.md) | <span data-ttu-id="c92ea-118">无。</span><span class="sxs-lookup"><span data-stu-id="c92ea-118">None.</span></span> | <span data-ttu-id="c92ea-119">对于呼叫用户分配了审阅者的任何 accessReviewInstanceDecisionItems，呼叫用户可以通过修补决策对象来记录决策。</span><span class="sxs-lookup"><span data-stu-id="c92ea-119">For any accessReviewInstanceDecisionItems that the calling user is assigned a reviewer on, calling user can record a decision by patching the decision object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c92ea-120">属性</span><span class="sxs-lookup"><span data-stu-id="c92ea-120">Properties</span></span>
| <span data-ttu-id="c92ea-121">属性</span><span class="sxs-lookup"><span data-stu-id="c92ea-121">Property</span></span> | <span data-ttu-id="c92ea-122">类型</span><span class="sxs-lookup"><span data-stu-id="c92ea-122">Type</span></span> |  <span data-ttu-id="c92ea-123">说明</span><span class="sxs-lookup"><span data-stu-id="c92ea-123">Description</span></span> |
| :---------------| :---- | :---------- |
| <span data-ttu-id="c92ea-124">id</span><span class="sxs-lookup"><span data-stu-id="c92ea-124">id</span></span> | <span data-ttu-id="c92ea-125">字符串</span><span class="sxs-lookup"><span data-stu-id="c92ea-125">String</span></span> | <span data-ttu-id="c92ea-126">决策的标识符。</span><span class="sxs-lookup"><span data-stu-id="c92ea-126">The identifier of the decision.</span></span> |
| <span data-ttu-id="c92ea-127">accessReviewId</span><span class="sxs-lookup"><span data-stu-id="c92ea-127">accessReviewId</span></span> | <span data-ttu-id="c92ea-128">字符串</span><span class="sxs-lookup"><span data-stu-id="c92ea-128">String</span></span> | <span data-ttu-id="c92ea-129">AccessReviewInstance 父级的标识符。</span><span class="sxs-lookup"><span data-stu-id="c92ea-129">The identifier of the accessReviewInstance parent.</span></span> |
| <span data-ttu-id="c92ea-130">reviewedBy</span><span class="sxs-lookup"><span data-stu-id="c92ea-130">reviewedBy</span></span> | [<span data-ttu-id="c92ea-131">userIdentity</span><span class="sxs-lookup"><span data-stu-id="c92ea-131">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="c92ea-132">审阅者的标识符。</span><span class="sxs-lookup"><span data-stu-id="c92ea-132">The identifier of the reviewer.</span></span> |
| <span data-ttu-id="c92ea-133">reviewedDateTime</span><span class="sxs-lookup"><span data-stu-id="c92ea-133">reviewedDateTime</span></span> | <span data-ttu-id="c92ea-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c92ea-134">DateTimeOffset</span></span> | <span data-ttu-id="c92ea-135">评审发生时的日期时间。</span><span class="sxs-lookup"><span data-stu-id="c92ea-135">The DateTime when the review occurred.</span></span> |
| <span data-ttu-id="c92ea-136">权</span><span class="sxs-lookup"><span data-stu-id="c92ea-136">decision</span></span> | <span data-ttu-id="c92ea-137">字符串</span><span class="sxs-lookup"><span data-stu-id="c92ea-137">String</span></span> | <span data-ttu-id="c92ea-138">评审的结果。</span><span class="sxs-lookup"><span data-stu-id="c92ea-138">Result of the review.</span></span> <span data-ttu-id="c92ea-139">可能的值： `Approve` 、、 `Deny` `NotReviewed` 或 `DontKnow` 。</span><span class="sxs-lookup"><span data-stu-id="c92ea-139">Possible values: `Approve`, `Deny`, `NotReviewed`, or `DontKnow`.</span></span> |
| <span data-ttu-id="c92ea-140">合理化</span><span class="sxs-lookup"><span data-stu-id="c92ea-140">justification</span></span> | <span data-ttu-id="c92ea-141">字符串</span><span class="sxs-lookup"><span data-stu-id="c92ea-141">String</span></span> | <span data-ttu-id="c92ea-142">评审决策理由。</span><span class="sxs-lookup"><span data-stu-id="c92ea-142">The review decision justification.</span></span> |
| <span data-ttu-id="c92ea-143">appliedBy</span><span class="sxs-lookup"><span data-stu-id="c92ea-143">appliedBy</span></span> | [<span data-ttu-id="c92ea-144">userIdentity</span><span class="sxs-lookup"><span data-stu-id="c92ea-144">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="c92ea-145">应用决策的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="c92ea-145">The identifier of the user who applied the decision.</span></span> |
| <span data-ttu-id="c92ea-146">appliedDateTime</span><span class="sxs-lookup"><span data-stu-id="c92ea-146">appliedDateTime</span></span> | <span data-ttu-id="c92ea-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c92ea-147">DateTimeOffset</span></span> | <span data-ttu-id="c92ea-148">应用审批决定时的日期时间。</span><span class="sxs-lookup"><span data-stu-id="c92ea-148">The DateTime when the approval decision was applied.</span></span> |
| <span data-ttu-id="c92ea-149">applyResult</span><span class="sxs-lookup"><span data-stu-id="c92ea-149">applyResult</span></span> | <span data-ttu-id="c92ea-150">字符串</span><span class="sxs-lookup"><span data-stu-id="c92ea-150">String</span></span> | <span data-ttu-id="c92ea-151">应用决策的结果。</span><span class="sxs-lookup"><span data-stu-id="c92ea-151">The result of applying the decision.</span></span> <span data-ttu-id="c92ea-152">可能的值： `NotApplied` 、 `Success` 、、 `Failed` `NotFound` 或 `NotSupported` 。</span><span class="sxs-lookup"><span data-stu-id="c92ea-152">Possible values: `NotApplied`, `Success`, `Failed`, `NotFound`, or `NotSupported`.</span></span> |
| <span data-ttu-id="c92ea-153">提出</span><span class="sxs-lookup"><span data-stu-id="c92ea-153">recommendation</span></span> | <span data-ttu-id="c92ea-154">字符串</span><span class="sxs-lookup"><span data-stu-id="c92ea-154">String</span></span> | <span data-ttu-id="c92ea-155">系统生成的审批决策建议。</span><span class="sxs-lookup"><span data-stu-id="c92ea-155">A system-generated recommendation for the approval decision.</span></span> <span data-ttu-id="c92ea-156">可能的值： `Approve` 、 `Deny` 或 `NotAvailable` 。</span><span class="sxs-lookup"><span data-stu-id="c92ea-156">Possible values: `Approve`, `Deny`, or `NotAvailable`.</span></span>  |
| <span data-ttu-id="c92ea-157">target</span><span class="sxs-lookup"><span data-stu-id="c92ea-157">target</span></span> | [<span data-ttu-id="c92ea-158">accessReviewInstanceDecisionItemTarget</span><span class="sxs-lookup"><span data-stu-id="c92ea-158">accessReviewInstanceDecisionItemTarget</span></span>](accessreviewinstancedecisionitemtarget.md)  | <span data-ttu-id="c92ea-159">此特定决策的目标。</span><span class="sxs-lookup"><span data-stu-id="c92ea-159">The target of this specific decision.</span></span> <span data-ttu-id="c92ea-160">决策目标可以是不同的类型–每种类型都有其自己的特定属性。</span><span class="sxs-lookup"><span data-stu-id="c92ea-160">Decision targets can be of different types – each one with its own specific properties.</span></span> <span data-ttu-id="c92ea-161">请参阅 [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md)。</span><span class="sxs-lookup"><span data-stu-id="c92ea-161">See [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="c92ea-162">关系</span><span class="sxs-lookup"><span data-stu-id="c92ea-162">Relationships</span></span>

| <span data-ttu-id="c92ea-163">关系</span><span class="sxs-lookup"><span data-stu-id="c92ea-163">Relationship</span></span> | <span data-ttu-id="c92ea-164">类型</span><span class="sxs-lookup"><span data-stu-id="c92ea-164">Type</span></span>   |<span data-ttu-id="c92ea-165">说明</span><span class="sxs-lookup"><span data-stu-id="c92ea-165">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c92ea-166">情况</span><span class="sxs-lookup"><span data-stu-id="c92ea-166">instance</span></span> |[<span data-ttu-id="c92ea-167">accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="c92ea-167">accessReviewInstance</span></span>](accessreviewinstance.md) | <span data-ttu-id="c92ea-168">与每个决策相关联的 accessReviewInstance 正好有一个。</span><span class="sxs-lookup"><span data-stu-id="c92ea-168">There is exactly one accessReviewInstance associated with each decision.</span></span> <span data-ttu-id="c92ea-169">该实例是决策项的父项，表示对进行决定的访问审核的重复。</span><span class="sxs-lookup"><span data-stu-id="c92ea-169">The instance is the parent of the decision item, representing the recurrence of the access review the decision is made on.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="c92ea-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c92ea-170">JSON representation</span></span>

<span data-ttu-id="c92ea-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c92ea-171">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem",
  "baseType": "",
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
