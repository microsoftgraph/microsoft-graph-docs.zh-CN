---
title: accessReviewScheduleDefinition 资源类型
description: 表示访问评审或访问评审系列。
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f95047602ec1a73549b6b5c4217e32890a5996e6
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161157"
---
# <a name="accessreviewscheduledefinition-resource-type"></a><span data-ttu-id="aa072-103">accessReviewScheduleDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="aa072-103">accessReviewScheduleDefinition resource type</span></span>

<span data-ttu-id="aa072-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa072-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa072-105">表示 Azure AD 访问评审 [的计划](accessreviewsv2-root.md)。</span><span class="sxs-lookup"><span data-stu-id="aa072-105">Represents the scheduling of an Azure AD [access review](accessreviewsv2-root.md).</span></span> 

<span data-ttu-id="aa072-106">accessReviewScheduleDefinition 包含 [accessReviewInstance 对象](accessreviewinstance.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="aa072-106">An accessReviewScheduleDefinition contains a list of [accessReviewInstance](accessreviewinstance.md) objects.</span></span> <span data-ttu-id="aa072-107">计划定义的每次重复都会创建一个实例。</span><span class="sxs-lookup"><span data-stu-id="aa072-107">Each recurrence of the schedule definition will create an instance.</span></span> <span data-ttu-id="aa072-108">实例还表示要审阅的每个唯一组。</span><span class="sxs-lookup"><span data-stu-id="aa072-108">Instances also represent each unique group being reviewed.</span></span> <span data-ttu-id="aa072-109">如果计划定义审阅多个组，则每个组将每个重复周期具有一个唯一实例。</span><span class="sxs-lookup"><span data-stu-id="aa072-109">If a schedule definition reviews multiple groups, each group will have a unique instance per each recurrence.</span></span> <span data-ttu-id="aa072-110">对于一次评审，每个组只会创建一个实例。</span><span class="sxs-lookup"><span data-stu-id="aa072-110">In the case of a one-time review, only one instance will be created per group.</span></span>

## <a name="methods"></a><span data-ttu-id="aa072-111">方法</span><span class="sxs-lookup"><span data-stu-id="aa072-111">Methods</span></span>

| <span data-ttu-id="aa072-112">方法</span><span class="sxs-lookup"><span data-stu-id="aa072-112">Method</span></span>           | <span data-ttu-id="aa072-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="aa072-113">Return Type</span></span>    |<span data-ttu-id="aa072-114">说明</span><span class="sxs-lookup"><span data-stu-id="aa072-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aa072-115">列出 accessReviewScheduleDefinitions</span><span class="sxs-lookup"><span data-stu-id="aa072-115">List accessReviewScheduleDefinitions</span></span>](../api/accessreviewscheduledefinition-list.md) | <span data-ttu-id="aa072-116">[accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aa072-116">[accessReviewScheduleDefinition](accessreviewscheduledefinition.md) collection</span></span> | <span data-ttu-id="aa072-117">列出每个 accessReviewScheduleDefinition。</span><span class="sxs-lookup"><span data-stu-id="aa072-117">Lists every accessReviewScheduleDefinition.</span></span> <span data-ttu-id="aa072-118">在列表中不包括关联的 accessReviewInstance 实例。</span><span class="sxs-lookup"><span data-stu-id="aa072-118">Does not include associated accessReviewInstance instances in listings.</span></span> |
|[<span data-ttu-id="aa072-119">获取 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="aa072-119">Get accessReviewScheduleDefinition</span></span>](../api/accessreviewscheduledefinition-get.md) | [<span data-ttu-id="aa072-120">accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="aa072-120">accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition.md) | <span data-ttu-id="aa072-121">获取具有指定 ID 的 accessReviewScheduleDefinition。</span><span class="sxs-lookup"><span data-stu-id="aa072-121">Get an accessReviewScheduleDefinition with a specified id.</span></span> |
|[<span data-ttu-id="aa072-122">创建 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="aa072-122">Create accessReviewScheduleDefinition</span></span>](../api/accessreviewscheduledefinition-create.md) | [<span data-ttu-id="aa072-123">accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="aa072-123">accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition.md) | <span data-ttu-id="aa072-124">创建新的 accessReviewScheduleDefinition。</span><span class="sxs-lookup"><span data-stu-id="aa072-124">Create a new accessReviewScheduleDefinition.</span></span> |
|[<span data-ttu-id="aa072-125">删除 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="aa072-125">Delete accessReviewScheduleDefinition</span></span>](../api/accessreviewscheduledefinition-delete.md) | <span data-ttu-id="aa072-126">无。</span><span class="sxs-lookup"><span data-stu-id="aa072-126">None.</span></span> | <span data-ttu-id="aa072-127">删除具有指定标识符的 accessReviewScheduleDefinition。</span><span class="sxs-lookup"><span data-stu-id="aa072-127">Delete an accessReviewScheduleDefinition with a specified identifier.</span></span> |
|[<span data-ttu-id="aa072-128">更新 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="aa072-128">Update accessReviewScheduleDefinition</span></span>](../api/accessreviewscheduledefinition-update.md) | <span data-ttu-id="aa072-129">无。</span><span class="sxs-lookup"><span data-stu-id="aa072-129">None.</span></span> | <span data-ttu-id="aa072-130">使用指定标识符更新 accessReviewScheduleDefinition 的属性。</span><span class="sxs-lookup"><span data-stu-id="aa072-130">Update properties of an accessReviewScheduleDefinition with a specified identifier.</span></span> |

## <a name="properties"></a><span data-ttu-id="aa072-131">属性</span><span class="sxs-lookup"><span data-stu-id="aa072-131">Properties</span></span>
| <span data-ttu-id="aa072-132">属性</span><span class="sxs-lookup"><span data-stu-id="aa072-132">Property</span></span> | <span data-ttu-id="aa072-133">类型</span><span class="sxs-lookup"><span data-stu-id="aa072-133">Type</span></span> | <span data-ttu-id="aa072-134">说明</span><span class="sxs-lookup"><span data-stu-id="aa072-134">Description</span></span> |
| :------------------| :-------------- | :---------- |
| <span data-ttu-id="aa072-135">id</span><span class="sxs-lookup"><span data-stu-id="aa072-135">id</span></span> | <span data-ttu-id="aa072-136">String</span><span class="sxs-lookup"><span data-stu-id="aa072-136">String</span></span> | <span data-ttu-id="aa072-137">访问评审的功能分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="aa072-137">The feature-assigned unique identifier of an access review.</span></span>|
| <span data-ttu-id="aa072-138">displayName</span><span class="sxs-lookup"><span data-stu-id="aa072-138">displayName</span></span> | <span data-ttu-id="aa072-139">String</span><span class="sxs-lookup"><span data-stu-id="aa072-139">String</span></span>   | <span data-ttu-id="aa072-140">访问评审系列的名称。</span><span class="sxs-lookup"><span data-stu-id="aa072-140">Name of access review series.</span></span> <span data-ttu-id="aa072-141">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="aa072-141">Required on create.</span></span> |
| <span data-ttu-id="aa072-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aa072-142">createdDateTime</span></span>  |<span data-ttu-id="aa072-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa072-143">DateTimeOffset</span></span>  | <span data-ttu-id="aa072-144">创建审阅系列时的日期时间。</span><span class="sxs-lookup"><span data-stu-id="aa072-144">DateTime when review series was created.</span></span> |
| <span data-ttu-id="aa072-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aa072-145">lastModifiedDateTime</span></span> | <span data-ttu-id="aa072-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa072-146">DateTimeOffset</span></span>   | <span data-ttu-id="aa072-147">上次修改审阅系列的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="aa072-147">DateTime when review series was last modified.</span></span>|
| <span data-ttu-id="aa072-148">状态</span><span class="sxs-lookup"><span data-stu-id="aa072-148">status</span></span>  |<span data-ttu-id="aa072-149">string</span><span class="sxs-lookup"><span data-stu-id="aa072-149">string</span></span>   | <span data-ttu-id="aa072-150">此只读字段指定 accessReview 的状态。</span><span class="sxs-lookup"><span data-stu-id="aa072-150">This read-only field specifies the status of an accessReview.</span></span> <span data-ttu-id="aa072-151">典型状态包括 `Initializing` 、 `NotStarted` `Starting` 、 、 、 `InProgress` `Completing` 和 `Completed` `AutoReviewing` `AutoReviewed` 。</span><span class="sxs-lookup"><span data-stu-id="aa072-151">The typical states include `Initializing`, `NotStarted`, `Starting`, `InProgress`, `Completing`, `Completed`, `AutoReviewing`, and `AutoReviewed`.</span></span> |
| <span data-ttu-id="aa072-152">descriptionForAdmins</span><span class="sxs-lookup"><span data-stu-id="aa072-152">descriptionForAdmins</span></span>  |<span data-ttu-id="aa072-153">string</span><span class="sxs-lookup"><span data-stu-id="aa072-153">string</span></span>  |  <span data-ttu-id="aa072-154">评价创建者提供的用于向管理员提供更多评价上下文的说明。</span><span class="sxs-lookup"><span data-stu-id="aa072-154">Description provided by review creators to provide more context of the review to admins.</span></span> |
| <span data-ttu-id="aa072-155">descriptionForReviewers</span><span class="sxs-lookup"><span data-stu-id="aa072-155">descriptionForReviewers</span></span> |<span data-ttu-id="aa072-156">string</span><span class="sxs-lookup"><span data-stu-id="aa072-156">string</span></span> | <span data-ttu-id="aa072-157">审阅创建者提供的用于向审阅者提供更多评论上下文的说明。</span><span class="sxs-lookup"><span data-stu-id="aa072-157">Description provided  by review creators to provide more context of the review to reviewers.</span></span> <span data-ttu-id="aa072-158">审阅者将在发送给他们请求审阅的电子邮件中看到此说明。</span><span class="sxs-lookup"><span data-stu-id="aa072-158">Reviewers will see this description in the email sent to them requesting their review.</span></span> |
| <span data-ttu-id="aa072-159">createdBy</span><span class="sxs-lookup"><span data-stu-id="aa072-159">createdBy</span></span>  |[<span data-ttu-id="aa072-160">userIdentity</span><span class="sxs-lookup"><span data-stu-id="aa072-160">userIdentity</span></span>](../resources/useridentity.md)  | <span data-ttu-id="aa072-161">创建此评论的用户。</span><span class="sxs-lookup"><span data-stu-id="aa072-161">User who created this review.</span></span> |
| <span data-ttu-id="aa072-162">范围</span><span class="sxs-lookup"><span data-stu-id="aa072-162">scope</span></span>  |[<span data-ttu-id="aa072-163">accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="aa072-163">accessReviewScope</span></span>](../resources/accessreviewscope.md)  | <span data-ttu-id="aa072-164">定义在组中审阅的用户范围。</span><span class="sxs-lookup"><span data-stu-id="aa072-164">Defines scope of users reviewed in a group.</span></span> <span data-ttu-id="aa072-165">有关支持的范围，请参阅 [accessReviewScope](accessreviewscope.md)。</span><span class="sxs-lookup"><span data-stu-id="aa072-165">For supported scopes, see [accessReviewScope](accessreviewscope.md).</span></span> <span data-ttu-id="aa072-166">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="aa072-166">Required on create.</span></span> |
| <span data-ttu-id="aa072-167">instanceEnumerationScope</span><span class="sxs-lookup"><span data-stu-id="aa072-167">instanceEnumerationScope</span></span>|[<span data-ttu-id="aa072-168">accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="aa072-168">accessReviewScope</span></span>](../resources/accessreviewscope.md)  | <span data-ttu-id="aa072-169">对于所有组审阅，这将确定将审阅哪些组的范围。</span><span class="sxs-lookup"><span data-stu-id="aa072-169">In the case of an all groups review, this determines the scope of which groups will be reviewed.</span></span> <span data-ttu-id="aa072-170">每个组将成为访问评审系列的唯一 accessReviewInstance。</span><span class="sxs-lookup"><span data-stu-id="aa072-170">Each group will become a unique accessReviewInstance of the access review series.</span></span>  <span data-ttu-id="aa072-171">有关支持的范围，请参阅 [accessReviewScope](accessreviewscope.md)。</span><span class="sxs-lookup"><span data-stu-id="aa072-171">For supported scopes, see [accessReviewScope](accessreviewscope.md).</span></span> | 
| <span data-ttu-id="aa072-172">设置</span><span class="sxs-lookup"><span data-stu-id="aa072-172">settings</span></span>  |[<span data-ttu-id="aa072-173">accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="aa072-173">accessReviewScheduleSettings</span></span>](../resources/accessreviewschedulesettings.md)| <span data-ttu-id="aa072-174">访问评审系列的设置，请参阅下面的类型定义。</span><span class="sxs-lookup"><span data-stu-id="aa072-174">The settings for an access review series, see type definition below.</span></span> |
| <span data-ttu-id="aa072-175">审阅者</span><span class="sxs-lookup"><span data-stu-id="aa072-175">reviewers</span></span>   |<span data-ttu-id="aa072-176">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aa072-176">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>| <span data-ttu-id="aa072-177">此访问评审范围集合用于定义审阅者。</span><span class="sxs-lookup"><span data-stu-id="aa072-177">This collection of access review scopes is used to define who are the reviewers.</span></span> <span data-ttu-id="aa072-178">请参阅 [accessReviewReviewerScope](accessreviewreviewerscope.md)。</span><span class="sxs-lookup"><span data-stu-id="aa072-178">See [accessReviewReviewerScope](accessreviewreviewerscope.md).</span></span> <span data-ttu-id="aa072-179">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="aa072-179">Required on create.</span></span> |
| <span data-ttu-id="aa072-180">backupReviewers</span><span class="sxs-lookup"><span data-stu-id="aa072-180">backupReviewers</span></span>   |<span data-ttu-id="aa072-181">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aa072-181">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>| <span data-ttu-id="aa072-182">此审阅者作用域集合用于定义回退审阅者列表。</span><span class="sxs-lookup"><span data-stu-id="aa072-182">This collection of reviewer scopes is used to define the list of fallback reviewers.</span></span> <span data-ttu-id="aa072-183">如果从指定的审阅者列表中未找到用户，将通知这些回退审阅者采取措施。</span><span class="sxs-lookup"><span data-stu-id="aa072-183">These fallback reviewers will be notified to take action if no users are found from the list of reviewers specified.</span></span> <span data-ttu-id="aa072-184">当组所有者被指定为审阅者，但组所有者不存在，或者经理被指定为审阅者，但用户的经理不存在时，可能会发生这种情况。</span><span class="sxs-lookup"><span data-stu-id="aa072-184">This could occur when either the group owner is specified as the reviewer but the group owner does not exist, or manager is specified as reviewer but a user's manager does not exist.</span></span> <span data-ttu-id="aa072-185">请参阅 [accessReviewReviewerScope](accessreviewreviewerscope.md)。</span><span class="sxs-lookup"><span data-stu-id="aa072-185">See [accessReviewReviewerScope](accessreviewreviewerscope.md).</span></span> |
| <span data-ttu-id="aa072-186">instances</span><span class="sxs-lookup"><span data-stu-id="aa072-186">instances</span></span> |<span data-ttu-id="aa072-187">集合 (microsoft.graph.accessReviewInstance) </span><span class="sxs-lookup"><span data-stu-id="aa072-187">Collection(microsoft.graph.accessReviewInstance)</span></span>|  <span data-ttu-id="aa072-188">此访问评审系列的访问评审实例集。</span><span class="sxs-lookup"><span data-stu-id="aa072-188">Set of access reviews instances for this access review series.</span></span> <span data-ttu-id="aa072-189">不重复的访问评审将只有一个实例;否则，将针对每个重复周期提供一个实例。</span><span class="sxs-lookup"><span data-stu-id="aa072-189">Access reviews that do not recur will only have one instance; otherwise, there will be an instance for each recurrence.</span></span> |

## <a name="relationships"></a><span data-ttu-id="aa072-190">关系</span><span class="sxs-lookup"><span data-stu-id="aa072-190">Relationships</span></span>

| <span data-ttu-id="aa072-191">关系</span><span class="sxs-lookup"><span data-stu-id="aa072-191">Relationship</span></span> | <span data-ttu-id="aa072-192">类型</span><span class="sxs-lookup"><span data-stu-id="aa072-192">Type</span></span>   |<span data-ttu-id="aa072-193">说明</span><span class="sxs-lookup"><span data-stu-id="aa072-193">Description</span></span>|
|:---------------|:--------|:----------|
| `instances`               |<span data-ttu-id="aa072-194">[accessReviewInstance](accessreviewinstance.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aa072-194">[accessReviewInstance](accessreviewinstance.md) collection</span></span>         | <span data-ttu-id="aa072-195">如果 `accessReviewScheduleDefinition` 定期访问评审，实例表示每个定期。</span><span class="sxs-lookup"><span data-stu-id="aa072-195">If the `accessReviewScheduleDefinition` is a recurring access review, instances represent each recurrence.</span></span> <span data-ttu-id="aa072-196">不重复的审阅将只具有一个实例。</span><span class="sxs-lookup"><span data-stu-id="aa072-196">A review that does not recur will have exactly one instance.</span></span> <span data-ttu-id="aa072-197">实例还表示正在审阅的每个唯一组 `accessReviewScheduleDefinition` 。</span><span class="sxs-lookup"><span data-stu-id="aa072-197">Instances also represent each unique group under review in the `accessReviewScheduleDefinition`.</span></span> <span data-ttu-id="aa072-198">如果审阅具有多个组和多个实例，则每个组将具有每个重复周期的唯一实例。</span><span class="sxs-lookup"><span data-stu-id="aa072-198">If a review has multiple groups and multiple instances, each group will have a unique instance for each recurrence.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="aa072-199">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aa072-199">JSON representation</span></span>
<span data-ttu-id="aa072-200">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa072-200">The following is a JSON representation of the resource.</span></span>
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
