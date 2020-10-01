---
title: accessReview 资源类型
description: '在 Azure AD access 评论功能中， `accessReview` 表示访问评审。  '
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2a63291d9cefb1b6a0c249b09a95430303b3597d
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330164"
---
# <a name="accessreview-resource-type"></a><span data-ttu-id="461cd-103">accessReview 资源类型</span><span class="sxs-lookup"><span data-stu-id="461cd-103">accessReview resource type</span></span>

<span data-ttu-id="461cd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="461cd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="461cd-105">表示 Azure AD [访问评审](accessreviews-root.md)。</span><span class="sxs-lookup"><span data-stu-id="461cd-105">Represents an Azure AD [access review](accessreviews-root.md).</span></span>  

## <a name="methods"></a><span data-ttu-id="461cd-106">方法</span><span class="sxs-lookup"><span data-stu-id="461cd-106">Methods</span></span>

| <span data-ttu-id="461cd-107">方法</span><span class="sxs-lookup"><span data-stu-id="461cd-107">Method</span></span>           | <span data-ttu-id="461cd-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="461cd-108">Return Type</span></span>    |<span data-ttu-id="461cd-109">说明</span><span class="sxs-lookup"><span data-stu-id="461cd-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="461cd-110">列出 accessReviews</span><span class="sxs-lookup"><span data-stu-id="461cd-110">List accessReviews</span></span>](../api/accessreview-list.md) | <span data-ttu-id="461cd-111">[accessReview](accessreview.md) 集合</span><span class="sxs-lookup"><span data-stu-id="461cd-111">[accessReview](accessreview.md) collection</span></span> | <span data-ttu-id="461cd-112">列出 businessFlowTemplate 的 accessReviews。</span><span class="sxs-lookup"><span data-stu-id="461cd-112">List accessReviews for a businessFlowTemplate.</span></span> |
|[<span data-ttu-id="461cd-113">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="461cd-113">Get accessReview</span></span>](../api/accessreview-get.md) |   [<span data-ttu-id="461cd-114">accessReview</span><span class="sxs-lookup"><span data-stu-id="461cd-114">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="461cd-115">获取具有特定 id 的访问评审。</span><span class="sxs-lookup"><span data-stu-id="461cd-115">Get an access review with a specific id.</span></span> |
|[<span data-ttu-id="461cd-116">创建 accessReview</span><span class="sxs-lookup"><span data-stu-id="461cd-116">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="461cd-117">accessReview</span><span class="sxs-lookup"><span data-stu-id="461cd-117">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="461cd-118">创建新的 accessReview。</span><span class="sxs-lookup"><span data-stu-id="461cd-118">Create a new accessReview.</span></span> |
|[<span data-ttu-id="461cd-119">更新 accessReview</span><span class="sxs-lookup"><span data-stu-id="461cd-119">Update accessReview</span></span>](../api/accessreview-update.md) | [<span data-ttu-id="461cd-120">accessReview</span><span class="sxs-lookup"><span data-stu-id="461cd-120">accessReview</span></span>](accessreview.md) | <span data-ttu-id="461cd-121">更新 accessReview。</span><span class="sxs-lookup"><span data-stu-id="461cd-121">Update an accessReview.</span></span> |
|[<span data-ttu-id="461cd-122">删除 accessReview</span><span class="sxs-lookup"><span data-stu-id="461cd-122">Delete accessReview</span></span>](../api/accessreview-delete.md) | <span data-ttu-id="461cd-123">无。</span><span class="sxs-lookup"><span data-stu-id="461cd-123">None.</span></span>   | <span data-ttu-id="461cd-124">删除 accessReview。</span><span class="sxs-lookup"><span data-stu-id="461cd-124">Delete an accessReview.</span></span> |
|[<span data-ttu-id="461cd-125">列出 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="461cd-125">List accessReview reviewers</span></span>](../api/accessreview-listreviewers.md) | <span data-ttu-id="461cd-126">[userIdentity](useridentity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="461cd-126">[userIdentity](useridentity.md) collection</span></span>|  <span data-ttu-id="461cd-127">获取 accessReview 的审阅者。</span><span class="sxs-lookup"><span data-stu-id="461cd-127">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="461cd-128">添加 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="461cd-128">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md) | <span data-ttu-id="461cd-129">无。</span><span class="sxs-lookup"><span data-stu-id="461cd-129">None.</span></span>    |   <span data-ttu-id="461cd-130">向 accessReview 添加审阅者。</span><span class="sxs-lookup"><span data-stu-id="461cd-130">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="461cd-131">删除 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="461cd-131">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="461cd-132">无。</span><span class="sxs-lookup"><span data-stu-id="461cd-132">None.</span></span> |    <span data-ttu-id="461cd-133">从 accessReview 中删除审阅者。</span><span class="sxs-lookup"><span data-stu-id="461cd-133">Remove a reviewer from an accessReview.</span></span> |
|[<span data-ttu-id="461cd-134">列出 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="461cd-134">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) | <span data-ttu-id="461cd-135">[accessReviewDecision](accessreviewdecision.md) 集合</span><span class="sxs-lookup"><span data-stu-id="461cd-135">[accessReviewDecision](accessreviewdecision.md) collection</span></span> | <span data-ttu-id="461cd-136">获取 accessReview 的决策。</span><span class="sxs-lookup"><span data-stu-id="461cd-136">Get the decisions of an accessReview.</span></span> |
|[<span data-ttu-id="461cd-137">列出我的 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="461cd-137">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) | <span data-ttu-id="461cd-138">[accessReviewDecision](accessreviewdecision.md) 集合</span><span class="sxs-lookup"><span data-stu-id="461cd-138">[accessReviewDecision](accessreviewdecision.md) collection</span></span> | <span data-ttu-id="461cd-139">作为审阅者，请 accessReview 的决策。</span><span class="sxs-lookup"><span data-stu-id="461cd-139">As a reviewer, get my decisions of an accessReview.</span></span> |
|[<span data-ttu-id="461cd-140">发送 accessReview 提醒</span><span class="sxs-lookup"><span data-stu-id="461cd-140">Send accessReview reminder</span></span>](../api/accessreview-sendreminder.md) | <span data-ttu-id="461cd-141">无。</span><span class="sxs-lookup"><span data-stu-id="461cd-141">None.</span></span> | <span data-ttu-id="461cd-142">向 accessReview 的审阅者发送提醒。</span><span class="sxs-lookup"><span data-stu-id="461cd-142">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="461cd-143">停止 accessReview</span><span class="sxs-lookup"><span data-stu-id="461cd-143">Stop accessReview</span></span>](../api/accessreview-stop.md) | <span data-ttu-id="461cd-144">无。</span><span class="sxs-lookup"><span data-stu-id="461cd-144">None.</span></span> | <span data-ttu-id="461cd-145">停止 accessReview。</span><span class="sxs-lookup"><span data-stu-id="461cd-145">Stop an accessReview.</span></span> |
|[<span data-ttu-id="461cd-146">重置 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="461cd-146">Reset accessReview decisions</span></span>](../api/accessreview-reset.md) | <span data-ttu-id="461cd-147">无。</span><span class="sxs-lookup"><span data-stu-id="461cd-147">None.</span></span>   |   <span data-ttu-id="461cd-148">在进行中的 accessReview 中重置决策。</span><span class="sxs-lookup"><span data-stu-id="461cd-148">Reset the decisions in an in-progress accessReview.</span></span> |
|[<span data-ttu-id="461cd-149">应用 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="461cd-149">Apply accessReview decisions</span></span>](../api/accessreview-apply.md) | <span data-ttu-id="461cd-150">无。</span><span class="sxs-lookup"><span data-stu-id="461cd-150">None.</span></span> | <span data-ttu-id="461cd-151">从已完成的 accessReview 应用决策。</span><span class="sxs-lookup"><span data-stu-id="461cd-151">Apply the decisions from a completed accessReview.</span></span> |

## <a name="properties"></a><span data-ttu-id="461cd-152">属性</span><span class="sxs-lookup"><span data-stu-id="461cd-152">Properties</span></span>

| <span data-ttu-id="461cd-153">属性</span><span class="sxs-lookup"><span data-stu-id="461cd-153">Property</span></span> | <span data-ttu-id="461cd-154">类型</span><span class="sxs-lookup"><span data-stu-id="461cd-154">Type</span></span>   | <span data-ttu-id="461cd-155">说明</span><span class="sxs-lookup"><span data-stu-id="461cd-155">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="461cd-156">id</span><span class="sxs-lookup"><span data-stu-id="461cd-156">id</span></span> | <span data-ttu-id="461cd-157">字符串</span><span class="sxs-lookup"><span data-stu-id="461cd-157">String</span></span> | <span data-ttu-id="461cd-158">用于访问评审的功能分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="461cd-158">The feature-assigned unique identifier of an access review.</span></span> |
| <span data-ttu-id="461cd-159">displayName</span><span class="sxs-lookup"><span data-stu-id="461cd-159">displayName</span></span> | <span data-ttu-id="461cd-160">字符串</span><span class="sxs-lookup"><span data-stu-id="461cd-160">String</span></span> | <span data-ttu-id="461cd-161">访问审阅名称。</span><span class="sxs-lookup"><span data-stu-id="461cd-161">The access review name.</span></span> <span data-ttu-id="461cd-162">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="461cd-162">Required on create.</span></span> |
| <span data-ttu-id="461cd-163">startDateTime</span><span class="sxs-lookup"><span data-stu-id="461cd-163">startDateTime</span></span> | <span data-ttu-id="461cd-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="461cd-164">DateTimeOffset</span></span> | <span data-ttu-id="461cd-165">计划开始评审时的日期时间。</span><span class="sxs-lookup"><span data-stu-id="461cd-165">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="461cd-166">这可能是将来的日期。</span><span class="sxs-lookup"><span data-stu-id="461cd-166">This could be a date in the future.</span></span>  <span data-ttu-id="461cd-167">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="461cd-167">Required on create.</span></span> |
| <span data-ttu-id="461cd-168">endDateTime</span><span class="sxs-lookup"><span data-stu-id="461cd-168">endDateTime</span></span> | <span data-ttu-id="461cd-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="461cd-169">DateTimeOffset</span></span> | <span data-ttu-id="461cd-170">计划结束评审时的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="461cd-170">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="461cd-171">此时间必须至少为一个晚于开始日期的一天。</span><span class="sxs-lookup"><span data-stu-id="461cd-171">This must be at least one day later than the start date.</span></span>  <span data-ttu-id="461cd-172">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="461cd-172">Required on create.</span></span> |
| <span data-ttu-id="461cd-173">状态</span><span class="sxs-lookup"><span data-stu-id="461cd-173">status</span></span> | <span data-ttu-id="461cd-174">字符串</span><span class="sxs-lookup"><span data-stu-id="461cd-174">String</span></span> | <span data-ttu-id="461cd-175">此只读字段指定 accessReview 的状态。</span><span class="sxs-lookup"><span data-stu-id="461cd-175">This read-only field specifies the status of an accessReview.</span></span> <span data-ttu-id="461cd-176">典型状态包括、、、、、、 `Initializing` `NotStarted` `Starting` `InProgress` `Completing` `Completed` `AutoReviewing` 和 `AutoReviewed` 。</span><span class="sxs-lookup"><span data-stu-id="461cd-176">The typical states include `Initializing`, `NotStarted`, `Starting`,`InProgress`, `Completing`, `Completed`, `AutoReviewing`, and `AutoReviewed`.</span></span> |
| <span data-ttu-id="461cd-177">description</span><span class="sxs-lookup"><span data-stu-id="461cd-177">description</span></span> | <span data-ttu-id="461cd-178">字符串</span><span class="sxs-lookup"><span data-stu-id="461cd-178">String</span></span> | <span data-ttu-id="461cd-179">由 access 评审创建者提供的说明，用于向审阅者显示。</span><span class="sxs-lookup"><span data-stu-id="461cd-179">The description provided by the access review creator, to show to the reviewers.</span></span> |
| <span data-ttu-id="461cd-180">businessFlowTemplateId</span><span class="sxs-lookup"><span data-stu-id="461cd-180">businessFlowTemplateId</span></span> | <span data-ttu-id="461cd-181">字符串</span><span class="sxs-lookup"><span data-stu-id="461cd-181">String</span></span> | <span data-ttu-id="461cd-182">业务流模板标识符。</span><span class="sxs-lookup"><span data-stu-id="461cd-182">The business flow template identifier.</span></span> <span data-ttu-id="461cd-183">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="461cd-183">Required on create.</span></span>  <span data-ttu-id="461cd-184">此值区分大小写。</span><span class="sxs-lookup"><span data-stu-id="461cd-184">This value is case sensitive.</span></span> |
| <span data-ttu-id="461cd-185">reviewerType</span><span class="sxs-lookup"><span data-stu-id="461cd-185">reviewerType</span></span> | <span data-ttu-id="461cd-186">字符串</span><span class="sxs-lookup"><span data-stu-id="461cd-186">String</span></span> | <span data-ttu-id="461cd-187">目标对象的审阅者的关系类型，一个 `self` `delegated` 或 `entityOwners` 。</span><span class="sxs-lookup"><span data-stu-id="461cd-187">The relationship type of reviewer to the target object, one of `self`, `delegated` or `entityOwners`.</span></span> <span data-ttu-id="461cd-188">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="461cd-188">Required on create.</span></span> | 
| <span data-ttu-id="461cd-189">createdBy</span><span class="sxs-lookup"><span data-stu-id="461cd-189">createdBy</span></span> | [<span data-ttu-id="461cd-190">userIdentity</span><span class="sxs-lookup"><span data-stu-id="461cd-190">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="461cd-191">创建此评审的用户。</span><span class="sxs-lookup"><span data-stu-id="461cd-191">The user who created this review.</span></span> |
| <span data-ttu-id="461cd-192">reviewedEntity</span><span class="sxs-lookup"><span data-stu-id="461cd-192">reviewedEntity</span></span> | [<span data-ttu-id="461cd-193">identity</span><span class="sxs-lookup"><span data-stu-id="461cd-193">identity</span></span>](identity.md) | <span data-ttu-id="461cd-194">访问权检查其访问权限分配的对象。</span><span class="sxs-lookup"><span data-stu-id="461cd-194">The object for which the access reviews is reviewing the access rights assignments.</span></span> <span data-ttu-id="461cd-195">此组可以是查看组中用户的成员身份的组，也可以是用于查看对应用程序的用户分配的应用程序。</span><span class="sxs-lookup"><span data-stu-id="461cd-195">This can be the group for the review of memberships of users in a group, or the app for a review of assignments of users to an application.</span></span> <span data-ttu-id="461cd-196">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="461cd-196">Required on create.</span></span> | 
| <span data-ttu-id="461cd-197">settings</span><span class="sxs-lookup"><span data-stu-id="461cd-197">settings</span></span> | [<span data-ttu-id="461cd-198">accessReviewSettings</span><span class="sxs-lookup"><span data-stu-id="461cd-198">accessReviewSettings</span></span>](accessreviewsettings.md) | <span data-ttu-id="461cd-199">AccessReview 的设置，请参阅下面的类型定义。</span><span class="sxs-lookup"><span data-stu-id="461cd-199">The settings of an accessReview, see type definition below.</span></span> |

## <a name="relationships"></a><span data-ttu-id="461cd-200">关系</span><span class="sxs-lookup"><span data-stu-id="461cd-200">Relationships</span></span>

| <span data-ttu-id="461cd-201">关系</span><span class="sxs-lookup"><span data-stu-id="461cd-201">Relationship</span></span> | <span data-ttu-id="461cd-202">类型</span><span class="sxs-lookup"><span data-stu-id="461cd-202">Type</span></span>   | <span data-ttu-id="461cd-203">说明</span><span class="sxs-lookup"><span data-stu-id="461cd-203">Description</span></span> |
|:------------ |:---- |:----------- |
| <span data-ttu-id="461cd-204">审批</span><span class="sxs-lookup"><span data-stu-id="461cd-204">reviewers</span></span> | <span data-ttu-id="461cd-205">[userIdentity](useridentity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="461cd-205">[userIdentity](useridentity.md) collection</span></span> | <span data-ttu-id="461cd-206">访问评审的审阅者的集合（如果 access 评审 reviewerType 的类型为） `delegated` 。</span><span class="sxs-lookup"><span data-stu-id="461cd-206">The collection of reviewers for an access review, if access review reviewerType is of type `delegated`.</span></span> |
| <span data-ttu-id="461cd-207">针对</span><span class="sxs-lookup"><span data-stu-id="461cd-207">decisions</span></span> | <span data-ttu-id="461cd-208">[accessReviewDecision](accessreviewdecision.md) 集合</span><span class="sxs-lookup"><span data-stu-id="461cd-208">[accessReviewDecision](accessreviewdecision.md) collection</span></span> | <span data-ttu-id="461cd-209">此访问评审的决策集合。</span><span class="sxs-lookup"><span data-stu-id="461cd-209">The collection of decisions for this access review.</span></span> |
| <span data-ttu-id="461cd-210">myDecisions</span><span class="sxs-lookup"><span data-stu-id="461cd-210">myDecisions</span></span> | <span data-ttu-id="461cd-211">[accessReviewDecision](accessreviewdecision.md) 集合</span><span class="sxs-lookup"><span data-stu-id="461cd-211">[accessReviewDecision](accessreviewdecision.md) collection</span></span> | <span data-ttu-id="461cd-212">如果呼叫者是审阅者，则为呼叫者做出决策的集合。</span><span class="sxs-lookup"><span data-stu-id="461cd-212">The collection of decisions for the caller, if the caller is a reviewer.</span></span> |
| <span data-ttu-id="461cd-213">instances</span><span class="sxs-lookup"><span data-stu-id="461cd-213">instances</span></span> | <span data-ttu-id="461cd-214">[accessReview](accessreview.md) 集合</span><span class="sxs-lookup"><span data-stu-id="461cd-214">[accessReview](accessreview.md) collection</span></span> | <span data-ttu-id="461cd-215">如果此对象是定期访问审核，则 access 的集合将审阅过去、现在和将来的实例。</span><span class="sxs-lookup"><span data-stu-id="461cd-215">The collection of access reviews instances past, present and future, if this object is a recurring access review.</span></span> |

<span data-ttu-id="461cd-216">对象中是否存在这些关系，取决于该对象是一次性访问评审、定期访问评审的系列，还是定期访问评审的实例。</span><span class="sxs-lookup"><span data-stu-id="461cd-216">Whether these relationships are present on an object, depends upon whether the object is a one-time access review, the series of a recurring access review, or an instance of a recurring access review.</span></span>

| <span data-ttu-id="461cd-217">方案</span><span class="sxs-lookup"><span data-stu-id="461cd-217">Scenario</span></span> | <span data-ttu-id="461cd-218">是否有审阅者？</span><span class="sxs-lookup"><span data-stu-id="461cd-218">Has reviewers?</span></span> | <span data-ttu-id="461cd-219">是否有决策和 myDecisions？</span><span class="sxs-lookup"><span data-stu-id="461cd-219">Has decisions and myDecisions?</span></span> | <span data-ttu-id="461cd-220">有实例吗？</span><span class="sxs-lookup"><span data-stu-id="461cd-220">Has instances?</span></span> |
|:-------- |:-------------- |:------------------------------ |:-------------- |
| <span data-ttu-id="461cd-221">一次性访问审核</span><span class="sxs-lookup"><span data-stu-id="461cd-221">One-time access review</span></span> | <span data-ttu-id="461cd-222">是</span><span class="sxs-lookup"><span data-stu-id="461cd-222">Yes</span></span> | <span data-ttu-id="461cd-223">是，启动后</span><span class="sxs-lookup"><span data-stu-id="461cd-223">Yes, once started</span></span> | <span data-ttu-id="461cd-224">否</span><span class="sxs-lookup"><span data-stu-id="461cd-224">No</span></span> |
| <span data-ttu-id="461cd-225">定期访问审核</span><span class="sxs-lookup"><span data-stu-id="461cd-225">Recurring access review</span></span> | <span data-ttu-id="461cd-226">是</span><span class="sxs-lookup"><span data-stu-id="461cd-226">Yes</span></span> | <span data-ttu-id="461cd-227">否</span><span class="sxs-lookup"><span data-stu-id="461cd-227">No</span></span> | <span data-ttu-id="461cd-228">是</span><span class="sxs-lookup"><span data-stu-id="461cd-228">Yes</span></span> |
| <span data-ttu-id="461cd-229">定期访问审核实例</span><span class="sxs-lookup"><span data-stu-id="461cd-229">Instance of a recurring access review</span></span> | <span data-ttu-id="461cd-230">是</span><span class="sxs-lookup"><span data-stu-id="461cd-230">Yes</span></span> | <span data-ttu-id="461cd-231">是，启动后</span><span class="sxs-lookup"><span data-stu-id="461cd-231">Yes, once started</span></span> | <span data-ttu-id="461cd-232">否</span><span class="sxs-lookup"><span data-stu-id="461cd-232">No</span></span> |

## <a name="json-representation"></a><span data-ttu-id="461cd-233">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="461cd-233">JSON representation</span></span>

<span data-ttu-id="461cd-234">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="461cd-234">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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
 "createdBy": {"@odata.type": "microsoft.graph.userIdentity"},
 "reviewedEntity": {"@odata.type": "microsoft.graph.identity"},
 "settings": {"@odata.type": "microsoft.graph.accessReviewSettings"},
 "reviewers": [{"@odata.type": "microsoft.graph.userIdentity"}]
}

```

<!--
{
  "type": "#page.annotation",
  "description": "accessReview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


