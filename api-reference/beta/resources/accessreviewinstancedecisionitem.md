---
title: accessReviewInstanceDecisionItem 资源类型
description: 表示有关用户访问 accessReviewInstance 的决定。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e5d9b64faafb7dfe4ec4e6f3487643e62885236a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952814"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a><span data-ttu-id="88ea0-103">accessReviewInstanceDecisionItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="88ea0-103">accessReviewInstanceDecisionItem resource type</span></span>

<span data-ttu-id="88ea0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88ea0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="88ea0-105">表示有关审阅 [实例](accessreviewsv2-root.md) 的 Azure AD 访问评审决定。</span><span class="sxs-lookup"><span data-stu-id="88ea0-105">Represents an Azure AD [access review](accessreviewsv2-root.md) decision on an instance of a review.</span></span> <span data-ttu-id="88ea0-106">此决定表示确定用户或服务主体对给定访问评审实例 [的访问权限](accessreviewinstance.md)。</span><span class="sxs-lookup"><span data-stu-id="88ea0-106">This decision represents the determination of a user or service principal's access for a given [access review instance](accessreviewinstance.md).</span></span>

## <a name="methods"></a><span data-ttu-id="88ea0-107">Methods</span><span class="sxs-lookup"><span data-stu-id="88ea0-107">Methods</span></span>

| <span data-ttu-id="88ea0-108">方法</span><span class="sxs-lookup"><span data-stu-id="88ea0-108">Method</span></span> | <span data-ttu-id="88ea0-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="88ea0-109">Return Type</span></span> | <span data-ttu-id="88ea0-110">说明</span><span class="sxs-lookup"><span data-stu-id="88ea0-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="88ea0-111">列出 accessReviewInstanceDecisionItems</span><span class="sxs-lookup"><span data-stu-id="88ea0-111">List accessReviewInstanceDecisionItems</span></span>](../api/accessreviewinstancedecisionitem-list.md) | <span data-ttu-id="88ea0-112">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="88ea0-112">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span></span> | <span data-ttu-id="88ea0-113">列出特定 accessReviewInstanceDecisionItem 的每个 accessReviewInstance。</span><span class="sxs-lookup"><span data-stu-id="88ea0-113">Lists every accessReviewInstanceDecisionItem for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="88ea0-114">列出 accessReviewInstanceDecisionItems 待审批</span><span class="sxs-lookup"><span data-stu-id="88ea0-114">List accessReviewInstanceDecisionItems pending approval</span></span>](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | <span data-ttu-id="88ea0-115">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="88ea0-115">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection.</span></span> | <span data-ttu-id="88ea0-116">获取分配给特定 accessReviewInstance 的调用用户的所有 accessReviewInstanceDecisionItems。</span><span class="sxs-lookup"><span data-stu-id="88ea0-116">Get all accessReviewInstanceDecisionItems assigned to the calling user, for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="88ea0-117">更新 accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="88ea0-117">Update accessReviewInstanceDecisionItem</span></span>](../api/accessreviewinstancedecisionitem-update.md) | <span data-ttu-id="88ea0-118">无。</span><span class="sxs-lookup"><span data-stu-id="88ea0-118">None.</span></span> | <span data-ttu-id="88ea0-119">对于为调用用户分配审阅者的任何 accessReviewInstanceDecisionItems，调用用户可以通过修补决策对象来记录决策。</span><span class="sxs-lookup"><span data-stu-id="88ea0-119">For any accessReviewInstanceDecisionItems that the calling user is assigned a reviewer on, calling user can record a decision by patching the decision object.</span></span> |

## <a name="properties"></a><span data-ttu-id="88ea0-120">属性</span><span class="sxs-lookup"><span data-stu-id="88ea0-120">Properties</span></span>
| <span data-ttu-id="88ea0-121">属性</span><span class="sxs-lookup"><span data-stu-id="88ea0-121">Property</span></span> | <span data-ttu-id="88ea0-122">类型</span><span class="sxs-lookup"><span data-stu-id="88ea0-122">Type</span></span> |  <span data-ttu-id="88ea0-123">说明</span><span class="sxs-lookup"><span data-stu-id="88ea0-123">Description</span></span> |
| :---------------| :---- | :---------- |
| <span data-ttu-id="88ea0-124">id</span><span class="sxs-lookup"><span data-stu-id="88ea0-124">id</span></span> | <span data-ttu-id="88ea0-125">String</span><span class="sxs-lookup"><span data-stu-id="88ea0-125">String</span></span> | <span data-ttu-id="88ea0-126">决策的标识符。</span><span class="sxs-lookup"><span data-stu-id="88ea0-126">The identifier of the decision.</span></span> |
| <span data-ttu-id="88ea0-127">accessReviewId</span><span class="sxs-lookup"><span data-stu-id="88ea0-127">accessReviewId</span></span> | <span data-ttu-id="88ea0-128">String</span><span class="sxs-lookup"><span data-stu-id="88ea0-128">String</span></span> | <span data-ttu-id="88ea0-129">accessReviewInstance 父项的标识符。</span><span class="sxs-lookup"><span data-stu-id="88ea0-129">The identifier of the accessReviewInstance parent.</span></span> |
| <span data-ttu-id="88ea0-130">reviewedBy</span><span class="sxs-lookup"><span data-stu-id="88ea0-130">reviewedBy</span></span> | [<span data-ttu-id="88ea0-131">userIdentity</span><span class="sxs-lookup"><span data-stu-id="88ea0-131">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="88ea0-132">审阅者的标识符。</span><span class="sxs-lookup"><span data-stu-id="88ea0-132">The identifier of the reviewer.</span></span> |
| <span data-ttu-id="88ea0-133">reviewedDateTime</span><span class="sxs-lookup"><span data-stu-id="88ea0-133">reviewedDateTime</span></span> | <span data-ttu-id="88ea0-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88ea0-134">DateTimeOffset</span></span> | <span data-ttu-id="88ea0-135">评价发生时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="88ea0-135">The timestamp when the review occurred.</span></span> |
| <span data-ttu-id="88ea0-136">decision</span><span class="sxs-lookup"><span data-stu-id="88ea0-136">decision</span></span> | <span data-ttu-id="88ea0-137">String</span><span class="sxs-lookup"><span data-stu-id="88ea0-137">String</span></span> | <span data-ttu-id="88ea0-138">评价的结果。</span><span class="sxs-lookup"><span data-stu-id="88ea0-138">Result of the review.</span></span> <span data-ttu-id="88ea0-139">可能的值 `Approve` `Deny` ：、、 `NotReviewed` 或 `DontKnow` 。</span><span class="sxs-lookup"><span data-stu-id="88ea0-139">Possible values: `Approve`, `Deny`, `NotReviewed`, or `DontKnow`.</span></span> |
| <span data-ttu-id="88ea0-140">justification</span><span class="sxs-lookup"><span data-stu-id="88ea0-140">justification</span></span> | <span data-ttu-id="88ea0-141">String</span><span class="sxs-lookup"><span data-stu-id="88ea0-141">String</span></span> | <span data-ttu-id="88ea0-142">审阅决策理由。</span><span class="sxs-lookup"><span data-stu-id="88ea0-142">The review decision justification.</span></span> |
| <span data-ttu-id="88ea0-143">appliedBy</span><span class="sxs-lookup"><span data-stu-id="88ea0-143">appliedBy</span></span> | [<span data-ttu-id="88ea0-144">userIdentity</span><span class="sxs-lookup"><span data-stu-id="88ea0-144">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="88ea0-145">应用了该决策的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="88ea0-145">The identifier of the user who applied the decision.</span></span> |
| <span data-ttu-id="88ea0-146">appliedDateTime</span><span class="sxs-lookup"><span data-stu-id="88ea0-146">appliedDateTime</span></span> | <span data-ttu-id="88ea0-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88ea0-147">DateTimeOffset</span></span> | <span data-ttu-id="88ea0-148">应用批准决策的时间戳。</span><span class="sxs-lookup"><span data-stu-id="88ea0-148">The timestamp when the approval decision was applied.</span></span> <span data-ttu-id="88ea0-149">DatetimeOffset 类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="88ea0-149">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="88ea0-150">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="88ea0-150">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
| <span data-ttu-id="88ea0-151">applyResult</span><span class="sxs-lookup"><span data-stu-id="88ea0-151">applyResult</span></span> | <span data-ttu-id="88ea0-152">String</span><span class="sxs-lookup"><span data-stu-id="88ea0-152">String</span></span> | <span data-ttu-id="88ea0-153">应用决策的结果。</span><span class="sxs-lookup"><span data-stu-id="88ea0-153">The result of applying the decision.</span></span> <span data-ttu-id="88ea0-154">可能的值 `NotApplied` `Success` `Failed` ：、、、 `NotFound` 或 `NotSupported` 。</span><span class="sxs-lookup"><span data-stu-id="88ea0-154">Possible values: `NotApplied`, `Success`, `Failed`, `NotFound`, or `NotSupported`.</span></span> |
| <span data-ttu-id="88ea0-155">建议</span><span class="sxs-lookup"><span data-stu-id="88ea0-155">recommendation</span></span> | <span data-ttu-id="88ea0-156">String</span><span class="sxs-lookup"><span data-stu-id="88ea0-156">String</span></span> | <span data-ttu-id="88ea0-157">针对审批决策的系统生成的建议。</span><span class="sxs-lookup"><span data-stu-id="88ea0-157">A system-generated recommendation for the approval decision.</span></span> <span data-ttu-id="88ea0-158">可能的值 `Approve` ：、 `Deny` 或 `NotAvailable` 。</span><span class="sxs-lookup"><span data-stu-id="88ea0-158">Possible values: `Approve`, `Deny`, or `NotAvailable`.</span></span>  |
| <span data-ttu-id="88ea0-159">target</span><span class="sxs-lookup"><span data-stu-id="88ea0-159">target</span></span> | [<span data-ttu-id="88ea0-160">accessReviewInstanceDecisionItemTarget</span><span class="sxs-lookup"><span data-stu-id="88ea0-160">accessReviewInstanceDecisionItemTarget</span></span>](accessreviewinstancedecisionitemtarget.md)  | <span data-ttu-id="88ea0-161">此特定决策的目标。</span><span class="sxs-lookup"><span data-stu-id="88ea0-161">The target of this specific decision.</span></span> <span data-ttu-id="88ea0-162">决策目标可以是不同类型的 ，每个类型都有其自己的特定属性。</span><span class="sxs-lookup"><span data-stu-id="88ea0-162">Decision targets can be of different types – each one with its own specific properties.</span></span> <span data-ttu-id="88ea0-163">请参阅 [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md)。</span><span class="sxs-lookup"><span data-stu-id="88ea0-163">See [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="88ea0-164">关系</span><span class="sxs-lookup"><span data-stu-id="88ea0-164">Relationships</span></span>

| <span data-ttu-id="88ea0-165">关系</span><span class="sxs-lookup"><span data-stu-id="88ea0-165">Relationship</span></span> | <span data-ttu-id="88ea0-166">类型</span><span class="sxs-lookup"><span data-stu-id="88ea0-166">Type</span></span>   |<span data-ttu-id="88ea0-167">说明</span><span class="sxs-lookup"><span data-stu-id="88ea0-167">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="88ea0-168">实例</span><span class="sxs-lookup"><span data-stu-id="88ea0-168">instance</span></span> |[<span data-ttu-id="88ea0-169">accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="88ea0-169">accessReviewInstance</span></span>](accessreviewinstance.md) | <span data-ttu-id="88ea0-170">每个决策只关联一个 accessReviewInstance。</span><span class="sxs-lookup"><span data-stu-id="88ea0-170">There is exactly one accessReviewInstance associated with each decision.</span></span> <span data-ttu-id="88ea0-171">实例是决策项的父项，代表做出该决策的访问评审的重复发生。</span><span class="sxs-lookup"><span data-stu-id="88ea0-171">The instance is the parent of the decision item, representing the recurrence of the access review the decision is made on.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="88ea0-172">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="88ea0-172">JSON representation</span></span>

<span data-ttu-id="88ea0-173">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88ea0-173">Here is a JSON representation of the resource.</span></span>

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
