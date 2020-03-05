---
title: accessReview 资源类型
description: '在 Azure AD access 评论功能中， `accessReview`表示访问评审。  '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0ef5ff461f906da6c9480f7f44ba73a870ebfe48
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508483"
---
# <a name="accessreview-resource-type"></a><span data-ttu-id="3c9aa-103">accessReview 资源类型</span><span class="sxs-lookup"><span data-stu-id="3c9aa-103">accessReview resource type</span></span>

<span data-ttu-id="3c9aa-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="3c9aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c9aa-105">在 Azure AD [access 评论](accessreviews-root.md)功能中， `accessReview`表示访问评审。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the `accessReview` represents an access review.</span></span>  


## <a name="methods"></a><span data-ttu-id="3c9aa-106">方法</span><span class="sxs-lookup"><span data-stu-id="3c9aa-106">Methods</span></span>

| <span data-ttu-id="3c9aa-107">方法</span><span class="sxs-lookup"><span data-stu-id="3c9aa-107">Method</span></span>           | <span data-ttu-id="3c9aa-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="3c9aa-108">Return Type</span></span>    |<span data-ttu-id="3c9aa-109">说明</span><span class="sxs-lookup"><span data-stu-id="3c9aa-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3c9aa-110">列出 accessReviews</span><span class="sxs-lookup"><span data-stu-id="3c9aa-110">List accessReviews</span></span>](../api/accessreview-list.md) | <span data-ttu-id="3c9aa-111">[accessReview](accessreview.md)集合</span><span class="sxs-lookup"><span data-stu-id="3c9aa-111">[accessReview](accessreview.md) collection</span></span> | <span data-ttu-id="3c9aa-112">列出 businessFlowTemplate 的 accessReviews。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-112">List accessReviews for a businessFlowTemplate.</span></span> |
|[<span data-ttu-id="3c9aa-113">获取 accessReview</span><span class="sxs-lookup"><span data-stu-id="3c9aa-113">Get accessReview</span></span>](../api/accessreview-get.md) |   [<span data-ttu-id="3c9aa-114">accessReview</span><span class="sxs-lookup"><span data-stu-id="3c9aa-114">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="3c9aa-115">获取具有特定 id 的访问评审。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-115">Get an access review with a specific id.</span></span> |
|[<span data-ttu-id="3c9aa-116">创建 accessReview</span><span class="sxs-lookup"><span data-stu-id="3c9aa-116">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="3c9aa-117">accessReview</span><span class="sxs-lookup"><span data-stu-id="3c9aa-117">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="3c9aa-118">创建新的 accessReview。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-118">Create a new accessReview.</span></span> |
|[<span data-ttu-id="3c9aa-119">更新 accessReview</span><span class="sxs-lookup"><span data-stu-id="3c9aa-119">Update accessReview</span></span>](../api/accessreview-update.md) | [<span data-ttu-id="3c9aa-120">accessReview</span><span class="sxs-lookup"><span data-stu-id="3c9aa-120">accessReview</span></span>](accessreview.md) | <span data-ttu-id="3c9aa-121">更新 accessReview。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-121">Update an accessReview.</span></span> |
|[<span data-ttu-id="3c9aa-122">删除 accessReview</span><span class="sxs-lookup"><span data-stu-id="3c9aa-122">Delete accessReview</span></span>](../api/accessreview-delete.md) | <span data-ttu-id="3c9aa-123">无。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-123">None.</span></span>   | <span data-ttu-id="3c9aa-124">删除 accessReview。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-124">Delete an accessReview.</span></span> |
|[<span data-ttu-id="3c9aa-125">列出 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="3c9aa-125">List accessReview reviewers</span></span>](../api/accessreview-listreviewers.md) |      <span data-ttu-id="3c9aa-126">[userIdentity](useridentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="3c9aa-126">[userIdentity](useridentity.md) collection</span></span>| <span data-ttu-id="3c9aa-127">获取 accessReview 的审阅者。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-127">Get the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="3c9aa-128">添加 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="3c9aa-128">Add accessReview reviewer</span></span>](../api/accessreview-addreviewer.md) |      <span data-ttu-id="3c9aa-129">无。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-129">None.</span></span>   |   <span data-ttu-id="3c9aa-130">向 accessReview 添加审阅者。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-130">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="3c9aa-131">删除 accessReview 审阅者</span><span class="sxs-lookup"><span data-stu-id="3c9aa-131">Remove accessReview reviewer</span></span>](../api/accessreview-removereviewer.md) | <span data-ttu-id="3c9aa-132">无。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-132">None.</span></span>  |   <span data-ttu-id="3c9aa-133">从 accessReview 中删除审阅者。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-133">Remove a reviewer from an accessReview.</span></span> |
|[<span data-ttu-id="3c9aa-134">列出 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="3c9aa-134">List accessReview decisions</span></span>](../api/accessreview-listdecisions.md) |      <span data-ttu-id="3c9aa-135">[accessReviewDecision](accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="3c9aa-135">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="3c9aa-136">获取 accessReview 的决策。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-136">Get the decisions of an accessReview.</span></span>|
|[<span data-ttu-id="3c9aa-137">列出我的 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="3c9aa-137">List my accessReview decisions</span></span>](../api/accessreview-listmydecisions.md) |     <span data-ttu-id="3c9aa-138">[accessReviewDecision](accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="3c9aa-138">[accessReviewDecision](accessreviewdecision.md) collection</span></span>| <span data-ttu-id="3c9aa-139">作为审阅者，请 accessReview 的决策。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-139">As a reviewer, get my decisions of an accessReview.</span></span>|
|[<span data-ttu-id="3c9aa-140">发送 accessReview 提醒</span><span class="sxs-lookup"><span data-stu-id="3c9aa-140">Send accessReview reminder</span></span>](../api/accessreview-sendreminder.md) |        <span data-ttu-id="3c9aa-141">无。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-141">None.</span></span>   |   <span data-ttu-id="3c9aa-142">向 accessReview 的审阅者发送提醒。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-142">Send a reminder to the reviewers of an accessReview.</span></span> |
|[<span data-ttu-id="3c9aa-143">停止 accessReview</span><span class="sxs-lookup"><span data-stu-id="3c9aa-143">Stop accessReview</span></span>](../api/accessreview-stop.md) |     <span data-ttu-id="3c9aa-144">无。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-144">None.</span></span>   |   <span data-ttu-id="3c9aa-145">停止 accessReview。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-145">Stop an accessReview.</span></span> |
|[<span data-ttu-id="3c9aa-146">重置 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="3c9aa-146">Reset accessReview decisions</span></span>](../api/accessreview-reset.md) |     <span data-ttu-id="3c9aa-147">无。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-147">None.</span></span>   |   <span data-ttu-id="3c9aa-148">在进行中的 accessReview 中重置决策。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-148">Reset the decisions in an in-progress accessReview.</span></span>|
|[<span data-ttu-id="3c9aa-149">应用 accessReview 决策</span><span class="sxs-lookup"><span data-stu-id="3c9aa-149">Apply accessReview decisions</span></span>](../api/accessreview-apply.md) |     <span data-ttu-id="3c9aa-150">无。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-150">None.</span></span>   |   <span data-ttu-id="3c9aa-151">从已完成的 accessReview 应用决策。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-151">Apply the decisions from a completed accessReview.</span></span>|

## <a name="properties"></a><span data-ttu-id="3c9aa-152">属性</span><span class="sxs-lookup"><span data-stu-id="3c9aa-152">Properties</span></span>
| <span data-ttu-id="3c9aa-153">属性</span><span class="sxs-lookup"><span data-stu-id="3c9aa-153">Property</span></span>     | <span data-ttu-id="3c9aa-154">类型</span><span class="sxs-lookup"><span data-stu-id="3c9aa-154">Type</span></span>   |<span data-ttu-id="3c9aa-155">说明</span><span class="sxs-lookup"><span data-stu-id="3c9aa-155">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                      |`String`                                                        | <span data-ttu-id="3c9aa-156">用于访问评审的功能分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-156">The feature-assigned unique identifier of an access review.</span></span> |
| `displayName`             |`String`                                                        | <span data-ttu-id="3c9aa-157">访问审阅名称。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-157">The access review name.</span></span> <span data-ttu-id="3c9aa-158">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-158">Required on create.</span></span> |
| `startDateTime`           |`DateTimeOffset`                                                | <span data-ttu-id="3c9aa-159">计划开始评审时的日期时间。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-159">The DateTime when the review is scheduled to be start.</span></span>  <span data-ttu-id="3c9aa-160">这可能是将来的日期。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-160">This could be a date in the future.</span></span>  <span data-ttu-id="3c9aa-161">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-161">Required on create.</span></span> |
| `endDateTime`             |`DateTimeOffset`                                                | <span data-ttu-id="3c9aa-162">计划结束评审时的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-162">The DateTime when the review is scheduled to end.</span></span> <span data-ttu-id="3c9aa-163">此时间必须至少为一个晚于开始日期的一天。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-163">This must be at least one day later than the start date.</span></span>  <span data-ttu-id="3c9aa-164">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-164">Required on create.</span></span> |
| `status`                  |`String`                                                        | <span data-ttu-id="3c9aa-165">此只读字段指定 accessReview 的状态。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-165">This read-only field specifies the status of an accessReview.</span></span> <span data-ttu-id="3c9aa-166">典型状态包括`Initializing`、 `NotStarted`、 `Starting``InProgress` `Completing` `Completed` `AutoReviewed`、、、、和。 `AutoReviewing`</span><span class="sxs-lookup"><span data-stu-id="3c9aa-166">The typical states include `Initializing`, `NotStarted`, `Starting`,`InProgress`, `Completing`, `Completed`, `AutoReviewing`, and `AutoReviewed`.</span></span> |
| `description`             |`String`                                                        | <span data-ttu-id="3c9aa-167">由 access 评审创建者提供的说明，用于向审阅者显示。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-167">The description provided by the access review creator, to show to the reviewers.</span></span> |
| `businessFlowTemplateId`  |`String`                                                        | <span data-ttu-id="3c9aa-168">业务流模板标识符。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-168">The business flow template identifier.</span></span> <span data-ttu-id="3c9aa-169">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-169">Required on create.</span></span>  <span data-ttu-id="3c9aa-170">此值区分大小写。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-170">This value is case sensitive.</span></span> |
| `reviewerType`            |`String`                                                        | <span data-ttu-id="3c9aa-171">目标对象的审阅者的关系类型，一个`self` `delegated`或。 `entityOwners`</span><span class="sxs-lookup"><span data-stu-id="3c9aa-171">The relationship type of reviewer to the target object, one of `self`, `delegated` or `entityOwners`.</span></span> <span data-ttu-id="3c9aa-172">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-172">Required on create.</span></span> | 
| `createdBy`               |[<span data-ttu-id="3c9aa-173">userIdentity</span><span class="sxs-lookup"><span data-stu-id="3c9aa-173">userIdentity</span></span>](useridentity.md)                                 | <span data-ttu-id="3c9aa-174">创建此评审的用户。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-174">The user who created this review.</span></span> |
| `reviewedEntity`          |[<span data-ttu-id="3c9aa-175">identity</span><span class="sxs-lookup"><span data-stu-id="3c9aa-175">identity</span></span>](identity.md)                                      | <span data-ttu-id="3c9aa-176">访问权检查其访问权限分配的对象。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-176">The object for which the access reviews is reviewing the access rights assignments.</span></span> <span data-ttu-id="3c9aa-177">此组可以是查看组中用户的成员身份的组，也可以是用于查看对应用程序的用户分配的应用程序。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-177">This can be the group for the review of memberships of users in a group, or the app for a review of assignments of users to an application.</span></span> <span data-ttu-id="3c9aa-178">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-178">Required on create.</span></span> | 
| `settings`                |`microsoft.graph.accessReviewSettings`             | <span data-ttu-id="3c9aa-179">AccessReview 的设置，请参阅下面的类型定义。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-179">The settings of an accessReview, see type definition below.</span></span> |



## <a name="relationships"></a><span data-ttu-id="3c9aa-180">关系</span><span class="sxs-lookup"><span data-stu-id="3c9aa-180">Relationships</span></span>




| <span data-ttu-id="3c9aa-181">关系</span><span class="sxs-lookup"><span data-stu-id="3c9aa-181">Relationship</span></span> | <span data-ttu-id="3c9aa-182">类型</span><span class="sxs-lookup"><span data-stu-id="3c9aa-182">Type</span></span>   |<span data-ttu-id="3c9aa-183">说明</span><span class="sxs-lookup"><span data-stu-id="3c9aa-183">Description</span></span>|
|:---------------|:--------|:----------|
| `reviewers`               |<span data-ttu-id="3c9aa-184">[userIdentity](useridentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="3c9aa-184">[userIdentity](useridentity.md) collection</span></span>                     | <span data-ttu-id="3c9aa-185">访问评审的审阅者的集合（如果 access 评审 reviewerType 的类型`delegate`为）。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-185">The collection of reviewers for an access review, if access review reviewerType is of type `delegate`.</span></span> |
| `decisions`               |<span data-ttu-id="3c9aa-186">[accessReviewDecision](accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="3c9aa-186">[accessReviewDecision](accessreviewdecision.md) collection</span></span> | <span data-ttu-id="3c9aa-187">此访问评审的决策集合。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-187">The collection of decisions for this access review.</span></span> |
| `myDecisions`             |<span data-ttu-id="3c9aa-188">[accessReviewDecision](accessreviewdecision.md)集合</span><span class="sxs-lookup"><span data-stu-id="3c9aa-188">[accessReviewDecision](accessreviewdecision.md) collection</span></span> | <span data-ttu-id="3c9aa-189">如果呼叫者是审阅者，则为呼叫者做出决策的集合。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-189">The collection of decisions for the caller, if the caller is a reviewer.</span></span> |
| `instances`               |<span data-ttu-id="3c9aa-190">[accessReview](accessreview.md)集合</span><span class="sxs-lookup"><span data-stu-id="3c9aa-190">[accessReview](accessreview.md) collection</span></span>         | <span data-ttu-id="3c9aa-191">如果此对象是定期访问审核，则 access 的集合将审阅过去、现在和将来的实例。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-191">The collection of access reviews instances past, present and future, if this object is a recurring access review.</span></span> |

<span data-ttu-id="3c9aa-192">对象中是否存在这些关系，取决于该对象是一次性访问评审、定期访问评审的系列，还是定期访问评审的实例。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-192">Whether these relationships are present on an object, depends upon whether the object is a one-time access review, the series of a recurring access review, or an instance of a recurring access review.</span></span>

| <span data-ttu-id="3c9aa-193">方案</span><span class="sxs-lookup"><span data-stu-id="3c9aa-193">Scenario</span></span> | <span data-ttu-id="3c9aa-194">是否有审阅者？</span><span class="sxs-lookup"><span data-stu-id="3c9aa-194">Has reviewers?</span></span> | <span data-ttu-id="3c9aa-195">是否有决策和 myDecisions？</span><span class="sxs-lookup"><span data-stu-id="3c9aa-195">Has decisions and myDecisions?</span></span> | <span data-ttu-id="3c9aa-196">有实例吗？</span><span class="sxs-lookup"><span data-stu-id="3c9aa-196">Has instances?</span></span> |
|:---------|:---------------|:---------------|:---------------|
|<span data-ttu-id="3c9aa-197">一次性访问审核</span><span class="sxs-lookup"><span data-stu-id="3c9aa-197">One-time access review</span></span>|<span data-ttu-id="3c9aa-198">是</span><span class="sxs-lookup"><span data-stu-id="3c9aa-198">Yes</span></span> | <span data-ttu-id="3c9aa-199">是，启动后</span><span class="sxs-lookup"><span data-stu-id="3c9aa-199">Yes, once started</span></span> | <span data-ttu-id="3c9aa-200">否</span><span class="sxs-lookup"><span data-stu-id="3c9aa-200">No</span></span> |
| <span data-ttu-id="3c9aa-201">定期访问审核</span><span class="sxs-lookup"><span data-stu-id="3c9aa-201">Recurring access review</span></span> | <span data-ttu-id="3c9aa-202">是</span><span class="sxs-lookup"><span data-stu-id="3c9aa-202">Yes</span></span> | <span data-ttu-id="3c9aa-203">否</span><span class="sxs-lookup"><span data-stu-id="3c9aa-203">No</span></span> | <span data-ttu-id="3c9aa-204">是</span><span class="sxs-lookup"><span data-stu-id="3c9aa-204">Yes</span></span> |
| <span data-ttu-id="3c9aa-205">定期访问审核实例</span><span class="sxs-lookup"><span data-stu-id="3c9aa-205">Instance of a recurring access review</span></span> | <span data-ttu-id="3c9aa-206">是</span><span class="sxs-lookup"><span data-stu-id="3c9aa-206">Yes</span></span> | <span data-ttu-id="3c9aa-207">是，启动后</span><span class="sxs-lookup"><span data-stu-id="3c9aa-207">Yes, once started</span></span> | <span data-ttu-id="3c9aa-208">否</span><span class="sxs-lookup"><span data-stu-id="3c9aa-208">No</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3c9aa-209">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3c9aa-209">JSON representation</span></span>

<span data-ttu-id="3c9aa-210">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-210">Here is a JSON representation of the resource.</span></span>

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

## <a name="the-accessreviewsettings-type"></a><span data-ttu-id="3c9aa-211">AccessReviewSettings 类型</span><span class="sxs-lookup"><span data-stu-id="3c9aa-211">The accessReviewSettings type</span></span>

<span data-ttu-id="3c9aa-212">在`accessReviewSettings`创建访问评审时提供其他设置，以在启动访问评审时控制功能行为。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-212">The `accessReviewSettings` provides additional settings when creating an access review, to control the feature behavior when starting an access review.</span></span>  <span data-ttu-id="3c9aa-213">此类型具有以下属性：</span><span class="sxs-lookup"><span data-stu-id="3c9aa-213">This type has the following properties:</span></span> 

| <span data-ttu-id="3c9aa-214">属性</span><span class="sxs-lookup"><span data-stu-id="3c9aa-214">Property</span></span>                     | <span data-ttu-id="3c9aa-215">类型</span><span class="sxs-lookup"><span data-stu-id="3c9aa-215">Type</span></span>                      | <span data-ttu-id="3c9aa-216">说明</span><span class="sxs-lookup"><span data-stu-id="3c9aa-216">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| `mailNotificationsEnabled`|`Boolean`                | <span data-ttu-id="3c9aa-217">指示是否已启用向审阅者发送邮件和审阅创建者的标志。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-217">Flag to indicate whether sending mails to reviewers and the review creator is enabled.</span></span>                |
| `remindersEnabled`|`Boolean`       | <span data-ttu-id="3c9aa-218">指示是否启用了向审阅者发送提醒电子邮件的标志。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-218">Flag to indicate whether sending reminder emails to reviewers are enabled.</span></span>       |
| `justificationRequiredOnApproval`|`Boolean` | <span data-ttu-id="3c9aa-219">指示审阅 access 时是否需要审阅者提供理由的标志。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-219">Flag to indicate whether reviewers are required to provide a justification when reviewing access.</span></span>|
| `activityDurationInDays`|`Int64` | <span data-ttu-id="3c9aa-220">向审阅者显示的用户活动的天数。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-220">The number of days of user activities to show to reviewers.</span></span> |
| `autoReviewEnabled`|`Boolean` | <span data-ttu-id="3c9aa-221">用于指示功能是否应在审阅者未提供且与自动应用一起使用时设置决策的标志。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-221">Flag to indicate whether the feature should set a decision if the reviewer did not supply one, for use with auto-apply, is enabled.</span></span> |
| `autoReviewSettings`|`microsoft.graph.autoReviewSettings` | <span data-ttu-id="3c9aa-222">有关功能应如何设置审阅决定（用于自动应用）的详细设置，请参阅下文所述。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-222">Detailed settings for how the feature should set the review decision, for use with auto-apply, described below.</span></span> |
| `recurrenceSettings`|`microsoft.graph.accessReviewRecurrenceSettings` | <span data-ttu-id="3c9aa-223">定期的详细设置，如下所述。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-223">Detailed settings for recurrence, described below.</span></span> |
| `autoApplyReviewResultsEnabled`|`Boolean` | <span data-ttu-id="3c9aa-224">用于指示是否启用自动更改目标对象访问资源的自动应用功能的标志。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-224">Flag to indicate whether auto-apply capability, to automatically change the target object access resource, is enabled.</span></span>  <span data-ttu-id="3c9aa-225">如果未启用，则用户必须在评审完成后应用访问评审。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-225">If not enabled, a user must, after the review completes, apply the access review.</span></span> |
| `accessRecommendationsEnabled`|`Boolean` | <span data-ttu-id="3c9aa-226">指示是否已启用向审阅者显示建议的标志。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-226">Flag to indicate whether showing recommendations to reviewers is enabled.</span></span> |

## <a name="the-autoreviewsettings-type"></a><span data-ttu-id="3c9aa-227">AutoReviewSettings 类型</span><span class="sxs-lookup"><span data-stu-id="3c9aa-227">The autoReviewSettings type</span></span>

<span data-ttu-id="3c9aa-228">`autoReviewSettings`嵌入访问审阅设置中，并指定访问评审完成时的功能行为。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-228">The `autoReviewSettings` is embedded within the access review settings, and specifies the behavior for the feature when an access review completes.</span></span>  <span data-ttu-id="3c9aa-229">类型具有一个属性`notReviewedResult`。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-229">The type has one property, `notReviewedResult`.</span></span>

| <span data-ttu-id="3c9aa-230">属性</span><span class="sxs-lookup"><span data-stu-id="3c9aa-230">Property</span></span>                     | <span data-ttu-id="3c9aa-231">类型</span><span class="sxs-lookup"><span data-stu-id="3c9aa-231">Type</span></span>     | <span data-ttu-id="3c9aa-232">说明</span><span class="sxs-lookup"><span data-stu-id="3c9aa-232">Description</span></span>                          |
| :--------------------------- | :------  | :----------                          |
| `notReviewedResult`          |`String`  | <span data-ttu-id="3c9aa-233">必须为 `Approve`、`Deny` 或 `Recommendation` 的其中一个。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-233">Must be one of `Approve`, `Deny`, or `Recommendation`.</span></span> |


## <a name="the-accessreviewrecurrencesettings-type"></a><span data-ttu-id="3c9aa-234">AccessReviewRecurrenceSettings 类型</span><span class="sxs-lookup"><span data-stu-id="3c9aa-234">The accessReviewRecurrenceSettings type</span></span>

<span data-ttu-id="3c9aa-235">嵌入`accessReviewRecurrenceSettings`到 access 评审设置中，并指定以固定间隔重复进行访问评审。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-235">The `accessReviewRecurrenceSettings` is embedded within the access review settings, and specifies that the access review recurs at regular intervals.</span></span>  <span data-ttu-id="3c9aa-236">此类型具有以下属性：</span><span class="sxs-lookup"><span data-stu-id="3c9aa-236">This type has the following properties:</span></span>

| <span data-ttu-id="3c9aa-237">属性</span><span class="sxs-lookup"><span data-stu-id="3c9aa-237">Property</span></span>                     | <span data-ttu-id="3c9aa-238">类型</span><span class="sxs-lookup"><span data-stu-id="3c9aa-238">Type</span></span>                                                                                                          | <span data-ttu-id="3c9aa-239">说明</span><span class="sxs-lookup"><span data-stu-id="3c9aa-239">Description</span></span> |
| :--------------------------- | :------------------------------------------------------------------------------------------------------------ | :---------- |
| `recurrenceType`|`String`    | <span data-ttu-id="3c9aa-240">定期`onetime`间隔，必须为、 `weekly`、 `monthly` `quarterly`、或`annual`的其中一个。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-240">The recurrence interval, which must be one of `onetime`, `weekly`, `monthly`, `quarterly`, or `annual`.</span></span>                                                                   |
| `recurrenceEndType`|`String` | <span data-ttu-id="3c9aa-241">重复周期的结束方式。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-241">How the recurrence ends.</span></span> <span data-ttu-id="3c9aa-242">如果是`never`，则不会出现定期系列的显式结束。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-242">If it is `never`, then there is no explicit end of the recurrence series.</span></span> <span data-ttu-id="3c9aa-243">如果是`endBy`，则重复周期将在特定日期结束。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-243">If it is `endBy`, then the recurrence ends at a certain date.</span></span> <span data-ttu-id="3c9aa-244">如果是`occurrences`，则在审阅的实例完成`recurrenceCount`后，该系列将结束。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-244">If it is `occurrences`, then the series ends after `recurrenceCount` instances of the review have completed.</span></span> |
| `durationInDays`|`Int32`     | <span data-ttu-id="3c9aa-245">定期的持续时间（以天为单位）。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-245">The duration in days for recurrence.</span></span>                                                                              |
| `recurrenceCount`|`Int32`    | <span data-ttu-id="3c9aa-246">如果值`recurrenceEndType`为，则为`occurrences`定期计数，否则为0。</span><span class="sxs-lookup"><span data-stu-id="3c9aa-246">The count of recurrences, if the value of `recurrenceEndType` is `occurrences`, or 0 otherwise.</span></span>                                                        |


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
