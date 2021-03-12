---
title: plannerTask 资源类型
description: '**plannerTask** 资源表示 Microsoft 365 中的规划器任务。规划器任务包含在计划内，可以分配给计划中的存储桶。每个任务对象具有可以包含此任务的更多信息的 details 对象。请参阅概述了解有关组、计划和任务之间的关系的详细信息。'
localization_priority: Priority
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 0504168a280c75d15276fbb1fa097c84cafcc1ce
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720604"
---
# <a name="plannertask-resource-type"></a><span data-ttu-id="1042a-106">plannerTask 资源类型</span><span class="sxs-lookup"><span data-stu-id="1042a-106">plannerTask resource type</span></span>

<span data-ttu-id="1042a-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1042a-107">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1042a-p102">**plannerTask** 资源表示 Microsoft 365 中的规划器任务。规划器任务包含在 [计划](plannerplan.md)内，可以分配给计划中的 [存储桶](plannerbucket.md)。每个任务对象具有可以包含此任务的更多信息的 [details](plannertaskdetails.md) 对象。请参阅 [概述](planner-overview.md)了解有关组、计划和任务之间的关系的详细信息。</span><span class="sxs-lookup"><span data-stu-id="1042a-p102">The **plannerTask** resource represents a Planner task in Microsoft 365. A Planner task is contained in a [plan](plannerplan.md) and can be assigned to a [bucket](plannerbucket.md) in a plan. Each task object has a [details](plannertaskdetails.md) object which can contain more information about the task. See [overview](planner-overview.md) for more information regarding relationships between group, plan and task.</span></span>


## <a name="methods"></a><span data-ttu-id="1042a-112">方法</span><span class="sxs-lookup"><span data-stu-id="1042a-112">Methods</span></span>

| <span data-ttu-id="1042a-113">方法</span><span class="sxs-lookup"><span data-stu-id="1042a-113">Method</span></span>           | <span data-ttu-id="1042a-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="1042a-114">Return Type</span></span>    |<span data-ttu-id="1042a-115">说明</span><span class="sxs-lookup"><span data-stu-id="1042a-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1042a-116">获取 plannerTask</span><span class="sxs-lookup"><span data-stu-id="1042a-116">Get plannerTask</span></span>](../api/plannertask-get.md) | [<span data-ttu-id="1042a-117">plannerTask</span><span class="sxs-lookup"><span data-stu-id="1042a-117">plannerTask</span></span>](plannertask.md) |<span data-ttu-id="1042a-118">读取 **plannerTask** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1042a-118">Read properties and relationships of **plannerTask** object.</span></span>|
|[<span data-ttu-id="1042a-119">更新</span><span class="sxs-lookup"><span data-stu-id="1042a-119">Update</span></span>](../api/plannertask-update.md) | [<span data-ttu-id="1042a-120">plannerTask</span><span class="sxs-lookup"><span data-stu-id="1042a-120">plannerTask</span></span>](plannertask.md) |<span data-ttu-id="1042a-121">更新 **plannerTask** 对象。</span><span class="sxs-lookup"><span data-stu-id="1042a-121">Update **plannerTask** object.</span></span> |
|[<span data-ttu-id="1042a-122">删除</span><span class="sxs-lookup"><span data-stu-id="1042a-122">Delete</span></span>](../api/plannertask-delete.md) | <span data-ttu-id="1042a-123">无</span><span class="sxs-lookup"><span data-stu-id="1042a-123">None</span></span> |<span data-ttu-id="1042a-124">删除 **plannerTask** 对象。</span><span class="sxs-lookup"><span data-stu-id="1042a-124">Delete **plannerTask** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1042a-125">属性</span><span class="sxs-lookup"><span data-stu-id="1042a-125">Properties</span></span>
| <span data-ttu-id="1042a-126">属性</span><span class="sxs-lookup"><span data-stu-id="1042a-126">Property</span></span>     | <span data-ttu-id="1042a-127">类型</span><span class="sxs-lookup"><span data-stu-id="1042a-127">Type</span></span>   |<span data-ttu-id="1042a-128">说明</span><span class="sxs-lookup"><span data-stu-id="1042a-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1042a-129">activeChecklistItemCount</span><span class="sxs-lookup"><span data-stu-id="1042a-129">activeChecklistItemCount</span></span>|<span data-ttu-id="1042a-130">Int32</span><span class="sxs-lookup"><span data-stu-id="1042a-130">Int32</span></span>|<span data-ttu-id="1042a-131">核对清单项的数量，其值设置为 `false`，表示项目不全。</span><span class="sxs-lookup"><span data-stu-id="1042a-131">Number of checklist items with value set to `false`, representing incomplete items.</span></span>|
|<span data-ttu-id="1042a-132">appliedCategories</span><span class="sxs-lookup"><span data-stu-id="1042a-132">appliedCategories</span></span>|[<span data-ttu-id="1042a-133">plannerAppliedCategories</span><span class="sxs-lookup"><span data-stu-id="1042a-133">plannerAppliedCategories</span></span>](plannerappliedcategories.md)|<span data-ttu-id="1042a-p103">此任务已应用的类别。有关可能的值，请参阅[已应用的类别](plannerappliedcategories.md)。</span><span class="sxs-lookup"><span data-stu-id="1042a-p103">The categories to which the task has been applied. See [applied Categories](plannerappliedcategories.md) for possible values.</span></span>|
|<span data-ttu-id="1042a-136">assigneePriority</span><span class="sxs-lookup"><span data-stu-id="1042a-136">assigneePriority</span></span>|<span data-ttu-id="1042a-137">String</span><span class="sxs-lookup"><span data-stu-id="1042a-137">String</span></span>|<span data-ttu-id="1042a-p104">用于为列表视图中的此类型项目排序的提示。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="1042a-p104">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="1042a-140">assignments</span><span class="sxs-lookup"><span data-stu-id="1042a-140">assignments</span></span>|[<span data-ttu-id="1042a-141">plannerAssignments</span><span class="sxs-lookup"><span data-stu-id="1042a-141">plannerAssignments</span></span>](plannerassignments.md)|<span data-ttu-id="1042a-142">被分配任务的接受者集合。</span><span class="sxs-lookup"><span data-stu-id="1042a-142">The set of assignees the task is assigned to.</span></span>|
|<span data-ttu-id="1042a-143">bucketId</span><span class="sxs-lookup"><span data-stu-id="1042a-143">bucketId</span></span>|<span data-ttu-id="1042a-144">String</span><span class="sxs-lookup"><span data-stu-id="1042a-144">String</span></span>|<span data-ttu-id="1042a-145">此任务所属的存储桶 ID。</span><span class="sxs-lookup"><span data-stu-id="1042a-145">Bucket ID to which the task belongs.</span></span> <span data-ttu-id="1042a-146">存储桶需要位于任务所在的计划中。</span><span class="sxs-lookup"><span data-stu-id="1042a-146">The bucket needs to be in the plan that the task is in.</span></span> <span data-ttu-id="1042a-147">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="1042a-147">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="1042a-148">[格式验证](planner-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="1042a-148">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span> |
|<span data-ttu-id="1042a-149">checklistItemCount</span><span class="sxs-lookup"><span data-stu-id="1042a-149">checklistItemCount</span></span>|<span data-ttu-id="1042a-150">Int32</span><span class="sxs-lookup"><span data-stu-id="1042a-150">Int32</span></span>|<span data-ttu-id="1042a-151">任务上存在的核对清单项的数目。</span><span class="sxs-lookup"><span data-stu-id="1042a-151">Number of checklist items that are present on the task.</span></span>|
|<span data-ttu-id="1042a-152">completedBy</span><span class="sxs-lookup"><span data-stu-id="1042a-152">completedBy</span></span>|[<span data-ttu-id="1042a-153">identitySet</span><span class="sxs-lookup"><span data-stu-id="1042a-153">identitySet</span></span>](identityset.md)|<span data-ttu-id="1042a-154">完成任务的用户的身份。</span><span class="sxs-lookup"><span data-stu-id="1042a-154">Identity of the user that completed the task.</span></span>|
|<span data-ttu-id="1042a-155">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="1042a-155">completedDateTime</span></span>|<span data-ttu-id="1042a-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1042a-156">DateTimeOffset</span></span>|<span data-ttu-id="1042a-157">只读。</span><span class="sxs-lookup"><span data-stu-id="1042a-157">Read-only.</span></span> <span data-ttu-id="1042a-158">任务的 `'percentComplete'` 被设置为 `'100'` 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1042a-158">Date and time at which the `'percentComplete'` of the task is set to `'100'`.</span></span> <span data-ttu-id="1042a-159">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="1042a-159">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1042a-160">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="1042a-160">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="1042a-161">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="1042a-161">conversationThreadId</span></span>|<span data-ttu-id="1042a-162">字符串</span><span class="sxs-lookup"><span data-stu-id="1042a-162">String</span></span>|<span data-ttu-id="1042a-p107">关于任务的对话的线程 ID。此为在组中创建的对话线程对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="1042a-p107">Thread ID of the conversation on the task. This is the ID of the conversation thread object created in the group.</span></span>|
|<span data-ttu-id="1042a-165">createdBy</span><span class="sxs-lookup"><span data-stu-id="1042a-165">createdBy</span></span>|[<span data-ttu-id="1042a-166">identitySet</span><span class="sxs-lookup"><span data-stu-id="1042a-166">identitySet</span></span>](identityset.md)|<span data-ttu-id="1042a-167">创建任务的用户的身份</span><span class="sxs-lookup"><span data-stu-id="1042a-167">Identity of the user that created the task.</span></span>|
|<span data-ttu-id="1042a-168">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1042a-168">createdDateTime</span></span>|<span data-ttu-id="1042a-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1042a-169">DateTimeOffset</span></span>|<span data-ttu-id="1042a-170">只读。</span><span class="sxs-lookup"><span data-stu-id="1042a-170">Read-only.</span></span> <span data-ttu-id="1042a-171">创建任务的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1042a-171">Date and time at which the task is created.</span></span> <span data-ttu-id="1042a-172">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="1042a-172">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1042a-173">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="1042a-173">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="1042a-174">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="1042a-174">dueDateTime</span></span>|<span data-ttu-id="1042a-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1042a-175">DateTimeOffset</span></span>|<span data-ttu-id="1042a-176">任务截止的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1042a-176">Date and time at which the task is due.</span></span> <span data-ttu-id="1042a-177">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="1042a-177">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1042a-178">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="1042a-178">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="1042a-179">hasDescription</span><span class="sxs-lookup"><span data-stu-id="1042a-179">hasDescription</span></span>|<span data-ttu-id="1042a-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="1042a-180">Boolean</span></span>|<span data-ttu-id="1042a-p110">只读。如果任务的 details 对象具有非空的说明，则值为 `true`，否则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="1042a-p110">Read-only. Value is `true` if the details object of the task has a non-empty description and `false` otherwise.</span></span>|
|<span data-ttu-id="1042a-183">id</span><span class="sxs-lookup"><span data-stu-id="1042a-183">id</span></span>|<span data-ttu-id="1042a-184">字符串</span><span class="sxs-lookup"><span data-stu-id="1042a-184">String</span></span>|<span data-ttu-id="1042a-185">只读。</span><span class="sxs-lookup"><span data-stu-id="1042a-185">Read-only.</span></span> <span data-ttu-id="1042a-186">任务的 ID。</span><span class="sxs-lookup"><span data-stu-id="1042a-186">ID of the task.</span></span> <span data-ttu-id="1042a-187">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="1042a-187">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="1042a-188">[格式验证](planner-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="1042a-188">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="1042a-189">orderHint</span><span class="sxs-lookup"><span data-stu-id="1042a-189">orderHint</span></span>|<span data-ttu-id="1042a-190">String</span><span class="sxs-lookup"><span data-stu-id="1042a-190">String</span></span>|<span data-ttu-id="1042a-p112">用于为列表视图中的此类型项目排序的提示。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="1042a-p112">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="1042a-193">percentComplete</span><span class="sxs-lookup"><span data-stu-id="1042a-193">percentComplete</span></span>|<span data-ttu-id="1042a-194">Int32</span><span class="sxs-lookup"><span data-stu-id="1042a-194">Int32</span></span>|<span data-ttu-id="1042a-p113">任务完成的百分比。当设置为 `100` 时，任务被视为完成。</span><span class="sxs-lookup"><span data-stu-id="1042a-p113">Percentage of task completion. When set to `100`, the task is considered completed.</span></span> |
|<span data-ttu-id="1042a-197">planId</span><span class="sxs-lookup"><span data-stu-id="1042a-197">planId</span></span>|<span data-ttu-id="1042a-198">String</span><span class="sxs-lookup"><span data-stu-id="1042a-198">String</span></span>|<span data-ttu-id="1042a-199">任务所属的计划 ID。</span><span class="sxs-lookup"><span data-stu-id="1042a-199">Plan ID to which the task belongs.</span></span>|
|<span data-ttu-id="1042a-200">previewType</span><span class="sxs-lookup"><span data-stu-id="1042a-200">previewType</span></span>|<span data-ttu-id="1042a-201">String</span><span class="sxs-lookup"><span data-stu-id="1042a-201">String</span></span>|<span data-ttu-id="1042a-202">这将设置显示在任务上的预览类型。</span><span class="sxs-lookup"><span data-stu-id="1042a-202">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="1042a-203">可能的值包括 `automatic`、`noPreview`、`checklist`、`description`、`reference`。</span><span class="sxs-lookup"><span data-stu-id="1042a-203">The possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span>|
|<span data-ttu-id="1042a-204">referenceCount</span><span class="sxs-lookup"><span data-stu-id="1042a-204">referenceCount</span></span>|<span data-ttu-id="1042a-205">Int32</span><span class="sxs-lookup"><span data-stu-id="1042a-205">Int32</span></span>|<span data-ttu-id="1042a-206">任务上存在的外部引用的数量。</span><span class="sxs-lookup"><span data-stu-id="1042a-206">Number of external references that exist on the task.</span></span>|
|<span data-ttu-id="1042a-207">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1042a-207">startDateTime</span></span>|<span data-ttu-id="1042a-208">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1042a-208">DateTimeOffset</span></span>|<span data-ttu-id="1042a-209">任务开始的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1042a-209">Date and time at which the task starts.</span></span> <span data-ttu-id="1042a-210">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="1042a-210">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1042a-211">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="1042a-211">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="1042a-212">title</span><span class="sxs-lookup"><span data-stu-id="1042a-212">title</span></span>|<span data-ttu-id="1042a-213">String</span><span class="sxs-lookup"><span data-stu-id="1042a-213">String</span></span>|<span data-ttu-id="1042a-214">任务的标题。</span><span class="sxs-lookup"><span data-stu-id="1042a-214">Title of the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1042a-215">关系</span><span class="sxs-lookup"><span data-stu-id="1042a-215">Relationships</span></span>
| <span data-ttu-id="1042a-216">关系</span><span class="sxs-lookup"><span data-stu-id="1042a-216">Relationship</span></span> | <span data-ttu-id="1042a-217">类型</span><span class="sxs-lookup"><span data-stu-id="1042a-217">Type</span></span>   |<span data-ttu-id="1042a-218">说明</span><span class="sxs-lookup"><span data-stu-id="1042a-218">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1042a-219">assignedToTaskBoardFormat</span><span class="sxs-lookup"><span data-stu-id="1042a-219">assignedToTaskBoardFormat</span></span>|[<span data-ttu-id="1042a-220">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="1042a-220">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)| <span data-ttu-id="1042a-p116">只读。可为 NULL。用于在按 assignedTo 分组时在任务板视图中正确呈现任务。</span><span class="sxs-lookup"><span data-stu-id="1042a-p116">Read-only. Nullable. Used to render the task correctly in the task board view when grouped by assignedTo.</span></span>|
|<span data-ttu-id="1042a-224">bucketTaskBoardFormat</span><span class="sxs-lookup"><span data-stu-id="1042a-224">bucketTaskBoardFormat</span></span>|[<span data-ttu-id="1042a-225">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="1042a-225">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)| <span data-ttu-id="1042a-p117">只读。可为 NULL。用于在按存储桶分组时在任务板视图中正确呈现任务。</span><span class="sxs-lookup"><span data-stu-id="1042a-p117">Read-only. Nullable. Used to render the task correctly in the task board view when grouped by bucket.</span></span>|
|<span data-ttu-id="1042a-229">详细信息</span><span class="sxs-lookup"><span data-stu-id="1042a-229">details</span></span>|[<span data-ttu-id="1042a-230">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="1042a-230">plannerTaskDetails</span></span>](plannertaskdetails.md)| <span data-ttu-id="1042a-p118">只读。可为 NULL。关于任务的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="1042a-p118">Read-only. Nullable. Additional details about the task.</span></span>|
|<span data-ttu-id="1042a-234">progressTaskBoardFormat</span><span class="sxs-lookup"><span data-stu-id="1042a-234">progressTaskBoardFormat</span></span>|[<span data-ttu-id="1042a-235">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="1042a-235">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)| <span data-ttu-id="1042a-p119">只读。可为 NULL。用于在按进度分组时在任务板视图中正确呈现任务。</span><span class="sxs-lookup"><span data-stu-id="1042a-p119">Read-only. Nullable. Used to render the task correctly in the task board view when grouped by progress.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1042a-239">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1042a-239">JSON representation</span></span>
<span data-ttu-id="1042a-240">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1042a-240">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerTask"
}-->

```json
{
  "activeChecklistItemCount": 1024,
  "appliedCategories": {"@odata.type": "microsoft.graph.plannerAppliedCategories"},
  "assigneePriority": "String",
  "assignments": {"@odata.type": "microsoft.graph.plannerAssignments"},
  "bucketId": "String",
  "checklistItemCount": 1024,
  "completedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "completedDateTime": "String (timestamp)",
  "conversationThreadId": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "dueDateTime": "String (timestamp)",
  "hasDescription": true,
  "id": "String (identifier)",
  "orderHint": "String",
  "percentComplete": 1024,
  "planId": "String",
  "previewType": "String",
  "referenceCount": 1024,
  "startDateTime": "String (timestamp)",
  "title": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerTask resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

