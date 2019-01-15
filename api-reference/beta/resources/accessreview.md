---
title: accessReview 资源类型
description: '在 Azure AD 中访问审阅功能，`accessReview`代表访问审阅。  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e9099b1ec55a8ed017f77757d527abbd7e45bdf6
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016735"
---
# <a name="accessreview-resource-type"></a><span data-ttu-id="e4c9a-103">accessReview 资源类型</span><span class="sxs-lookup"><span data-stu-id="e4c9a-103">accessReview resource type</span></span>

> <span data-ttu-id="e4c9a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4c9a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e4c9a-106">在 Azure AD[访问审阅](accessreviews-root.md)功能中，`accessReview`代表访问审阅。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-106">In the Azure AD [access reviews](accessreviews-root.md) feature, the `accessReview` represents an access review.</span></span>  


## <a name="methods"></a><span data-ttu-id="e4c9a-107">方法</span><span class="sxs-lookup"><span data-stu-id="e4c9a-107">Methods</span></span>

| <span data-ttu-id="e4c9a-108">方法</span><span class="sxs-lookup"><span data-stu-id="e4c9a-108">Method</span></span>           | <span data-ttu-id="e4c9a-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e4c9a-109">Return Type</span></span>    |<span data-ttu-id="e4c9a-110">说明</span><span class="sxs-lookup"><span data-stu-id="e4c9a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e4c9a-111">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="e4c9a-111">Get accessReview</span></span>](../api/accessreview-get.md) |   [<span data-ttu-id="e4c9a-112">accessReview</span><span class="sxs-lookup"><span data-stu-id="e4c9a-112">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="e4c9a-113">获取与特定 id 访问审阅。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-113">Get an access review with a specific id.</span></span> |
|[<span data-ttu-id="e4c9a-114">创建 accessReview</span><span class="sxs-lookup"><span data-stu-id="e4c9a-114">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="e4c9a-115">accessReview</span><span class="sxs-lookup"><span data-stu-id="e4c9a-115">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="e4c9a-116">创建新 accessReview。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-116">Create a new accessReview.</span></span> |
|[<span data-ttu-id="e4c9a-117">删除 accessReview</span><span class="sxs-lookup"><span data-stu-id="e4c9a-117">Delete accessReview</span></span>](../api/accessreview-delete.md) | <span data-ttu-id="e4c9a-118">无。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-118">None.</span></span>   | <span data-ttu-id="e4c9a-119">删除 accessReview。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-119">Delete an accessReview.</span></span> |
|[<span data-ttu-id="e4c9a-120">更新 accessReview</span><span class="sxs-lookup"><span data-stu-id="e4c9a-120">Update accessReview</span></span>](../api/accessreview-update.md) | [<span data-ttu-id="e4c9a-121">accessReview</span><span class="sxs-lookup"><span data-stu-id="e4c9a-121">accessReview</span></span>](accessreview.md) | <span data-ttu-id="e4c9a-122">更新 accessReview。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-122">Update an accessReview.</span></span> |
|[<span data-ttu-id="e4c9a-123">列表 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="e4c9a-123">List accessReview reviewers</span></span>](../api/accessreview-listreviewers.md) |      <span data-ttu-id="e4c9a-124">[userIdentity](useridentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="e4c9a-124">[userIdentity](useridentity.md) collection</span></span>| <span data-ttu-id="e4c9a-125">要获取 accessReview 审阅的者。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-125">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="e4c9a-126">添加 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="e4c9a-126">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md) |      <span data-ttu-id="e4c9a-127">无。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-127">None.</span></span>   |   <span data-ttu-id="e4c9a-128">将审阅者添加到 accessReview。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-128">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="e4c9a-129">删除 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="e4c9a-129">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="e4c9a-130">无。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-130">None.</span></span>  |   <span data-ttu-id="e4c9a-131">删除 accessReview 审阅者。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-131">Remove a reviewer from an accessReview.</span></span> |
|[<span data-ttu-id="e4c9a-132">列表 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="e4c9a-132">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) |      <span data-ttu-id="e4c9a-133">[accessReviewDecision](accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="e4c9a-133">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="e4c9a-134">获取 accessReview 的决策。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-134">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="e4c9a-135">列出我 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="e4c9a-135">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) |     <span data-ttu-id="e4c9a-136">[accessReviewDecision](accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="e4c9a-136">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="e4c9a-137">审阅者，以获取 accessReview 我决策。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-137">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="e4c9a-138">发送 accessReview 提醒</span><span class="sxs-lookup"><span data-stu-id="e4c9a-138">Send accessReview reminder</span></span>](../api/accessreview-sendreminder.md) |        <span data-ttu-id="e4c9a-139">无。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-139">None.</span></span>   |   <span data-ttu-id="e4c9a-140">向审阅者的 accessReview 发送提醒。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-140">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="e4c9a-141">停止 accessReview</span><span class="sxs-lookup"><span data-stu-id="e4c9a-141">Stop accessReview</span></span>](../api/accessreview-stop.md) |     <span data-ttu-id="e4c9a-142">无。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-142">None.</span></span>   |   <span data-ttu-id="e4c9a-143">停止 accessReview。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-143">Stop an accessReview.</span></span> |
|[<span data-ttu-id="e4c9a-144">重置 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="e4c9a-144">Reset accessReview decisions</span></span>](../api/accessreview-reset.md) |     <span data-ttu-id="e4c9a-145">无。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-145">None.</span></span>   |   <span data-ttu-id="e4c9a-146">重置正在进行 accessReview 决策。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-146">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="e4c9a-147">应用 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="e4c9a-147">Apply accessReview decisions</span></span>](../api/accessreview-apply.md) |     <span data-ttu-id="e4c9a-148">无。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-148">None.</span></span>   |   <span data-ttu-id="e4c9a-149">应用已完成 accessReview 从的决策。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-149">Apply the decisions from a completed accessReview.</span></span>|

## <a name="permissions"></a><span data-ttu-id="e4c9a-150">权限</span><span class="sxs-lookup"><span data-stu-id="e4c9a-150">Permissions</span></span>

|<span data-ttu-id="e4c9a-151">权限类型</span><span class="sxs-lookup"><span data-stu-id="e4c9a-151">Permission type</span></span>                        | <span data-ttu-id="e4c9a-152">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e4c9a-152">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4c9a-153">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e4c9a-153">Delegated (work or school account)</span></span>     | <span data-ttu-id="e4c9a-154">AccessReview.Read.All AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4c9a-154">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="e4c9a-155">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e4c9a-155">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4c9a-156">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-156">Not supported.</span></span> |
|<span data-ttu-id="e4c9a-157">应用程序</span><span class="sxs-lookup"><span data-stu-id="e4c9a-157">Application</span></span>                            | <span data-ttu-id="e4c9a-158">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-158">Not supported.</span></span> |


## <a name="properties"></a><span data-ttu-id="e4c9a-159">属性</span><span class="sxs-lookup"><span data-stu-id="e4c9a-159">Properties</span></span>
| <span data-ttu-id="e4c9a-160">属性</span><span class="sxs-lookup"><span data-stu-id="e4c9a-160">Property</span></span>     | <span data-ttu-id="e4c9a-161">类型</span><span class="sxs-lookup"><span data-stu-id="e4c9a-161">Type</span></span>   |<span data-ttu-id="e4c9a-162">说明</span><span class="sxs-lookup"><span data-stu-id="e4c9a-162">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                      |`String`                                                        | <span data-ttu-id="e4c9a-163">功能分配的唯一标识符访问审阅。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-163">The feature-assigned unique identifier of an access review.</span></span> |
| `displayName`             |`String`                                                        | <span data-ttu-id="e4c9a-164">访问审阅名称。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-164">The access review name.</span></span> <span data-ttu-id="e4c9a-165">所需在创建。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-165">Required on create.</span></span> |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="e4c9a-166">审阅安排在启动时 DateTime。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-166">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="e4c9a-167">这可能是在将来的日期。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-167">This could be a date in the future.</span></span>  <span data-ttu-id="e4c9a-168">所需在创建。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-168">Required on create.</span></span> |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="e4c9a-169">审阅安排结束时 DateTime。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-169">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="e4c9a-170">这必须是至少一个日期晚于开始日期。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-170">This must be at least one day later than the start date.</span></span>  <span data-ttu-id="e4c9a-171">所需在创建。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-171">Required on create.</span></span> |
| `status`                  |`String`                                                        | <span data-ttu-id="e4c9a-172">此只读字段指定 accessReview 的状态。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-172">This read-only field specifies the status of an accessReview.</span></span> <span data-ttu-id="e4c9a-173">典型的状态包括`Initializing`， `NotStarted`， `Starting`，`InProgress`， `Completing`， `Completed`， `AutoReviewing`，和`AutoReviewed`。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-173">The typical states include `Initializing`, `NotStarted`, `Starting`,`InProgress`, `Completing`, `Completed`, `AutoReviewing`, and `AutoReviewed`.</span></span> |
| `description`             |`String`                                                        | <span data-ttu-id="e4c9a-174">访问审阅创建者提供，向审阅者显示说明。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-174">The description provided by the access review creator, to show to the reviewers.</span></span> |
| `businessFlowTemplateId`  |`String`                                                        | <span data-ttu-id="e4c9a-175">业务流程模板标识符。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-175">The business flow template identifier.</span></span> <span data-ttu-id="e4c9a-176">所需在创建。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-176">Required on create.</span></span> |
| `reviewerType`            |`String`                                                        | <span data-ttu-id="e4c9a-177">对目标对象，之一的审阅者的关系类型`self`，`delegated`或`entityOwners`。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-177">The relationship type of reviewer to the target object, one of `self`, `delegated` or `entityOwners`.</span></span> <span data-ttu-id="e4c9a-178">所需在创建。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-178">Required on create.</span></span> | 
| `createdBy`               |[<span data-ttu-id="e4c9a-179">userIdentity</span><span class="sxs-lookup"><span data-stu-id="e4c9a-179">userIdentity</span></span>](useridentity.md)                                 | <span data-ttu-id="e4c9a-180">创建此审查的用户。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-180">The user who created this review.</span></span> |
| `reviewedEntity`          |`microsoft.graph.identity`                                      | <span data-ttu-id="e4c9a-181">为其 access 会检查该对象查看的访问权限分配。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-181">The object for which the access reviews is reviewing the access rights assignments.</span></span> <span data-ttu-id="e4c9a-182">这可以在组中，用户组的成员身份的审阅或应用程序的用户迁移到应用程序的工作分配回顾。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-182">This can be the group for the review of memberships of users in a group, or the app for a review of assignments of users to an application.</span></span> <span data-ttu-id="e4c9a-183">所需在创建。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-183">Required on create.</span></span> | 
| `settings`                |`microsoft.graph.accessReviewSettings`             | <span data-ttu-id="e4c9a-184">AccessReview 的设置，，请参阅下面的类型定义。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-184">The settings of an accessReview, see type definition below.</span></span> |



## <a name="relationships"></a><span data-ttu-id="e4c9a-185">Relationships</span><span class="sxs-lookup"><span data-stu-id="e4c9a-185">Relationships</span></span>




| <span data-ttu-id="e4c9a-186">关系</span><span class="sxs-lookup"><span data-stu-id="e4c9a-186">Relationship</span></span> | <span data-ttu-id="e4c9a-187">类型</span><span class="sxs-lookup"><span data-stu-id="e4c9a-187">Type</span></span>   |<span data-ttu-id="e4c9a-188">说明</span><span class="sxs-lookup"><span data-stu-id="e4c9a-188">Description</span></span>|
|:---------------|:--------|:----------|
| `reviewers`               |<span data-ttu-id="e4c9a-189">[userIdentity](useridentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="e4c9a-189">[userIdentity](useridentity.md) collection</span></span>                     | <span data-ttu-id="e4c9a-190">访问审阅，如果访问审阅 reviewerType 的类型的审阅者的集合`delegate`。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-190">The collection of reviewers for an access review, if access review reviewerType is of type `delegate`.</span></span> |
| `decisions`               |<span data-ttu-id="e4c9a-191">[accessReviewDecision](accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="e4c9a-191">[accessReviewDecision](accessreviewdecision.md) collection</span></span> | <span data-ttu-id="e4c9a-192">此访问审查的决策的集合。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-192">The collection of decisions for this access review.</span></span> |
| `myDecisions`             |<span data-ttu-id="e4c9a-193">[accessReviewDecision](accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="e4c9a-193">[accessReviewDecision](accessreviewdecision.md) collection</span></span> | <span data-ttu-id="e4c9a-194">呼叫者，呼叫者是否审阅者的决策的集合。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-194">The collection of decisions for the caller, if the caller is a reviewer.</span></span> |
| `instances`               |<span data-ttu-id="e4c9a-195">[accessReview](accessreview.md)集合</span><span class="sxs-lookup"><span data-stu-id="e4c9a-195">[accessReview](accessreview.md) collection</span></span>         | <span data-ttu-id="e4c9a-196">访问评论一实例过去、 存在和未来，如果此对象是定期访问回顾。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-196">The collection of access reviews instances past, present and future, if this object is a recurring access review.</span></span> |

<span data-ttu-id="e4c9a-197">是否在对象上存在这些关系，取决于对象是否是一次性访问回顾、 的一系列定期访问审阅或定期访问回顾的实例。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-197">Whether these relationships are present on an object, depends upon whether the object is a one-time access review, the series of a recurring access review, or an instance of a recurring access review.</span></span>

| <span data-ttu-id="e4c9a-198">应用场景</span><span class="sxs-lookup"><span data-stu-id="e4c9a-198">Scenario</span></span> | <span data-ttu-id="e4c9a-199">有审阅者？</span><span class="sxs-lookup"><span data-stu-id="e4c9a-199">Has reviewers?</span></span> | <span data-ttu-id="e4c9a-200">具有决策和 myDecisions？</span><span class="sxs-lookup"><span data-stu-id="e4c9a-200">Has decisions and myDecisions?</span></span> | <span data-ttu-id="e4c9a-201">具有实例？</span><span class="sxs-lookup"><span data-stu-id="e4c9a-201">Has instances?</span></span> |
|:---------|:---------------|:---------------|:---------------|
|<span data-ttu-id="e4c9a-202">一次性访问审阅</span><span class="sxs-lookup"><span data-stu-id="e4c9a-202">One-time access review</span></span>|<span data-ttu-id="e4c9a-203">是</span><span class="sxs-lookup"><span data-stu-id="e4c9a-203">Yes</span></span> | <span data-ttu-id="e4c9a-204">是，一次启动</span><span class="sxs-lookup"><span data-stu-id="e4c9a-204">Yes, once started</span></span> | <span data-ttu-id="e4c9a-205">否</span><span class="sxs-lookup"><span data-stu-id="e4c9a-205">No</span></span> |
| <span data-ttu-id="e4c9a-206">定期访问审阅</span><span class="sxs-lookup"><span data-stu-id="e4c9a-206">Recurring access review</span></span> | <span data-ttu-id="e4c9a-207">是</span><span class="sxs-lookup"><span data-stu-id="e4c9a-207">Yes</span></span> | <span data-ttu-id="e4c9a-208">否</span><span class="sxs-lookup"><span data-stu-id="e4c9a-208">No</span></span> | <span data-ttu-id="e4c9a-209">是</span><span class="sxs-lookup"><span data-stu-id="e4c9a-209">Yes</span></span> |
| <span data-ttu-id="e4c9a-210">定期访问回顾的实例</span><span class="sxs-lookup"><span data-stu-id="e4c9a-210">Instance of a recurring access review</span></span> | <span data-ttu-id="e4c9a-211">是</span><span class="sxs-lookup"><span data-stu-id="e4c9a-211">Yes</span></span> | <span data-ttu-id="e4c9a-212">是，一次启动</span><span class="sxs-lookup"><span data-stu-id="e4c9a-212">Yes, once started</span></span> | <span data-ttu-id="e4c9a-213">否</span><span class="sxs-lookup"><span data-stu-id="e4c9a-213">No</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e4c9a-214">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e4c9a-214">JSON representation</span></span>

<span data-ttu-id="e4c9a-215">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-215">Here is a JSON representation of the resource.</span></span>

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
 "createdBy": "microsoft.graph.userIdentity",
 "reviewedEntity": "microsoft.graph.identity",
 "settings": "microsoft.graph.accessReviewSettings",
 "reviewers": "Collection(microsoft.graph.userIdentity)"
}

```

## <a name="the-accessreviewsettings-type"></a><span data-ttu-id="e4c9a-216">AccessReviewSettings 类型</span><span class="sxs-lookup"><span data-stu-id="e4c9a-216">The accessReviewSettings type</span></span>

<span data-ttu-id="e4c9a-217">`accessReviewSettings`创建访问检查，以控制时开始访问审阅功能行为时提供其他设置。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-217">The `accessReviewSettings` provides additional settings when creating an access review, to control the feature behavior when starting an access review.</span></span>  <span data-ttu-id="e4c9a-218">此类型具有以下属性：</span><span class="sxs-lookup"><span data-stu-id="e4c9a-218">This type has the following properties:</span></span> 

| <span data-ttu-id="e4c9a-219">属性</span><span class="sxs-lookup"><span data-stu-id="e4c9a-219">Property</span></span>                     | <span data-ttu-id="e4c9a-220">类型</span><span class="sxs-lookup"><span data-stu-id="e4c9a-220">Type</span></span>                      | <span data-ttu-id="e4c9a-221">说明</span><span class="sxs-lookup"><span data-stu-id="e4c9a-221">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| `mailNotificationsEnabled`|`Boolean`                | <span data-ttu-id="e4c9a-222">用于指示是否启用将邮件发送给审阅者和审阅创建者的标志。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-222">Flag to indicate whether sending mails to reviewers and the review creator is enabled.</span></span>                |
| `remindersEnabled`|`Boolean`       | <span data-ttu-id="e4c9a-223">用于指示是否启用发送给审阅者的提醒电子邮件标志。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-223">Flag to indicate whether sending reminder emails to reviewers are enabled.</span></span>       |
| `justificationRequiredOnApproval`|`Boolean` | <span data-ttu-id="e4c9a-224">用于指示审阅者是否需要提供理由审阅访问时的标志。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-224">Flag to indicate whether reviewers are required to provide a justification when reviewing access.</span></span>|
| `activityDurationInDays`|`Int64` | <span data-ttu-id="e4c9a-225">用户活动以向审阅者显示的天数。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-225">The number of days of user activities to show to reviewers.</span></span> |
| `autoReviewEnabled`|`Boolean` | <span data-ttu-id="e4c9a-226">启用标志以指示是否审阅者未提供一个用于 auto-apply，该功能是否应设置决定。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-226">Flag to indicate whether the feature should set a decision if the reviewer did not supply one, for use with auto-apply, is enabled.</span></span> |
| `autoReviewSettings`|`microsoft.graph.autoReviewSettings` | <span data-ttu-id="e4c9a-227">功能设置的审阅决策，用于 auto-apply，如下所述的方式的详细的设置。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-227">Detailed settings for how the feature should set the review decision, for use with auto-apply, described below.</span></span> |
| `recurrenceSettings`|`microsoft.graph.accessReviewRecurrenceSettings` | <span data-ttu-id="e4c9a-228">详细的定期，如下所述的设置。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-228">Detailed settings for recurrence, described below.</span></span> |
| `autoApplyReviewResultsEnabled`|`Boolean` | <span data-ttu-id="e4c9a-229">标志，指示是否自动应用启用功能，自动更改目标对象访问资源。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-229">Flag to indicate whether auto-apply capability, to automatically change the target object access resource, is enabled.</span></span>  <span data-ttu-id="e4c9a-230">如果未启用，用户必须审阅完成后，应用访问审阅。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-230">If not enabled, a user must, after the review completes, apply the access review.</span></span> |
| `accessRecommendationsEnabled`|`Boolean` | <span data-ttu-id="e4c9a-231">用于指示是否启用向审阅者显示建议的标志。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-231">Flag to indicate whether showing recommendations to reviewers is enabled.</span></span> |



## <a name="the-autoreviewsettings-type"></a><span data-ttu-id="e4c9a-232">AutoReviewSettings 类型</span><span class="sxs-lookup"><span data-stu-id="e4c9a-232">The autoReviewSettings type</span></span>

<span data-ttu-id="e4c9a-233">`autoReviewSettings`嵌入访问查看设置，并访问查看完成时指定功能的行为。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-233">The `autoReviewSettings` is embedded within the access review settings, and specifies the behavior for the feature when an access review completes.</span></span>  <span data-ttu-id="e4c9a-234">该类型具有一个属性， `notReviewedResult`。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-234">The type has one property, `notReviewedResult`.</span></span>

| <span data-ttu-id="e4c9a-235">属性</span><span class="sxs-lookup"><span data-stu-id="e4c9a-235">Property</span></span>                     | <span data-ttu-id="e4c9a-236">类型</span><span class="sxs-lookup"><span data-stu-id="e4c9a-236">Type</span></span>     | <span data-ttu-id="e4c9a-237">说明</span><span class="sxs-lookup"><span data-stu-id="e4c9a-237">Description</span></span>                          |
| :--------------------------- | :------  | :----------                          |
| `notReviewedResult`          |`String`  | <span data-ttu-id="e4c9a-238">必须为 `Approve`、`Deny` 或 `Recommendation` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-238">Must be one of `Approve`, `Deny`, or `Recommendation`.</span></span> |


## <a name="the-accessreviewrecurrencesettings-type"></a><span data-ttu-id="e4c9a-239">AccessReviewRecurrenceSettings 类型</span><span class="sxs-lookup"><span data-stu-id="e4c9a-239">The accessReviewRecurrenceSettings type</span></span>

<span data-ttu-id="e4c9a-240">`accessReviewRecurrenceSettings`嵌入访问查看设置，并指定访问审阅重复的时间间隔定期。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-240">The `accessReviewRecurrenceSettings` is embedded within the access review settings, and specifies that the access review recurs at regular intervals.</span></span>  <span data-ttu-id="e4c9a-241">此类型具有以下属性：</span><span class="sxs-lookup"><span data-stu-id="e4c9a-241">This type has the following properties:</span></span>

| <span data-ttu-id="e4c9a-242">属性</span><span class="sxs-lookup"><span data-stu-id="e4c9a-242">Property</span></span>                     | <span data-ttu-id="e4c9a-243">类型</span><span class="sxs-lookup"><span data-stu-id="e4c9a-243">Type</span></span>                                                                                                          | <span data-ttu-id="e4c9a-244">说明</span><span class="sxs-lookup"><span data-stu-id="e4c9a-244">Description</span></span> |
| :--------------------------- | :------------------------------------------------------------------------------------------------------------ | :---------- |
| `recurrenceType`|`String`    | <span data-ttu-id="e4c9a-245">重复出现的间隔，其必须是下列之一的`onetime`， `weekly`， `monthly`， `quarterly`，或`annual`。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-245">The recurrence interval, which must be one of `onetime`, `weekly`, `monthly`, `quarterly`, or `annual`.</span></span>                                                                   |
| `recurrenceEndType`|`String` | <span data-ttu-id="e4c9a-246">如何定期结束。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-246">How the recurrence ends.</span></span> <span data-ttu-id="e4c9a-247">如果`Never`，然后没有重复系列没有明确结束。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-247">If it is `Never`, then there is no explicit end of the recurrence series.</span></span> <span data-ttu-id="e4c9a-248">如果`endBy`，然后将定期结束于某个日期。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-248">If it is `endBy`, then the recurrence ends at a certain date.</span></span> <span data-ttu-id="e4c9a-249">如果`occurrences`，然后系列结束后`recurrentCount`审阅的实例完成。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-249">If it is `occurrences`, then the series ends after `recurrentCount` instances of the review have completed.</span></span> |
| `durationInDays`|`Int32`     | <span data-ttu-id="e4c9a-250">持续的定期的天数。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-250">The duration in days for recurrence.</span></span>                                                                              |
| `recurrenceCount`|`Int32`    | <span data-ttu-id="e4c9a-251">定期事件的计数如果的值`recurrenceEndType`是`occurrences`，否则为 0 或。</span><span class="sxs-lookup"><span data-stu-id="e4c9a-251">The count of recurrences, if the value of `recurrenceEndType` is `occurrences`, or 0 otherwise.</span></span>                                                        |



<!-- {
  "type": "#page.annotation",
  "description": "accessReview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
