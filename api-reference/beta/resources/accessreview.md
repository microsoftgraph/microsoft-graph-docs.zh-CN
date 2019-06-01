---
title: accessReview 资源类型
description: '在 Azure AD access 评论功能中, `accessReview`表示访问评审。  '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b1801a7f7cbd52375e4fbbfb42847b29539a2dde
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657733"
---
# <a name="accessreview-resource-type"></a><span data-ttu-id="187db-103">accessReview 资源类型</span><span class="sxs-lookup"><span data-stu-id="187db-103">accessReview resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="187db-104">在 Azure AD [access 评论](accessreviews-root.md)功能中, `accessReview`表示访问评审。</span><span class="sxs-lookup"><span data-stu-id="187db-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the `accessReview` represents an access review.</span></span>  


## <a name="methods"></a><span data-ttu-id="187db-105">方法</span><span class="sxs-lookup"><span data-stu-id="187db-105">Methods</span></span>

| <span data-ttu-id="187db-106">方法</span><span class="sxs-lookup"><span data-stu-id="187db-106">Method</span></span>           | <span data-ttu-id="187db-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="187db-107">Return Type</span></span>    |<span data-ttu-id="187db-108">说明</span><span class="sxs-lookup"><span data-stu-id="187db-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="187db-109">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="187db-109">Get accessReview</span></span>](../api/accessreview-get.md) |   [<span data-ttu-id="187db-110">accessReview</span><span class="sxs-lookup"><span data-stu-id="187db-110">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="187db-111">获取具有特定 id 的访问评审。</span><span class="sxs-lookup"><span data-stu-id="187db-111">Get an access review with a specific id.</span></span> |
|[<span data-ttu-id="187db-112">创建 accessReview</span><span class="sxs-lookup"><span data-stu-id="187db-112">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="187db-113">accessReview</span><span class="sxs-lookup"><span data-stu-id="187db-113">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="187db-114">创建新的 accessReview。</span><span class="sxs-lookup"><span data-stu-id="187db-114">Create a new accessReview.</span></span> |
|[<span data-ttu-id="187db-115">删除 accessReview</span><span class="sxs-lookup"><span data-stu-id="187db-115">Delete accessReview</span></span>](../api/accessreview-delete.md) | <span data-ttu-id="187db-116">无。</span><span class="sxs-lookup"><span data-stu-id="187db-116">None.</span></span>   | <span data-ttu-id="187db-117">删除 accessReview。</span><span class="sxs-lookup"><span data-stu-id="187db-117">Delete an accessReview.</span></span> |
|[<span data-ttu-id="187db-118">更新 accessReview</span><span class="sxs-lookup"><span data-stu-id="187db-118">Update accessReview</span></span>](../api/accessreview-update.md) | [<span data-ttu-id="187db-119">accessReview</span><span class="sxs-lookup"><span data-stu-id="187db-119">accessReview</span></span>](accessreview.md) | <span data-ttu-id="187db-120">更新 accessReview。</span><span class="sxs-lookup"><span data-stu-id="187db-120">Update an accessReview.</span></span> |
|[<span data-ttu-id="187db-121">列出 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="187db-121">List accessReview reviewers</span></span>](../api/accessreview-listreviewers.md) |      <span data-ttu-id="187db-122">[userIdentity](useridentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="187db-122">[userIdentity](useridentity.md) collection</span></span>| <span data-ttu-id="187db-123">获取 accessReview 的审阅者。</span><span class="sxs-lookup"><span data-stu-id="187db-123">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="187db-124">添加 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="187db-124">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md) |      <span data-ttu-id="187db-125">无。</span><span class="sxs-lookup"><span data-stu-id="187db-125">None.</span></span>   |   <span data-ttu-id="187db-126">向 accessReview 添加审阅者。</span><span class="sxs-lookup"><span data-stu-id="187db-126">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="187db-127">删除 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="187db-127">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="187db-128">无。</span><span class="sxs-lookup"><span data-stu-id="187db-128">None.</span></span>  |   <span data-ttu-id="187db-129">从 accessReview 中删除审阅者。</span><span class="sxs-lookup"><span data-stu-id="187db-129">Remove a reviewer from an accessReview.</span></span> |
|[<span data-ttu-id="187db-130">列出 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="187db-130">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) |      <span data-ttu-id="187db-131">[accessReviewDecision](accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="187db-131">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="187db-132">获取 accessReview 的决策。</span><span class="sxs-lookup"><span data-stu-id="187db-132">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="187db-133">列出我的 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="187db-133">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) |     <span data-ttu-id="187db-134">[accessReviewDecision](accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="187db-134">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="187db-135">作为审阅者, 请 accessReview 的决策。</span><span class="sxs-lookup"><span data-stu-id="187db-135">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="187db-136">发送 accessReview 提醒</span><span class="sxs-lookup"><span data-stu-id="187db-136">Send accessReview reminder</span></span>](../api/accessreview-sendreminder.md) |        <span data-ttu-id="187db-137">无。</span><span class="sxs-lookup"><span data-stu-id="187db-137">None.</span></span>   |   <span data-ttu-id="187db-138">向 accessReview 的审阅者发送提醒。</span><span class="sxs-lookup"><span data-stu-id="187db-138">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="187db-139">停止 accessReview</span><span class="sxs-lookup"><span data-stu-id="187db-139">Stop accessReview</span></span>](../api/accessreview-stop.md) |     <span data-ttu-id="187db-140">无。</span><span class="sxs-lookup"><span data-stu-id="187db-140">None.</span></span>   |   <span data-ttu-id="187db-141">停止 accessReview。</span><span class="sxs-lookup"><span data-stu-id="187db-141">Stop an accessReview.</span></span> |
|[<span data-ttu-id="187db-142">重置 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="187db-142">Reset accessReview decisions</span></span>](../api/accessreview-reset.md) |     <span data-ttu-id="187db-143">无。</span><span class="sxs-lookup"><span data-stu-id="187db-143">None.</span></span>   |   <span data-ttu-id="187db-144">在进行中的 accessReview 中重置决策。</span><span class="sxs-lookup"><span data-stu-id="187db-144">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="187db-145">应用 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="187db-145">Apply accessReview decisions</span></span>](../api/accessreview-apply.md) |     <span data-ttu-id="187db-146">无。</span><span class="sxs-lookup"><span data-stu-id="187db-146">None.</span></span>   |   <span data-ttu-id="187db-147">从已完成的 accessReview 应用决策。</span><span class="sxs-lookup"><span data-stu-id="187db-147">Apply the decisions from a completed accessReview.</span></span>|

## <a name="properties"></a><span data-ttu-id="187db-148">属性</span><span class="sxs-lookup"><span data-stu-id="187db-148">Properties</span></span>
| <span data-ttu-id="187db-149">属性</span><span class="sxs-lookup"><span data-stu-id="187db-149">Property</span></span>     | <span data-ttu-id="187db-150">类型</span><span class="sxs-lookup"><span data-stu-id="187db-150">Type</span></span>   |<span data-ttu-id="187db-151">说明</span><span class="sxs-lookup"><span data-stu-id="187db-151">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                      |`String`                                                        | <span data-ttu-id="187db-152">用于访问评审的功能分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="187db-152">The feature-assigned unique identifier of an access review.</span></span> |
| `displayName`             |`String`                                                        | <span data-ttu-id="187db-153">访问审阅名称。</span><span class="sxs-lookup"><span data-stu-id="187db-153">The access review name.</span></span> <span data-ttu-id="187db-154">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="187db-154">Required on create.</span></span> |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="187db-155">计划开始评审时的日期时间。</span><span class="sxs-lookup"><span data-stu-id="187db-155">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="187db-156">这可能是将来的日期。</span><span class="sxs-lookup"><span data-stu-id="187db-156">This could be a date in the future.</span></span>  <span data-ttu-id="187db-157">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="187db-157">Required on create.</span></span> |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="187db-158">计划结束评审时的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="187db-158">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="187db-159">此时间必须至少为一个晚于开始日期的一天。</span><span class="sxs-lookup"><span data-stu-id="187db-159">This must be at least one day later than the start date.</span></span>  <span data-ttu-id="187db-160">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="187db-160">Required on create.</span></span> |
| `status`                  |`String`                                                        | <span data-ttu-id="187db-161">此只读字段指定 accessReview 的状态。</span><span class="sxs-lookup"><span data-stu-id="187db-161">This read-only field specifies the status of an accessReview.</span></span> <span data-ttu-id="187db-162">典型状态包括`Initializing`、 `NotStarted`、 `Starting``InProgress` `Completing` `Completed` `AutoReviewed`、、、、和。 `AutoReviewing`</span><span class="sxs-lookup"><span data-stu-id="187db-162">The typical states include `Initializing`, `NotStarted`, `Starting`,`InProgress`, `Completing`, `Completed`, `AutoReviewing`, and `AutoReviewed`.</span></span> |
| `description`             |`String`                                                        | <span data-ttu-id="187db-163">由 access 评审创建者提供的说明, 用于向审阅者显示。</span><span class="sxs-lookup"><span data-stu-id="187db-163">The description provided by the access review creator, to show to the reviewers.</span></span> |
| `businessFlowTemplateId`  |`String`                                                        | <span data-ttu-id="187db-164">业务流模板标识符。</span><span class="sxs-lookup"><span data-stu-id="187db-164">The business flow template identifier.</span></span> <span data-ttu-id="187db-165">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="187db-165">Required on create.</span></span> |
| `reviewerType`            |`String`                                                        | <span data-ttu-id="187db-166">目标对象的审阅者的关系类型, 一个`self` `delegated`或。 `entityOwners`</span><span class="sxs-lookup"><span data-stu-id="187db-166">The relationship type of reviewer to the target object, one of `self`, `delegated` or `entityOwners`.</span></span> <span data-ttu-id="187db-167">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="187db-167">Required on create.</span></span> | 
| `createdBy`               |[<span data-ttu-id="187db-168">userIdentity</span><span class="sxs-lookup"><span data-stu-id="187db-168">userIdentity</span></span>](useridentity.md)                                 | <span data-ttu-id="187db-169">创建此评审的用户。</span><span class="sxs-lookup"><span data-stu-id="187db-169">The user who created this review.</span></span> |
| `reviewedEntity`          |[<span data-ttu-id="187db-170">identity</span><span class="sxs-lookup"><span data-stu-id="187db-170">identity</span></span>](identity.md)                                      | <span data-ttu-id="187db-171">访问权检查其访问权限分配的对象。</span><span class="sxs-lookup"><span data-stu-id="187db-171">The object for which the access reviews is reviewing the access rights assignments.</span></span> <span data-ttu-id="187db-172">此组可以是查看组中用户的成员身份的组, 也可以是用于查看对应用程序的用户分配的应用程序。</span><span class="sxs-lookup"><span data-stu-id="187db-172">This can be the group for the review of memberships of users in a group, or the app for a review of assignments of users to an application.</span></span> <span data-ttu-id="187db-173">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="187db-173">Required on create.</span></span> | 
| `settings`                |`microsoft.graph.accessReviewSettings`             | <span data-ttu-id="187db-174">AccessReview 的设置, 请参阅下面的类型定义。</span><span class="sxs-lookup"><span data-stu-id="187db-174">The settings of an accessReview, see type definition below.</span></span> |



## <a name="relationships"></a><span data-ttu-id="187db-175">关系</span><span class="sxs-lookup"><span data-stu-id="187db-175">Relationships</span></span>




| <span data-ttu-id="187db-176">关系</span><span class="sxs-lookup"><span data-stu-id="187db-176">Relationship</span></span> | <span data-ttu-id="187db-177">类型</span><span class="sxs-lookup"><span data-stu-id="187db-177">Type</span></span>   |<span data-ttu-id="187db-178">说明</span><span class="sxs-lookup"><span data-stu-id="187db-178">Description</span></span>|
|:---------------|:--------|:----------|
| `reviewers`               |<span data-ttu-id="187db-179">[userIdentity](useridentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="187db-179">[userIdentity](useridentity.md) collection</span></span>                     | <span data-ttu-id="187db-180">访问评审的审阅者的集合 (如果 access 评审 reviewerType 的类型`delegate`为)。</span><span class="sxs-lookup"><span data-stu-id="187db-180">The collection of reviewers for an access review, if access review reviewerType is of type `delegate`.</span></span> |
| `decisions`               |<span data-ttu-id="187db-181">[accessReviewDecision](accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="187db-181">[accessReviewDecision](accessreviewdecision.md) collection</span></span> | <span data-ttu-id="187db-182">此访问评审的决策集合。</span><span class="sxs-lookup"><span data-stu-id="187db-182">The collection of decisions for this access review.</span></span> |
| `myDecisions`             |<span data-ttu-id="187db-183">[accessReviewDecision](accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="187db-183">[accessReviewDecision](accessreviewdecision.md) collection</span></span> | <span data-ttu-id="187db-184">如果呼叫者是审阅者, 则为呼叫者做出决策的集合。</span><span class="sxs-lookup"><span data-stu-id="187db-184">The collection of decisions for the caller, if the caller is a reviewer.</span></span> |
| `instances`               |<span data-ttu-id="187db-185">[accessReview](accessreview.md)集合</span><span class="sxs-lookup"><span data-stu-id="187db-185">[accessReview](accessreview.md) collection</span></span>         | <span data-ttu-id="187db-186">如果此对象是定期访问审核, 则 access 的集合将审阅过去、现在和将来的实例。</span><span class="sxs-lookup"><span data-stu-id="187db-186">The collection of access reviews instances past, present and future, if this object is a recurring access review.</span></span> |

<span data-ttu-id="187db-187">对象中是否存在这些关系, 取决于该对象是一次性访问评审、定期访问评审的系列, 还是定期访问评审的实例。</span><span class="sxs-lookup"><span data-stu-id="187db-187">Whether these relationships are present on an object, depends upon whether the object is a one-time access review, the series of a recurring access review, or an instance of a recurring access review.</span></span>

| <span data-ttu-id="187db-188">应用场景</span><span class="sxs-lookup"><span data-stu-id="187db-188">Scenario</span></span> | <span data-ttu-id="187db-189">是否有审阅者？</span><span class="sxs-lookup"><span data-stu-id="187db-189">Has reviewers?</span></span> | <span data-ttu-id="187db-190">是否有决策和 myDecisions？</span><span class="sxs-lookup"><span data-stu-id="187db-190">Has decisions and myDecisions?</span></span> | <span data-ttu-id="187db-191">有实例吗？</span><span class="sxs-lookup"><span data-stu-id="187db-191">Has instances?</span></span> |
|:---------|:---------------|:---------------|:---------------|
|<span data-ttu-id="187db-192">一次性访问审核</span><span class="sxs-lookup"><span data-stu-id="187db-192">One-time access review</span></span>|<span data-ttu-id="187db-193">是</span><span class="sxs-lookup"><span data-stu-id="187db-193">Yes</span></span> | <span data-ttu-id="187db-194">是, 启动后</span><span class="sxs-lookup"><span data-stu-id="187db-194">Yes, once started</span></span> | <span data-ttu-id="187db-195">否</span><span class="sxs-lookup"><span data-stu-id="187db-195">No</span></span> |
| <span data-ttu-id="187db-196">定期访问审核</span><span class="sxs-lookup"><span data-stu-id="187db-196">Recurring access review</span></span> | <span data-ttu-id="187db-197">是</span><span class="sxs-lookup"><span data-stu-id="187db-197">Yes</span></span> | <span data-ttu-id="187db-198">否</span><span class="sxs-lookup"><span data-stu-id="187db-198">No</span></span> | <span data-ttu-id="187db-199">是</span><span class="sxs-lookup"><span data-stu-id="187db-199">Yes</span></span> |
| <span data-ttu-id="187db-200">定期访问审核实例</span><span class="sxs-lookup"><span data-stu-id="187db-200">Instance of a recurring access review</span></span> | <span data-ttu-id="187db-201">是</span><span class="sxs-lookup"><span data-stu-id="187db-201">Yes</span></span> | <span data-ttu-id="187db-202">是, 启动后</span><span class="sxs-lookup"><span data-stu-id="187db-202">Yes, once started</span></span> | <span data-ttu-id="187db-203">否</span><span class="sxs-lookup"><span data-stu-id="187db-203">No</span></span> |

## <a name="json-representation"></a><span data-ttu-id="187db-204">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="187db-204">JSON representation</span></span>

<span data-ttu-id="187db-205">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="187db-205">Here is a JSON representation of the resource.</span></span>

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
 "createdBy": "microsoft.graph.userIdentity",
 "reviewedEntity": "microsoft.graph.identity",
 "settings": "microsoft.graph.accessReviewSettings",
 "reviewers": "Collection(microsoft.graph.userIdentity)"
}

```

## <a name="the-accessreviewsettings-type"></a><span data-ttu-id="187db-206">AccessReviewSettings 类型</span><span class="sxs-lookup"><span data-stu-id="187db-206">The accessReviewSettings type</span></span>

<span data-ttu-id="187db-207">在`accessReviewSettings`创建访问评审时提供其他设置, 以在启动访问评审时控制功能行为。</span><span class="sxs-lookup"><span data-stu-id="187db-207">The `accessReviewSettings` provides additional settings when creating an access review, to control the feature behavior when starting an access review.</span></span>  <span data-ttu-id="187db-208">此类型具有以下属性:</span><span class="sxs-lookup"><span data-stu-id="187db-208">This type has the following properties:</span></span> 

| <span data-ttu-id="187db-209">属性</span><span class="sxs-lookup"><span data-stu-id="187db-209">Property</span></span>                     | <span data-ttu-id="187db-210">类型</span><span class="sxs-lookup"><span data-stu-id="187db-210">Type</span></span>                      | <span data-ttu-id="187db-211">说明</span><span class="sxs-lookup"><span data-stu-id="187db-211">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| `mailNotificationsEnabled`|`Boolean`                | <span data-ttu-id="187db-212">指示是否已启用向审阅者发送邮件和审阅创建者的标志。</span><span class="sxs-lookup"><span data-stu-id="187db-212">Flag to indicate whether sending mails to reviewers and the review creator is enabled.</span></span>                |
| `remindersEnabled`|`Boolean`       | <span data-ttu-id="187db-213">指示是否启用了向审阅者发送提醒电子邮件的标志。</span><span class="sxs-lookup"><span data-stu-id="187db-213">Flag to indicate whether sending reminder emails to reviewers are enabled.</span></span>       |
| `justificationRequiredOnApproval`|`Boolean` | <span data-ttu-id="187db-214">指示审阅 access 时是否需要审阅者提供理由的标志。</span><span class="sxs-lookup"><span data-stu-id="187db-214">Flag to indicate whether reviewers are required to provide a justification when reviewing access.</span></span>|
| `activityDurationInDays`|`Int64` | <span data-ttu-id="187db-215">向审阅者显示的用户活动的天数。</span><span class="sxs-lookup"><span data-stu-id="187db-215">The number of days of user activities to show to reviewers.</span></span> |
| `autoReviewEnabled`|`Boolean` | <span data-ttu-id="187db-216">用于指示功能是否应在审阅者未提供且与自动应用一起使用时设置决策的标志。</span><span class="sxs-lookup"><span data-stu-id="187db-216">Flag to indicate whether the feature should set a decision if the reviewer did not supply one, for use with auto-apply, is enabled.</span></span> |
| `autoReviewSettings`|`microsoft.graph.autoReviewSettings` | <span data-ttu-id="187db-217">有关功能应如何设置审阅决定 (用于自动应用) 的详细设置, 请参阅下文所述。</span><span class="sxs-lookup"><span data-stu-id="187db-217">Detailed settings for how the feature should set the review decision, for use with auto-apply, described below.</span></span> |
| `recurrenceSettings`|`microsoft.graph.accessReviewRecurrenceSettings` | <span data-ttu-id="187db-218">定期的详细设置, 如下所述。</span><span class="sxs-lookup"><span data-stu-id="187db-218">Detailed settings for recurrence, described below.</span></span> |
| `autoApplyReviewResultsEnabled`|`Boolean` | <span data-ttu-id="187db-219">用于指示是否启用自动更改目标对象访问资源的自动应用功能的标志。</span><span class="sxs-lookup"><span data-stu-id="187db-219">Flag to indicate whether auto-apply capability, to automatically change the target object access resource, is enabled.</span></span>  <span data-ttu-id="187db-220">如果未启用, 则用户必须在评审完成后应用访问评审。</span><span class="sxs-lookup"><span data-stu-id="187db-220">If not enabled, a user must, after the review completes, apply the access review.</span></span> |
| `accessRecommendationsEnabled`|`Boolean` | <span data-ttu-id="187db-221">指示是否已启用向审阅者显示建议的标志。</span><span class="sxs-lookup"><span data-stu-id="187db-221">Flag to indicate whether showing recommendations to reviewers is enabled.</span></span> |

## <a name="the-autoreviewsettings-type"></a><span data-ttu-id="187db-222">AutoReviewSettings 类型</span><span class="sxs-lookup"><span data-stu-id="187db-222">The autoReviewSettings type</span></span>

<span data-ttu-id="187db-223">`autoReviewSettings`嵌入访问审阅设置中, 并指定访问评审完成时的功能行为。</span><span class="sxs-lookup"><span data-stu-id="187db-223">The `autoReviewSettings` is embedded within the access review settings, and specifies the behavior for the feature when an access review completes.</span></span>  <span data-ttu-id="187db-224">类型具有一个属性`notReviewedResult`。</span><span class="sxs-lookup"><span data-stu-id="187db-224">The type has one property, `notReviewedResult`.</span></span>

| <span data-ttu-id="187db-225">属性</span><span class="sxs-lookup"><span data-stu-id="187db-225">Property</span></span>                     | <span data-ttu-id="187db-226">类型</span><span class="sxs-lookup"><span data-stu-id="187db-226">Type</span></span>     | <span data-ttu-id="187db-227">说明</span><span class="sxs-lookup"><span data-stu-id="187db-227">Description</span></span>                          |
| :--------------------------- | :------  | :----------                          |
| `notReviewedResult`          |`String`  | <span data-ttu-id="187db-228">必须为 `Approve`、`Deny` 或 `Recommendation` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="187db-228">Must be one of `Approve`, `Deny`, or `Recommendation`.</span></span> |


## <a name="the-accessreviewrecurrencesettings-type"></a><span data-ttu-id="187db-229">AccessReviewRecurrenceSettings 类型</span><span class="sxs-lookup"><span data-stu-id="187db-229">The accessReviewRecurrenceSettings type</span></span>

<span data-ttu-id="187db-230">嵌入`accessReviewRecurrenceSettings`到 access 评审设置中, 并指定以固定间隔重复进行访问评审。</span><span class="sxs-lookup"><span data-stu-id="187db-230">The `accessReviewRecurrenceSettings` is embedded within the access review settings, and specifies that the access review recurs at regular intervals.</span></span>  <span data-ttu-id="187db-231">此类型具有以下属性:</span><span class="sxs-lookup"><span data-stu-id="187db-231">This type has the following properties:</span></span>

| <span data-ttu-id="187db-232">属性</span><span class="sxs-lookup"><span data-stu-id="187db-232">Property</span></span>                     | <span data-ttu-id="187db-233">类型</span><span class="sxs-lookup"><span data-stu-id="187db-233">Type</span></span>                                                                                                          | <span data-ttu-id="187db-234">说明</span><span class="sxs-lookup"><span data-stu-id="187db-234">Description</span></span> |
| :--------------------------- | :------------------------------------------------------------------------------------------------------------ | :---------- |
| `recurrenceType`|`String`    | <span data-ttu-id="187db-235">定期`onetime`间隔, 必须为、 `weekly`、 `monthly` `quarterly`、或`annual`的其中一个。</span><span class="sxs-lookup"><span data-stu-id="187db-235">The recurrence interval, which must be one of `onetime`, `weekly`, `monthly`, `quarterly`, or `annual`.</span></span>                                                                   |
| `recurrenceEndType`|`String` | <span data-ttu-id="187db-236">重复周期的结束方式。</span><span class="sxs-lookup"><span data-stu-id="187db-236">How the recurrence ends.</span></span> <span data-ttu-id="187db-237">如果是`Never`, 则不会出现定期系列的显式结束。</span><span class="sxs-lookup"><span data-stu-id="187db-237">If it is `Never`, then there is no explicit end of the recurrence series.</span></span> <span data-ttu-id="187db-238">如果是`endBy`, 则重复周期将在特定日期结束。</span><span class="sxs-lookup"><span data-stu-id="187db-238">If it is `endBy`, then the recurrence ends at a certain date.</span></span> <span data-ttu-id="187db-239">如果是`occurrences`, 则在审阅的实例完成`recurrentCount`后, 该系列将结束。</span><span class="sxs-lookup"><span data-stu-id="187db-239">If it is `occurrences`, then the series ends after `recurrentCount` instances of the review have completed.</span></span> |
| `durationInDays`|`Int32`     | <span data-ttu-id="187db-240">定期的持续时间 (以天为单位)。</span><span class="sxs-lookup"><span data-stu-id="187db-240">The duration in days for recurrence.</span></span>                                                                              |
| `recurrenceCount`|`Int32`    | <span data-ttu-id="187db-241">如果值`recurrenceEndType`为, 则为`occurrences`定期计数, 否则为0。</span><span class="sxs-lookup"><span data-stu-id="187db-241">The count of recurrences, if the value of `recurrenceEndType` is `occurrences`, or 0 otherwise.</span></span>                                                        |


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
