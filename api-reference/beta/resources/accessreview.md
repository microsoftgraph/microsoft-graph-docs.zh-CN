---
title: accessReview 资源类型
description: '在 Azure AD 访问评审功能中， `accessReview` 表示访问评审。  '
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: da155d49eedf03cdc935eeefc6b6808847176a41
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292712"
---
# <a name="accessreview-resource-type"></a><span data-ttu-id="47bae-103">accessReview 资源类型</span><span class="sxs-lookup"><span data-stu-id="47bae-103">accessReview resource type</span></span>

<span data-ttu-id="47bae-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47bae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

<span data-ttu-id="47bae-105">表示 Azure AD [访问评审](accessreviews-root.md)。</span><span class="sxs-lookup"><span data-stu-id="47bae-105">Represents an Azure AD [access review](accessreviews-root.md).</span></span>  

## <a name="methods"></a><span data-ttu-id="47bae-106">方法</span><span class="sxs-lookup"><span data-stu-id="47bae-106">Methods</span></span>

| <span data-ttu-id="47bae-107">方法</span><span class="sxs-lookup"><span data-stu-id="47bae-107">Method</span></span>           | <span data-ttu-id="47bae-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="47bae-108">Return Type</span></span>    |<span data-ttu-id="47bae-109">说明</span><span class="sxs-lookup"><span data-stu-id="47bae-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="47bae-110">列出 accessReviews</span><span class="sxs-lookup"><span data-stu-id="47bae-110">List accessReviews</span></span>](../api/accessreview-list.md) | <span data-ttu-id="47bae-111">[accessReview](accessreview.md) 集合</span><span class="sxs-lookup"><span data-stu-id="47bae-111">[accessReview](accessreview.md) collection</span></span> | <span data-ttu-id="47bae-112">列出 businessFlowTemplate 的 accessReviews。</span><span class="sxs-lookup"><span data-stu-id="47bae-112">List accessReviews for a businessFlowTemplate.</span></span> |
|[<span data-ttu-id="47bae-113">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="47bae-113">Get accessReview</span></span>](../api/accessreview-get.md) |   [<span data-ttu-id="47bae-114">accessReview</span><span class="sxs-lookup"><span data-stu-id="47bae-114">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="47bae-115">获取具有特定 ID 的访问评审。</span><span class="sxs-lookup"><span data-stu-id="47bae-115">Get an access review with a specific id.</span></span> |
|[<span data-ttu-id="47bae-116">创建 accessReview</span><span class="sxs-lookup"><span data-stu-id="47bae-116">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="47bae-117">accessReview</span><span class="sxs-lookup"><span data-stu-id="47bae-117">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="47bae-118">创建新的 accessReview。</span><span class="sxs-lookup"><span data-stu-id="47bae-118">Create a new accessReview.</span></span> |
|[<span data-ttu-id="47bae-119">更新 accessReview</span><span class="sxs-lookup"><span data-stu-id="47bae-119">Update accessReview</span></span>](../api/accessreview-update.md) | [<span data-ttu-id="47bae-120">accessReview</span><span class="sxs-lookup"><span data-stu-id="47bae-120">accessReview</span></span>](accessreview.md) | <span data-ttu-id="47bae-121">更新 accessReview。</span><span class="sxs-lookup"><span data-stu-id="47bae-121">Update an accessReview.</span></span> |
|[<span data-ttu-id="47bae-122">删除 accessReview</span><span class="sxs-lookup"><span data-stu-id="47bae-122">Delete accessReview</span></span>](../api/accessreview-delete.md) | <span data-ttu-id="47bae-123">无。</span><span class="sxs-lookup"><span data-stu-id="47bae-123">None.</span></span>   | <span data-ttu-id="47bae-124">删除 accessReview。</span><span class="sxs-lookup"><span data-stu-id="47bae-124">Delete an accessReview.</span></span> |
|[<span data-ttu-id="47bae-125">列出 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="47bae-125">List accessReview reviewers</span></span>](../api/accessreview-listreviewers.md) | <span data-ttu-id="47bae-126">[userIdentity](useridentity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="47bae-126">[userIdentity](useridentity.md) collection</span></span>|  <span data-ttu-id="47bae-127">获取 accessReview 的审阅者。</span><span class="sxs-lookup"><span data-stu-id="47bae-127">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="47bae-128">添加 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="47bae-128">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md) | <span data-ttu-id="47bae-129">无。</span><span class="sxs-lookup"><span data-stu-id="47bae-129">None.</span></span>    |   <span data-ttu-id="47bae-130">将审阅者添加到 accessReview。</span><span class="sxs-lookup"><span data-stu-id="47bae-130">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="47bae-131">删除 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="47bae-131">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="47bae-132">无。</span><span class="sxs-lookup"><span data-stu-id="47bae-132">None.</span></span> |    <span data-ttu-id="47bae-133">从 accessReview 中删除审阅者。</span><span class="sxs-lookup"><span data-stu-id="47bae-133">Remove a reviewer from an accessReview.</span></span> |
|[<span data-ttu-id="47bae-134">列出 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="47bae-134">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) | <span data-ttu-id="47bae-135">[accessReviewDecision](accessreviewdecision.md) 集合</span><span class="sxs-lookup"><span data-stu-id="47bae-135">[accessReviewDecision](accessreviewdecision.md) collection</span></span> | <span data-ttu-id="47bae-136">获取 accessReview 的决策。</span><span class="sxs-lookup"><span data-stu-id="47bae-136">Get the decisions of an accessReview.</span></span> |
|[<span data-ttu-id="47bae-137">列出我的 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="47bae-137">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) | <span data-ttu-id="47bae-138">[accessReviewDecision](accessreviewdecision.md) 集合</span><span class="sxs-lookup"><span data-stu-id="47bae-138">[accessReviewDecision](accessreviewdecision.md) collection</span></span> | <span data-ttu-id="47bae-139">作为审阅者，获取我关于 accessReview 的决定。</span><span class="sxs-lookup"><span data-stu-id="47bae-139">As a reviewer, get my decisions of an accessReview.</span></span> |
|[<span data-ttu-id="47bae-140">发送 accessReview 提醒</span><span class="sxs-lookup"><span data-stu-id="47bae-140">Send accessReview reminder</span></span>](../api/accessreview-sendreminder.md) | <span data-ttu-id="47bae-141">无。</span><span class="sxs-lookup"><span data-stu-id="47bae-141">None.</span></span> | <span data-ttu-id="47bae-142">向 accessReview 的审阅者发送提醒。</span><span class="sxs-lookup"><span data-stu-id="47bae-142">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="47bae-143">Stop accessReview</span><span class="sxs-lookup"><span data-stu-id="47bae-143">Stop accessReview</span></span>](../api/accessreview-stop.md) | <span data-ttu-id="47bae-144">无。</span><span class="sxs-lookup"><span data-stu-id="47bae-144">None.</span></span> | <span data-ttu-id="47bae-145">停止 accessReview。</span><span class="sxs-lookup"><span data-stu-id="47bae-145">Stop an accessReview.</span></span> |
|[<span data-ttu-id="47bae-146">重置 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="47bae-146">Reset accessReview decisions</span></span>](../api/accessreview-reset.md) | <span data-ttu-id="47bae-147">无。</span><span class="sxs-lookup"><span data-stu-id="47bae-147">None.</span></span>   |   <span data-ttu-id="47bae-148">重置正在进行中的 accessReview 中的决策。</span><span class="sxs-lookup"><span data-stu-id="47bae-148">Reset the decisions in an in-progress accessReview.</span></span> |
|[<span data-ttu-id="47bae-149">应用 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="47bae-149">Apply accessReview decisions</span></span>](../api/accessreview-apply.md) | <span data-ttu-id="47bae-150">无。</span><span class="sxs-lookup"><span data-stu-id="47bae-150">None.</span></span> | <span data-ttu-id="47bae-151">从已完成的 accessReview 应用决策。</span><span class="sxs-lookup"><span data-stu-id="47bae-151">Apply the decisions from a completed accessReview.</span></span> |

## <a name="properties"></a><span data-ttu-id="47bae-152">属性</span><span class="sxs-lookup"><span data-stu-id="47bae-152">Properties</span></span>

| <span data-ttu-id="47bae-153">属性</span><span class="sxs-lookup"><span data-stu-id="47bae-153">Property</span></span> | <span data-ttu-id="47bae-154">类型</span><span class="sxs-lookup"><span data-stu-id="47bae-154">Type</span></span>   | <span data-ttu-id="47bae-155">说明</span><span class="sxs-lookup"><span data-stu-id="47bae-155">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="47bae-156">id</span><span class="sxs-lookup"><span data-stu-id="47bae-156">id</span></span> | <span data-ttu-id="47bae-157">String</span><span class="sxs-lookup"><span data-stu-id="47bae-157">String</span></span> | <span data-ttu-id="47bae-158">访问评审的功能分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="47bae-158">The feature-assigned unique identifier of an access review.</span></span> |
| <span data-ttu-id="47bae-159">displayName</span><span class="sxs-lookup"><span data-stu-id="47bae-159">displayName</span></span> | <span data-ttu-id="47bae-160">String</span><span class="sxs-lookup"><span data-stu-id="47bae-160">String</span></span> | <span data-ttu-id="47bae-161">访问评审名称。</span><span class="sxs-lookup"><span data-stu-id="47bae-161">The access review name.</span></span> <span data-ttu-id="47bae-162">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="47bae-162">Required on create.</span></span> |
| <span data-ttu-id="47bae-163">startDateTime</span><span class="sxs-lookup"><span data-stu-id="47bae-163">startDateTime</span></span> | <span data-ttu-id="47bae-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47bae-164">DateTimeOffset</span></span> | <span data-ttu-id="47bae-165">计划开始审阅的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="47bae-165">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="47bae-166">这可能是将来的日期。</span><span class="sxs-lookup"><span data-stu-id="47bae-166">This could be a date in the future.</span></span>  <span data-ttu-id="47bae-167">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="47bae-167">Required on create.</span></span> |
| <span data-ttu-id="47bae-168">endDateTime</span><span class="sxs-lookup"><span data-stu-id="47bae-168">endDateTime</span></span> | <span data-ttu-id="47bae-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47bae-169">DateTimeOffset</span></span> | <span data-ttu-id="47bae-170">计划结束审阅的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="47bae-170">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="47bae-171">这必须至少比开始日期晚一天。</span><span class="sxs-lookup"><span data-stu-id="47bae-171">This must be at least one day later than the start date.</span></span>  <span data-ttu-id="47bae-172">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="47bae-172">Required on create.</span></span> |
| <span data-ttu-id="47bae-173">status</span><span class="sxs-lookup"><span data-stu-id="47bae-173">status</span></span> | <span data-ttu-id="47bae-174">String</span><span class="sxs-lookup"><span data-stu-id="47bae-174">String</span></span> | <span data-ttu-id="47bae-175">此只读字段指定 accessReview 的状态。</span><span class="sxs-lookup"><span data-stu-id="47bae-175">This read-only field specifies the status of an accessReview.</span></span> <span data-ttu-id="47bae-176">典型状态包括 `Initializing` 、 `NotStarted` `Starting` 、 、 、 `InProgress` `Completing` 和 `Completed` `AutoReviewing` `AutoReviewed` 。</span><span class="sxs-lookup"><span data-stu-id="47bae-176">The typical states include `Initializing`, `NotStarted`, `Starting`,`InProgress`, `Completing`, `Completed`, `AutoReviewing`, and `AutoReviewed`.</span></span> |
| <span data-ttu-id="47bae-177">description</span><span class="sxs-lookup"><span data-stu-id="47bae-177">description</span></span> | <span data-ttu-id="47bae-178">String</span><span class="sxs-lookup"><span data-stu-id="47bae-178">String</span></span> | <span data-ttu-id="47bae-179">访问评审创建者提供的说明，向审阅者显示。</span><span class="sxs-lookup"><span data-stu-id="47bae-179">The description provided by the access review creator, to show to the reviewers.</span></span> |
| <span data-ttu-id="47bae-180">businessFlowTemplateId</span><span class="sxs-lookup"><span data-stu-id="47bae-180">businessFlowTemplateId</span></span> | <span data-ttu-id="47bae-181">String</span><span class="sxs-lookup"><span data-stu-id="47bae-181">String</span></span> | <span data-ttu-id="47bae-182">业务流程模板标识符。</span><span class="sxs-lookup"><span data-stu-id="47bae-182">The business flow template identifier.</span></span> <span data-ttu-id="47bae-183">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="47bae-183">Required on create.</span></span>  <span data-ttu-id="47bae-184">此值区分大小写。</span><span class="sxs-lookup"><span data-stu-id="47bae-184">This value is case sensitive.</span></span> |
| <span data-ttu-id="47bae-185">reviewerType</span><span class="sxs-lookup"><span data-stu-id="47bae-185">reviewerType</span></span> | <span data-ttu-id="47bae-186">String</span><span class="sxs-lookup"><span data-stu-id="47bae-186">String</span></span> | <span data-ttu-id="47bae-187">审阅者与目标对象的关系类型，其中一个 `self` 或 `delegated` `entityOwners` 。</span><span class="sxs-lookup"><span data-stu-id="47bae-187">The relationship type of reviewer to the target object, one of `self`, `delegated` or `entityOwners`.</span></span> <span data-ttu-id="47bae-188">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="47bae-188">Required on create.</span></span> | 
| <span data-ttu-id="47bae-189">createdBy</span><span class="sxs-lookup"><span data-stu-id="47bae-189">createdBy</span></span> | [<span data-ttu-id="47bae-190">userIdentity</span><span class="sxs-lookup"><span data-stu-id="47bae-190">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="47bae-191">创建此评价的用户。</span><span class="sxs-lookup"><span data-stu-id="47bae-191">The user who created this review.</span></span> |
| <span data-ttu-id="47bae-192">reviewedEntity</span><span class="sxs-lookup"><span data-stu-id="47bae-192">reviewedEntity</span></span> | [<span data-ttu-id="47bae-193">identity</span><span class="sxs-lookup"><span data-stu-id="47bae-193">identity</span></span>](identity.md) | <span data-ttu-id="47bae-194">访问评审正在审阅其访问权限分配的对象。</span><span class="sxs-lookup"><span data-stu-id="47bae-194">The object for which the access reviews is reviewing the access rights assignments.</span></span> <span data-ttu-id="47bae-195">此组可以是审阅组中用户成员身份的组，或者是查看用户到应用程序的分配的应用。</span><span class="sxs-lookup"><span data-stu-id="47bae-195">This can be the group for the review of memberships of users in a group, or the app for a review of assignments of users to an application.</span></span> <span data-ttu-id="47bae-196">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="47bae-196">Required on create.</span></span> | 
| <span data-ttu-id="47bae-197">settings</span><span class="sxs-lookup"><span data-stu-id="47bae-197">settings</span></span> | [<span data-ttu-id="47bae-198">accessReviewSettings</span><span class="sxs-lookup"><span data-stu-id="47bae-198">accessReviewSettings</span></span>](accessreviewsettings.md) | <span data-ttu-id="47bae-199">accessReview 的设置，请参阅下面的类型定义。</span><span class="sxs-lookup"><span data-stu-id="47bae-199">The settings of an accessReview, see type definition below.</span></span> |

## <a name="relationships"></a><span data-ttu-id="47bae-200">关系</span><span class="sxs-lookup"><span data-stu-id="47bae-200">Relationships</span></span>

| <span data-ttu-id="47bae-201">关系</span><span class="sxs-lookup"><span data-stu-id="47bae-201">Relationship</span></span> | <span data-ttu-id="47bae-202">类型</span><span class="sxs-lookup"><span data-stu-id="47bae-202">Type</span></span>   | <span data-ttu-id="47bae-203">说明</span><span class="sxs-lookup"><span data-stu-id="47bae-203">Description</span></span> |
|:------------ |:---- |:----------- |
| <span data-ttu-id="47bae-204">审阅者</span><span class="sxs-lookup"><span data-stu-id="47bae-204">reviewers</span></span> | <span data-ttu-id="47bae-205">[userIdentity](useridentity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="47bae-205">[userIdentity](useridentity.md) collection</span></span> | <span data-ttu-id="47bae-206">访问评审审阅者的集合，如果访问审阅审阅者Type 的类型 `delegated` 。</span><span class="sxs-lookup"><span data-stu-id="47bae-206">The collection of reviewers for an access review, if access review reviewerType is of type `delegated`.</span></span> |
| <span data-ttu-id="47bae-207">决策</span><span class="sxs-lookup"><span data-stu-id="47bae-207">decisions</span></span> | <span data-ttu-id="47bae-208">[accessReviewDecision](accessreviewdecision.md) 集合</span><span class="sxs-lookup"><span data-stu-id="47bae-208">[accessReviewDecision](accessreviewdecision.md) collection</span></span> | <span data-ttu-id="47bae-209">此访问评审的决策集合。</span><span class="sxs-lookup"><span data-stu-id="47bae-209">The collection of decisions for this access review.</span></span> |
| <span data-ttu-id="47bae-210">myDecisions</span><span class="sxs-lookup"><span data-stu-id="47bae-210">myDecisions</span></span> | <span data-ttu-id="47bae-211">[accessReviewDecision](accessreviewdecision.md) 集合</span><span class="sxs-lookup"><span data-stu-id="47bae-211">[accessReviewDecision](accessreviewdecision.md) collection</span></span> | <span data-ttu-id="47bae-212">呼叫者的决策集合（如果呼叫者是审阅者）。</span><span class="sxs-lookup"><span data-stu-id="47bae-212">The collection of decisions for the caller, if the caller is a reviewer.</span></span> |
| <span data-ttu-id="47bae-213">instances</span><span class="sxs-lookup"><span data-stu-id="47bae-213">instances</span></span> | <span data-ttu-id="47bae-214">[accessReview](accessreview.md) 集合</span><span class="sxs-lookup"><span data-stu-id="47bae-214">[accessReview](accessreview.md) collection</span></span> | <span data-ttu-id="47bae-215">如果此对象是定期访问评审，则访问评审实例的集合将过去、现在和未来。</span><span class="sxs-lookup"><span data-stu-id="47bae-215">The collection of access reviews instances past, present and future, if this object is a recurring access review.</span></span> |

<span data-ttu-id="47bae-216">这些关系是否存在于对象上取决于对象是一次性访问评审、定期访问评审系列还是定期访问评审的实例。</span><span class="sxs-lookup"><span data-stu-id="47bae-216">Whether these relationships are present on an object, depends upon whether the object is a one-time access review, the series of a recurring access review, or an instance of a recurring access review.</span></span>

| <span data-ttu-id="47bae-217">应用场景</span><span class="sxs-lookup"><span data-stu-id="47bae-217">Scenario</span></span> | <span data-ttu-id="47bae-218">有审阅者吗？</span><span class="sxs-lookup"><span data-stu-id="47bae-218">Has reviewers?</span></span> | <span data-ttu-id="47bae-219">有决策和 myDecisions 吗？</span><span class="sxs-lookup"><span data-stu-id="47bae-219">Has decisions and myDecisions?</span></span> | <span data-ttu-id="47bae-220">具有实例？</span><span class="sxs-lookup"><span data-stu-id="47bae-220">Has instances?</span></span> |
|:-------- |:-------------- |:------------------------------ |:-------------- |
| <span data-ttu-id="47bae-221">一次访问评审</span><span class="sxs-lookup"><span data-stu-id="47bae-221">One-time access review</span></span> | <span data-ttu-id="47bae-222">是</span><span class="sxs-lookup"><span data-stu-id="47bae-222">Yes</span></span> | <span data-ttu-id="47bae-223">是，一旦启动</span><span class="sxs-lookup"><span data-stu-id="47bae-223">Yes, once started</span></span> | <span data-ttu-id="47bae-224">否</span><span class="sxs-lookup"><span data-stu-id="47bae-224">No</span></span> |
| <span data-ttu-id="47bae-225">定期访问评审</span><span class="sxs-lookup"><span data-stu-id="47bae-225">Recurring access review</span></span> | <span data-ttu-id="47bae-226">是</span><span class="sxs-lookup"><span data-stu-id="47bae-226">Yes</span></span> | <span data-ttu-id="47bae-227">否</span><span class="sxs-lookup"><span data-stu-id="47bae-227">No</span></span> | <span data-ttu-id="47bae-228">是</span><span class="sxs-lookup"><span data-stu-id="47bae-228">Yes</span></span> |
| <span data-ttu-id="47bae-229">定期访问评审的实例</span><span class="sxs-lookup"><span data-stu-id="47bae-229">Instance of a recurring access review</span></span> | <span data-ttu-id="47bae-230">是</span><span class="sxs-lookup"><span data-stu-id="47bae-230">Yes</span></span> | <span data-ttu-id="47bae-231">是，一旦启动</span><span class="sxs-lookup"><span data-stu-id="47bae-231">Yes, once started</span></span> | <span data-ttu-id="47bae-232">否</span><span class="sxs-lookup"><span data-stu-id="47bae-232">No</span></span> |

## <a name="json-representation"></a><span data-ttu-id="47bae-233">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="47bae-233">JSON representation</span></span>

<span data-ttu-id="47bae-234">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="47bae-234">Here is a JSON representation of the resource.</span></span>

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


