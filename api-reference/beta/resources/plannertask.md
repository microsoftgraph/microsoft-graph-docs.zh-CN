---
title: plannerTask 资源类型
description: '**PlannerTask**资源表示 Microsoft 365 中的 Planner 任务。计划中包含规划器任务，可将其分配给计划中的存储桶。每个任务对象都有一个详细信息对象，该对象可包含有关任务的详细信息。有关组、计划和任务之间的关系的详细信息，请参阅概述。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 07374c6e8dc2dfaee1caba9f7283a1404627fb22
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897342"
---
# <a name="plannertask-resource-type"></a><span data-ttu-id="0fd17-106">plannerTask 资源类型</span><span class="sxs-lookup"><span data-stu-id="0fd17-106">plannerTask resource type</span></span>

<span data-ttu-id="0fd17-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fd17-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0fd17-p102">**PlannerTask**资源表示 Microsoft 365 中的 Planner 任务。[计划](plannerplan.md)中包含规划器任务，可将其分配给计划中的[存储桶](plannerbucket.md)。每个任务对象都有一个[详细](plannertaskdetails.md)信息对象，该对象可包含有关任务的详细信息。有关组、计划和任务之间的关系的详细信息，请参阅[概述](planner-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="0fd17-p102">The **plannerTask** resource represents a Planner task in Microsoft 365. A Planner task is contained in a [plan](plannerplan.md) and can be assigned to a [bucket](plannerbucket.md) in a plan. Each task object has a [details](plannertaskdetails.md) object which can contain more information about the task. See [overview](planner-overview.md) for more information regarding relationships between group, plan and task.</span></span>


## <a name="methods"></a><span data-ttu-id="0fd17-112">方法</span><span class="sxs-lookup"><span data-stu-id="0fd17-112">Methods</span></span>

| <span data-ttu-id="0fd17-113">方法</span><span class="sxs-lookup"><span data-stu-id="0fd17-113">Method</span></span>           | <span data-ttu-id="0fd17-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="0fd17-114">Return Type</span></span>    |<span data-ttu-id="0fd17-115">说明</span><span class="sxs-lookup"><span data-stu-id="0fd17-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0fd17-116">获取 plannerTask</span><span class="sxs-lookup"><span data-stu-id="0fd17-116">Get plannerTask</span></span>](../api/plannertask-get.md) | [<span data-ttu-id="0fd17-117">plannerTask</span><span class="sxs-lookup"><span data-stu-id="0fd17-117">plannerTask</span></span>](plannertask.md) |<span data-ttu-id="0fd17-118">读取 **plannerTask** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0fd17-118">Read properties and relationships of **plannerTask** object.</span></span>|
|[<span data-ttu-id="0fd17-119">更新</span><span class="sxs-lookup"><span data-stu-id="0fd17-119">Update</span></span>](../api/plannertask-update.md) | [<span data-ttu-id="0fd17-120">plannerTask</span><span class="sxs-lookup"><span data-stu-id="0fd17-120">plannerTask</span></span>](plannertask.md) |<span data-ttu-id="0fd17-121">更新 **plannerTask** 对象。</span><span class="sxs-lookup"><span data-stu-id="0fd17-121">Update **plannerTask** object.</span></span> |
|[<span data-ttu-id="0fd17-122">删除</span><span class="sxs-lookup"><span data-stu-id="0fd17-122">Delete</span></span>](../api/plannertask-delete.md) | <span data-ttu-id="0fd17-123">无</span><span class="sxs-lookup"><span data-stu-id="0fd17-123">None</span></span> |<span data-ttu-id="0fd17-124">删除 **plannerTask** 对象。</span><span class="sxs-lookup"><span data-stu-id="0fd17-124">Delete **plannerTask** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0fd17-125">属性</span><span class="sxs-lookup"><span data-stu-id="0fd17-125">Properties</span></span>
| <span data-ttu-id="0fd17-126">属性</span><span class="sxs-lookup"><span data-stu-id="0fd17-126">Property</span></span>     | <span data-ttu-id="0fd17-127">类型</span><span class="sxs-lookup"><span data-stu-id="0fd17-127">Type</span></span>   |<span data-ttu-id="0fd17-128">说明</span><span class="sxs-lookup"><span data-stu-id="0fd17-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0fd17-129">activeChecklistItemCount</span><span class="sxs-lookup"><span data-stu-id="0fd17-129">activeChecklistItemCount</span></span>|<span data-ttu-id="0fd17-130">Int32</span><span class="sxs-lookup"><span data-stu-id="0fd17-130">Int32</span></span>|<span data-ttu-id="0fd17-131">核对清单项的数量，其值设置为 `false`，表示项目不全。</span><span class="sxs-lookup"><span data-stu-id="0fd17-131">Number of checklist items with value set to `false`, representing incomplete items.</span></span>|
|<span data-ttu-id="0fd17-132">appliedCategories</span><span class="sxs-lookup"><span data-stu-id="0fd17-132">appliedCategories</span></span>|[<span data-ttu-id="0fd17-133">plannerAppliedCategories</span><span class="sxs-lookup"><span data-stu-id="0fd17-133">plannerAppliedCategories</span></span>](plannerappliedcategories.md)|<span data-ttu-id="0fd17-p103">此任务已应用的类别。有关可能的值，请参阅[已应用的类别](plannerappliedcategories.md)。</span><span class="sxs-lookup"><span data-stu-id="0fd17-p103">The categories to which the task has been applied. See [applied Categories](plannerappliedcategories.md) for possible values.</span></span>|
|<span data-ttu-id="0fd17-136">assigneePriority</span><span class="sxs-lookup"><span data-stu-id="0fd17-136">assigneePriority</span></span>|<span data-ttu-id="0fd17-137">String</span><span class="sxs-lookup"><span data-stu-id="0fd17-137">String</span></span>|<span data-ttu-id="0fd17-p104">用于为列表视图中的此类型项目排序的提示。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="0fd17-p104">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="0fd17-140">assignments</span><span class="sxs-lookup"><span data-stu-id="0fd17-140">assignments</span></span>|[<span data-ttu-id="0fd17-141">plannerAssignments</span><span class="sxs-lookup"><span data-stu-id="0fd17-141">plannerAssignments</span></span>](plannerassignments.md)|<span data-ttu-id="0fd17-142">被分配任务的接受者集合。</span><span class="sxs-lookup"><span data-stu-id="0fd17-142">The set of assignees the task is assigned to.</span></span>|
|<span data-ttu-id="0fd17-143">bucketId</span><span class="sxs-lookup"><span data-stu-id="0fd17-143">bucketId</span></span>|<span data-ttu-id="0fd17-144">String</span><span class="sxs-lookup"><span data-stu-id="0fd17-144">String</span></span>|<span data-ttu-id="0fd17-145">此任务所属的存储桶 ID。</span><span class="sxs-lookup"><span data-stu-id="0fd17-145">Bucket ID to which the task belongs.</span></span> <span data-ttu-id="0fd17-146">存储桶需要位于任务所在的计划中。</span><span class="sxs-lookup"><span data-stu-id="0fd17-146">The bucket needs to be in the plan that the task is in.</span></span> <span data-ttu-id="0fd17-147">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="0fd17-147">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="0fd17-148">[格式验证](tasks-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="0fd17-148">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span> |
|<span data-ttu-id="0fd17-149">checklistItemCount</span><span class="sxs-lookup"><span data-stu-id="0fd17-149">checklistItemCount</span></span>|<span data-ttu-id="0fd17-150">Int32</span><span class="sxs-lookup"><span data-stu-id="0fd17-150">Int32</span></span>|<span data-ttu-id="0fd17-151">任务上存在的核对清单项的数目。</span><span class="sxs-lookup"><span data-stu-id="0fd17-151">Number of checklist items that are present on the task.</span></span>|
|<span data-ttu-id="0fd17-152">completedBy</span><span class="sxs-lookup"><span data-stu-id="0fd17-152">completedBy</span></span>|[<span data-ttu-id="0fd17-153">identitySet</span><span class="sxs-lookup"><span data-stu-id="0fd17-153">identitySet</span></span>](identityset.md)|<span data-ttu-id="0fd17-154">完成任务的用户的身份。</span><span class="sxs-lookup"><span data-stu-id="0fd17-154">Identity of the user that completed the task.</span></span>|
|<span data-ttu-id="0fd17-155">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="0fd17-155">completedDateTime</span></span>|<span data-ttu-id="0fd17-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fd17-156">DateTimeOffset</span></span>|<span data-ttu-id="0fd17-p106">只读。任务的 `'percentComplete'` 被设置为 `'100'` 的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="0fd17-p106">Read-only. Date and time at which the `'percentComplete'` of the task is set to `'100'`. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0fd17-161">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="0fd17-161">conversationThreadId</span></span>|<span data-ttu-id="0fd17-162">字符串</span><span class="sxs-lookup"><span data-stu-id="0fd17-162">String</span></span>|<span data-ttu-id="0fd17-p107">关于任务的对话的线程 ID。此为在组中创建的对话线程对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="0fd17-p107">Thread ID of the conversation on the task. This is the ID of the conversation thread object created in the group.</span></span>|
|<span data-ttu-id="0fd17-165">createdBy</span><span class="sxs-lookup"><span data-stu-id="0fd17-165">createdBy</span></span>|[<span data-ttu-id="0fd17-166">identitySet</span><span class="sxs-lookup"><span data-stu-id="0fd17-166">identitySet</span></span>](identityset.md)|<span data-ttu-id="0fd17-167">创建任务的用户的身份</span><span class="sxs-lookup"><span data-stu-id="0fd17-167">Identity of the user that created the task.</span></span>|
|<span data-ttu-id="0fd17-168">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0fd17-168">createdDateTime</span></span>|<span data-ttu-id="0fd17-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fd17-169">DateTimeOffset</span></span>|<span data-ttu-id="0fd17-p108">只读。创建任务的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="0fd17-p108">Read-only. Date and time at which the task is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0fd17-174">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="0fd17-174">dueDateTime</span></span>|<span data-ttu-id="0fd17-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fd17-175">DateTimeOffset</span></span>|<span data-ttu-id="0fd17-p109">任务截止的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="0fd17-p109">Date and time at which the task is due. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0fd17-179">hasDescription</span><span class="sxs-lookup"><span data-stu-id="0fd17-179">hasDescription</span></span>|<span data-ttu-id="0fd17-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="0fd17-180">Boolean</span></span>|<span data-ttu-id="0fd17-p110">只读。如果任务的 details 对象具有非空的说明，则值为 `true`，否则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="0fd17-p110">Read-only. Value is `true` if the details object of the task has a non-empty description and `false` otherwise.</span></span>|
|<span data-ttu-id="0fd17-183">id</span><span class="sxs-lookup"><span data-stu-id="0fd17-183">id</span></span>|<span data-ttu-id="0fd17-184">String</span><span class="sxs-lookup"><span data-stu-id="0fd17-184">String</span></span>|<span data-ttu-id="0fd17-185">只读。</span><span class="sxs-lookup"><span data-stu-id="0fd17-185">Read-only.</span></span> <span data-ttu-id="0fd17-186">任务的 ID。</span><span class="sxs-lookup"><span data-stu-id="0fd17-186">ID of the task.</span></span> <span data-ttu-id="0fd17-187">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="0fd17-187">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="0fd17-188">[格式验证](tasks-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="0fd17-188">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="0fd17-189">orderHint</span><span class="sxs-lookup"><span data-stu-id="0fd17-189">orderHint</span></span>|<span data-ttu-id="0fd17-190">String</span><span class="sxs-lookup"><span data-stu-id="0fd17-190">String</span></span>|<span data-ttu-id="0fd17-p112">用于为列表视图中的此类型项目排序的提示。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="0fd17-p112">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="0fd17-193">percentComplete</span><span class="sxs-lookup"><span data-stu-id="0fd17-193">percentComplete</span></span>|<span data-ttu-id="0fd17-194">Int32</span><span class="sxs-lookup"><span data-stu-id="0fd17-194">Int32</span></span>|<span data-ttu-id="0fd17-p113">任务完成的百分比。当设置为 `100` 时，任务被视为完成。</span><span class="sxs-lookup"><span data-stu-id="0fd17-p113">Percentage of task completion. When set to `100`, the task is considered completed.</span></span> |
|<span data-ttu-id="0fd17-197">priority</span><span class="sxs-lookup"><span data-stu-id="0fd17-197">priority</span></span>|<span data-ttu-id="0fd17-198">Int32</span><span class="sxs-lookup"><span data-stu-id="0fd17-198">Int32</span></span>|<span data-ttu-id="0fd17-199">任务的优先级。</span><span class="sxs-lookup"><span data-stu-id="0fd17-199">Priority of the task.</span></span> <span data-ttu-id="0fd17-200">值的有效范围介于 `0` 和 `10` （含）之间，并且值越低，优先级越低（ `0` 具有最高优先级， `10` 优先级最低）。</span><span class="sxs-lookup"><span data-stu-id="0fd17-200">Valid range of values is between `0` and `10` (inclusive), with increasing value being lower priority (`0` has the highest priority and `10` has the lowest priority).</span></span>  <span data-ttu-id="0fd17-201">目前，规划者将值 `0` 和 `1` "紧急"， `2` 以及 `3` `4` "重要"、、、、和 " `5` `6` `7` `8` `9` `10` 低" 的值解释为 "中"。</span><span class="sxs-lookup"><span data-stu-id="0fd17-201">Currently, Planner interprets values `0` and `1` as "urgent", `2` and `3` and `4` as "important", `5`, `6`, and `7` as "medium", and `8`, `9`, and `10` as "low".</span></span>  <span data-ttu-id="0fd17-202">目前，规划器将设置 `1` "紧急"、" `3` 重要"、" `5` 中" 和 `9` "低" 的值。</span><span class="sxs-lookup"><span data-stu-id="0fd17-202">Currently, Planner sets the value `1` for "urgent", `3` for "important", `5` for "medium", and `9` for "low".</span></span>|
|<span data-ttu-id="0fd17-203">planId</span><span class="sxs-lookup"><span data-stu-id="0fd17-203">planId</span></span>|<span data-ttu-id="0fd17-204">String</span><span class="sxs-lookup"><span data-stu-id="0fd17-204">String</span></span>|<span data-ttu-id="0fd17-205">任务所属的计划 ID。</span><span class="sxs-lookup"><span data-stu-id="0fd17-205">Plan ID to which the task belongs.</span></span>|
|<span data-ttu-id="0fd17-206">previewType</span><span class="sxs-lookup"><span data-stu-id="0fd17-206">previewType</span></span>|<span data-ttu-id="0fd17-207">String</span><span class="sxs-lookup"><span data-stu-id="0fd17-207">String</span></span>|<span data-ttu-id="0fd17-208">这将设置显示在任务上的预览类型。</span><span class="sxs-lookup"><span data-stu-id="0fd17-208">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="0fd17-209">可取值为：`automatic`、`noPreview`、`checklist`、`description`、`reference`。</span><span class="sxs-lookup"><span data-stu-id="0fd17-209">Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span>|
|<span data-ttu-id="0fd17-210">referenceCount</span><span class="sxs-lookup"><span data-stu-id="0fd17-210">referenceCount</span></span>|<span data-ttu-id="0fd17-211">Int32</span><span class="sxs-lookup"><span data-stu-id="0fd17-211">Int32</span></span>|<span data-ttu-id="0fd17-212">任务上存在的外部引用的数量。</span><span class="sxs-lookup"><span data-stu-id="0fd17-212">Number of external references that exist on the task.</span></span>|
|<span data-ttu-id="0fd17-213">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0fd17-213">startDateTime</span></span>|<span data-ttu-id="0fd17-214">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fd17-214">DateTimeOffset</span></span>|<span data-ttu-id="0fd17-p116">任务开始的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="0fd17-p116">Date and time at which the task starts. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0fd17-218">title</span><span class="sxs-lookup"><span data-stu-id="0fd17-218">title</span></span>|<span data-ttu-id="0fd17-219">String</span><span class="sxs-lookup"><span data-stu-id="0fd17-219">String</span></span>|<span data-ttu-id="0fd17-220">任务的标题。</span><span class="sxs-lookup"><span data-stu-id="0fd17-220">Title of the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0fd17-221">关系</span><span class="sxs-lookup"><span data-stu-id="0fd17-221">Relationships</span></span>
| <span data-ttu-id="0fd17-222">关系</span><span class="sxs-lookup"><span data-stu-id="0fd17-222">Relationship</span></span> | <span data-ttu-id="0fd17-223">类型</span><span class="sxs-lookup"><span data-stu-id="0fd17-223">Type</span></span>   |<span data-ttu-id="0fd17-224">说明</span><span class="sxs-lookup"><span data-stu-id="0fd17-224">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0fd17-225">assignedToTaskBoardFormat</span><span class="sxs-lookup"><span data-stu-id="0fd17-225">assignedToTaskBoardFormat</span></span>|[<span data-ttu-id="0fd17-226">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="0fd17-226">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)| <span data-ttu-id="0fd17-p117">只读。可为 NULL。用于在按 assignedTo 分组时在任务板视图中正确呈现任务。</span><span class="sxs-lookup"><span data-stu-id="0fd17-p117">Read-only. Nullable. Used to render the task correctly in the task board view when grouped by assignedTo.</span></span>|
|<span data-ttu-id="0fd17-230">bucketTaskBoardFormat</span><span class="sxs-lookup"><span data-stu-id="0fd17-230">bucketTaskBoardFormat</span></span>|[<span data-ttu-id="0fd17-231">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="0fd17-231">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)| <span data-ttu-id="0fd17-p118">只读。可为 NULL。用于在按存储桶分组时在任务板视图中正确呈现任务。</span><span class="sxs-lookup"><span data-stu-id="0fd17-p118">Read-only. Nullable. Used to render the task correctly in the task board view when grouped by bucket.</span></span>|
|<span data-ttu-id="0fd17-235">详细信息</span><span class="sxs-lookup"><span data-stu-id="0fd17-235">details</span></span>|[<span data-ttu-id="0fd17-236">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="0fd17-236">plannerTaskDetails</span></span>](plannertaskdetails.md)| <span data-ttu-id="0fd17-p119">只读。可为 NULL。关于任务的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="0fd17-p119">Read-only. Nullable. Additional details about the task.</span></span>|
|<span data-ttu-id="0fd17-240">progressTaskBoardFormat</span><span class="sxs-lookup"><span data-stu-id="0fd17-240">progressTaskBoardFormat</span></span>|[<span data-ttu-id="0fd17-241">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="0fd17-241">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)| <span data-ttu-id="0fd17-p120">只读。可为 NULL。用于在按进度分组时在任务板视图中正确呈现任务。</span><span class="sxs-lookup"><span data-stu-id="0fd17-p120">Read-only. Nullable. Used to render the task correctly in the task board view when grouped by progress.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0fd17-245">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0fd17-245">JSON representation</span></span>
<span data-ttu-id="0fd17-246">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0fd17-246">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
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
  "priority": 1024,
  "planId": "String",
  "previewType": "String",
  "referenceCount": 1024,
  "startDateTime": "String (timestamp)",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerTask resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
