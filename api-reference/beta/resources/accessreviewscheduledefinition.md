---
title: accessReviewScheduleDefinition 资源类型
description: 代表访问评审或访问评审系列。
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f8ee04dde7ee19d24be5de58237f08b4fb538e8c
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000830"
---
# <a name="accessreviewscheduledefinition-resource-type"></a><span data-ttu-id="5bfb3-103">accessReviewScheduleDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="5bfb3-103">accessReviewScheduleDefinition resource type</span></span>

<span data-ttu-id="5bfb3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bfb3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bfb3-105">表示 Azure AD [访问评审](accessreviewsv2-root.md)的日程安排。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-105">Represents the scheduling of an Azure AD [access review](accessreviewsv2-root.md).</span></span> 

<span data-ttu-id="5bfb3-106">AccessReviewScheduleDefinition 包含 [accessReviewInstance](accessreviewinstance.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-106">An accessReviewScheduleDefinition contains a list of [accessReviewInstance](accessreviewinstance.md) objects.</span></span> <span data-ttu-id="5bfb3-107">计划定义的每个重复将创建一个实例。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-107">Each recurrence of the schedule definition will create an instance.</span></span> <span data-ttu-id="5bfb3-108">实例还表示要审阅的每个唯一组。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-108">Instances also represent each unique group being reviewed.</span></span> <span data-ttu-id="5bfb3-109">如果计划定义检查多个组，每个组将为每个重复周期提供一个唯一的实例。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-109">If a schedule definition reviews multiple groups, each group will have a unique instance per each recurrence.</span></span> <span data-ttu-id="5bfb3-110">在一次性审核的情况下，每个组只会创建一个实例。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-110">In the case of a one-time review, only one instance will be created per group.</span></span>

## <a name="methods"></a><span data-ttu-id="5bfb3-111">方法</span><span class="sxs-lookup"><span data-stu-id="5bfb3-111">Methods</span></span>

| <span data-ttu-id="5bfb3-112">方法</span><span class="sxs-lookup"><span data-stu-id="5bfb3-112">Method</span></span>           | <span data-ttu-id="5bfb3-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="5bfb3-113">Return Type</span></span>    |<span data-ttu-id="5bfb3-114">说明</span><span class="sxs-lookup"><span data-stu-id="5bfb3-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5bfb3-115">列出 accessReviewScheduleDefinitions</span><span class="sxs-lookup"><span data-stu-id="5bfb3-115">List accessReviewScheduleDefinitions</span></span>](../api/accessreviewscheduledefinition-list.md) | <span data-ttu-id="5bfb3-116">[accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5bfb3-116">[accessReviewScheduleDefinition](accessreviewscheduledefinition.md) collection</span></span> | <span data-ttu-id="5bfb3-117">列出每个 accessReviewScheduleDefinition。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-117">Lists every accessReviewScheduleDefinition.</span></span> <span data-ttu-id="5bfb3-118">不包括列表中关联的 accessReviewInstance 实例。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-118">Does not include associated accessReviewInstance instances in listings.</span></span> |
|[<span data-ttu-id="5bfb3-119">获取 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="5bfb3-119">Get accessReviewScheduleDefinition</span></span>](../api/accessreviewscheduledefinition-get.md) | [<span data-ttu-id="5bfb3-120">accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="5bfb3-120">accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition.md) | <span data-ttu-id="5bfb3-121">获取具有指定 id 的 accessReviewScheduleDefinition。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-121">Get an accessReviewScheduleDefinition with a specified id.</span></span> |
|[<span data-ttu-id="5bfb3-122">创建 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="5bfb3-122">Create accessReviewScheduleDefinition</span></span>](../api/accessreviewscheduledefinition-create.md) | [<span data-ttu-id="5bfb3-123">accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="5bfb3-123">accessReviewScheduleDefinition</span></span>](accessreviewscheduledefinition.md) | <span data-ttu-id="5bfb3-124">创建新的 accessReviewScheduleDefinition。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-124">Create a new accessReviewScheduleDefinition.</span></span> |
|[<span data-ttu-id="5bfb3-125">删除 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="5bfb3-125">Delete accessReviewScheduleDefinition</span></span>](../api/accessreviewscheduledefinition-delete.md) | <span data-ttu-id="5bfb3-126">无。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-126">None.</span></span> | <span data-ttu-id="5bfb3-127">删除具有指定标识符的 accessReviewScheduleDefinition。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-127">Delete an accessReviewScheduleDefinition with a specified identifier.</span></span> |
|[<span data-ttu-id="5bfb3-128">更新 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="5bfb3-128">Update accessReviewScheduleDefinition</span></span>](../api/accessreviewscheduledefinition-update.md) | <span data-ttu-id="5bfb3-129">无。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-129">None.</span></span> | <span data-ttu-id="5bfb3-130">使用指定的标识符更新 accessReviewScheduleDefinition 的属性。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-130">Update properties of an accessReviewScheduleDefinition with a specified identifier.</span></span> |

## <a name="properties"></a><span data-ttu-id="5bfb3-131">属性</span><span class="sxs-lookup"><span data-stu-id="5bfb3-131">Properties</span></span>
| <span data-ttu-id="5bfb3-132">属性</span><span class="sxs-lookup"><span data-stu-id="5bfb3-132">Property</span></span> | <span data-ttu-id="5bfb3-133">类型</span><span class="sxs-lookup"><span data-stu-id="5bfb3-133">Type</span></span> | <span data-ttu-id="5bfb3-134">说明</span><span class="sxs-lookup"><span data-stu-id="5bfb3-134">Description</span></span> |
| :------------------| :-------------- | :---------- |
| <span data-ttu-id="5bfb3-135">id</span><span class="sxs-lookup"><span data-stu-id="5bfb3-135">id</span></span> | <span data-ttu-id="5bfb3-136">字符串</span><span class="sxs-lookup"><span data-stu-id="5bfb3-136">String</span></span> | <span data-ttu-id="5bfb3-137">用于访问评审的功能分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-137">The feature-assigned unique identifier of an access review.</span></span>|
| <span data-ttu-id="5bfb3-138">displayName</span><span class="sxs-lookup"><span data-stu-id="5bfb3-138">displayName</span></span> | <span data-ttu-id="5bfb3-139">字符串</span><span class="sxs-lookup"><span data-stu-id="5bfb3-139">String</span></span>   | <span data-ttu-id="5bfb3-140">访问审阅系列的名称。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-140">Name of access review series.</span></span> <span data-ttu-id="5bfb3-141">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-141">Required on create.</span></span> |
| <span data-ttu-id="5bfb3-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5bfb3-142">createdDateTime</span></span>  |<span data-ttu-id="5bfb3-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bfb3-143">DateTimeOffset</span></span>  | <span data-ttu-id="5bfb3-144">创建审阅系列时的日期时间。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-144">DateTime when review series was created.</span></span> |
| <span data-ttu-id="5bfb3-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5bfb3-145">lastModifiedDateTime</span></span> | <span data-ttu-id="5bfb3-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bfb3-146">DateTimeOffset</span></span>   | <span data-ttu-id="5bfb3-147">上次修改审阅系列的日期时间。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-147">DateTime when review series was last modified.</span></span>|
| <span data-ttu-id="5bfb3-148">状态</span><span class="sxs-lookup"><span data-stu-id="5bfb3-148">status</span></span>  |<span data-ttu-id="5bfb3-149">string</span><span class="sxs-lookup"><span data-stu-id="5bfb3-149">string</span></span>   | <span data-ttu-id="5bfb3-150">此只读字段指定 accessReview 的状态。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-150">This read-only field specifies the status of an accessReview.</span></span> <span data-ttu-id="5bfb3-151">典型状态包括、、、、、、 `Initializing` `NotStarted` `Starting` `InProgress` `Completing` `Completed` `AutoReviewing` 和 `AutoReviewed` 。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-151">The typical states include `Initializing`, `NotStarted`, `Starting`, `InProgress`, `Completing`, `Completed`, `AutoReviewing`, and `AutoReviewed`.</span></span> |
| <span data-ttu-id="5bfb3-152">descriptionForAdmins</span><span class="sxs-lookup"><span data-stu-id="5bfb3-152">descriptionForAdmins</span></span>  |<span data-ttu-id="5bfb3-153">string</span><span class="sxs-lookup"><span data-stu-id="5bfb3-153">string</span></span>  |  <span data-ttu-id="5bfb3-154">由审阅创建者提供的说明，用于向管理员提供评审的更多上下文。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-154">Description provided by review creators to provide more context of the review to admins.</span></span> |
| <span data-ttu-id="5bfb3-155">descriptionForReviewers</span><span class="sxs-lookup"><span data-stu-id="5bfb3-155">descriptionForReviewers</span></span> |<span data-ttu-id="5bfb3-156">string</span><span class="sxs-lookup"><span data-stu-id="5bfb3-156">string</span></span> | <span data-ttu-id="5bfb3-157">由审阅创建者提供的说明，用于向审阅者提供评审的更多上下文。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-157">Description provided  by review creators to provide more context of the review to reviewers.</span></span> <span data-ttu-id="5bfb3-158">审阅者将在发送给他们的电子邮件中看到此说明，以请求他们进行审阅。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-158">Reviewers will see this description in the email sent to them requesting their review.</span></span> |
| <span data-ttu-id="5bfb3-159">createdBy</span><span class="sxs-lookup"><span data-stu-id="5bfb3-159">createdBy</span></span>  |[<span data-ttu-id="5bfb3-160">userIdentity</span><span class="sxs-lookup"><span data-stu-id="5bfb3-160">userIdentity</span></span>](../resources/useridentity.md)  | <span data-ttu-id="5bfb3-161">创建此评审的用户。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-161">User who created this review.</span></span> |
| <span data-ttu-id="5bfb3-162">范围</span><span class="sxs-lookup"><span data-stu-id="5bfb3-162">scope</span></span>  |[<span data-ttu-id="5bfb3-163">accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="5bfb3-163">accessReviewScope</span></span>](../resources/accessreviewscope.md)  | <span data-ttu-id="5bfb3-164">定义在组中审阅的用户的范围。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-164">Defines scope of users reviewed in a group.</span></span> <span data-ttu-id="5bfb3-165">有关支持的作用域，请参阅 [accessReviewScope](accessreviewscope.md)。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-165">For supported scopes, see [accessReviewScope](accessreviewscope.md).</span></span> <span data-ttu-id="5bfb3-166">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-166">Required on create.</span></span> |
| <span data-ttu-id="5bfb3-167">instanceEnumerationScope</span><span class="sxs-lookup"><span data-stu-id="5bfb3-167">instanceEnumerationScope</span></span>|[<span data-ttu-id="5bfb3-168">accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="5bfb3-168">accessReviewScope</span></span>](../resources/accessreviewscope.md)  | <span data-ttu-id="5bfb3-169">在所有组评审的情况下，这将确定将检查哪些组的范围。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-169">In the case of an all groups review, this determines the scope of which groups will be reviewed.</span></span> <span data-ttu-id="5bfb3-170">每个组将成为 access 审阅系列的唯一 accessReviewInstance。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-170">Each group will become a unique accessReviewInstance of the access review series.</span></span>  <span data-ttu-id="5bfb3-171">有关支持的作用域，请参阅 [accessReviewScope](accessreviewscope.md)。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-171">For supported scopes, see [accessReviewScope](accessreviewscope.md).</span></span> | 
| <span data-ttu-id="5bfb3-172">settings</span><span class="sxs-lookup"><span data-stu-id="5bfb3-172">settings</span></span>  |[<span data-ttu-id="5bfb3-173">accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="5bfb3-173">accessReviewScheduleSettings</span></span>](../resources/accessreviewschedulesettings.md)| <span data-ttu-id="5bfb3-174">Access 审阅系列的设置，请参阅下面的类型定义。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-174">The settings for an access review series, see type definition below.</span></span> |
| <span data-ttu-id="5bfb3-175">审批</span><span class="sxs-lookup"><span data-stu-id="5bfb3-175">reviewers</span></span>   |<span data-ttu-id="5bfb3-176">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5bfb3-176">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>| <span data-ttu-id="5bfb3-177">此访问审核作用域集用于定义谁是审阅者。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-177">This collection of access review scopes is used to define who are the reviewers.</span></span> <span data-ttu-id="5bfb3-178">请参阅 [accessReviewReviewerScope](accessreviewreviewerscope.md)。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-178">See [accessReviewReviewerScope](accessreviewreviewerscope.md).</span></span> <span data-ttu-id="5bfb3-179">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-179">Required on create.</span></span> |
| <span data-ttu-id="5bfb3-180">backupReviewers</span><span class="sxs-lookup"><span data-stu-id="5bfb3-180">backupReviewers</span></span>   |<span data-ttu-id="5bfb3-181">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5bfb3-181">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>| <span data-ttu-id="5bfb3-182">这一组审阅者范围用于定义回退审阅者的列表。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-182">This collection of reviewer scopes is used to define the list of fallback reviewers.</span></span> <span data-ttu-id="5bfb3-183">如果在指定的审阅者列表中找不到用户，将会通知这些回退审阅者采取行动。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-183">These fallback reviewers will be notified to take action if no users are found from the list of reviewers specified.</span></span> <span data-ttu-id="5bfb3-184">如果将组所有者指定为审阅者，但组所有者不存在，或将经理指定为审阅者但用户的经理不存在，则可能会出现此情况。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-184">This could occur when either the group owner is specified as the reviewer but the group owner does not exist, or manager is specified as reviewer but a user's manager does not exist.</span></span> <span data-ttu-id="5bfb3-185">请参阅 [accessReviewReviewerScope](accessreviewreviewerscope.md)。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-185">See [accessReviewReviewerScope](accessreviewreviewerscope.md).</span></span> |
| <span data-ttu-id="5bfb3-186">实例</span><span class="sxs-lookup"><span data-stu-id="5bfb3-186">instances</span></span> |<span data-ttu-id="5bfb3-187">AccessReviewInstance) 的集合 (</span><span class="sxs-lookup"><span data-stu-id="5bfb3-187">Collection(microsoft.graph.accessReviewInstance)</span></span>|  <span data-ttu-id="5bfb3-188">此访问评审系列的一组访问审核实例。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-188">Set of access reviews instances for this access review series.</span></span> <span data-ttu-id="5bfb3-189">不重复的 Access 审阅将只有一个实例;否则，每个定期都将有一个实例。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-189">Access reviews that do not recur will only have one instance; otherwise, there will be an instance for each recurrence.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5bfb3-190">关系</span><span class="sxs-lookup"><span data-stu-id="5bfb3-190">Relationships</span></span>

| <span data-ttu-id="5bfb3-191">关系</span><span class="sxs-lookup"><span data-stu-id="5bfb3-191">Relationship</span></span> | <span data-ttu-id="5bfb3-192">类型</span><span class="sxs-lookup"><span data-stu-id="5bfb3-192">Type</span></span>   |<span data-ttu-id="5bfb3-193">说明</span><span class="sxs-lookup"><span data-stu-id="5bfb3-193">Description</span></span>|
|:---------------|:--------|:----------|
| `instances`               |<span data-ttu-id="5bfb3-194">[accessReviewInstance](accessreviewinstance.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5bfb3-194">[accessReviewInstance](accessreviewinstance.md) collection</span></span>         | <span data-ttu-id="5bfb3-195">如果 `accessReviewScheduleDefinition` 是定期访问审核，则实例表示每个重复周期。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-195">If the `accessReviewScheduleDefinition` is a recurring access review, instances represent each recurrence.</span></span> <span data-ttu-id="5bfb3-196">不重复的审阅将只有一个实例。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-196">A review that does not recur will have exactly one instance.</span></span> <span data-ttu-id="5bfb3-197">实例还表示中的 "查看" 下的每个唯一组 `accessReviewScheduleDefinition` 。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-197">Instances also represent each unique group under review in the `accessReviewScheduleDefinition`.</span></span> <span data-ttu-id="5bfb3-198">如果评审包含多个组和多个实例，则每个组都将具有每个重复的唯一实例。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-198">If a review has multiple groups and multiple instances, each group will have a unique instance for each recurrence.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5bfb3-199">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5bfb3-199">JSON representation</span></span>
<span data-ttu-id="5bfb3-200">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5bfb3-200">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition",
  "baseType": "",
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
