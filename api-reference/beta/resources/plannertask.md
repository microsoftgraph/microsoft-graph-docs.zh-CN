---
title: plannerTask 资源类型
description: '**plannerTask** 资源表示 Microsoft 365 中的规划器任务。规划器任务包含在计划内，可以分配给计划中的存储桶。每个任务对象具有可以包含此任务的更多信息的 details 对象。请参阅概述了解有关组、计划和任务之间的关系的详细信息。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: dd3e96e035c0097830e7ce797da0fa91ea28aac5
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883200"
---
# <a name="plannertask-resource-type"></a><span data-ttu-id="806a8-106">plannerTask 资源类型</span><span class="sxs-lookup"><span data-stu-id="806a8-106">plannerTask resource type</span></span>

<span data-ttu-id="806a8-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="806a8-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="806a8-p102">**plannerTask** 资源表示 Microsoft 365 中的规划器任务。规划器任务包含在 [计划](plannerplan.md)内，可以分配给计划中的 [存储桶](plannerbucket.md)。每个任务对象具有可以包含此任务的更多信息的 [details](plannertaskdetails.md) 对象。请参阅 [概述](planner-overview.md)了解有关组、计划和任务之间的关系的详细信息。</span><span class="sxs-lookup"><span data-stu-id="806a8-p102">The **plannerTask** resource represents a Planner task in Microsoft 365. A Planner task is contained in a [plan](plannerplan.md) and can be assigned to a [bucket](plannerbucket.md) in a plan. Each task object has a [details](plannertaskdetails.md) object which can contain more information about the task. See [overview](planner-overview.md) for more information regarding relationships between group, plan and task.</span></span>


## <a name="methods"></a><span data-ttu-id="806a8-112">方法</span><span class="sxs-lookup"><span data-stu-id="806a8-112">Methods</span></span>

| <span data-ttu-id="806a8-113">方法</span><span class="sxs-lookup"><span data-stu-id="806a8-113">Method</span></span>           | <span data-ttu-id="806a8-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="806a8-114">Return Type</span></span>    |<span data-ttu-id="806a8-115">说明</span><span class="sxs-lookup"><span data-stu-id="806a8-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="806a8-116">获取 plannerTask</span><span class="sxs-lookup"><span data-stu-id="806a8-116">Get plannerTask</span></span>](../api/plannertask-get.md) | [<span data-ttu-id="806a8-117">plannerTask</span><span class="sxs-lookup"><span data-stu-id="806a8-117">plannerTask</span></span>](plannertask.md) |<span data-ttu-id="806a8-118">读取 **plannerTask** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="806a8-118">Read properties and relationships of **plannerTask** object.</span></span>|
|[<span data-ttu-id="806a8-119">更新</span><span class="sxs-lookup"><span data-stu-id="806a8-119">Update</span></span>](../api/plannertask-update.md) | [<span data-ttu-id="806a8-120">plannerTask</span><span class="sxs-lookup"><span data-stu-id="806a8-120">plannerTask</span></span>](plannertask.md) |<span data-ttu-id="806a8-121">更新 **plannerTask** 对象。</span><span class="sxs-lookup"><span data-stu-id="806a8-121">Update **plannerTask** object.</span></span> |
|[<span data-ttu-id="806a8-122">删除</span><span class="sxs-lookup"><span data-stu-id="806a8-122">Delete</span></span>](../api/plannertask-delete.md) | <span data-ttu-id="806a8-123">无</span><span class="sxs-lookup"><span data-stu-id="806a8-123">None</span></span> |<span data-ttu-id="806a8-124">删除 **plannerTask** 对象。</span><span class="sxs-lookup"><span data-stu-id="806a8-124">Delete **plannerTask** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="806a8-125">属性</span><span class="sxs-lookup"><span data-stu-id="806a8-125">Properties</span></span>
| <span data-ttu-id="806a8-126">属性</span><span class="sxs-lookup"><span data-stu-id="806a8-126">Property</span></span>     | <span data-ttu-id="806a8-127">类型</span><span class="sxs-lookup"><span data-stu-id="806a8-127">Type</span></span>   |<span data-ttu-id="806a8-128">说明</span><span class="sxs-lookup"><span data-stu-id="806a8-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="806a8-129">activeChecklistItemCount</span><span class="sxs-lookup"><span data-stu-id="806a8-129">activeChecklistItemCount</span></span>|<span data-ttu-id="806a8-130">Int32</span><span class="sxs-lookup"><span data-stu-id="806a8-130">Int32</span></span>|<span data-ttu-id="806a8-131">核对清单项的数量，其值设置为 `false`，表示项目不全。</span><span class="sxs-lookup"><span data-stu-id="806a8-131">Number of checklist items with value set to `false`, representing incomplete items.</span></span>|
|<span data-ttu-id="806a8-132">appliedCategories</span><span class="sxs-lookup"><span data-stu-id="806a8-132">appliedCategories</span></span>|[<span data-ttu-id="806a8-133">plannerAppliedCategories</span><span class="sxs-lookup"><span data-stu-id="806a8-133">plannerAppliedCategories</span></span>](plannerappliedcategories.md)|<span data-ttu-id="806a8-p103">此任务已应用的类别。有关可能的值，请参阅[已应用的类别](plannerappliedcategories.md)。</span><span class="sxs-lookup"><span data-stu-id="806a8-p103">The categories to which the task has been applied. See [applied Categories](plannerappliedcategories.md) for possible values.</span></span>|
|<span data-ttu-id="806a8-136">assigneePriority</span><span class="sxs-lookup"><span data-stu-id="806a8-136">assigneePriority</span></span>|<span data-ttu-id="806a8-137">String</span><span class="sxs-lookup"><span data-stu-id="806a8-137">String</span></span>|<span data-ttu-id="806a8-p104">用于为列表视图中的此类型项目排序的提示。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="806a8-p104">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="806a8-140">assignments</span><span class="sxs-lookup"><span data-stu-id="806a8-140">assignments</span></span>|[<span data-ttu-id="806a8-141">plannerAssignments</span><span class="sxs-lookup"><span data-stu-id="806a8-141">plannerAssignments</span></span>](plannerassignments.md)|<span data-ttu-id="806a8-142">被分配任务的接受者集合。</span><span class="sxs-lookup"><span data-stu-id="806a8-142">The set of assignees the task is assigned to.</span></span>|
|<span data-ttu-id="806a8-143">bucketId</span><span class="sxs-lookup"><span data-stu-id="806a8-143">bucketId</span></span>|<span data-ttu-id="806a8-144">String</span><span class="sxs-lookup"><span data-stu-id="806a8-144">String</span></span>|<span data-ttu-id="806a8-145">此任务所属的存储桶 ID。</span><span class="sxs-lookup"><span data-stu-id="806a8-145">Bucket ID to which the task belongs.</span></span> <span data-ttu-id="806a8-146">存储桶需要位于任务所在的计划中。</span><span class="sxs-lookup"><span data-stu-id="806a8-146">The bucket needs to be in the plan that the task is in.</span></span> <span data-ttu-id="806a8-147">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="806a8-147">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="806a8-148">[格式验证](tasks-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="806a8-148">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span> |
|<span data-ttu-id="806a8-149">checklistItemCount</span><span class="sxs-lookup"><span data-stu-id="806a8-149">checklistItemCount</span></span>|<span data-ttu-id="806a8-150">Int32</span><span class="sxs-lookup"><span data-stu-id="806a8-150">Int32</span></span>|<span data-ttu-id="806a8-151">任务上存在的核对清单项的数目。</span><span class="sxs-lookup"><span data-stu-id="806a8-151">Number of checklist items that are present on the task.</span></span>|
|<span data-ttu-id="806a8-152">completedBy</span><span class="sxs-lookup"><span data-stu-id="806a8-152">completedBy</span></span>|[<span data-ttu-id="806a8-153">identitySet</span><span class="sxs-lookup"><span data-stu-id="806a8-153">identitySet</span></span>](identityset.md)|<span data-ttu-id="806a8-154">完成任务的用户的身份。</span><span class="sxs-lookup"><span data-stu-id="806a8-154">Identity of the user that completed the task.</span></span>|
|<span data-ttu-id="806a8-155">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="806a8-155">completedDateTime</span></span>|<span data-ttu-id="806a8-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="806a8-156">DateTimeOffset</span></span>|<span data-ttu-id="806a8-p106">只读。任务的 `'percentComplete'` 被设置为 `'100'` 的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="806a8-p106">Read-only. Date and time at which the `'percentComplete'` of the task is set to `'100'`. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="806a8-161">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="806a8-161">conversationThreadId</span></span>|<span data-ttu-id="806a8-162">字符串</span><span class="sxs-lookup"><span data-stu-id="806a8-162">String</span></span>|<span data-ttu-id="806a8-p107">关于任务的对话的线程 ID。此为在组中创建的对话线程对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="806a8-p107">Thread ID of the conversation on the task. This is the ID of the conversation thread object created in the group.</span></span>|
|<span data-ttu-id="806a8-165">createdBy</span><span class="sxs-lookup"><span data-stu-id="806a8-165">createdBy</span></span>|[<span data-ttu-id="806a8-166">identitySet</span><span class="sxs-lookup"><span data-stu-id="806a8-166">identitySet</span></span>](identityset.md)|<span data-ttu-id="806a8-167">创建任务的用户的身份</span><span class="sxs-lookup"><span data-stu-id="806a8-167">Identity of the user that created the task.</span></span>|
|<span data-ttu-id="806a8-168">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="806a8-168">createdDateTime</span></span>|<span data-ttu-id="806a8-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="806a8-169">DateTimeOffset</span></span>|<span data-ttu-id="806a8-p108">只读。创建任务的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="806a8-p108">Read-only. Date and time at which the task is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="806a8-174">creationSource</span><span class="sxs-lookup"><span data-stu-id="806a8-174">creationSource</span></span>|[<span data-ttu-id="806a8-175">plannerTaskCreation</span><span class="sxs-lookup"><span data-stu-id="806a8-175">plannerTaskCreation</span></span>](../resources/plannertaskcreation.md)|<span data-ttu-id="806a8-176">包含有关任务源的信息。</span><span class="sxs-lookup"><span data-stu-id="806a8-176">Contains information about the origin of the task.</span></span>|
|<span data-ttu-id="806a8-177">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="806a8-177">dueDateTime</span></span>|<span data-ttu-id="806a8-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="806a8-178">DateTimeOffset</span></span>|<span data-ttu-id="806a8-p109">任务截止的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="806a8-p109">Date and time at which the task is due. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="806a8-182">hasDescription</span><span class="sxs-lookup"><span data-stu-id="806a8-182">hasDescription</span></span>|<span data-ttu-id="806a8-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="806a8-183">Boolean</span></span>|<span data-ttu-id="806a8-p110">只读。如果任务的 details 对象具有非空的说明，则值为 `true`，否则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="806a8-p110">Read-only. Value is `true` if the details object of the task has a non-empty description and `false` otherwise.</span></span>|
|<span data-ttu-id="806a8-186">id</span><span class="sxs-lookup"><span data-stu-id="806a8-186">id</span></span>|<span data-ttu-id="806a8-187">String</span><span class="sxs-lookup"><span data-stu-id="806a8-187">String</span></span>|<span data-ttu-id="806a8-188">只读。</span><span class="sxs-lookup"><span data-stu-id="806a8-188">Read-only.</span></span> <span data-ttu-id="806a8-189">任务的 ID。</span><span class="sxs-lookup"><span data-stu-id="806a8-189">ID of the task.</span></span> <span data-ttu-id="806a8-190">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="806a8-190">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="806a8-191">[格式验证](tasks-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="806a8-191">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="806a8-192">orderHint</span><span class="sxs-lookup"><span data-stu-id="806a8-192">orderHint</span></span>|<span data-ttu-id="806a8-193">String</span><span class="sxs-lookup"><span data-stu-id="806a8-193">String</span></span>|<span data-ttu-id="806a8-p112">用于为列表视图中的此类型项目排序的提示。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="806a8-p112">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="806a8-196">percentComplete</span><span class="sxs-lookup"><span data-stu-id="806a8-196">percentComplete</span></span>|<span data-ttu-id="806a8-197">Int32</span><span class="sxs-lookup"><span data-stu-id="806a8-197">Int32</span></span>|<span data-ttu-id="806a8-p113">任务完成的百分比。当设置为 `100` 时，任务被视为完成。</span><span class="sxs-lookup"><span data-stu-id="806a8-p113">Percentage of task completion. When set to `100`, the task is considered completed.</span></span> |
|<span data-ttu-id="806a8-200">priority</span><span class="sxs-lookup"><span data-stu-id="806a8-200">priority</span></span>|<span data-ttu-id="806a8-201">Int32</span><span class="sxs-lookup"><span data-stu-id="806a8-201">Int32</span></span>|<span data-ttu-id="806a8-202">任务的优先级。</span><span class="sxs-lookup"><span data-stu-id="806a8-202">Priority of the task.</span></span> <span data-ttu-id="806a8-203">有效值范围介于非独占 (之间) ，而增加的值优先级较低 (优先级最高，优先级最低 `0` `10` `0` `10`) 。</span><span class="sxs-lookup"><span data-stu-id="806a8-203">Valid range of values is between `0` and `10` (inclusive), with increasing value being lower priority (`0` has the highest priority and `10` has the lowest priority).</span></span>  <span data-ttu-id="806a8-204">目前，Planner 将值解释为"紧急"，并解释为"重要"、"中"和，以及" `0` `1` `2` `3` `4` `5` `6` `7` `8` `9` `10` 低"。</span><span class="sxs-lookup"><span data-stu-id="806a8-204">Currently, Planner interprets values `0` and `1` as "urgent", `2` and `3` and `4` as "important", `5`, `6`, and `7` as "medium", and `8`, `9`, and `10` as "low".</span></span>  <span data-ttu-id="806a8-205">目前，Planner 会设置 `1` `3` "urgent"、"important"、"medium"和 `5` `9` "low"的值。</span><span class="sxs-lookup"><span data-stu-id="806a8-205">Currently, Planner sets the value `1` for "urgent", `3` for "important", `5` for "medium", and `9` for "low".</span></span>|
|<span data-ttu-id="806a8-206">planId</span><span class="sxs-lookup"><span data-stu-id="806a8-206">planId</span></span>|<span data-ttu-id="806a8-207">String</span><span class="sxs-lookup"><span data-stu-id="806a8-207">String</span></span>|<span data-ttu-id="806a8-208">任务所属的计划 ID。</span><span class="sxs-lookup"><span data-stu-id="806a8-208">Plan ID to which the task belongs.</span></span>|
|<span data-ttu-id="806a8-209">previewType</span><span class="sxs-lookup"><span data-stu-id="806a8-209">previewType</span></span>|<span data-ttu-id="806a8-210">String</span><span class="sxs-lookup"><span data-stu-id="806a8-210">String</span></span>|<span data-ttu-id="806a8-211">这将设置显示在任务上的预览类型。</span><span class="sxs-lookup"><span data-stu-id="806a8-211">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="806a8-212">可取值为：`automatic`、`noPreview`、`checklist`、`description`、`reference`。</span><span class="sxs-lookup"><span data-stu-id="806a8-212">Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span>|
|<span data-ttu-id="806a8-213">referenceCount</span><span class="sxs-lookup"><span data-stu-id="806a8-213">referenceCount</span></span>|<span data-ttu-id="806a8-214">Int32</span><span class="sxs-lookup"><span data-stu-id="806a8-214">Int32</span></span>|<span data-ttu-id="806a8-215">任务上存在的外部引用的数量。</span><span class="sxs-lookup"><span data-stu-id="806a8-215">Number of external references that exist on the task.</span></span>|
|<span data-ttu-id="806a8-216">startDateTime</span><span class="sxs-lookup"><span data-stu-id="806a8-216">startDateTime</span></span>|<span data-ttu-id="806a8-217">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="806a8-217">DateTimeOffset</span></span>|<span data-ttu-id="806a8-p116">任务开始的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="806a8-p116">Date and time at which the task starts. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="806a8-221">title</span><span class="sxs-lookup"><span data-stu-id="806a8-221">title</span></span>|<span data-ttu-id="806a8-222">String</span><span class="sxs-lookup"><span data-stu-id="806a8-222">String</span></span>|<span data-ttu-id="806a8-223">任务的标题。</span><span class="sxs-lookup"><span data-stu-id="806a8-223">Title of the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="806a8-224">关系</span><span class="sxs-lookup"><span data-stu-id="806a8-224">Relationships</span></span>
| <span data-ttu-id="806a8-225">关系</span><span class="sxs-lookup"><span data-stu-id="806a8-225">Relationship</span></span> | <span data-ttu-id="806a8-226">类型</span><span class="sxs-lookup"><span data-stu-id="806a8-226">Type</span></span>   |<span data-ttu-id="806a8-227">说明</span><span class="sxs-lookup"><span data-stu-id="806a8-227">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="806a8-228">assignedToTaskBoardFormat</span><span class="sxs-lookup"><span data-stu-id="806a8-228">assignedToTaskBoardFormat</span></span>|[<span data-ttu-id="806a8-229">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="806a8-229">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)| <span data-ttu-id="806a8-p117">只读。可为 NULL。用于在按 assignedTo 分组时在任务板视图中正确呈现任务。</span><span class="sxs-lookup"><span data-stu-id="806a8-p117">Read-only. Nullable. Used to render the task correctly in the task board view when grouped by assignedTo.</span></span>|
|<span data-ttu-id="806a8-233">bucketTaskBoardFormat</span><span class="sxs-lookup"><span data-stu-id="806a8-233">bucketTaskBoardFormat</span></span>|[<span data-ttu-id="806a8-234">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="806a8-234">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)| <span data-ttu-id="806a8-p118">只读。可为 NULL。用于在按存储桶分组时在任务板视图中正确呈现任务。</span><span class="sxs-lookup"><span data-stu-id="806a8-p118">Read-only. Nullable. Used to render the task correctly in the task board view when grouped by bucket.</span></span>|
|<span data-ttu-id="806a8-238">详细信息</span><span class="sxs-lookup"><span data-stu-id="806a8-238">details</span></span>|[<span data-ttu-id="806a8-239">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="806a8-239">plannerTaskDetails</span></span>](plannertaskdetails.md)| <span data-ttu-id="806a8-p119">只读。可为 NULL。关于任务的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="806a8-p119">Read-only. Nullable. Additional details about the task.</span></span>|
|<span data-ttu-id="806a8-243">progressTaskBoardFormat</span><span class="sxs-lookup"><span data-stu-id="806a8-243">progressTaskBoardFormat</span></span>|[<span data-ttu-id="806a8-244">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="806a8-244">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)| <span data-ttu-id="806a8-p120">只读。可为 NULL。用于在按进度分组时在任务板视图中正确呈现任务。</span><span class="sxs-lookup"><span data-stu-id="806a8-p120">Read-only. Nullable. Used to render the task correctly in the task board view when grouped by progress.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="806a8-248">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="806a8-248">JSON representation</span></span>
<span data-ttu-id="806a8-249">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="806a8-249">Here is a JSON representation of the resource.</span></span>

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


