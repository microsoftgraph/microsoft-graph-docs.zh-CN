---
title: accessReview 资源类型
description: '在 Azure AD 中访问审阅功能，`accessReview`代表访问审阅。  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a02cc7cfe74bf9f12c4e2a8568c764934cb0c842
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576344"
---
# <a name="accessreview-resource-type"></a><span data-ttu-id="9d013-103">accessReview 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d013-103">accessReview resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d013-104">在 Azure AD[访问审阅](accessreviews-root.md)功能中，`accessReview`代表访问审阅。</span><span class="sxs-lookup"><span data-stu-id="9d013-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the `accessReview` represents an access review.</span></span>  


## <a name="methods"></a><span data-ttu-id="9d013-105">方法</span><span class="sxs-lookup"><span data-stu-id="9d013-105">Methods</span></span>

| <span data-ttu-id="9d013-106">方法</span><span class="sxs-lookup"><span data-stu-id="9d013-106">Method</span></span>           | <span data-ttu-id="9d013-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="9d013-107">Return Type</span></span>    |<span data-ttu-id="9d013-108">说明</span><span class="sxs-lookup"><span data-stu-id="9d013-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9d013-109">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="9d013-109">Get accessReview</span></span>](../api/accessreview-get.md) |   [<span data-ttu-id="9d013-110">accessReview</span><span class="sxs-lookup"><span data-stu-id="9d013-110">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="9d013-111">获取与特定 id 访问审阅。</span><span class="sxs-lookup"><span data-stu-id="9d013-111">Get an access review with a specific id.</span></span> |
|[<span data-ttu-id="9d013-112">创建 accessReview</span><span class="sxs-lookup"><span data-stu-id="9d013-112">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="9d013-113">accessReview</span><span class="sxs-lookup"><span data-stu-id="9d013-113">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="9d013-114">创建新 accessReview。</span><span class="sxs-lookup"><span data-stu-id="9d013-114">Create a new accessReview.</span></span> |
|[<span data-ttu-id="9d013-115">删除 accessReview</span><span class="sxs-lookup"><span data-stu-id="9d013-115">Delete accessReview</span></span>](../api/accessreview-delete.md) | <span data-ttu-id="9d013-116">无。</span><span class="sxs-lookup"><span data-stu-id="9d013-116">None.</span></span>   | <span data-ttu-id="9d013-117">删除 accessReview。</span><span class="sxs-lookup"><span data-stu-id="9d013-117">Delete an accessReview.</span></span> |
|[<span data-ttu-id="9d013-118">更新 accessReview</span><span class="sxs-lookup"><span data-stu-id="9d013-118">Update accessReview</span></span>](../api/accessreview-update.md) | [<span data-ttu-id="9d013-119">accessReview</span><span class="sxs-lookup"><span data-stu-id="9d013-119">accessReview</span></span>](accessreview.md) | <span data-ttu-id="9d013-120">更新 accessReview。</span><span class="sxs-lookup"><span data-stu-id="9d013-120">Update an accessReview.</span></span> |
|[<span data-ttu-id="9d013-121">列表 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="9d013-121">List accessReview reviewers</span></span>](../api/accessreview-listreviewers.md) |      <span data-ttu-id="9d013-122">[userIdentity](useridentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="9d013-122">[userIdentity](useridentity.md) collection</span></span>| <span data-ttu-id="9d013-123">要获取 accessReview 审阅的者。</span><span class="sxs-lookup"><span data-stu-id="9d013-123">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="9d013-124">添加 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="9d013-124">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md) |      <span data-ttu-id="9d013-125">无。</span><span class="sxs-lookup"><span data-stu-id="9d013-125">None.</span></span>   |   <span data-ttu-id="9d013-126">将审阅者添加到 accessReview。</span><span class="sxs-lookup"><span data-stu-id="9d013-126">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="9d013-127">删除 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="9d013-127">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="9d013-128">无。</span><span class="sxs-lookup"><span data-stu-id="9d013-128">None.</span></span>  |   <span data-ttu-id="9d013-129">删除 accessReview 审阅者。</span><span class="sxs-lookup"><span data-stu-id="9d013-129">Remove a reviewer from an accessReview.</span></span> |
|[<span data-ttu-id="9d013-130">列表 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="9d013-130">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) |      <span data-ttu-id="9d013-131">[accessReviewDecision](accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="9d013-131">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="9d013-132">获取 accessReview 的决策。</span><span class="sxs-lookup"><span data-stu-id="9d013-132">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="9d013-133">列出我 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="9d013-133">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) |     <span data-ttu-id="9d013-134">[accessReviewDecision](accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="9d013-134">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="9d013-135">审阅者，以获取 accessReview 我决策。</span><span class="sxs-lookup"><span data-stu-id="9d013-135">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="9d013-136">发送 accessReview 提醒</span><span class="sxs-lookup"><span data-stu-id="9d013-136">Send accessReview reminder</span></span>](../api/accessreview-sendreminder.md) |        <span data-ttu-id="9d013-137">无。</span><span class="sxs-lookup"><span data-stu-id="9d013-137">None.</span></span>   |   <span data-ttu-id="9d013-138">向审阅者的 accessReview 发送提醒。</span><span class="sxs-lookup"><span data-stu-id="9d013-138">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="9d013-139">停止 accessReview</span><span class="sxs-lookup"><span data-stu-id="9d013-139">Stop accessReview</span></span>](../api/accessreview-stop.md) |     <span data-ttu-id="9d013-140">无。</span><span class="sxs-lookup"><span data-stu-id="9d013-140">None.</span></span>   |   <span data-ttu-id="9d013-141">停止 accessReview。</span><span class="sxs-lookup"><span data-stu-id="9d013-141">Stop an accessReview.</span></span> |
|[<span data-ttu-id="9d013-142">重置 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="9d013-142">Reset accessReview decisions</span></span>](../api/accessreview-reset.md) |     <span data-ttu-id="9d013-143">无。</span><span class="sxs-lookup"><span data-stu-id="9d013-143">None.</span></span>   |   <span data-ttu-id="9d013-144">重置正在进行 accessReview 决策。</span><span class="sxs-lookup"><span data-stu-id="9d013-144">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="9d013-145">应用 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="9d013-145">Apply accessReview decisions</span></span>](../api/accessreview-apply.md) |     <span data-ttu-id="9d013-146">无。</span><span class="sxs-lookup"><span data-stu-id="9d013-146">None.</span></span>   |   <span data-ttu-id="9d013-147">应用已完成 accessReview 从的决策。</span><span class="sxs-lookup"><span data-stu-id="9d013-147">Apply the decisions from a completed accessReview.</span></span>|

## <a name="permissions"></a><span data-ttu-id="9d013-148">权限</span><span class="sxs-lookup"><span data-stu-id="9d013-148">Permissions</span></span>

|<span data-ttu-id="9d013-149">权限类型</span><span class="sxs-lookup"><span data-stu-id="9d013-149">Permission type</span></span>                        | <span data-ttu-id="9d013-150">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9d013-150">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d013-151">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9d013-151">Delegated (work or school account)</span></span>     | <span data-ttu-id="9d013-152">AccessReview.Read.All AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d013-152">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="9d013-153">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9d013-153">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d013-154">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d013-154">Not supported.</span></span> |
|<span data-ttu-id="9d013-155">应用程序</span><span class="sxs-lookup"><span data-stu-id="9d013-155">Application</span></span>                            | <span data-ttu-id="9d013-156">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d013-156">Not supported.</span></span> |


## <a name="properties"></a><span data-ttu-id="9d013-157">属性</span><span class="sxs-lookup"><span data-stu-id="9d013-157">Properties</span></span>
| <span data-ttu-id="9d013-158">属性</span><span class="sxs-lookup"><span data-stu-id="9d013-158">Property</span></span>     | <span data-ttu-id="9d013-159">类型</span><span class="sxs-lookup"><span data-stu-id="9d013-159">Type</span></span>   |<span data-ttu-id="9d013-160">说明</span><span class="sxs-lookup"><span data-stu-id="9d013-160">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                      |`String`                                                        | <span data-ttu-id="9d013-161">功能分配的唯一标识符访问审阅。</span><span class="sxs-lookup"><span data-stu-id="9d013-161">The feature-assigned unique identifier of an access review.</span></span> |
| `displayName`             |`String`                                                        | <span data-ttu-id="9d013-162">访问审阅名称。</span><span class="sxs-lookup"><span data-stu-id="9d013-162">The access review name.</span></span> <span data-ttu-id="9d013-163">所需在创建。</span><span class="sxs-lookup"><span data-stu-id="9d013-163">Required on create.</span></span> |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="9d013-164">审阅安排在启动时 DateTime。</span><span class="sxs-lookup"><span data-stu-id="9d013-164">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="9d013-165">这可能是在将来的日期。</span><span class="sxs-lookup"><span data-stu-id="9d013-165">This could be a date in the future.</span></span>  <span data-ttu-id="9d013-166">所需在创建。</span><span class="sxs-lookup"><span data-stu-id="9d013-166">Required on create.</span></span> |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="9d013-167">审阅安排结束时 DateTime。</span><span class="sxs-lookup"><span data-stu-id="9d013-167">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="9d013-168">这必须是至少一个日期晚于开始日期。</span><span class="sxs-lookup"><span data-stu-id="9d013-168">This must be at least one day later than the start date.</span></span>  <span data-ttu-id="9d013-169">所需在创建。</span><span class="sxs-lookup"><span data-stu-id="9d013-169">Required on create.</span></span> |
| `status`                  |`String`                                                        | <span data-ttu-id="9d013-170">此只读字段指定 accessReview 的状态。</span><span class="sxs-lookup"><span data-stu-id="9d013-170">This read-only field specifies the status of an accessReview.</span></span> <span data-ttu-id="9d013-171">典型的状态包括`Initializing`， `NotStarted`， `Starting`，`InProgress`， `Completing`， `Completed`， `AutoReviewing`，和`AutoReviewed`。</span><span class="sxs-lookup"><span data-stu-id="9d013-171">The typical states include `Initializing`, `NotStarted`, `Starting`,`InProgress`, `Completing`, `Completed`, `AutoReviewing`, and `AutoReviewed`.</span></span> |
| `description`             |`String`                                                        | <span data-ttu-id="9d013-172">访问审阅创建者提供，向审阅者显示说明。</span><span class="sxs-lookup"><span data-stu-id="9d013-172">The description provided by the access review creator, to show to the reviewers.</span></span> |
| `businessFlowTemplateId`  |`String`                                                        | <span data-ttu-id="9d013-173">业务流程模板标识符。</span><span class="sxs-lookup"><span data-stu-id="9d013-173">The business flow template identifier.</span></span> <span data-ttu-id="9d013-174">所需在创建。</span><span class="sxs-lookup"><span data-stu-id="9d013-174">Required on create.</span></span> |
| `reviewerType`            |`String`                                                        | <span data-ttu-id="9d013-175">对目标对象，之一的审阅者的关系类型`self`，`delegated`或`entityOwners`。</span><span class="sxs-lookup"><span data-stu-id="9d013-175">The relationship type of reviewer to the target object, one of `self`, `delegated` or `entityOwners`.</span></span> <span data-ttu-id="9d013-176">所需在创建。</span><span class="sxs-lookup"><span data-stu-id="9d013-176">Required on create.</span></span> | 
| `createdBy`               |[<span data-ttu-id="9d013-177">userIdentity</span><span class="sxs-lookup"><span data-stu-id="9d013-177">userIdentity</span></span>](useridentity.md)                                 | <span data-ttu-id="9d013-178">创建此审查的用户。</span><span class="sxs-lookup"><span data-stu-id="9d013-178">The user who created this review.</span></span> |
| `reviewedEntity`          |`microsoft.graph.identity`                                      | <span data-ttu-id="9d013-179">为其 access 会检查该对象查看的访问权限分配。</span><span class="sxs-lookup"><span data-stu-id="9d013-179">The object for which the access reviews is reviewing the access rights assignments.</span></span> <span data-ttu-id="9d013-180">这可以在组中，用户组的成员身份的审阅或应用程序的用户迁移到应用程序的工作分配回顾。</span><span class="sxs-lookup"><span data-stu-id="9d013-180">This can be the group for the review of memberships of users in a group, or the app for a review of assignments of users to an application.</span></span> <span data-ttu-id="9d013-181">所需在创建。</span><span class="sxs-lookup"><span data-stu-id="9d013-181">Required on create.</span></span> | 
| `settings`                |`microsoft.graph.accessReviewSettings`             | <span data-ttu-id="9d013-182">AccessReview 的设置，，请参阅下面的类型定义。</span><span class="sxs-lookup"><span data-stu-id="9d013-182">The settings of an accessReview, see type definition below.</span></span> |



## <a name="relationships"></a><span data-ttu-id="9d013-183">关系</span><span class="sxs-lookup"><span data-stu-id="9d013-183">Relationships</span></span>




| <span data-ttu-id="9d013-184">关系</span><span class="sxs-lookup"><span data-stu-id="9d013-184">Relationship</span></span> | <span data-ttu-id="9d013-185">类型</span><span class="sxs-lookup"><span data-stu-id="9d013-185">Type</span></span>   |<span data-ttu-id="9d013-186">说明</span><span class="sxs-lookup"><span data-stu-id="9d013-186">Description</span></span>|
|:---------------|:--------|:----------|
| `reviewers`               |<span data-ttu-id="9d013-187">[userIdentity](useridentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="9d013-187">[userIdentity](useridentity.md) collection</span></span>                     | <span data-ttu-id="9d013-188">访问审阅，如果访问审阅 reviewerType 的类型的审阅者的集合`delegate`。</span><span class="sxs-lookup"><span data-stu-id="9d013-188">The collection of reviewers for an access review, if access review reviewerType is of type `delegate`.</span></span> |
| `decisions`               |<span data-ttu-id="9d013-189">[accessReviewDecision](accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="9d013-189">[accessReviewDecision](accessreviewdecision.md) collection</span></span> | <span data-ttu-id="9d013-190">此访问审查的决策的集合。</span><span class="sxs-lookup"><span data-stu-id="9d013-190">The collection of decisions for this access review.</span></span> |
| `myDecisions`             |<span data-ttu-id="9d013-191">[accessReviewDecision](accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="9d013-191">[accessReviewDecision](accessreviewdecision.md) collection</span></span> | <span data-ttu-id="9d013-192">呼叫者，呼叫者是否审阅者的决策的集合。</span><span class="sxs-lookup"><span data-stu-id="9d013-192">The collection of decisions for the caller, if the caller is a reviewer.</span></span> |
| `instances`               |<span data-ttu-id="9d013-193">[accessReview](accessreview.md)集合</span><span class="sxs-lookup"><span data-stu-id="9d013-193">[accessReview](accessreview.md) collection</span></span>         | <span data-ttu-id="9d013-194">访问评论一实例过去、 存在和未来，如果此对象是定期访问回顾。</span><span class="sxs-lookup"><span data-stu-id="9d013-194">The collection of access reviews instances past, present and future, if this object is a recurring access review.</span></span> |

<span data-ttu-id="9d013-195">是否在对象上存在这些关系，取决于对象是否是一次性访问回顾、 的一系列定期访问审阅或定期访问回顾的实例。</span><span class="sxs-lookup"><span data-stu-id="9d013-195">Whether these relationships are present on an object, depends upon whether the object is a one-time access review, the series of a recurring access review, or an instance of a recurring access review.</span></span>

| <span data-ttu-id="9d013-196">应用场景</span><span class="sxs-lookup"><span data-stu-id="9d013-196">Scenario</span></span> | <span data-ttu-id="9d013-197">有审阅者？</span><span class="sxs-lookup"><span data-stu-id="9d013-197">Has reviewers?</span></span> | <span data-ttu-id="9d013-198">具有决策和 myDecisions？</span><span class="sxs-lookup"><span data-stu-id="9d013-198">Has decisions and myDecisions?</span></span> | <span data-ttu-id="9d013-199">具有实例？</span><span class="sxs-lookup"><span data-stu-id="9d013-199">Has instances?</span></span> |
|:---------|:---------------|:---------------|:---------------|
|<span data-ttu-id="9d013-200">一次性访问审阅</span><span class="sxs-lookup"><span data-stu-id="9d013-200">One-time access review</span></span>|<span data-ttu-id="9d013-201">是</span><span class="sxs-lookup"><span data-stu-id="9d013-201">Yes</span></span> | <span data-ttu-id="9d013-202">是，一次启动</span><span class="sxs-lookup"><span data-stu-id="9d013-202">Yes, once started</span></span> | <span data-ttu-id="9d013-203">否</span><span class="sxs-lookup"><span data-stu-id="9d013-203">No</span></span> |
| <span data-ttu-id="9d013-204">定期访问审阅</span><span class="sxs-lookup"><span data-stu-id="9d013-204">Recurring access review</span></span> | <span data-ttu-id="9d013-205">是</span><span class="sxs-lookup"><span data-stu-id="9d013-205">Yes</span></span> | <span data-ttu-id="9d013-206">否</span><span class="sxs-lookup"><span data-stu-id="9d013-206">No</span></span> | <span data-ttu-id="9d013-207">是</span><span class="sxs-lookup"><span data-stu-id="9d013-207">Yes</span></span> |
| <span data-ttu-id="9d013-208">定期访问回顾的实例</span><span class="sxs-lookup"><span data-stu-id="9d013-208">Instance of a recurring access review</span></span> | <span data-ttu-id="9d013-209">是</span><span class="sxs-lookup"><span data-stu-id="9d013-209">Yes</span></span> | <span data-ttu-id="9d013-210">是，一次启动</span><span class="sxs-lookup"><span data-stu-id="9d013-210">Yes, once started</span></span> | <span data-ttu-id="9d013-211">否</span><span class="sxs-lookup"><span data-stu-id="9d013-211">No</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9d013-212">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d013-212">JSON representation</span></span>

<span data-ttu-id="9d013-213">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d013-213">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessReview"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string",
 "startDateTime": "string (timestamp)",
 "endDateTime": "string (timestamp)",
 "status": "string",
 "description": "string",
 "businessFlowTemplateId": "string (identifier)",
 "reviewerType": "string",
 "createdBy": "microsoft.graph.useridentity",
 "reviewedEntity": "microsoft.graph.entity",
 "settings": "microsoft.graph.entity",
 "reviewers": [ { "@odata.type": "#microsoft.graph.useridentity" } ]
}

```

## <a name="the-accessreviewsettings-type"></a><span data-ttu-id="9d013-214">AccessReviewSettings 类型</span><span class="sxs-lookup"><span data-stu-id="9d013-214">The accessReviewSettings type</span></span>

<span data-ttu-id="9d013-215">`accessReviewSettings`创建访问检查，以控制时开始访问审阅功能行为时提供其他设置。</span><span class="sxs-lookup"><span data-stu-id="9d013-215">The `accessReviewSettings` provides additional settings when creating an access review, to control the feature behavior when starting an access review.</span></span>  <span data-ttu-id="9d013-216">此类型具有以下属性：</span><span class="sxs-lookup"><span data-stu-id="9d013-216">This type has the following properties:</span></span> 

| <span data-ttu-id="9d013-217">属性</span><span class="sxs-lookup"><span data-stu-id="9d013-217">Property</span></span>                     | <span data-ttu-id="9d013-218">类型</span><span class="sxs-lookup"><span data-stu-id="9d013-218">Type</span></span>                      | <span data-ttu-id="9d013-219">说明</span><span class="sxs-lookup"><span data-stu-id="9d013-219">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| `mailNotificationsEnabled`|`Boolean`                | <span data-ttu-id="9d013-220">用于指示是否启用将邮件发送给审阅者和审阅创建者的标志。</span><span class="sxs-lookup"><span data-stu-id="9d013-220">Flag to indicate whether sending mails to reviewers and the review creator is enabled.</span></span>                |
| `remindersEnabled`|`Boolean`       | <span data-ttu-id="9d013-221">用于指示是否启用发送给审阅者的提醒电子邮件标志。</span><span class="sxs-lookup"><span data-stu-id="9d013-221">Flag to indicate whether sending reminder emails to reviewers are enabled.</span></span>       |
| `justificationRequiredOnApproval`|`Boolean` | <span data-ttu-id="9d013-222">用于指示审阅者是否需要提供理由审阅访问时的标志。</span><span class="sxs-lookup"><span data-stu-id="9d013-222">Flag to indicate whether reviewers are required to provide a justification when reviewing access.</span></span>|
| `activityDurationInDays`|`Int64` | <span data-ttu-id="9d013-223">用户活动以向审阅者显示的天数。</span><span class="sxs-lookup"><span data-stu-id="9d013-223">The number of days of user activities to show to reviewers.</span></span> |
| `autoReviewEnabled`|`Boolean` | <span data-ttu-id="9d013-224">启用标志以指示是否审阅者未提供一个用于 auto-apply，该功能是否应设置决定。</span><span class="sxs-lookup"><span data-stu-id="9d013-224">Flag to indicate whether the feature should set a decision if the reviewer did not supply one, for use with auto-apply, is enabled.</span></span> |
| `autoReviewSettings`|`microsoft.graph.autoReviewSettings` | <span data-ttu-id="9d013-225">功能设置的审阅决策，用于 auto-apply，如下所述的方式的详细的设置。</span><span class="sxs-lookup"><span data-stu-id="9d013-225">Detailed settings for how the feature should set the review decision, for use with auto-apply, described below.</span></span> |
| `recurrenceSettings`|`microsoft.graph.accessReviewRecurrenceSettings` | <span data-ttu-id="9d013-226">详细的定期，如下所述的设置。</span><span class="sxs-lookup"><span data-stu-id="9d013-226">Detailed settings for recurrence, described below.</span></span> |
| `autoApplyReviewResultsEnabled`|`Boolean` | <span data-ttu-id="9d013-227">标志，指示是否自动应用启用功能，自动更改目标对象访问资源。</span><span class="sxs-lookup"><span data-stu-id="9d013-227">Flag to indicate whether auto-apply capability, to automatically change the target object access resource, is enabled.</span></span>  <span data-ttu-id="9d013-228">如果未启用，用户必须审阅完成后，应用访问审阅。</span><span class="sxs-lookup"><span data-stu-id="9d013-228">If not enabled, a user must, after the review completes, apply the access review.</span></span> |
| `accessRecommendationsEnabled`|`Boolean` | <span data-ttu-id="9d013-229">用于指示是否启用向审阅者显示建议的标志。</span><span class="sxs-lookup"><span data-stu-id="9d013-229">Flag to indicate whether showing recommendations to reviewers is enabled.</span></span> |



## <a name="the-autoreviewsettings-type"></a><span data-ttu-id="9d013-230">AutoReviewSettings 类型</span><span class="sxs-lookup"><span data-stu-id="9d013-230">The autoReviewSettings type</span></span>

<span data-ttu-id="9d013-231">`autoReviewSettings`嵌入访问查看设置，并访问查看完成时指定功能的行为。</span><span class="sxs-lookup"><span data-stu-id="9d013-231">The `autoReviewSettings` is embedded within the access review settings, and specifies the behavior for the feature when an access review completes.</span></span>  <span data-ttu-id="9d013-232">该类型具有一个属性， `notReviewedResult`。</span><span class="sxs-lookup"><span data-stu-id="9d013-232">The type has one property, `notReviewedResult`.</span></span>

| <span data-ttu-id="9d013-233">属性</span><span class="sxs-lookup"><span data-stu-id="9d013-233">Property</span></span>                     | <span data-ttu-id="9d013-234">类型</span><span class="sxs-lookup"><span data-stu-id="9d013-234">Type</span></span>     | <span data-ttu-id="9d013-235">说明</span><span class="sxs-lookup"><span data-stu-id="9d013-235">Description</span></span>                          |
| :--------------------------- | :------  | :----------                          |
| `notReviewedResult`          |`String`  | <span data-ttu-id="9d013-236">必须为 `Approve`、`Deny` 或 `Recommendation` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="9d013-236">Must be one of `Approve`, `Deny`, or `Recommendation`.</span></span> |


## <a name="the-accessreviewrecurrencesettings-type"></a><span data-ttu-id="9d013-237">AccessReviewRecurrenceSettings 类型</span><span class="sxs-lookup"><span data-stu-id="9d013-237">The accessReviewRecurrenceSettings type</span></span>

<span data-ttu-id="9d013-238">`accessReviewRecurrenceSettings`嵌入访问查看设置，并指定访问审阅重复的时间间隔定期。</span><span class="sxs-lookup"><span data-stu-id="9d013-238">The `accessReviewRecurrenceSettings` is embedded within the access review settings, and specifies that the access review recurs at regular intervals.</span></span>  <span data-ttu-id="9d013-239">此类型具有以下属性：</span><span class="sxs-lookup"><span data-stu-id="9d013-239">This type has the following properties:</span></span>

| <span data-ttu-id="9d013-240">属性</span><span class="sxs-lookup"><span data-stu-id="9d013-240">Property</span></span>                     | <span data-ttu-id="9d013-241">类型</span><span class="sxs-lookup"><span data-stu-id="9d013-241">Type</span></span>                                                                                                          | <span data-ttu-id="9d013-242">说明</span><span class="sxs-lookup"><span data-stu-id="9d013-242">Description</span></span> |
| :--------------------------- | :------------------------------------------------------------------------------------------------------------ | :---------- |
| `recurrenceType`|`String`    | <span data-ttu-id="9d013-243">重复出现的间隔，其必须是下列之一的`onetime`， `weekly`， `monthly`， `quarterly`，或`annual`。</span><span class="sxs-lookup"><span data-stu-id="9d013-243">The recurrence interval, which must be one of `onetime`, `weekly`, `monthly`, `quarterly`, or `annual`.</span></span>                                                                   |
| `recurrenceEndType`|`String` | <span data-ttu-id="9d013-244">如何定期结束。</span><span class="sxs-lookup"><span data-stu-id="9d013-244">How the recurrence ends.</span></span> <span data-ttu-id="9d013-245">如果`Never`，然后没有重复系列没有明确结束。</span><span class="sxs-lookup"><span data-stu-id="9d013-245">If it is `Never`, then there is no explicit end of the recurrence series.</span></span> <span data-ttu-id="9d013-246">如果`endBy`，然后将定期结束于某个日期。</span><span class="sxs-lookup"><span data-stu-id="9d013-246">If it is `endBy`, then the recurrence ends at a certain date.</span></span> <span data-ttu-id="9d013-247">如果`occurrences`，然后系列结束后`recurrentCount`审阅的实例完成。</span><span class="sxs-lookup"><span data-stu-id="9d013-247">If it is `occurrences`, then the series ends after `recurrentCount` instances of the review have completed.</span></span> |
| `durationInDays`|`Int32`     | <span data-ttu-id="9d013-248">持续的定期的天数。</span><span class="sxs-lookup"><span data-stu-id="9d013-248">The duration in days for recurrence.</span></span>                                                                              |
| `recurrenceCount`|`Int32`    | <span data-ttu-id="9d013-249">定期事件的计数如果的值`recurrenceEndType`是`occurrences`，否则为 0 或。</span><span class="sxs-lookup"><span data-stu-id="9d013-249">The count of recurrences, if the value of `recurrenceEndType` is `occurrences`, or 0 otherwise.</span></span>                                                        |



<!--
{
  "type": "#page.annotation",
  "description": "accessReview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/accessreview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
