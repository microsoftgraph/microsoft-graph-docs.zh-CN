---
title: accessReview 资源类型
description: '在 Azure AD 访问评审功能中， `accessReview` 表示访问评审。  '
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b6f24316e3ad45197b1630fdcdc4e249655ae19b
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133565"
---
# <a name="accessreview-resource-type"></a><span data-ttu-id="1bbd6-103">accessReview 资源类型</span><span class="sxs-lookup"><span data-stu-id="1bbd6-103">accessReview resource type</span></span>

<span data-ttu-id="1bbd6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bbd6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1bbd6-105">表示 Azure AD [访问评审](accessreviews-root.md)。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-105">Represents an Azure AD [access review](accessreviews-root.md).</span></span>  

## <a name="methods"></a><span data-ttu-id="1bbd6-106">方法</span><span class="sxs-lookup"><span data-stu-id="1bbd6-106">Methods</span></span>

| <span data-ttu-id="1bbd6-107">方法</span><span class="sxs-lookup"><span data-stu-id="1bbd6-107">Method</span></span>           | <span data-ttu-id="1bbd6-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="1bbd6-108">Return Type</span></span>    |<span data-ttu-id="1bbd6-109">说明</span><span class="sxs-lookup"><span data-stu-id="1bbd6-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1bbd6-110">列出 accessReviews</span><span class="sxs-lookup"><span data-stu-id="1bbd6-110">List accessReviews</span></span>](../api/accessreview-list.md) | <span data-ttu-id="1bbd6-111">[accessReview](accessreview.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1bbd6-111">[accessReview](accessreview.md) collection</span></span> | <span data-ttu-id="1bbd6-112">列出 businessFlowTemplate 的 accessReviews。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-112">List accessReviews for a businessFlowTemplate.</span></span> |
|[<span data-ttu-id="1bbd6-113">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="1bbd6-113">Get accessReview</span></span>](../api/accessreview-get.md) |   [<span data-ttu-id="1bbd6-114">accessReview</span><span class="sxs-lookup"><span data-stu-id="1bbd6-114">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="1bbd6-115">获取具有特定 ID 的访问评审。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-115">Get an access review with a specific id.</span></span> |
|[<span data-ttu-id="1bbd6-116">创建 accessReview</span><span class="sxs-lookup"><span data-stu-id="1bbd6-116">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="1bbd6-117">accessReview</span><span class="sxs-lookup"><span data-stu-id="1bbd6-117">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="1bbd6-118">创建新的 accessReview。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-118">Create a new accessReview.</span></span> |
|[<span data-ttu-id="1bbd6-119">更新 accessReview</span><span class="sxs-lookup"><span data-stu-id="1bbd6-119">Update accessReview</span></span>](../api/accessreview-update.md) | [<span data-ttu-id="1bbd6-120">accessReview</span><span class="sxs-lookup"><span data-stu-id="1bbd6-120">accessReview</span></span>](accessreview.md) | <span data-ttu-id="1bbd6-121">更新 accessReview。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-121">Update an accessReview.</span></span> |
|[<span data-ttu-id="1bbd6-122">删除 accessReview</span><span class="sxs-lookup"><span data-stu-id="1bbd6-122">Delete accessReview</span></span>](../api/accessreview-delete.md) | <span data-ttu-id="1bbd6-123">无。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-123">None.</span></span>   | <span data-ttu-id="1bbd6-124">删除 accessReview。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-124">Delete an accessReview.</span></span> |
|[<span data-ttu-id="1bbd6-125">列出 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="1bbd6-125">List accessReview reviewers</span></span>](../api/accessreview-listreviewers.md) | <span data-ttu-id="1bbd6-126">[userIdentity](useridentity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1bbd6-126">[userIdentity](useridentity.md) collection</span></span>|  <span data-ttu-id="1bbd6-127">获取 accessReview 的审阅者。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-127">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="1bbd6-128">添加 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="1bbd6-128">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md) | <span data-ttu-id="1bbd6-129">无。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-129">None.</span></span>    |   <span data-ttu-id="1bbd6-130">将审阅者添加到 accessReview。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-130">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="1bbd6-131">删除 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="1bbd6-131">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="1bbd6-132">无。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-132">None.</span></span> |    <span data-ttu-id="1bbd6-133">从 accessReview 中删除审阅者。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-133">Remove a reviewer from an accessReview.</span></span> |
|[<span data-ttu-id="1bbd6-134">列出 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="1bbd6-134">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) | <span data-ttu-id="1bbd6-135">[accessReviewDecision](accessreviewdecision.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1bbd6-135">[accessReviewDecision](accessreviewdecision.md) collection</span></span> | <span data-ttu-id="1bbd6-136">获取 accessReview 的决策。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-136">Get the decisions of an accessReview.</span></span> |
|[<span data-ttu-id="1bbd6-137">列出我的 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="1bbd6-137">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) | <span data-ttu-id="1bbd6-138">[accessReviewDecision](accessreviewdecision.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1bbd6-138">[accessReviewDecision](accessreviewdecision.md) collection</span></span> | <span data-ttu-id="1bbd6-139">作为审阅者，获取我有关 accessReview 的决定。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-139">As a reviewer, get my decisions of an accessReview.</span></span> |
|[<span data-ttu-id="1bbd6-140">发送 accessReview 提醒</span><span class="sxs-lookup"><span data-stu-id="1bbd6-140">Send accessReview reminder</span></span>](../api/accessreview-sendreminder.md) | <span data-ttu-id="1bbd6-141">无。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-141">None.</span></span> | <span data-ttu-id="1bbd6-142">向 accessReview 的审阅者发送提醒。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-142">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="1bbd6-143">Stop accessReview</span><span class="sxs-lookup"><span data-stu-id="1bbd6-143">Stop accessReview</span></span>](../api/accessreview-stop.md) | <span data-ttu-id="1bbd6-144">无。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-144">None.</span></span> | <span data-ttu-id="1bbd6-145">停止 accessReview。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-145">Stop an accessReview.</span></span> |
|[<span data-ttu-id="1bbd6-146">重置 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="1bbd6-146">Reset accessReview decisions</span></span>](../api/accessreview-reset.md) | <span data-ttu-id="1bbd6-147">无。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-147">None.</span></span>   |   <span data-ttu-id="1bbd6-148">重置正在进行中的 accessReview 中的决策。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-148">Reset the decisions in an in-progress accessReview.</span></span> |
|[<span data-ttu-id="1bbd6-149">应用 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="1bbd6-149">Apply accessReview decisions</span></span>](../api/accessreview-apply.md) | <span data-ttu-id="1bbd6-150">无。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-150">None.</span></span> | <span data-ttu-id="1bbd6-151">从已完成的 accessReview 应用决策。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-151">Apply the decisions from a completed accessReview.</span></span> |

## <a name="properties"></a><span data-ttu-id="1bbd6-152">属性</span><span class="sxs-lookup"><span data-stu-id="1bbd6-152">Properties</span></span>

| <span data-ttu-id="1bbd6-153">属性</span><span class="sxs-lookup"><span data-stu-id="1bbd6-153">Property</span></span> | <span data-ttu-id="1bbd6-154">类型</span><span class="sxs-lookup"><span data-stu-id="1bbd6-154">Type</span></span>   | <span data-ttu-id="1bbd6-155">说明</span><span class="sxs-lookup"><span data-stu-id="1bbd6-155">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="1bbd6-156">id</span><span class="sxs-lookup"><span data-stu-id="1bbd6-156">id</span></span> | <span data-ttu-id="1bbd6-157">字符串</span><span class="sxs-lookup"><span data-stu-id="1bbd6-157">String</span></span> | <span data-ttu-id="1bbd6-158">访问评审的功能分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-158">The feature-assigned unique identifier of an access review.</span></span> |
| <span data-ttu-id="1bbd6-159">displayName</span><span class="sxs-lookup"><span data-stu-id="1bbd6-159">displayName</span></span> | <span data-ttu-id="1bbd6-160">字符串</span><span class="sxs-lookup"><span data-stu-id="1bbd6-160">String</span></span> | <span data-ttu-id="1bbd6-161">访问评审名称。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-161">The access review name.</span></span> <span data-ttu-id="1bbd6-162">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-162">Required on create.</span></span> |
| <span data-ttu-id="1bbd6-163">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1bbd6-163">startDateTime</span></span> | <span data-ttu-id="1bbd6-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1bbd6-164">DateTimeOffset</span></span> | <span data-ttu-id="1bbd6-165">计划开始审阅的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-165">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="1bbd6-166">这可能是将来的日期。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-166">This could be a date in the future.</span></span>  <span data-ttu-id="1bbd6-167">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-167">Required on create.</span></span> |
| <span data-ttu-id="1bbd6-168">endDateTime</span><span class="sxs-lookup"><span data-stu-id="1bbd6-168">endDateTime</span></span> | <span data-ttu-id="1bbd6-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1bbd6-169">DateTimeOffset</span></span> | <span data-ttu-id="1bbd6-170">计划结束审阅的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-170">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="1bbd6-171">这必须至少比开始日期晚一天。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-171">This must be at least one day later than the start date.</span></span>  <span data-ttu-id="1bbd6-172">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-172">Required on create.</span></span> |
| <span data-ttu-id="1bbd6-173">status</span><span class="sxs-lookup"><span data-stu-id="1bbd6-173">status</span></span> | <span data-ttu-id="1bbd6-174">字符串</span><span class="sxs-lookup"><span data-stu-id="1bbd6-174">String</span></span> | <span data-ttu-id="1bbd6-175">此只读字段指定 accessReview 的状态。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-175">This read-only field specifies the status of an accessReview.</span></span> <span data-ttu-id="1bbd6-176">典型状态包括 `Initializing` 、 `NotStarted` `Starting` 、 、 、 `InProgress` `Completing` 和 `Completed` `AutoReviewing` `AutoReviewed` 。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-176">The typical states include `Initializing`, `NotStarted`, `Starting`,`InProgress`, `Completing`, `Completed`, `AutoReviewing`, and `AutoReviewed`.</span></span> |
| <span data-ttu-id="1bbd6-177">说明</span><span class="sxs-lookup"><span data-stu-id="1bbd6-177">description</span></span> | <span data-ttu-id="1bbd6-178">字符串</span><span class="sxs-lookup"><span data-stu-id="1bbd6-178">String</span></span> | <span data-ttu-id="1bbd6-179">访问评审创建者提供的向审阅者显示的说明。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-179">The description provided by the access review creator, to show to the reviewers.</span></span> |
| <span data-ttu-id="1bbd6-180">businessFlowTemplateId</span><span class="sxs-lookup"><span data-stu-id="1bbd6-180">businessFlowTemplateId</span></span> | <span data-ttu-id="1bbd6-181">字符串</span><span class="sxs-lookup"><span data-stu-id="1bbd6-181">String</span></span> | <span data-ttu-id="1bbd6-182">业务流程模板标识符。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-182">The business flow template identifier.</span></span> <span data-ttu-id="1bbd6-183">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-183">Required on create.</span></span>  <span data-ttu-id="1bbd6-184">此值区分大小写。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-184">This value is case sensitive.</span></span> |
| <span data-ttu-id="1bbd6-185">reviewerType</span><span class="sxs-lookup"><span data-stu-id="1bbd6-185">reviewerType</span></span> | <span data-ttu-id="1bbd6-186">字符串</span><span class="sxs-lookup"><span data-stu-id="1bbd6-186">String</span></span> | <span data-ttu-id="1bbd6-187">审阅者与目标对象的关系类型，其中一 `self` 个或 `delegated` `entityOwners` 。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-187">The relationship type of reviewer to the target object, one of `self`, `delegated` or `entityOwners`.</span></span> <span data-ttu-id="1bbd6-188">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-188">Required on create.</span></span> | 
| <span data-ttu-id="1bbd6-189">createdBy</span><span class="sxs-lookup"><span data-stu-id="1bbd6-189">createdBy</span></span> | [<span data-ttu-id="1bbd6-190">userIdentity</span><span class="sxs-lookup"><span data-stu-id="1bbd6-190">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="1bbd6-191">创建此评价的用户。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-191">The user who created this review.</span></span> |
| <span data-ttu-id="1bbd6-192">reviewedEntity</span><span class="sxs-lookup"><span data-stu-id="1bbd6-192">reviewedEntity</span></span> | [<span data-ttu-id="1bbd6-193">identity</span><span class="sxs-lookup"><span data-stu-id="1bbd6-193">identity</span></span>](identity.md) | <span data-ttu-id="1bbd6-194">访问评审正在审阅其访问权限分配的对象。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-194">The object for which the access reviews is reviewing the access rights assignments.</span></span> <span data-ttu-id="1bbd6-195">它可以是审阅组中用户成员身份的组，或者是用于查看用户到应用程序的分配的应用。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-195">This can be the group for the review of memberships of users in a group, or the app for a review of assignments of users to an application.</span></span> <span data-ttu-id="1bbd6-196">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-196">Required on create.</span></span> | 
| <span data-ttu-id="1bbd6-197">设置</span><span class="sxs-lookup"><span data-stu-id="1bbd6-197">settings</span></span> | [<span data-ttu-id="1bbd6-198">accessReviewSettings</span><span class="sxs-lookup"><span data-stu-id="1bbd6-198">accessReviewSettings</span></span>](accessreviewsettings.md) | <span data-ttu-id="1bbd6-199">accessReview 的设置，请参阅下面的类型定义。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-199">The settings of an accessReview, see type definition below.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1bbd6-200">关系</span><span class="sxs-lookup"><span data-stu-id="1bbd6-200">Relationships</span></span>

| <span data-ttu-id="1bbd6-201">关系</span><span class="sxs-lookup"><span data-stu-id="1bbd6-201">Relationship</span></span> | <span data-ttu-id="1bbd6-202">类型</span><span class="sxs-lookup"><span data-stu-id="1bbd6-202">Type</span></span>   | <span data-ttu-id="1bbd6-203">说明</span><span class="sxs-lookup"><span data-stu-id="1bbd6-203">Description</span></span> |
|:------------ |:---- |:----------- |
| <span data-ttu-id="1bbd6-204">审阅者</span><span class="sxs-lookup"><span data-stu-id="1bbd6-204">reviewers</span></span> | <span data-ttu-id="1bbd6-205">[userIdentity](useridentity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1bbd6-205">[userIdentity](useridentity.md) collection</span></span> | <span data-ttu-id="1bbd6-206">访问评审审阅审阅者的集合，如果访问审阅审阅者类型 `delegated` 。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-206">The collection of reviewers for an access review, if access review reviewerType is of type `delegated`.</span></span> |
| <span data-ttu-id="1bbd6-207">决策</span><span class="sxs-lookup"><span data-stu-id="1bbd6-207">decisions</span></span> | <span data-ttu-id="1bbd6-208">[accessReviewDecision](accessreviewdecision.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1bbd6-208">[accessReviewDecision](accessreviewdecision.md) collection</span></span> | <span data-ttu-id="1bbd6-209">此访问评审的决策集合。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-209">The collection of decisions for this access review.</span></span> |
| <span data-ttu-id="1bbd6-210">myDecisions</span><span class="sxs-lookup"><span data-stu-id="1bbd6-210">myDecisions</span></span> | <span data-ttu-id="1bbd6-211">[accessReviewDecision](accessreviewdecision.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1bbd6-211">[accessReviewDecision](accessreviewdecision.md) collection</span></span> | <span data-ttu-id="1bbd6-212">调用方的决策集合（如果呼叫者是审阅者）。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-212">The collection of decisions for the caller, if the caller is a reviewer.</span></span> |
| <span data-ttu-id="1bbd6-213">instances</span><span class="sxs-lookup"><span data-stu-id="1bbd6-213">instances</span></span> | <span data-ttu-id="1bbd6-214">[accessReview](accessreview.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1bbd6-214">[accessReview](accessreview.md) collection</span></span> | <span data-ttu-id="1bbd6-215">如果此对象是定期访问评审，访问评审实例的集合将过去、现在和未来。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-215">The collection of access reviews instances past, present and future, if this object is a recurring access review.</span></span> |

<span data-ttu-id="1bbd6-216">这些关系是否存在于对象上取决于对象是一次性访问评审、一系列定期访问评审还是定期访问评审的实例。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-216">Whether these relationships are present on an object, depends upon whether the object is a one-time access review, the series of a recurring access review, or an instance of a recurring access review.</span></span>

| <span data-ttu-id="1bbd6-217">应用场景</span><span class="sxs-lookup"><span data-stu-id="1bbd6-217">Scenario</span></span> | <span data-ttu-id="1bbd6-218">有审阅者吗？</span><span class="sxs-lookup"><span data-stu-id="1bbd6-218">Has reviewers?</span></span> | <span data-ttu-id="1bbd6-219">有决策和 myDecisions 吗？</span><span class="sxs-lookup"><span data-stu-id="1bbd6-219">Has decisions and myDecisions?</span></span> | <span data-ttu-id="1bbd6-220">具有实例？</span><span class="sxs-lookup"><span data-stu-id="1bbd6-220">Has instances?</span></span> |
|:-------- |:-------------- |:------------------------------ |:-------------- |
| <span data-ttu-id="1bbd6-221">一次访问评审</span><span class="sxs-lookup"><span data-stu-id="1bbd6-221">One-time access review</span></span> | <span data-ttu-id="1bbd6-222">是</span><span class="sxs-lookup"><span data-stu-id="1bbd6-222">Yes</span></span> | <span data-ttu-id="1bbd6-223">是，一旦启动</span><span class="sxs-lookup"><span data-stu-id="1bbd6-223">Yes, once started</span></span> | <span data-ttu-id="1bbd6-224">否</span><span class="sxs-lookup"><span data-stu-id="1bbd6-224">No</span></span> |
| <span data-ttu-id="1bbd6-225">定期访问评审</span><span class="sxs-lookup"><span data-stu-id="1bbd6-225">Recurring access review</span></span> | <span data-ttu-id="1bbd6-226">是</span><span class="sxs-lookup"><span data-stu-id="1bbd6-226">Yes</span></span> | <span data-ttu-id="1bbd6-227">否</span><span class="sxs-lookup"><span data-stu-id="1bbd6-227">No</span></span> | <span data-ttu-id="1bbd6-228">是</span><span class="sxs-lookup"><span data-stu-id="1bbd6-228">Yes</span></span> |
| <span data-ttu-id="1bbd6-229">定期访问评审的实例</span><span class="sxs-lookup"><span data-stu-id="1bbd6-229">Instance of a recurring access review</span></span> | <span data-ttu-id="1bbd6-230">是</span><span class="sxs-lookup"><span data-stu-id="1bbd6-230">Yes</span></span> | <span data-ttu-id="1bbd6-231">是，一旦启动</span><span class="sxs-lookup"><span data-stu-id="1bbd6-231">Yes, once started</span></span> | <span data-ttu-id="1bbd6-232">否</span><span class="sxs-lookup"><span data-stu-id="1bbd6-232">No</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1bbd6-233">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1bbd6-233">JSON representation</span></span>

<span data-ttu-id="1bbd6-234">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1bbd6-234">Here is a JSON representation of the resource.</span></span>

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


