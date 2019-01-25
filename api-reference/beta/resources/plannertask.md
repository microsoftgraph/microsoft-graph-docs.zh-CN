---
title: plannerTask 资源类型
description: '**plannerTask** 资源表示 Office 365 中的规划器任务。规划器任务包含在计划内，可以分配给计划中的存储桶。每个任务对象具有可以包含此任务的更多信息的 details 对象。请参阅概述了解有关组、计划和任务之间的关系的详细信息。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 2313b31e0a962f27fa728af8c8953b646210397a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511210"
---
# <a name="plannertask-resource-type"></a><span data-ttu-id="149cd-106">plannerTask 资源类型</span><span class="sxs-lookup"><span data-stu-id="149cd-106">plannerTask resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="149cd-p102">**plannerTask** 资源表示 Office 365 中的规划器任务。规划器任务包含在[计划](plannerplan.md)内，可以分配给计划中的[存储桶](plannerbucket.md)。每个任务对象具有可以包含此任务的更多信息的 [details](plannertaskdetails.md) 对象。请参阅[概述](planner-overview.md)了解有关组、计划和任务之间的关系的详细信息。</span><span class="sxs-lookup"><span data-stu-id="149cd-p102">The **plannerTask** resource represents a Planner task in Office 365. A Planner task is contained in a [plan](plannerplan.md) and can be assigned to a [bucket](plannerbucket.md) in a plan. Each task object has a [details](plannertaskdetails.md) object which can contain more information about the task. See [overview](planner-overview.md) for more information regarding relationships between group, plan and task.</span></span>


## <a name="methods"></a><span data-ttu-id="149cd-111">方法</span><span class="sxs-lookup"><span data-stu-id="149cd-111">Methods</span></span>

| <span data-ttu-id="149cd-112">方法</span><span class="sxs-lookup"><span data-stu-id="149cd-112">Method</span></span>           | <span data-ttu-id="149cd-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="149cd-113">Return Type</span></span>    |<span data-ttu-id="149cd-114">说明</span><span class="sxs-lookup"><span data-stu-id="149cd-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="149cd-115">获取 plannerTask</span><span class="sxs-lookup"><span data-stu-id="149cd-115">Get plannerTask</span></span>](../api/plannertask-get.md) | [<span data-ttu-id="149cd-116">plannerTask</span><span class="sxs-lookup"><span data-stu-id="149cd-116">plannerTask</span></span>](plannertask.md) |<span data-ttu-id="149cd-117">读取 **plannerTask** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="149cd-117">Read properties and relationships of **plannerTask** object.</span></span>|
|[<span data-ttu-id="149cd-118">更新</span><span class="sxs-lookup"><span data-stu-id="149cd-118">Update</span></span>](../api/plannertask-update.md) | [<span data-ttu-id="149cd-119">plannerTask</span><span class="sxs-lookup"><span data-stu-id="149cd-119">plannerTask</span></span>](plannertask.md) |<span data-ttu-id="149cd-120">更新 **plannerTask** 对象。</span><span class="sxs-lookup"><span data-stu-id="149cd-120">Update **plannerTask** object.</span></span> |
|[<span data-ttu-id="149cd-121">删除</span><span class="sxs-lookup"><span data-stu-id="149cd-121">Delete</span></span>](../api/plannertask-delete.md) | <span data-ttu-id="149cd-122">无</span><span class="sxs-lookup"><span data-stu-id="149cd-122">None</span></span> |<span data-ttu-id="149cd-123">删除 **plannerTask** 对象。</span><span class="sxs-lookup"><span data-stu-id="149cd-123">Delete **plannerTask** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="149cd-124">属性</span><span class="sxs-lookup"><span data-stu-id="149cd-124">Properties</span></span>
| <span data-ttu-id="149cd-125">属性</span><span class="sxs-lookup"><span data-stu-id="149cd-125">Property</span></span>     | <span data-ttu-id="149cd-126">类型</span><span class="sxs-lookup"><span data-stu-id="149cd-126">Type</span></span>   |<span data-ttu-id="149cd-127">说明</span><span class="sxs-lookup"><span data-stu-id="149cd-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="149cd-128">activeChecklistItemCount</span><span class="sxs-lookup"><span data-stu-id="149cd-128">activeChecklistItemCount</span></span>|<span data-ttu-id="149cd-129">Int32</span><span class="sxs-lookup"><span data-stu-id="149cd-129">Int32</span></span>|<span data-ttu-id="149cd-130">核对清单项的数量，其值设置为“false”，表示项目不全。</span><span class="sxs-lookup"><span data-stu-id="149cd-130">Number of checklist items with value set to 'false', representing incomplete items.</span></span>|
|<span data-ttu-id="149cd-131">appliedCategories</span><span class="sxs-lookup"><span data-stu-id="149cd-131">appliedCategories</span></span>|[<span data-ttu-id="149cd-132">plannerAppliedCategories</span><span class="sxs-lookup"><span data-stu-id="149cd-132">plannerAppliedCategories</span></span>](plannerappliedcategories.md)|<span data-ttu-id="149cd-p103">此任务已应用的类别。有关可能的值，请参阅[已应用的类别](plannerappliedcategories.md)。</span><span class="sxs-lookup"><span data-stu-id="149cd-p103">The categories to which the task has been applied. See [applied Categories](plannerappliedcategories.md) for possible values.</span></span>|
|<span data-ttu-id="149cd-135">assigneePriority</span><span class="sxs-lookup"><span data-stu-id="149cd-135">assigneePriority</span></span>|<span data-ttu-id="149cd-136">String</span><span class="sxs-lookup"><span data-stu-id="149cd-136">String</span></span>|<span data-ttu-id="149cd-p104">用于为列表视图中的此类型项目排序的提示。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="149cd-p104">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="149cd-139">assignments</span><span class="sxs-lookup"><span data-stu-id="149cd-139">assignments</span></span>|[<span data-ttu-id="149cd-140">plannerAssignments</span><span class="sxs-lookup"><span data-stu-id="149cd-140">plannerAssignments</span></span>](plannerassignments.md)|<span data-ttu-id="149cd-141">被分配任务的接受者集合。</span><span class="sxs-lookup"><span data-stu-id="149cd-141">The set of assignees the task is assigned to.</span></span>|
|<span data-ttu-id="149cd-142">bucketId</span><span class="sxs-lookup"><span data-stu-id="149cd-142">bucketId</span></span>|<span data-ttu-id="149cd-143">String</span><span class="sxs-lookup"><span data-stu-id="149cd-143">String</span></span>|<span data-ttu-id="149cd-144">任务所属的地址散列表元 ID。</span><span class="sxs-lookup"><span data-stu-id="149cd-144">Bucket ID to which the task belongs.</span></span> <span data-ttu-id="149cd-145">地址散列表元需要在计划中的任务。</span><span class="sxs-lookup"><span data-stu-id="149cd-145">The bucket needs to be in the plan that the task is in.</span></span> <span data-ttu-id="149cd-146">它是 28 字符长度和区分大小写。</span><span class="sxs-lookup"><span data-stu-id="149cd-146">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="149cd-147">服务上执行[格式验证](tasks-identifiers-disclaimer.md)。</span><span class="sxs-lookup"><span data-stu-id="149cd-147">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span> |
|<span data-ttu-id="149cd-148">checklistItemCount</span><span class="sxs-lookup"><span data-stu-id="149cd-148">checklistItemCount</span></span>|<span data-ttu-id="149cd-149">Int32</span><span class="sxs-lookup"><span data-stu-id="149cd-149">Int32</span></span>|<span data-ttu-id="149cd-150">任务上存在的核对清单项的数目。</span><span class="sxs-lookup"><span data-stu-id="149cd-150">Number of checklist items that are present on the task.</span></span>|
|<span data-ttu-id="149cd-151">completedBy</span><span class="sxs-lookup"><span data-stu-id="149cd-151">completedBy</span></span>|[<span data-ttu-id="149cd-152">identitySet</span><span class="sxs-lookup"><span data-stu-id="149cd-152">identitySet</span></span>](identityset.md)|<span data-ttu-id="149cd-153">完成任务的用户的身份。</span><span class="sxs-lookup"><span data-stu-id="149cd-153">Identity of the user that completed the task.</span></span>|
|<span data-ttu-id="149cd-154">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="149cd-154">completedDateTime</span></span>|<span data-ttu-id="149cd-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="149cd-155">DateTimeOffset</span></span>|<span data-ttu-id="149cd-p106">只读。任务的 `'percentComplete'` 被设置为 `'100'` 的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="149cd-p106">Read-only. Date and time at which the `'percentComplete'` of the task is set to `'100'`. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="149cd-160">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="149cd-160">conversationThreadId</span></span>|<span data-ttu-id="149cd-161">字符串</span><span class="sxs-lookup"><span data-stu-id="149cd-161">String</span></span>|<span data-ttu-id="149cd-p107">关于任务的对话的线程 ID。此为在组中创建的对话线程对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="149cd-p107">Thread ID of the conversation on the task. This is the ID of the conversation thread object created in the group.</span></span>|
|<span data-ttu-id="149cd-164">createdBy</span><span class="sxs-lookup"><span data-stu-id="149cd-164">createdBy</span></span>|[<span data-ttu-id="149cd-165">identitySet</span><span class="sxs-lookup"><span data-stu-id="149cd-165">identitySet</span></span>](identityset.md)|<span data-ttu-id="149cd-166">创建任务的用户的身份</span><span class="sxs-lookup"><span data-stu-id="149cd-166">Identity of the user that created the task.</span></span>|
|<span data-ttu-id="149cd-167">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="149cd-167">createdDateTime</span></span>|<span data-ttu-id="149cd-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="149cd-168">DateTimeOffset</span></span>|<span data-ttu-id="149cd-p108">只读。创建任务的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="149cd-p108">Read-only. Date and time at which the task is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="149cd-173">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="149cd-173">dueDateTime</span></span>|<span data-ttu-id="149cd-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="149cd-174">DateTimeOffset</span></span>|<span data-ttu-id="149cd-p109">任务截止的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="149cd-p109">Date and time at which the task is due. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="149cd-178">hasDescription</span><span class="sxs-lookup"><span data-stu-id="149cd-178">hasDescription</span></span>|<span data-ttu-id="149cd-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="149cd-179">Boolean</span></span>|<span data-ttu-id="149cd-p110">只读。如果任务的 details 对象具有非空的说明，则值为 `true`，否则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="149cd-p110">Read-only. Value is `true` if the details object of the task has a non-empty description and `false` otherwise.</span></span>|
|<span data-ttu-id="149cd-182">id</span><span class="sxs-lookup"><span data-stu-id="149cd-182">id</span></span>|<span data-ttu-id="149cd-183">String</span><span class="sxs-lookup"><span data-stu-id="149cd-183">String</span></span>|<span data-ttu-id="149cd-184">只读。</span><span class="sxs-lookup"><span data-stu-id="149cd-184">Read-only.</span></span> <span data-ttu-id="149cd-185">任务的 ID。</span><span class="sxs-lookup"><span data-stu-id="149cd-185">ID of the task.</span></span> <span data-ttu-id="149cd-186">它是 28 字符长度和区分大小写。</span><span class="sxs-lookup"><span data-stu-id="149cd-186">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="149cd-187">服务上执行[格式验证](tasks-identifiers-disclaimer.md)。</span><span class="sxs-lookup"><span data-stu-id="149cd-187">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="149cd-188">orderHint</span><span class="sxs-lookup"><span data-stu-id="149cd-188">orderHint</span></span>|<span data-ttu-id="149cd-189">String</span><span class="sxs-lookup"><span data-stu-id="149cd-189">String</span></span>|<span data-ttu-id="149cd-p112">提示用于为列表视图中的此类项目排序。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="149cd-p112">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="149cd-192">percentComplete</span><span class="sxs-lookup"><span data-stu-id="149cd-192">percentComplete</span></span>|<span data-ttu-id="149cd-193">Int32</span><span class="sxs-lookup"><span data-stu-id="149cd-193">Int32</span></span>|<span data-ttu-id="149cd-p113">任务完成的百分比。当设置为 `100` 时，任务被视为完成。</span><span class="sxs-lookup"><span data-stu-id="149cd-p113">Percentage of task completion. When set to `100`, the task is considered completed.</span></span> |
|<span data-ttu-id="149cd-196">planId</span><span class="sxs-lookup"><span data-stu-id="149cd-196">planId</span></span>|<span data-ttu-id="149cd-197">String</span><span class="sxs-lookup"><span data-stu-id="149cd-197">String</span></span>|<span data-ttu-id="149cd-198">任务所属的计划 ID。</span><span class="sxs-lookup"><span data-stu-id="149cd-198">Plan ID to which the task belongs.</span></span>|
|<span data-ttu-id="149cd-199">previewType</span><span class="sxs-lookup"><span data-stu-id="149cd-199">previewType</span></span>|<span data-ttu-id="149cd-200">string</span><span class="sxs-lookup"><span data-stu-id="149cd-200">string</span></span>|<span data-ttu-id="149cd-p114">这将设置显示在任务上的预览类型。可能的值是：`automatic`、`noPreview`、`checklist`、`description`、`reference`。</span><span class="sxs-lookup"><span data-stu-id="149cd-p114">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span>|
|<span data-ttu-id="149cd-203">referenceCount</span><span class="sxs-lookup"><span data-stu-id="149cd-203">referenceCount</span></span>|<span data-ttu-id="149cd-204">Int32</span><span class="sxs-lookup"><span data-stu-id="149cd-204">Int32</span></span>|<span data-ttu-id="149cd-205">任务上存在的外部引用的数量。</span><span class="sxs-lookup"><span data-stu-id="149cd-205">Number of external references that exist on the task.</span></span>|
|<span data-ttu-id="149cd-206">startDateTime</span><span class="sxs-lookup"><span data-stu-id="149cd-206">startDateTime</span></span>|<span data-ttu-id="149cd-207">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="149cd-207">DateTimeOffset</span></span>|<span data-ttu-id="149cd-p115">任务开始的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="149cd-p115">Date and time at which the task starts. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="149cd-211">title</span><span class="sxs-lookup"><span data-stu-id="149cd-211">title</span></span>|<span data-ttu-id="149cd-212">String</span><span class="sxs-lookup"><span data-stu-id="149cd-212">String</span></span>|<span data-ttu-id="149cd-213">任务的标题。</span><span class="sxs-lookup"><span data-stu-id="149cd-213">Title of the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="149cd-214">关系</span><span class="sxs-lookup"><span data-stu-id="149cd-214">Relationships</span></span>
| <span data-ttu-id="149cd-215">关系</span><span class="sxs-lookup"><span data-stu-id="149cd-215">Relationship</span></span> | <span data-ttu-id="149cd-216">类型</span><span class="sxs-lookup"><span data-stu-id="149cd-216">Type</span></span>   |<span data-ttu-id="149cd-217">说明</span><span class="sxs-lookup"><span data-stu-id="149cd-217">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="149cd-218">assignedToTaskBoardFormat</span><span class="sxs-lookup"><span data-stu-id="149cd-218">assignedToTaskBoardFormat</span></span>|[<span data-ttu-id="149cd-219">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="149cd-219">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)| <span data-ttu-id="149cd-p116">只读。可为 NULL。用于在按 assignedTo 分组时在任务板视图中正确呈现任务。</span><span class="sxs-lookup"><span data-stu-id="149cd-p116">Read-only. Nullable. Used to render the task correctly in the task board view when grouped by assignedTo.</span></span>|
|<span data-ttu-id="149cd-223">bucketTaskBoardFormat</span><span class="sxs-lookup"><span data-stu-id="149cd-223">bucketTaskBoardFormat</span></span>|[<span data-ttu-id="149cd-224">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="149cd-224">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)| <span data-ttu-id="149cd-p117">只读。可为 NULL。用于在按存储桶分组时在任务板视图中正确呈现任务。</span><span class="sxs-lookup"><span data-stu-id="149cd-p117">Read-only. Nullable. Used to render the task correctly in the task board view when grouped by bucket.</span></span>|
|<span data-ttu-id="149cd-228">详细信息</span><span class="sxs-lookup"><span data-stu-id="149cd-228">details</span></span>|[<span data-ttu-id="149cd-229">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="149cd-229">plannerTaskDetails</span></span>](plannertaskdetails.md)| <span data-ttu-id="149cd-p118">只读。可为 NULL。关于任务的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="149cd-p118">Read-only. Nullable. Additional details about the task.</span></span>|
|<span data-ttu-id="149cd-233">progressTaskBoardFormat</span><span class="sxs-lookup"><span data-stu-id="149cd-233">progressTaskBoardFormat</span></span>|[<span data-ttu-id="149cd-234">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="149cd-234">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)| <span data-ttu-id="149cd-p119">只读。可为 NULL。用于在按进度分组时在任务板视图中正确呈现任务。</span><span class="sxs-lookup"><span data-stu-id="149cd-p119">Read-only. Nullable. Used to render the task correctly in the task board view when grouped by progress.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="149cd-238">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="149cd-238">JSON representation</span></span>
<span data-ttu-id="149cd-239">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="149cd-239">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
<!--
{
  "type": "#page.annotation",
  "description": "plannerTask resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannertask.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
