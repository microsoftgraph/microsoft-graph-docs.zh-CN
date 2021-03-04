---
title: accessReviewScheduleDefinition 资源类型
description: 表示访问评审或访问评审系列。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e4820cf85d3160c04372df79072b4b40708ef868
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443174"
---
# <a name="accessreviewscheduledefinition-resource-type"></a><span data-ttu-id="91630-103">accessReviewScheduleDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="91630-103">accessReviewScheduleDefinition resource type</span></span>

<span data-ttu-id="91630-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91630-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="91630-105">表示 Azure AD 访问评审 [的计划](accessreviewsv2-root.md)。</span><span class="sxs-lookup"><span data-stu-id="91630-105">Represents the scheduling of an Azure AD [access review](accessreviewsv2-root.md).</span></span> 

<span data-ttu-id="91630-106">accessReviewScheduleDefinition 包含 [accessReviewInstance](accessreviewinstance.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="91630-106">An accessReviewScheduleDefinition contains a list of [accessReviewInstance](accessreviewinstance.md) objects.</span></span> <span data-ttu-id="91630-107">计划定义的每次重复都会创建一个实例。</span><span class="sxs-lookup"><span data-stu-id="91630-107">Each recurrence of the schedule definition will create an instance.</span></span> <span data-ttu-id="91630-108">实例还表示要审阅的每个唯一组。</span><span class="sxs-lookup"><span data-stu-id="91630-108">Instances also represent each unique group being reviewed.</span></span> <span data-ttu-id="91630-109">如果计划定义检查多个组，则每个组将具有每个重复周期的唯一实例。</span><span class="sxs-lookup"><span data-stu-id="91630-109">If a schedule definition reviews multiple groups, each group will have a unique instance per each recurrence.</span></span> <span data-ttu-id="91630-110">对于一次检查，每个组将仅创建一个实例。</span><span class="sxs-lookup"><span data-stu-id="91630-110">In the case of a one-time review, only one instance will be created per group.</span></span>

## <a name="methods"></a><span data-ttu-id="91630-111">Methods</span><span class="sxs-lookup"><span data-stu-id="91630-111">Methods</span></span>

| <span data-ttu-id="91630-112">方法</span><span class="sxs-lookup"><span data-stu-id="91630-112">Method</span></span>           | <span data-ttu-id="91630-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="91630-113">Return Type</span></span>    |<span data-ttu-id="91630-114">说明</span><span class="sxs-lookup"><span data-stu-id="91630-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="91630-115">列出 accessReviewScheduleDefinitions</span><span class="sxs-lookup"><span data-stu-id="91630-115">List accessReviewScheduleDefinitions</span></span>](../api/accessreviewscheduledefinition-list.md) | <span data-ttu-id="91630-116">[accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="91630-116">[accessReviewScheduleDefinition](accessreviewscheduledefinition.md) collection</span></span> | <span data-ttu-id="91630-117">列出每个 accessReviewScheduleDefinition。</span><span class="sxs-lookup"><span data-stu-id="91630-117">Lists every accessReviewScheduleDefinition.</span></span> <span data-ttu-id="91630-118">在列表中不包括关联的 accessReviewInstance 实例。</span><span class="sxs-lookup"><span data-stu-id="91630-118">Does not include associated accessReviewInstance instances in listings.</span></span> |
|[<span data-ttu-id="91630-119">获取 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="91630-119">Get accessReviewScheduleDefinition</span></span>](../api/accessreviewscheduledefinition-get.md) | [<span data-ttu-id="91630-120">accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="91630-120">accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition.md) | <span data-ttu-id="91630-121">获取具有指定 ID 的 accessReviewScheduleDefinition。</span><span class="sxs-lookup"><span data-stu-id="91630-121">Get an accessReviewScheduleDefinition with a specified id.</span></span> |
|[<span data-ttu-id="91630-122">创建 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="91630-122">Create accessReviewScheduleDefinition</span></span>](../api/accessreviewscheduledefinition-create.md) | [<span data-ttu-id="91630-123">accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="91630-123">accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition.md) | <span data-ttu-id="91630-124">创建新的 accessReviewScheduleDefinition。</span><span class="sxs-lookup"><span data-stu-id="91630-124">Create a new accessReviewScheduleDefinition.</span></span> |
|[<span data-ttu-id="91630-125">删除 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="91630-125">Delete accessReviewScheduleDefinition</span></span>](../api/accessreviewscheduledefinition-delete.md) | <span data-ttu-id="91630-126">无。</span><span class="sxs-lookup"><span data-stu-id="91630-126">None.</span></span> | <span data-ttu-id="91630-127">删除具有指定标识符的 accessReviewScheduleDefinition。</span><span class="sxs-lookup"><span data-stu-id="91630-127">Delete an accessReviewScheduleDefinition with a specified identifier.</span></span> |
|[<span data-ttu-id="91630-128">更新 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="91630-128">Update accessReviewScheduleDefinition</span></span>](../api/accessreviewscheduledefinition-update.md) | <span data-ttu-id="91630-129">无。</span><span class="sxs-lookup"><span data-stu-id="91630-129">None.</span></span> | <span data-ttu-id="91630-130">使用指定的标识符更新 accessReviewScheduleDefinition 的属性。</span><span class="sxs-lookup"><span data-stu-id="91630-130">Update properties of an accessReviewScheduleDefinition with a specified identifier.</span></span> |

## <a name="properties"></a><span data-ttu-id="91630-131">属性</span><span class="sxs-lookup"><span data-stu-id="91630-131">Properties</span></span>
| <span data-ttu-id="91630-132">属性</span><span class="sxs-lookup"><span data-stu-id="91630-132">Property</span></span> | <span data-ttu-id="91630-133">类型</span><span class="sxs-lookup"><span data-stu-id="91630-133">Type</span></span> | <span data-ttu-id="91630-134">说明</span><span class="sxs-lookup"><span data-stu-id="91630-134">Description</span></span> |
| :------------------| :-------------- | :---------- |
| <span data-ttu-id="91630-135">id</span><span class="sxs-lookup"><span data-stu-id="91630-135">id</span></span> | <span data-ttu-id="91630-136">String</span><span class="sxs-lookup"><span data-stu-id="91630-136">String</span></span> | <span data-ttu-id="91630-137">访问评审的功能分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="91630-137">The feature-assigned unique identifier of an access review.</span></span>|
| <span data-ttu-id="91630-138">displayName</span><span class="sxs-lookup"><span data-stu-id="91630-138">displayName</span></span> | <span data-ttu-id="91630-139">String</span><span class="sxs-lookup"><span data-stu-id="91630-139">String</span></span>   | <span data-ttu-id="91630-140">访问评审系列的名称。</span><span class="sxs-lookup"><span data-stu-id="91630-140">Name of access review series.</span></span> <span data-ttu-id="91630-141">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="91630-141">Required on create.</span></span> |
| <span data-ttu-id="91630-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="91630-142">createdDateTime</span></span>  |<span data-ttu-id="91630-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91630-143">DateTimeOffset</span></span>  | <span data-ttu-id="91630-144">创建审阅系列的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="91630-144">DateTime when review series was created.</span></span> |
| <span data-ttu-id="91630-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="91630-145">lastModifiedDateTime</span></span> | <span data-ttu-id="91630-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91630-146">DateTimeOffset</span></span>   | <span data-ttu-id="91630-147">上次修改审阅系列的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="91630-147">DateTime when review series was last modified.</span></span>|
| <span data-ttu-id="91630-148">状态</span><span class="sxs-lookup"><span data-stu-id="91630-148">status</span></span>  |<span data-ttu-id="91630-149">string</span><span class="sxs-lookup"><span data-stu-id="91630-149">string</span></span>   | <span data-ttu-id="91630-150">此只读字段指定 accessReview 的状态。</span><span class="sxs-lookup"><span data-stu-id="91630-150">This read-only field specifies the status of an accessReview.</span></span> <span data-ttu-id="91630-151">典型状态包括 `Initializing` 、 `NotStarted` `Starting` 、 、 、 `InProgress` `Completing` 和 `Completed` `AutoReviewing` `AutoReviewed` 。</span><span class="sxs-lookup"><span data-stu-id="91630-151">The typical states include `Initializing`, `NotStarted`, `Starting`, `InProgress`, `Completing`, `Completed`, `AutoReviewing`, and `AutoReviewed`.</span></span> |
| <span data-ttu-id="91630-152">descriptionForAdmins</span><span class="sxs-lookup"><span data-stu-id="91630-152">descriptionForAdmins</span></span>  |<span data-ttu-id="91630-153">string</span><span class="sxs-lookup"><span data-stu-id="91630-153">string</span></span>  |  <span data-ttu-id="91630-154">评价创建者提供的用于向管理员提供更多评价上下文的说明。</span><span class="sxs-lookup"><span data-stu-id="91630-154">Description provided by review creators to provide more context of the review to admins.</span></span> |
| <span data-ttu-id="91630-155">descriptionForReviewers</span><span class="sxs-lookup"><span data-stu-id="91630-155">descriptionForReviewers</span></span> |<span data-ttu-id="91630-156">string</span><span class="sxs-lookup"><span data-stu-id="91630-156">string</span></span> | <span data-ttu-id="91630-157">审阅创建者提供的用于向审阅者提供更多审阅上下文的说明。</span><span class="sxs-lookup"><span data-stu-id="91630-157">Description provided  by review creators to provide more context of the review to reviewers.</span></span> <span data-ttu-id="91630-158">审阅者将在发送给其请求审阅的电子邮件中看到此说明。</span><span class="sxs-lookup"><span data-stu-id="91630-158">Reviewers will see this description in the email sent to them requesting their review.</span></span> |
| <span data-ttu-id="91630-159">createdBy</span><span class="sxs-lookup"><span data-stu-id="91630-159">createdBy</span></span>  |[<span data-ttu-id="91630-160">userIdentity</span><span class="sxs-lookup"><span data-stu-id="91630-160">userIdentity</span></span>](../resources/useridentity.md)  | <span data-ttu-id="91630-161">创建此评价的用户。</span><span class="sxs-lookup"><span data-stu-id="91630-161">User who created this review.</span></span> |
| <span data-ttu-id="91630-162">范围</span><span class="sxs-lookup"><span data-stu-id="91630-162">scope</span></span>  |[<span data-ttu-id="91630-163">accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="91630-163">accessReviewScope</span></span>](../resources/accessreviewscope.md)  | <span data-ttu-id="91630-164">定义已审阅用户的范围。</span><span class="sxs-lookup"><span data-stu-id="91630-164">Defines scope of users reviewed.</span></span> <span data-ttu-id="91630-165">有关支持的范围，请参阅 [accessReviewScope](accessreviewscope.md)。</span><span class="sxs-lookup"><span data-stu-id="91630-165">For supported scopes, see [accessReviewScope](accessreviewscope.md).</span></span> <span data-ttu-id="91630-166">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="91630-166">Required on create.</span></span> |
| <span data-ttu-id="91630-167">instanceEnumerationScope</span><span class="sxs-lookup"><span data-stu-id="91630-167">instanceEnumerationScope</span></span>|[<span data-ttu-id="91630-168">accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="91630-168">accessReviewScope</span></span>](../resources/accessreviewscope.md)  | <span data-ttu-id="91630-169">如果审阅所有 Microsoft 365 组的来宾用户，这将确定将审阅哪些组的范围。</span><span class="sxs-lookup"><span data-stu-id="91630-169">In the case of a review of guest users across all Microsoft 365 groups, this determines the scope of which groups will be reviewed.</span></span> <span data-ttu-id="91630-170">每个组将成为访问评审系列的唯一 accessReviewInstance。</span><span class="sxs-lookup"><span data-stu-id="91630-170">Each group will become a unique accessReviewInstance of the access review series.</span></span>  <span data-ttu-id="91630-171">有关支持的范围，请参阅 [accessReviewScope](accessreviewscope.md)。</span><span class="sxs-lookup"><span data-stu-id="91630-171">For supported scopes, see [accessReviewScope](accessreviewscope.md).</span></span> | 
| <span data-ttu-id="91630-172">settings</span><span class="sxs-lookup"><span data-stu-id="91630-172">settings</span></span>  |[<span data-ttu-id="91630-173">accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="91630-173">accessReviewScheduleSettings</span></span>](../resources/accessreviewschedulesettings.md)| <span data-ttu-id="91630-174">访问评审系列的设置，请参阅下面的类型定义。</span><span class="sxs-lookup"><span data-stu-id="91630-174">The settings for an access review series, see type definition below.</span></span> |
| <span data-ttu-id="91630-175">审阅者</span><span class="sxs-lookup"><span data-stu-id="91630-175">reviewers</span></span>   |<span data-ttu-id="91630-176">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="91630-176">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>| <span data-ttu-id="91630-177">此访问评审范围集合用于定义审阅者。</span><span class="sxs-lookup"><span data-stu-id="91630-177">This collection of access review scopes is used to define who are the reviewers.</span></span> <span data-ttu-id="91630-178">请参阅 [accessReviewReviewerScope](accessreviewreviewerscope.md)。</span><span class="sxs-lookup"><span data-stu-id="91630-178">See [accessReviewReviewerScope](accessreviewreviewerscope.md).</span></span> <span data-ttu-id="91630-179">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="91630-179">Required on create.</span></span> |
| <span data-ttu-id="91630-180">backupReviewers</span><span class="sxs-lookup"><span data-stu-id="91630-180">backupReviewers</span></span>   |<span data-ttu-id="91630-181">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="91630-181">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>| <span data-ttu-id="91630-182">此审阅者作用域集合用于定义回退审阅者列表。</span><span class="sxs-lookup"><span data-stu-id="91630-182">This collection of reviewer scopes is used to define the list of fallback reviewers.</span></span> <span data-ttu-id="91630-183">如果从指定的审阅者列表中找不到用户，将通知这些回退审阅者采取措施。</span><span class="sxs-lookup"><span data-stu-id="91630-183">These fallback reviewers will be notified to take action if no users are found from the list of reviewers specified.</span></span> <span data-ttu-id="91630-184">如果组所有者被指定为审阅者，但组所有者不存在，或者经理被指定为审阅者，但用户的经理不存在，则可能发生此情况。</span><span class="sxs-lookup"><span data-stu-id="91630-184">This could occur when either the group owner is specified as the reviewer but the group owner does not exist, or manager is specified as reviewer but a user's manager does not exist.</span></span> <span data-ttu-id="91630-185">请参阅 [accessReviewReviewerScope](accessreviewreviewerscope.md)。</span><span class="sxs-lookup"><span data-stu-id="91630-185">See [accessReviewReviewerScope](accessreviewreviewerscope.md).</span></span> |
| <span data-ttu-id="91630-186">instances</span><span class="sxs-lookup"><span data-stu-id="91630-186">instances</span></span> |<span data-ttu-id="91630-187">集合 (microsoft.graph.accessReviewInstance) </span><span class="sxs-lookup"><span data-stu-id="91630-187">Collection(microsoft.graph.accessReviewInstance)</span></span>|  <span data-ttu-id="91630-188">此访问评审系列的访问评审实例集。</span><span class="sxs-lookup"><span data-stu-id="91630-188">Set of access reviews instances for this access review series.</span></span> <span data-ttu-id="91630-189">不重复的访问评审将只有一个实例;否则，将存在每个重复周期的实例。</span><span class="sxs-lookup"><span data-stu-id="91630-189">Access reviews that do not recur will only have one instance; otherwise, there will be an instance for each recurrence.</span></span> |

## <a name="relationships"></a><span data-ttu-id="91630-190">关系</span><span class="sxs-lookup"><span data-stu-id="91630-190">Relationships</span></span>

| <span data-ttu-id="91630-191">关系</span><span class="sxs-lookup"><span data-stu-id="91630-191">Relationship</span></span> | <span data-ttu-id="91630-192">类型</span><span class="sxs-lookup"><span data-stu-id="91630-192">Type</span></span>   |<span data-ttu-id="91630-193">说明</span><span class="sxs-lookup"><span data-stu-id="91630-193">Description</span></span>|
|:---------------|:--------|:----------|
| `instances`               |<span data-ttu-id="91630-194">[accessReviewInstance](accessreviewinstance.md) 集合</span><span class="sxs-lookup"><span data-stu-id="91630-194">[accessReviewInstance](accessreviewinstance.md) collection</span></span>         | <span data-ttu-id="91630-195">如果是 `accessReviewScheduleDefinition` 定期访问评审，则实例表示每个重复周期。</span><span class="sxs-lookup"><span data-stu-id="91630-195">If the `accessReviewScheduleDefinition` is a recurring access review, instances represent each recurrence.</span></span> <span data-ttu-id="91630-196">不重复的审阅将只具有一个实例。</span><span class="sxs-lookup"><span data-stu-id="91630-196">A review that does not recur will have exactly one instance.</span></span> <span data-ttu-id="91630-197">实例还表示正在审阅的每个唯一资源 `accessReviewScheduleDefinition` 。</span><span class="sxs-lookup"><span data-stu-id="91630-197">Instances also represent each unique resource under review in the `accessReviewScheduleDefinition`.</span></span> <span data-ttu-id="91630-198">如果审阅具有多个资源和多个实例，则每个资源将具有每个重复周期的唯一实例。</span><span class="sxs-lookup"><span data-stu-id="91630-198">If a review has multiple resources and multiple instances, each resource will have a unique instance for each recurrence.</span></span> |

### <a name="supported-queries-for-accessreviewscheduledefinition"></a><span data-ttu-id="91630-199">accessReviewScheduleDefinition 支持的查询</span><span class="sxs-lookup"><span data-stu-id="91630-199">Supported queries for accessReviewScheduleDefinition</span></span>
<span data-ttu-id="91630-200">以下是基于[accessReviewScope](accessreviewscope.md)的[accessReviewScheduleDefinition](accessreviewscheduledefinition.md)上支持的查询。</span><span class="sxs-lookup"><span data-stu-id="91630-200">The following are queries supported on an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) based on the [accessReviewScope](accessreviewscope.md).</span></span>

|<span data-ttu-id="91630-201">应用场景</span><span class="sxs-lookup"><span data-stu-id="91630-201">Scenario</span></span>| <span data-ttu-id="91630-202">查询</span><span class="sxs-lookup"><span data-stu-id="91630-202">Query</span></span> |
|--|--|
| <span data-ttu-id="91630-203">列出每个组 (排除作用域为具有来宾用户的所有 `accessReviewScheduleDefinition` Microsoft 365 组) </span><span class="sxs-lookup"><span data-stu-id="91630-203">List every `accessReviewScheduleDefinition` on individual groups (excludes definitions scoped to all Microsoft 365 groups with guest users)</span></span> | <span data-ttu-id="91630-204">/beta/identityGovernance/accessReviews/definitions？$filter=contains (scope/query， '/groups') </span><span class="sxs-lookup"><span data-stu-id="91630-204">/beta/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')</span></span> |
| <span data-ttu-id="91630-205">列出特定组上的每个 (不包括作用域为具有来宾用户的所有 `accessReviewScheduleDefinition` Microsoft 365 组) </span><span class="sxs-lookup"><span data-stu-id="91630-205">List every `accessReviewScheduleDefinition` on a specific group (excludes definitions scoped to all Microsoft 365 groups with guest users)</span></span> | <span data-ttu-id="91630-206">/beta/identityGovernance/accessReviews/definitions？$filter=contains (scope/query， '/groups/{group id}') </span><span class="sxs-lookup"><span data-stu-id="91630-206">/beta/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups/{group id}')</span></span> |
| <span data-ttu-id="91630-207">列出 `accessReviewScheduleDefinition` 每个作用域为具有来宾用户的 Microsoft 365 组</span><span class="sxs-lookup"><span data-stu-id="91630-207">List every `accessReviewScheduleDefinition` scoped to all Microsoft 365 groups with guest users</span></span> | <span data-ttu-id="91630-208">/beta/identityGovernance/accessReviews/definitions？$filter=contains (scope/query， './members') </span><span class="sxs-lookup"><span data-stu-id="91630-208">/beta/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, './members')</span></span> |

## <a name="json-representation"></a><span data-ttu-id="91630-209">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="91630-209">JSON representation</span></span>
<span data-ttu-id="91630-210">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91630-210">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewScheduleDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "status": "String",
  "descriptionForAdmins": "String",
  "descriptionForReviewers": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "scope": {
    "@odata.type": "microsoft.graph.accessReviewScope"
  },
  "reviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewerScope"
    }
  ],
  "instanceEnumerationScope": {
    "@odata.type": "microsoft.graph.accessReviewScope"
  },
  "settings": {
    "@odata.type": "microsoft.graph.accessReviewScheduleSettings"
  }
}
```
<!--
{
  "type": "#page.annotation",
  "description": "accessReviewScheduleDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
