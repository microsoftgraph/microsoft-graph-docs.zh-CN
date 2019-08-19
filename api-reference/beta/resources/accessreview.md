---
title: accessReview 资源类型
description: '在 Azure AD access 评论功能中, `accessReview`表示访问评审。  '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f42124a5b69027d16b2c8adc54d001fd8cf81c0e
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36460751"
---
# <a name="accessreview-resource-type"></a><span data-ttu-id="1693f-103">accessReview 资源类型</span><span class="sxs-lookup"><span data-stu-id="1693f-103">accessReview resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1693f-104">在 Azure AD [access 评论](accessreviews-root.md)功能中, `accessReview`表示访问评审。</span><span class="sxs-lookup"><span data-stu-id="1693f-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the `accessReview` represents an access review.</span></span>  


## <a name="methods"></a><span data-ttu-id="1693f-105">方法</span><span class="sxs-lookup"><span data-stu-id="1693f-105">Methods</span></span>

| <span data-ttu-id="1693f-106">方法</span><span class="sxs-lookup"><span data-stu-id="1693f-106">Method</span></span>           | <span data-ttu-id="1693f-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="1693f-107">Return Type</span></span>    |<span data-ttu-id="1693f-108">说明</span><span class="sxs-lookup"><span data-stu-id="1693f-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1693f-109">列出 accessReviews</span><span class="sxs-lookup"><span data-stu-id="1693f-109">List accessReviews</span></span>](../api/accessreview-list.md) | <span data-ttu-id="1693f-110">[accessReview](accessreview.md)集合</span><span class="sxs-lookup"><span data-stu-id="1693f-110">[accessReview](accessreview.md) collection</span></span> | <span data-ttu-id="1693f-111">列出 businessFlowTemplate 的 accessReviews。</span><span class="sxs-lookup"><span data-stu-id="1693f-111">List accessReviews for a businessFlowTemplate.</span></span> |
|[<span data-ttu-id="1693f-112">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="1693f-112">Get accessReview</span></span>](../api/accessreview-get.md) |   [<span data-ttu-id="1693f-113">accessReview</span><span class="sxs-lookup"><span data-stu-id="1693f-113">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="1693f-114">获取具有特定 id 的访问评审。</span><span class="sxs-lookup"><span data-stu-id="1693f-114">Get an access review with a specific id.</span></span> |
|[<span data-ttu-id="1693f-115">创建 accessReview</span><span class="sxs-lookup"><span data-stu-id="1693f-115">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="1693f-116">accessReview</span><span class="sxs-lookup"><span data-stu-id="1693f-116">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="1693f-117">创建新的 accessReview。</span><span class="sxs-lookup"><span data-stu-id="1693f-117">Create a new accessReview.</span></span> |
|[<span data-ttu-id="1693f-118">更新 accessReview</span><span class="sxs-lookup"><span data-stu-id="1693f-118">Update accessReview</span></span>](../api/accessreview-update.md) | [<span data-ttu-id="1693f-119">accessReview</span><span class="sxs-lookup"><span data-stu-id="1693f-119">accessReview</span></span>](accessreview.md) | <span data-ttu-id="1693f-120">更新 accessReview。</span><span class="sxs-lookup"><span data-stu-id="1693f-120">Update an accessReview.</span></span> |
|[<span data-ttu-id="1693f-121">删除 accessReview</span><span class="sxs-lookup"><span data-stu-id="1693f-121">Delete accessReview</span></span>](../api/accessreview-delete.md) | <span data-ttu-id="1693f-122">无。</span><span class="sxs-lookup"><span data-stu-id="1693f-122">None.</span></span>   | <span data-ttu-id="1693f-123">删除 accessReview。</span><span class="sxs-lookup"><span data-stu-id="1693f-123">Delete an accessReview.</span></span> |
|[<span data-ttu-id="1693f-124">列出 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="1693f-124">List accessReview reviewers</span></span>](../api/accessreview-listreviewers.md) |      <span data-ttu-id="1693f-125">[userIdentity](useridentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="1693f-125">[userIdentity](useridentity.md) collection</span></span>| <span data-ttu-id="1693f-126">获取 accessReview 的审阅者。</span><span class="sxs-lookup"><span data-stu-id="1693f-126">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="1693f-127">添加 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="1693f-127">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md) |      <span data-ttu-id="1693f-128">无。</span><span class="sxs-lookup"><span data-stu-id="1693f-128">None.</span></span>   |   <span data-ttu-id="1693f-129">向 accessReview 添加审阅者。</span><span class="sxs-lookup"><span data-stu-id="1693f-129">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="1693f-130">删除 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="1693f-130">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="1693f-131">无。</span><span class="sxs-lookup"><span data-stu-id="1693f-131">None.</span></span>  |   <span data-ttu-id="1693f-132">从 accessReview 中删除审阅者。</span><span class="sxs-lookup"><span data-stu-id="1693f-132">Remove a reviewer from an accessReview.</span></span> |
|[<span data-ttu-id="1693f-133">列出 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="1693f-133">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) |      <span data-ttu-id="1693f-134">[accessReviewDecision](accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="1693f-134">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="1693f-135">获取 accessReview 的决策。</span><span class="sxs-lookup"><span data-stu-id="1693f-135">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="1693f-136">列出我的 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="1693f-136">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) |     <span data-ttu-id="1693f-137">[accessReviewDecision](accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="1693f-137">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="1693f-138">作为审阅者, 请 accessReview 的决策。</span><span class="sxs-lookup"><span data-stu-id="1693f-138">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="1693f-139">发送 accessReview 提醒</span><span class="sxs-lookup"><span data-stu-id="1693f-139">Send accessReview reminder</span></span>](../api/accessreview-sendreminder.md) |        <span data-ttu-id="1693f-140">无。</span><span class="sxs-lookup"><span data-stu-id="1693f-140">None.</span></span>   |   <span data-ttu-id="1693f-141">向 accessReview 的审阅者发送提醒。</span><span class="sxs-lookup"><span data-stu-id="1693f-141">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="1693f-142">停止 accessReview</span><span class="sxs-lookup"><span data-stu-id="1693f-142">Stop accessReview</span></span>](../api/accessreview-stop.md) |     <span data-ttu-id="1693f-143">无。</span><span class="sxs-lookup"><span data-stu-id="1693f-143">None.</span></span>   |   <span data-ttu-id="1693f-144">停止 accessReview。</span><span class="sxs-lookup"><span data-stu-id="1693f-144">Stop an accessReview.</span></span> |
|[<span data-ttu-id="1693f-145">重置 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="1693f-145">Reset accessReview decisions</span></span>](../api/accessreview-reset.md) |     <span data-ttu-id="1693f-146">无。</span><span class="sxs-lookup"><span data-stu-id="1693f-146">None.</span></span>   |   <span data-ttu-id="1693f-147">在进行中的 accessReview 中重置决策。</span><span class="sxs-lookup"><span data-stu-id="1693f-147">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="1693f-148">应用 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="1693f-148">Apply accessReview decisions</span></span>](../api/accessreview-apply.md) |     <span data-ttu-id="1693f-149">无。</span><span class="sxs-lookup"><span data-stu-id="1693f-149">None.</span></span>   |   <span data-ttu-id="1693f-150">从已完成的 accessReview 应用决策。</span><span class="sxs-lookup"><span data-stu-id="1693f-150">Apply the decisions from a completed accessReview.</span></span>|

## <a name="properties"></a><span data-ttu-id="1693f-151">属性</span><span class="sxs-lookup"><span data-stu-id="1693f-151">Properties</span></span>
| <span data-ttu-id="1693f-152">属性</span><span class="sxs-lookup"><span data-stu-id="1693f-152">Property</span></span>     | <span data-ttu-id="1693f-153">类型</span><span class="sxs-lookup"><span data-stu-id="1693f-153">Type</span></span>   |<span data-ttu-id="1693f-154">说明</span><span class="sxs-lookup"><span data-stu-id="1693f-154">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                      |`String`                                                        | <span data-ttu-id="1693f-155">用于访问评审的功能分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1693f-155">The feature-assigned unique identifier of an access review.</span></span> |
| `displayName`             |`String`                                                        | <span data-ttu-id="1693f-156">访问审阅名称。</span><span class="sxs-lookup"><span data-stu-id="1693f-156">The access review name.</span></span> <span data-ttu-id="1693f-157">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="1693f-157">Required on create.</span></span> |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="1693f-158">计划开始评审时的日期时间。</span><span class="sxs-lookup"><span data-stu-id="1693f-158">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="1693f-159">这可能是将来的日期。</span><span class="sxs-lookup"><span data-stu-id="1693f-159">This could be a date in the future.</span></span>  <span data-ttu-id="1693f-160">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="1693f-160">Required on create.</span></span> |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="1693f-161">计划结束评审时的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1693f-161">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="1693f-162">此时间必须至少为一个晚于开始日期的一天。</span><span class="sxs-lookup"><span data-stu-id="1693f-162">This must be at least one day later than the start date.</span></span>  <span data-ttu-id="1693f-163">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="1693f-163">Required on create.</span></span> |
| `status`                  |`String`                                                        | <span data-ttu-id="1693f-164">此只读字段指定 accessReview 的状态。</span><span class="sxs-lookup"><span data-stu-id="1693f-164">This read-only field specifies the status of an accessReview.</span></span> <span data-ttu-id="1693f-165">典型状态包括`Initializing`、 `NotStarted`、 `Starting``InProgress` `Completing` `Completed` `AutoReviewed`、、、、和。 `AutoReviewing`</span><span class="sxs-lookup"><span data-stu-id="1693f-165">The typical states include `Initializing`, `NotStarted`, `Starting`,`InProgress`, `Completing`, `Completed`, `AutoReviewing`, and `AutoReviewed`.</span></span> |
| `description`             |`String`                                                        | <span data-ttu-id="1693f-166">由 access 评审创建者提供的说明, 用于向审阅者显示。</span><span class="sxs-lookup"><span data-stu-id="1693f-166">The description provided by the access review creator, to show to the reviewers.</span></span> |
| `businessFlowTemplateId`  |`String`                                                        | <span data-ttu-id="1693f-167">业务流模板标识符。</span><span class="sxs-lookup"><span data-stu-id="1693f-167">The business flow template identifier.</span></span> <span data-ttu-id="1693f-168">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="1693f-168">Required on create.</span></span> |
| `reviewerType`            |`String`                                                        | <span data-ttu-id="1693f-169">目标对象的审阅者的关系类型, 一个`self` `delegated`或。 `entityOwners`</span><span class="sxs-lookup"><span data-stu-id="1693f-169">The relationship type of reviewer to the target object, one of `self`, `delegated` or `entityOwners`.</span></span> <span data-ttu-id="1693f-170">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="1693f-170">Required on create.</span></span> | 
| `createdBy`               |[<span data-ttu-id="1693f-171">userIdentity</span><span class="sxs-lookup"><span data-stu-id="1693f-171">userIdentity</span></span>](useridentity.md)                                 | <span data-ttu-id="1693f-172">创建此评审的用户。</span><span class="sxs-lookup"><span data-stu-id="1693f-172">The user who created this review.</span></span> |
| `reviewedEntity`          |[<span data-ttu-id="1693f-173">identity</span><span class="sxs-lookup"><span data-stu-id="1693f-173">identity</span></span>](identity.md)                                      | <span data-ttu-id="1693f-174">访问权检查其访问权限分配的对象。</span><span class="sxs-lookup"><span data-stu-id="1693f-174">The object for which the access reviews is reviewing the access rights assignments.</span></span> <span data-ttu-id="1693f-175">此组可以是查看组中用户的成员身份的组, 也可以是用于查看对应用程序的用户分配的应用程序。</span><span class="sxs-lookup"><span data-stu-id="1693f-175">This can be the group for the review of memberships of users in a group, or the app for a review of assignments of users to an application.</span></span> <span data-ttu-id="1693f-176">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="1693f-176">Required on create.</span></span> | 
| `settings`                |`microsoft.graph.accessReviewSettings`             | <span data-ttu-id="1693f-177">AccessReview 的设置, 请参阅下面的类型定义。</span><span class="sxs-lookup"><span data-stu-id="1693f-177">The settings of an accessReview, see type definition below.</span></span> |



## <a name="relationships"></a><span data-ttu-id="1693f-178">关系</span><span class="sxs-lookup"><span data-stu-id="1693f-178">Relationships</span></span>




| <span data-ttu-id="1693f-179">关系</span><span class="sxs-lookup"><span data-stu-id="1693f-179">Relationship</span></span> | <span data-ttu-id="1693f-180">类型</span><span class="sxs-lookup"><span data-stu-id="1693f-180">Type</span></span>   |<span data-ttu-id="1693f-181">说明</span><span class="sxs-lookup"><span data-stu-id="1693f-181">Description</span></span>|
|:---------------|:--------|:----------|
| `reviewers`               |<span data-ttu-id="1693f-182">[userIdentity](useridentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="1693f-182">[userIdentity](useridentity.md) collection</span></span>                     | <span data-ttu-id="1693f-183">访问评审的审阅者的集合 (如果 access 评审 reviewerType 的类型`delegate`为)。</span><span class="sxs-lookup"><span data-stu-id="1693f-183">The collection of reviewers for an access review, if access review reviewerType is of type `delegate`.</span></span> |
| `decisions`               |<span data-ttu-id="1693f-184">[accessReviewDecision](accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="1693f-184">[accessReviewDecision](accessreviewdecision.md) collection</span></span> | <span data-ttu-id="1693f-185">此访问评审的决策集合。</span><span class="sxs-lookup"><span data-stu-id="1693f-185">The collection of decisions for this access review.</span></span> |
| `myDecisions`             |<span data-ttu-id="1693f-186">[accessReviewDecision](accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="1693f-186">[accessReviewDecision](accessreviewdecision.md) collection</span></span> | <span data-ttu-id="1693f-187">如果呼叫者是审阅者, 则为呼叫者做出决策的集合。</span><span class="sxs-lookup"><span data-stu-id="1693f-187">The collection of decisions for the caller, if the caller is a reviewer.</span></span> |
| `instances`               |<span data-ttu-id="1693f-188">[accessReview](accessreview.md)集合</span><span class="sxs-lookup"><span data-stu-id="1693f-188">[accessReview](accessreview.md) collection</span></span>         | <span data-ttu-id="1693f-189">如果此对象是定期访问审核, 则 access 的集合将审阅过去、现在和将来的实例。</span><span class="sxs-lookup"><span data-stu-id="1693f-189">The collection of access reviews instances past, present and future, if this object is a recurring access review.</span></span> |

<span data-ttu-id="1693f-190">对象中是否存在这些关系, 取决于该对象是一次性访问评审、定期访问评审的系列, 还是定期访问评审的实例。</span><span class="sxs-lookup"><span data-stu-id="1693f-190">Whether these relationships are present on an object, depends upon whether the object is a one-time access review, the series of a recurring access review, or an instance of a recurring access review.</span></span>

| <span data-ttu-id="1693f-191">应用场景</span><span class="sxs-lookup"><span data-stu-id="1693f-191">Scenario</span></span> | <span data-ttu-id="1693f-192">是否有审阅者？</span><span class="sxs-lookup"><span data-stu-id="1693f-192">Has reviewers?</span></span> | <span data-ttu-id="1693f-193">是否有决策和 myDecisions？</span><span class="sxs-lookup"><span data-stu-id="1693f-193">Has decisions and myDecisions?</span></span> | <span data-ttu-id="1693f-194">有实例吗？</span><span class="sxs-lookup"><span data-stu-id="1693f-194">Has instances?</span></span> |
|:---------|:---------------|:---------------|:---------------|
|<span data-ttu-id="1693f-195">一次性访问审核</span><span class="sxs-lookup"><span data-stu-id="1693f-195">One-time access review</span></span>|<span data-ttu-id="1693f-196">是</span><span class="sxs-lookup"><span data-stu-id="1693f-196">Yes</span></span> | <span data-ttu-id="1693f-197">是, 启动后</span><span class="sxs-lookup"><span data-stu-id="1693f-197">Yes, once started</span></span> | <span data-ttu-id="1693f-198">否</span><span class="sxs-lookup"><span data-stu-id="1693f-198">No</span></span> |
| <span data-ttu-id="1693f-199">定期访问审核</span><span class="sxs-lookup"><span data-stu-id="1693f-199">Recurring access review</span></span> | <span data-ttu-id="1693f-200">是</span><span class="sxs-lookup"><span data-stu-id="1693f-200">Yes</span></span> | <span data-ttu-id="1693f-201">否</span><span class="sxs-lookup"><span data-stu-id="1693f-201">No</span></span> | <span data-ttu-id="1693f-202">是</span><span class="sxs-lookup"><span data-stu-id="1693f-202">Yes</span></span> |
| <span data-ttu-id="1693f-203">定期访问审核实例</span><span class="sxs-lookup"><span data-stu-id="1693f-203">Instance of a recurring access review</span></span> | <span data-ttu-id="1693f-204">是</span><span class="sxs-lookup"><span data-stu-id="1693f-204">Yes</span></span> | <span data-ttu-id="1693f-205">是, 启动后</span><span class="sxs-lookup"><span data-stu-id="1693f-205">Yes, once started</span></span> | <span data-ttu-id="1693f-206">否</span><span class="sxs-lookup"><span data-stu-id="1693f-206">No</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1693f-207">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1693f-207">JSON representation</span></span>

<span data-ttu-id="1693f-208">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1693f-208">Here is a JSON representation of the resource.</span></span>

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

## <a name="the-accessreviewsettings-type"></a><span data-ttu-id="1693f-209">AccessReviewSettings 类型</span><span class="sxs-lookup"><span data-stu-id="1693f-209">The accessReviewSettings type</span></span>

<span data-ttu-id="1693f-210">在`accessReviewSettings`创建访问评审时提供其他设置, 以在启动访问评审时控制功能行为。</span><span class="sxs-lookup"><span data-stu-id="1693f-210">The `accessReviewSettings` provides additional settings when creating an access review, to control the feature behavior when starting an access review.</span></span>  <span data-ttu-id="1693f-211">此类型具有以下属性:</span><span class="sxs-lookup"><span data-stu-id="1693f-211">This type has the following properties:</span></span> 

| <span data-ttu-id="1693f-212">属性</span><span class="sxs-lookup"><span data-stu-id="1693f-212">Property</span></span>                     | <span data-ttu-id="1693f-213">类型</span><span class="sxs-lookup"><span data-stu-id="1693f-213">Type</span></span>                      | <span data-ttu-id="1693f-214">说明</span><span class="sxs-lookup"><span data-stu-id="1693f-214">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| `mailNotificationsEnabled`|`Boolean`                | <span data-ttu-id="1693f-215">指示是否已启用向审阅者发送邮件和审阅创建者的标志。</span><span class="sxs-lookup"><span data-stu-id="1693f-215">Flag to indicate whether sending mails to reviewers and the review creator is enabled.</span></span>                |
| `remindersEnabled`|`Boolean`       | <span data-ttu-id="1693f-216">指示是否启用了向审阅者发送提醒电子邮件的标志。</span><span class="sxs-lookup"><span data-stu-id="1693f-216">Flag to indicate whether sending reminder emails to reviewers are enabled.</span></span>       |
| `justificationRequiredOnApproval`|`Boolean` | <span data-ttu-id="1693f-217">指示审阅 access 时是否需要审阅者提供理由的标志。</span><span class="sxs-lookup"><span data-stu-id="1693f-217">Flag to indicate whether reviewers are required to provide a justification when reviewing access.</span></span>|
| `activityDurationInDays`|`Int64` | <span data-ttu-id="1693f-218">向审阅者显示的用户活动的天数。</span><span class="sxs-lookup"><span data-stu-id="1693f-218">The number of days of user activities to show to reviewers.</span></span> |
| `autoReviewEnabled`|`Boolean` | <span data-ttu-id="1693f-219">用于指示功能是否应在审阅者未提供且与自动应用一起使用时设置决策的标志。</span><span class="sxs-lookup"><span data-stu-id="1693f-219">Flag to indicate whether the feature should set a decision if the reviewer did not supply one, for use with auto-apply, is enabled.</span></span> |
| `autoReviewSettings`|`microsoft.graph.autoReviewSettings` | <span data-ttu-id="1693f-220">有关功能应如何设置审阅决定 (用于自动应用) 的详细设置, 请参阅下文所述。</span><span class="sxs-lookup"><span data-stu-id="1693f-220">Detailed settings for how the feature should set the review decision, for use with auto-apply, described below.</span></span> |
| `recurrenceSettings`|`microsoft.graph.accessReviewRecurrenceSettings` | <span data-ttu-id="1693f-221">定期的详细设置, 如下所述。</span><span class="sxs-lookup"><span data-stu-id="1693f-221">Detailed settings for recurrence, described below.</span></span> |
| `autoApplyReviewResultsEnabled`|`Boolean` | <span data-ttu-id="1693f-222">用于指示是否启用自动更改目标对象访问资源的自动应用功能的标志。</span><span class="sxs-lookup"><span data-stu-id="1693f-222">Flag to indicate whether auto-apply capability, to automatically change the target object access resource, is enabled.</span></span>  <span data-ttu-id="1693f-223">如果未启用, 则用户必须在评审完成后应用访问评审。</span><span class="sxs-lookup"><span data-stu-id="1693f-223">If not enabled, a user must, after the review completes, apply the access review.</span></span> |
| `accessRecommendationsEnabled`|`Boolean` | <span data-ttu-id="1693f-224">指示是否已启用向审阅者显示建议的标志。</span><span class="sxs-lookup"><span data-stu-id="1693f-224">Flag to indicate whether showing recommendations to reviewers is enabled.</span></span> |

## <a name="the-autoreviewsettings-type"></a><span data-ttu-id="1693f-225">AutoReviewSettings 类型</span><span class="sxs-lookup"><span data-stu-id="1693f-225">The autoReviewSettings type</span></span>

<span data-ttu-id="1693f-226">`autoReviewSettings`嵌入访问审阅设置中, 并指定访问评审完成时的功能行为。</span><span class="sxs-lookup"><span data-stu-id="1693f-226">The `autoReviewSettings` is embedded within the access review settings, and specifies the behavior for the feature when an access review completes.</span></span>  <span data-ttu-id="1693f-227">类型具有一个属性`notReviewedResult`。</span><span class="sxs-lookup"><span data-stu-id="1693f-227">The type has one property, `notReviewedResult`.</span></span>

| <span data-ttu-id="1693f-228">属性</span><span class="sxs-lookup"><span data-stu-id="1693f-228">Property</span></span>                     | <span data-ttu-id="1693f-229">类型</span><span class="sxs-lookup"><span data-stu-id="1693f-229">Type</span></span>     | <span data-ttu-id="1693f-230">说明</span><span class="sxs-lookup"><span data-stu-id="1693f-230">Description</span></span>                          |
| :--------------------------- | :------  | :----------                          |
| `notReviewedResult`          |`String`  | <span data-ttu-id="1693f-231">必须为 `Approve`、`Deny` 或 `Recommendation` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="1693f-231">Must be one of `Approve`, `Deny`, or `Recommendation`.</span></span> |


## <a name="the-accessreviewrecurrencesettings-type"></a><span data-ttu-id="1693f-232">AccessReviewRecurrenceSettings 类型</span><span class="sxs-lookup"><span data-stu-id="1693f-232">The accessReviewRecurrenceSettings type</span></span>

<span data-ttu-id="1693f-233">嵌入`accessReviewRecurrenceSettings`到 access 评审设置中, 并指定以固定间隔重复进行访问评审。</span><span class="sxs-lookup"><span data-stu-id="1693f-233">The `accessReviewRecurrenceSettings` is embedded within the access review settings, and specifies that the access review recurs at regular intervals.</span></span>  <span data-ttu-id="1693f-234">此类型具有以下属性:</span><span class="sxs-lookup"><span data-stu-id="1693f-234">This type has the following properties:</span></span>

| <span data-ttu-id="1693f-235">属性</span><span class="sxs-lookup"><span data-stu-id="1693f-235">Property</span></span>                     | <span data-ttu-id="1693f-236">类型</span><span class="sxs-lookup"><span data-stu-id="1693f-236">Type</span></span>                                                                                                          | <span data-ttu-id="1693f-237">说明</span><span class="sxs-lookup"><span data-stu-id="1693f-237">Description</span></span> |
| :--------------------------- | :------------------------------------------------------------------------------------------------------------ | :---------- |
| `recurrenceType`|`String`    | <span data-ttu-id="1693f-238">定期`onetime`间隔, 必须为、 `weekly`、 `monthly` `quarterly`、或`annual`的其中一个。</span><span class="sxs-lookup"><span data-stu-id="1693f-238">The recurrence interval, which must be one of `onetime`, `weekly`, `monthly`, `quarterly`, or `annual`.</span></span>                                                                   |
| `recurrenceEndType`|`String` | <span data-ttu-id="1693f-239">重复周期的结束方式。</span><span class="sxs-lookup"><span data-stu-id="1693f-239">How the recurrence ends.</span></span> <span data-ttu-id="1693f-240">如果是`Never`, 则不会出现定期系列的显式结束。</span><span class="sxs-lookup"><span data-stu-id="1693f-240">If it is `Never`, then there is no explicit end of the recurrence series.</span></span> <span data-ttu-id="1693f-241">如果是`endBy`, 则重复周期将在特定日期结束。</span><span class="sxs-lookup"><span data-stu-id="1693f-241">If it is `endBy`, then the recurrence ends at a certain date.</span></span> <span data-ttu-id="1693f-242">如果是`occurrences`, 则在审阅的实例完成`recurrentCount`后, 该系列将结束。</span><span class="sxs-lookup"><span data-stu-id="1693f-242">If it is `occurrences`, then the series ends after `recurrentCount` instances of the review have completed.</span></span> |
| `durationInDays`|`Int32`     | <span data-ttu-id="1693f-243">定期的持续时间 (以天为单位)。</span><span class="sxs-lookup"><span data-stu-id="1693f-243">The duration in days for recurrence.</span></span>                                                                              |
| `recurrenceCount`|`Int32`    | <span data-ttu-id="1693f-244">如果值`recurrenceEndType`为, 则为`occurrences`定期计数, 否则为0。</span><span class="sxs-lookup"><span data-stu-id="1693f-244">The count of recurrences, if the value of `recurrenceEndType` is `occurrences`, or 0 otherwise.</span></span>                                                        |


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
