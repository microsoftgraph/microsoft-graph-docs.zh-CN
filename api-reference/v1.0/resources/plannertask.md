---
title: plannerTask 资源类型
description: '**plannerTask** 资源表示 Office 365 中的规划器任务。规划器任务包含在计划内，可以分配给计划中的存储桶。每个任务对象具有可以包含此任务的更多信息的 details 对象。请参阅概述了解有关组、计划和任务之间的关系的详细信息。'
localization_priority: Priority
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 3a90dcdc2cbad09355619c1afe1ff3200181fb39
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917585"
---
# <a name="plannertask-resource-type"></a><span data-ttu-id="525be-106">plannerTask 资源类型</span><span class="sxs-lookup"><span data-stu-id="525be-106">plannerTask resource type</span></span>

<span data-ttu-id="525be-p102">**plannerTask** 资源表示 Office 365 中的规划器任务。规划器任务包含在[计划](plannerplan.md)内，可以分配给计划中的[存储桶](plannerbucket.md)。每个任务对象具有可以包含此任务的更多信息的 [details](plannertaskdetails.md) 对象。请参阅[概述](planner-overview.md)了解有关组、计划和任务之间的关系的详细信息。</span><span class="sxs-lookup"><span data-stu-id="525be-p102">The **plannerTask** resource represents a Planner task in Office 365. A Planner task is contained in a [plan](plannerplan.md) and can be assigned to a [bucket](plannerbucket.md) in a plan. Each task object has a [details](plannertaskdetails.md) object which can contain more information about the task. See [overview](planner-overview.md) for more information regarding relationships between group, plan and task.</span></span>


## <a name="methods"></a><span data-ttu-id="525be-111">方法</span><span class="sxs-lookup"><span data-stu-id="525be-111">Methods</span></span>

| <span data-ttu-id="525be-112">方法</span><span class="sxs-lookup"><span data-stu-id="525be-112">Method</span></span>           | <span data-ttu-id="525be-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="525be-113">Return Type</span></span>    |<span data-ttu-id="525be-114">说明</span><span class="sxs-lookup"><span data-stu-id="525be-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="525be-115">获取 plannerTask</span><span class="sxs-lookup"><span data-stu-id="525be-115">Get plannerTask</span></span>](../api/plannertask-get.md) | [<span data-ttu-id="525be-116">plannerTask</span><span class="sxs-lookup"><span data-stu-id="525be-116">plannerTask</span></span>](plannertask.md) |<span data-ttu-id="525be-117">读取 **plannerTask** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="525be-117">Read properties and relationships of **plannerTask** object.</span></span>|
|[<span data-ttu-id="525be-118">更新</span><span class="sxs-lookup"><span data-stu-id="525be-118">Update</span></span>](../api/plannertask-update.md) | [<span data-ttu-id="525be-119">plannerTask</span><span class="sxs-lookup"><span data-stu-id="525be-119">plannerTask</span></span>](plannertask.md) |<span data-ttu-id="525be-120">更新 **plannerTask** 对象。</span><span class="sxs-lookup"><span data-stu-id="525be-120">Update **plannerTask** object.</span></span> |
|[<span data-ttu-id="525be-121">删除</span><span class="sxs-lookup"><span data-stu-id="525be-121">Delete</span></span>](../api/plannertask-delete.md) | <span data-ttu-id="525be-122">无</span><span class="sxs-lookup"><span data-stu-id="525be-122">None</span></span> |<span data-ttu-id="525be-123">删除 **plannerTask** 对象。</span><span class="sxs-lookup"><span data-stu-id="525be-123">Delete **plannerTask** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="525be-124">属性</span><span class="sxs-lookup"><span data-stu-id="525be-124">Properties</span></span>
| <span data-ttu-id="525be-125">属性</span><span class="sxs-lookup"><span data-stu-id="525be-125">Property</span></span>     | <span data-ttu-id="525be-126">类型</span><span class="sxs-lookup"><span data-stu-id="525be-126">Type</span></span>   |<span data-ttu-id="525be-127">说明</span><span class="sxs-lookup"><span data-stu-id="525be-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="525be-128">activeChecklistItemCount</span><span class="sxs-lookup"><span data-stu-id="525be-128">activeChecklistItemCount</span></span>|<span data-ttu-id="525be-129">Int32</span><span class="sxs-lookup"><span data-stu-id="525be-129">Int32</span></span>|<span data-ttu-id="525be-130">核对清单项的数量，其值设置为“false”，表示项目不全。</span><span class="sxs-lookup"><span data-stu-id="525be-130">Number of checklist items with value set to 'false', representing incomplete items.</span></span>|
|<span data-ttu-id="525be-131">appliedCategories</span><span class="sxs-lookup"><span data-stu-id="525be-131">appliedCategories</span></span>|[<span data-ttu-id="525be-132">plannerAppliedCategories</span><span class="sxs-lookup"><span data-stu-id="525be-132">plannerAppliedCategories</span></span>](plannerappliedcategories.md)|<span data-ttu-id="525be-p103">此任务已应用的类别。有关可能的值，请参阅[已应用的类别](plannerappliedcategories.md)。</span><span class="sxs-lookup"><span data-stu-id="525be-p103">The categories to which the task has been applied. See [applied Categories](plannerappliedcategories.md) for possible values.</span></span>|
|<span data-ttu-id="525be-135">assigneePriority</span><span class="sxs-lookup"><span data-stu-id="525be-135">assigneePriority</span></span>|<span data-ttu-id="525be-136">String</span><span class="sxs-lookup"><span data-stu-id="525be-136">String</span></span>|<span data-ttu-id="525be-p104">提示用于为列表视图中的此类项目排序。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="525be-p104">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="525be-139">assignments</span><span class="sxs-lookup"><span data-stu-id="525be-139">assignments</span></span>|[<span data-ttu-id="525be-140">plannerAssignments</span><span class="sxs-lookup"><span data-stu-id="525be-140">plannerAssignments</span></span>](plannerassignments.md)|<span data-ttu-id="525be-141">被分配任务的接受者集合。</span><span class="sxs-lookup"><span data-stu-id="525be-141">The set of assignees the task is assigned to.</span></span>|
|<span data-ttu-id="525be-142">bucketId</span><span class="sxs-lookup"><span data-stu-id="525be-142">bucketId</span></span>|<span data-ttu-id="525be-143">字符串</span><span class="sxs-lookup"><span data-stu-id="525be-143">String</span></span>|<span data-ttu-id="525be-144">任务所属的地址散列表元 ID。</span><span class="sxs-lookup"><span data-stu-id="525be-144">Bucket ID to which the task belongs.</span></span> <span data-ttu-id="525be-145">地址散列表元需要在计划中的任务。</span><span class="sxs-lookup"><span data-stu-id="525be-145">The bucket needs to be in the plan that the task is in.</span></span> <span data-ttu-id="525be-146">它是 28 字符长度和区分大小写。</span><span class="sxs-lookup"><span data-stu-id="525be-146">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="525be-147">服务上执行[格式验证](planner-identifiers-disclaimer.md)。</span><span class="sxs-lookup"><span data-stu-id="525be-147">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span> |
|<span data-ttu-id="525be-148">checklistItemCount</span><span class="sxs-lookup"><span data-stu-id="525be-148">checklistItemCount</span></span>|<span data-ttu-id="525be-149">Int32</span><span class="sxs-lookup"><span data-stu-id="525be-149">Int32</span></span>|<span data-ttu-id="525be-150">任务上存在的核对清单项的数目。</span><span class="sxs-lookup"><span data-stu-id="525be-150">Number of checklist items that are present on the task.</span></span>|
|<span data-ttu-id="525be-151">completedBy</span><span class="sxs-lookup"><span data-stu-id="525be-151">completedBy</span></span>|[<span data-ttu-id="525be-152">identitySet</span><span class="sxs-lookup"><span data-stu-id="525be-152">identitySet</span></span>](identityset.md)|<span data-ttu-id="525be-153">完成任务的用户的身份。</span><span class="sxs-lookup"><span data-stu-id="525be-153">Identity of the user that completed the task.</span></span>|
|<span data-ttu-id="525be-154">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="525be-154">completedDateTime</span></span>|<span data-ttu-id="525be-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="525be-155">DateTimeOffset</span></span>|<span data-ttu-id="525be-p106">只读。任务的 `'percentComplete'` 被设置为 `'100'` 的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="525be-p106">Read-only. Date and time at which the `'percentComplete'` of the task is set to `'100'`. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="525be-160">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="525be-160">conversationThreadId</span></span>|<span data-ttu-id="525be-161">字符串</span><span class="sxs-lookup"><span data-stu-id="525be-161">String</span></span>|<span data-ttu-id="525be-p107">关于任务的对话的线程 ID。此为在组中创建的对话线程对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="525be-p107">Thread ID of the conversation on the task. This is the ID of the conversation thread object created in the group.</span></span>|
|<span data-ttu-id="525be-164">createdBy</span><span class="sxs-lookup"><span data-stu-id="525be-164">createdBy</span></span>|[<span data-ttu-id="525be-165">identitySet</span><span class="sxs-lookup"><span data-stu-id="525be-165">identitySet</span></span>](identityset.md)|<span data-ttu-id="525be-166">创建任务的用户的身份</span><span class="sxs-lookup"><span data-stu-id="525be-166">Identity of the user that created the task.</span></span>|
|<span data-ttu-id="525be-167">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="525be-167">createdDateTime</span></span>|<span data-ttu-id="525be-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="525be-168">DateTimeOffset</span></span>|<span data-ttu-id="525be-p108">只读。创建任务的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="525be-p108">Read-only. Date and time at which the task is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="525be-173">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="525be-173">dueDateTime</span></span>|<span data-ttu-id="525be-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="525be-174">DateTimeOffset</span></span>|<span data-ttu-id="525be-p109">任务截止的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="525be-p109">Date and time at which the task is due. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="525be-178">hasDescription</span><span class="sxs-lookup"><span data-stu-id="525be-178">hasDescription</span></span>|<span data-ttu-id="525be-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="525be-179">Boolean</span></span>|<span data-ttu-id="525be-p110">只读。如果任务的 details 对象具有非空的说明，则值为 `true`，否则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="525be-p110">Read-only. Value is `true` if the details object of the task has a non-empty description and `false` otherwise.</span></span>|
|<span data-ttu-id="525be-182">id</span><span class="sxs-lookup"><span data-stu-id="525be-182">id</span></span>|<span data-ttu-id="525be-183">String</span><span class="sxs-lookup"><span data-stu-id="525be-183">String</span></span>|<span data-ttu-id="525be-184">只读。</span><span class="sxs-lookup"><span data-stu-id="525be-184">Read-only.</span></span> <span data-ttu-id="525be-185">任务的 ID。</span><span class="sxs-lookup"><span data-stu-id="525be-185">ID of the task.</span></span> <span data-ttu-id="525be-186">它是 28 字符长度和区分大小写。</span><span class="sxs-lookup"><span data-stu-id="525be-186">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="525be-187">服务上执行[格式验证](planner-identifiers-disclaimer.md)。</span><span class="sxs-lookup"><span data-stu-id="525be-187">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="525be-188">orderHint</span><span class="sxs-lookup"><span data-stu-id="525be-188">orderHint</span></span>|<span data-ttu-id="525be-189">String</span><span class="sxs-lookup"><span data-stu-id="525be-189">String</span></span>|<span data-ttu-id="525be-p112">提示用于为列表视图中的此类项目排序。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="525be-p112">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="525be-192">percentComplete</span><span class="sxs-lookup"><span data-stu-id="525be-192">percentComplete</span></span>|<span data-ttu-id="525be-193">Int32</span><span class="sxs-lookup"><span data-stu-id="525be-193">Int32</span></span>|<span data-ttu-id="525be-p113">任务完成的百分比。当设置为 `100` 时，任务被视为完成。</span><span class="sxs-lookup"><span data-stu-id="525be-p113">Percentage of task completion. When set to `100`, the task is considered completed.</span></span> |
|<span data-ttu-id="525be-196">planId</span><span class="sxs-lookup"><span data-stu-id="525be-196">planId</span></span>|<span data-ttu-id="525be-197">String</span><span class="sxs-lookup"><span data-stu-id="525be-197">String</span></span>|<span data-ttu-id="525be-198">任务所属的计划 ID。</span><span class="sxs-lookup"><span data-stu-id="525be-198">Plan ID to which the task belongs.</span></span>|
|<span data-ttu-id="525be-199">previewType</span><span class="sxs-lookup"><span data-stu-id="525be-199">previewType</span></span>|<span data-ttu-id="525be-200">plannerPreviewType</span><span class="sxs-lookup"><span data-stu-id="525be-200">plannerPreviewType</span></span>|<span data-ttu-id="525be-201">这将设置显示任务的预览的类型。</span><span class="sxs-lookup"><span data-stu-id="525be-201">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="525be-202">可能的值为： `automatic`， `noPreview`， `checklist`， `description`， `reference`。</span><span class="sxs-lookup"><span data-stu-id="525be-202">The possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span>|
|<span data-ttu-id="525be-203">referenceCount</span><span class="sxs-lookup"><span data-stu-id="525be-203">referenceCount</span></span>|<span data-ttu-id="525be-204">Int32</span><span class="sxs-lookup"><span data-stu-id="525be-204">Int32</span></span>|<span data-ttu-id="525be-205">任务上存在的外部引用的数量。</span><span class="sxs-lookup"><span data-stu-id="525be-205">Number of external references that exist on the task.</span></span>|
|<span data-ttu-id="525be-206">startDateTime</span><span class="sxs-lookup"><span data-stu-id="525be-206">startDateTime</span></span>|<span data-ttu-id="525be-207">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="525be-207">DateTimeOffset</span></span>|<span data-ttu-id="525be-p115">任务开始的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="525be-p115">Date and time at which the task starts. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="525be-211">title</span><span class="sxs-lookup"><span data-stu-id="525be-211">title</span></span>|<span data-ttu-id="525be-212">String</span><span class="sxs-lookup"><span data-stu-id="525be-212">String</span></span>|<span data-ttu-id="525be-213">任务的标题。</span><span class="sxs-lookup"><span data-stu-id="525be-213">Title of the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="525be-214">关系</span><span class="sxs-lookup"><span data-stu-id="525be-214">Relationships</span></span>
| <span data-ttu-id="525be-215">关系</span><span class="sxs-lookup"><span data-stu-id="525be-215">Relationship</span></span> | <span data-ttu-id="525be-216">类型</span><span class="sxs-lookup"><span data-stu-id="525be-216">Type</span></span>   |<span data-ttu-id="525be-217">说明</span><span class="sxs-lookup"><span data-stu-id="525be-217">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="525be-218">assignedToTaskBoardFormat</span><span class="sxs-lookup"><span data-stu-id="525be-218">assignedToTaskBoardFormat</span></span>|[<span data-ttu-id="525be-219">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="525be-219">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)| <span data-ttu-id="525be-p116">只读。可为 NULL。用于在按 assignedTo 分组时在任务板视图中正确呈现任务。</span><span class="sxs-lookup"><span data-stu-id="525be-p116">Read-only. Nullable. Used to render the task correctly in the task board view when grouped by assignedTo.</span></span>|
|<span data-ttu-id="525be-223">bucketTaskBoardFormat</span><span class="sxs-lookup"><span data-stu-id="525be-223">bucketTaskBoardFormat</span></span>|[<span data-ttu-id="525be-224">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="525be-224">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)| <span data-ttu-id="525be-p117">只读。可为 NULL。用于在按存储桶分组时在任务板视图中正确呈现任务。</span><span class="sxs-lookup"><span data-stu-id="525be-p117">Read-only. Nullable. Used to render the task correctly in the task board view when grouped by bucket.</span></span>|
|<span data-ttu-id="525be-228">详细信息</span><span class="sxs-lookup"><span data-stu-id="525be-228">details</span></span>|[<span data-ttu-id="525be-229">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="525be-229">plannerTaskDetails</span></span>](plannertaskdetails.md)| <span data-ttu-id="525be-p118">只读。可为 NULL。关于任务的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="525be-p118">Read-only. Nullable. Additional details about the task.</span></span>|
|<span data-ttu-id="525be-233">progressTaskBoardFormat</span><span class="sxs-lookup"><span data-stu-id="525be-233">progressTaskBoardFormat</span></span>|[<span data-ttu-id="525be-234">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="525be-234">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)| <span data-ttu-id="525be-p119">只读。可为 NULL。用于在按进度分组时在任务板视图中正确呈现任务。</span><span class="sxs-lookup"><span data-stu-id="525be-p119">Read-only. Nullable. Used to render the task correctly in the task board view when grouped by progress.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="525be-238">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="525be-238">JSON representation</span></span>
<span data-ttu-id="525be-239">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="525be-239">Here is a JSON representation of the resource.</span></span>

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
  "previewType": "string",
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
