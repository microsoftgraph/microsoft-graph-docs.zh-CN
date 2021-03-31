---
title: accessReviewInstanceDecisionItem 资源类型
description: 表示有关用户访问 accessReviewInstance 的决定。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 968af49a9033ea749522132204d63b4f55ba25c7
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469239"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a><span data-ttu-id="008b3-103">accessReviewInstanceDecisionItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="008b3-103">accessReviewInstanceDecisionItem resource type</span></span>

<span data-ttu-id="008b3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="008b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

>[!NOTE]
><span data-ttu-id="008b3-105">属性 `target` 将在 v1.0 中弃用，并替换为 属性 `principal` 和 `resource` 。</span><span class="sxs-lookup"><span data-stu-id="008b3-105">The property `target` will be deprecated in v1.0 and replaced by properties `principal` and `resource`.</span></span>

<span data-ttu-id="008b3-106">表示有关审阅 [实例](accessreviewsv2-root.md) 的 Azure AD 访问评审决定。</span><span class="sxs-lookup"><span data-stu-id="008b3-106">Represents an Azure AD [access review](accessreviewsv2-root.md) decision on an instance of a review.</span></span> <span data-ttu-id="008b3-107">此决定表示确定用户或服务主体对给定访问评审实例 [的访问权限](accessreviewinstance.md)。</span><span class="sxs-lookup"><span data-stu-id="008b3-107">This decision represents the determination of a user or service principal's access for a given [access review instance](accessreviewinstance.md).</span></span>

## <a name="methods"></a><span data-ttu-id="008b3-108">方法</span><span class="sxs-lookup"><span data-stu-id="008b3-108">Methods</span></span>

| <span data-ttu-id="008b3-109">方法</span><span class="sxs-lookup"><span data-stu-id="008b3-109">Method</span></span> | <span data-ttu-id="008b3-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="008b3-110">Return Type</span></span> | <span data-ttu-id="008b3-111">说明</span><span class="sxs-lookup"><span data-stu-id="008b3-111">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="008b3-112">列出 accessReviewInstanceDecisionItems</span><span class="sxs-lookup"><span data-stu-id="008b3-112">List accessReviewInstanceDecisionItems</span></span>](../api/accessreviewinstancedecisionitem-list.md) | <span data-ttu-id="008b3-113">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="008b3-113">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection</span></span> | <span data-ttu-id="008b3-114">列出特定 accessReviewInstanceDecisionItem 的每个 accessReviewInstance。</span><span class="sxs-lookup"><span data-stu-id="008b3-114">Lists every accessReviewInstanceDecisionItem for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="008b3-115">列出 accessReviewInstanceDecisionItems 待审批</span><span class="sxs-lookup"><span data-stu-id="008b3-115">List accessReviewInstanceDecisionItems pending approval</span></span>](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | <span data-ttu-id="008b3-116">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="008b3-116">[accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) collection.</span></span> | <span data-ttu-id="008b3-117">获取分配给特定 accessReviewInstance 的调用用户的所有 accessReviewInstanceDecisionItems。</span><span class="sxs-lookup"><span data-stu-id="008b3-117">Get all accessReviewInstanceDecisionItems assigned to the calling user, for a specific accessReviewInstance.</span></span> |
|[<span data-ttu-id="008b3-118">更新 accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="008b3-118">Update accessReviewInstanceDecisionItem</span></span>](../api/accessreviewinstancedecisionitem-update.md) | <span data-ttu-id="008b3-119">无。</span><span class="sxs-lookup"><span data-stu-id="008b3-119">None.</span></span> | <span data-ttu-id="008b3-120">对于为调用用户分配审阅者的任何 accessReviewInstanceDecisionItems，调用用户可以通过修补决策对象来记录决策。</span><span class="sxs-lookup"><span data-stu-id="008b3-120">For any accessReviewInstanceDecisionItems that the calling user is assigned a reviewer on, calling user can record a decision by patching the decision object.</span></span> |

## <a name="properties"></a><span data-ttu-id="008b3-121">属性</span><span class="sxs-lookup"><span data-stu-id="008b3-121">Properties</span></span>
| <span data-ttu-id="008b3-122">属性</span><span class="sxs-lookup"><span data-stu-id="008b3-122">Property</span></span> | <span data-ttu-id="008b3-123">类型</span><span class="sxs-lookup"><span data-stu-id="008b3-123">Type</span></span> |  <span data-ttu-id="008b3-124">说明</span><span class="sxs-lookup"><span data-stu-id="008b3-124">Description</span></span> |
| :---------------| :---- | :---------- |
| <span data-ttu-id="008b3-125">id</span><span class="sxs-lookup"><span data-stu-id="008b3-125">id</span></span> | <span data-ttu-id="008b3-126">String</span><span class="sxs-lookup"><span data-stu-id="008b3-126">String</span></span> | <span data-ttu-id="008b3-127">决策的标识符。</span><span class="sxs-lookup"><span data-stu-id="008b3-127">The identifier of the decision.</span></span> |
| <span data-ttu-id="008b3-128">accessReviewId</span><span class="sxs-lookup"><span data-stu-id="008b3-128">accessReviewId</span></span> | <span data-ttu-id="008b3-129">String</span><span class="sxs-lookup"><span data-stu-id="008b3-129">String</span></span> | <span data-ttu-id="008b3-130">accessReviewInstance 父项的标识符。</span><span class="sxs-lookup"><span data-stu-id="008b3-130">The identifier of the accessReviewInstance parent.</span></span> |
| <span data-ttu-id="008b3-131">reviewedBy</span><span class="sxs-lookup"><span data-stu-id="008b3-131">reviewedBy</span></span> | [<span data-ttu-id="008b3-132">userIdentity</span><span class="sxs-lookup"><span data-stu-id="008b3-132">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="008b3-133">审阅者的标识符。</span><span class="sxs-lookup"><span data-stu-id="008b3-133">The identifier of the reviewer.</span></span> |
| <span data-ttu-id="008b3-134">reviewedDateTime</span><span class="sxs-lookup"><span data-stu-id="008b3-134">reviewedDateTime</span></span> | <span data-ttu-id="008b3-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="008b3-135">DateTimeOffset</span></span> | <span data-ttu-id="008b3-136">评价发生时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="008b3-136">The timestamp when the review occurred.</span></span> |
| <span data-ttu-id="008b3-137">decision</span><span class="sxs-lookup"><span data-stu-id="008b3-137">decision</span></span> | <span data-ttu-id="008b3-138">String</span><span class="sxs-lookup"><span data-stu-id="008b3-138">String</span></span> | <span data-ttu-id="008b3-139">评价的结果。</span><span class="sxs-lookup"><span data-stu-id="008b3-139">Result of the review.</span></span> <span data-ttu-id="008b3-140">可能的值 `Approve` `Deny` ：、、 `NotReviewed` 或 `DontKnow` 。</span><span class="sxs-lookup"><span data-stu-id="008b3-140">Possible values: `Approve`, `Deny`, `NotReviewed`, or `DontKnow`.</span></span> |
| <span data-ttu-id="008b3-141">justification</span><span class="sxs-lookup"><span data-stu-id="008b3-141">justification</span></span> | <span data-ttu-id="008b3-142">String</span><span class="sxs-lookup"><span data-stu-id="008b3-142">String</span></span> | <span data-ttu-id="008b3-143">审阅决策理由。</span><span class="sxs-lookup"><span data-stu-id="008b3-143">The review decision justification.</span></span> |
| <span data-ttu-id="008b3-144">appliedBy</span><span class="sxs-lookup"><span data-stu-id="008b3-144">appliedBy</span></span> | [<span data-ttu-id="008b3-145">userIdentity</span><span class="sxs-lookup"><span data-stu-id="008b3-145">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="008b3-146">应用了该决策的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="008b3-146">The identifier of the user who applied the decision.</span></span> |
| <span data-ttu-id="008b3-147">appliedDateTime</span><span class="sxs-lookup"><span data-stu-id="008b3-147">appliedDateTime</span></span> | <span data-ttu-id="008b3-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="008b3-148">DateTimeOffset</span></span> | <span data-ttu-id="008b3-149">应用批准决策的时间戳。</span><span class="sxs-lookup"><span data-stu-id="008b3-149">The timestamp when the approval decision was applied.</span></span> <span data-ttu-id="008b3-150">DatetimeOffset 类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="008b3-150">The DatetimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="008b3-151">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="008b3-151">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
| <span data-ttu-id="008b3-152">applyResult</span><span class="sxs-lookup"><span data-stu-id="008b3-152">applyResult</span></span> | <span data-ttu-id="008b3-153">String</span><span class="sxs-lookup"><span data-stu-id="008b3-153">String</span></span> | <span data-ttu-id="008b3-154">应用决策的结果。</span><span class="sxs-lookup"><span data-stu-id="008b3-154">The result of applying the decision.</span></span> <span data-ttu-id="008b3-155">可能的值 `NotApplied` `Success` `Failed` ：、、、 `NotFound` 或 `NotSupported` 。</span><span class="sxs-lookup"><span data-stu-id="008b3-155">Possible values: `NotApplied`, `Success`, `Failed`, `NotFound`, or `NotSupported`.</span></span> |
| <span data-ttu-id="008b3-156">建议</span><span class="sxs-lookup"><span data-stu-id="008b3-156">recommendation</span></span> | <span data-ttu-id="008b3-157">String</span><span class="sxs-lookup"><span data-stu-id="008b3-157">String</span></span> | <span data-ttu-id="008b3-158">针对审批决策的系统生成的建议。</span><span class="sxs-lookup"><span data-stu-id="008b3-158">A system-generated recommendation for the approval decision.</span></span> <span data-ttu-id="008b3-159">可能的值 `Approve` ：、 `Deny` 或 `NotAvailable` 。</span><span class="sxs-lookup"><span data-stu-id="008b3-159">Possible values: `Approve`, `Deny`, or `NotAvailable`.</span></span>  |
| <span data-ttu-id="008b3-160">target</span><span class="sxs-lookup"><span data-stu-id="008b3-160">target</span></span> | [<span data-ttu-id="008b3-161">accessReviewInstanceDecisionItemTarget</span><span class="sxs-lookup"><span data-stu-id="008b3-161">accessReviewInstanceDecisionItemTarget</span></span>](accessreviewinstancedecisionitemtarget.md)  | <span data-ttu-id="008b3-162">此特定决策的目标。</span><span class="sxs-lookup"><span data-stu-id="008b3-162">The target of this specific decision.</span></span> <span data-ttu-id="008b3-163">决策目标可以是不同类型的 ，每个类型都有其自己的特定属性。</span><span class="sxs-lookup"><span data-stu-id="008b3-163">Decision targets can be of different types – each one with its own specific properties.</span></span> <span data-ttu-id="008b3-164">请参阅 [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md)。</span><span class="sxs-lookup"><span data-stu-id="008b3-164">See [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md).</span></span> |
|<span data-ttu-id="008b3-165">principal</span><span class="sxs-lookup"><span data-stu-id="008b3-165">principal</span></span>|[<span data-ttu-id="008b3-166">identity</span><span class="sxs-lookup"><span data-stu-id="008b3-166">identity</span></span>](../resources/identity.md)|<span data-ttu-id="008b3-167">访问评审中的每个决策项表示主体对资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="008b3-167">Every decision item in an access review represents a principal's access to a resource.</span></span> <span data-ttu-id="008b3-168">此属性表示主体的详细信息。</span><span class="sxs-lookup"><span data-stu-id="008b3-168">This property represents details of the principal.</span></span> <span data-ttu-id="008b3-169">例如，如果某个决策项表示用户"Bob"对组"Sales"的访问权限 - 主体为"Bob"，资源为"Sales"。</span><span class="sxs-lookup"><span data-stu-id="008b3-169">For example, if a decision item represents access of User "Bob" to Group "Sales" - The principal is "Bob" and the resource is "Sales".</span></span> <span data-ttu-id="008b3-170">主体可以是两种类型 - userIdentity 和 servicePrincipalIdentity。</span><span class="sxs-lookup"><span data-stu-id="008b3-170">Principals can be of two types - userIdentity and servicePrincipalIdentity.</span></span>|
|<span data-ttu-id="008b3-171">resource</span><span class="sxs-lookup"><span data-stu-id="008b3-171">resource</span></span>|[<span data-ttu-id="008b3-172">accessReviewInstanceDecisionItemResource</span><span class="sxs-lookup"><span data-stu-id="008b3-172">accessReviewInstanceDecisionItemResource</span></span>](../resources/accessreviewinstancedecisionitemresource.md)|<span data-ttu-id="008b3-173">访问评审中的每个决策项表示主体对资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="008b3-173">Every decision item in an access review represents a principal's access to a resource.</span></span> <span data-ttu-id="008b3-174">此属性表示资源的详细信息。</span><span class="sxs-lookup"><span data-stu-id="008b3-174">This property represents details of the resource.</span></span> <span data-ttu-id="008b3-175">例如，如果决策项表示用户"Bob"对组"销售"的访问权限 - 主体为 Bob，资源为"Sales"。</span><span class="sxs-lookup"><span data-stu-id="008b3-175">For example, if a decision item represents access of User "Bob" to Group "Sales" - The principal is Bob and the resource is "Sales".</span></span> <span data-ttu-id="008b3-176">资源可以是多种类型的。</span><span class="sxs-lookup"><span data-stu-id="008b3-176">Resources can be of multiple types.</span></span> <span data-ttu-id="008b3-177">请参阅 [accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md)</span><span class="sxs-lookup"><span data-stu-id="008b3-177">See [accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="008b3-178">关系</span><span class="sxs-lookup"><span data-stu-id="008b3-178">Relationships</span></span>

| <span data-ttu-id="008b3-179">关系</span><span class="sxs-lookup"><span data-stu-id="008b3-179">Relationship</span></span> | <span data-ttu-id="008b3-180">类型</span><span class="sxs-lookup"><span data-stu-id="008b3-180">Type</span></span>   |<span data-ttu-id="008b3-181">说明</span><span class="sxs-lookup"><span data-stu-id="008b3-181">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="008b3-182">实例</span><span class="sxs-lookup"><span data-stu-id="008b3-182">instance</span></span> |[<span data-ttu-id="008b3-183">accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="008b3-183">accessReviewInstance</span></span>](accessreviewinstance.md) | <span data-ttu-id="008b3-184">每个决策只关联一个 accessReviewInstance。</span><span class="sxs-lookup"><span data-stu-id="008b3-184">There is exactly one accessReviewInstance associated with each decision.</span></span> <span data-ttu-id="008b3-185">实例是决策项的父项，代表做出该决策的访问评审的重复发生。</span><span class="sxs-lookup"><span data-stu-id="008b3-185">The instance is the parent of the decision item, representing the recurrence of the access review the decision is made on.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="008b3-186">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="008b3-186">JSON representation</span></span>

<span data-ttu-id="008b3-187">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="008b3-187">Here is a JSON representation of the resource.</span></span>

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
  "id": "String (identifier)",
  "accessReviewId": "String",
  "reviewedBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "reviewedDateTime": "String (timestamp)",
  "decision": "String",
  "justification": "String",
  "appliedBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "appliedDateTime": "String (timestamp)",
  "applyResult": "String",
  "recommendation": "String",
  "target": {
    "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemTarget"
  },
  "principal": {
    "@odata.type": "microsoft.graph.identity"
  },
  "resource": {
    "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemResource"
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
