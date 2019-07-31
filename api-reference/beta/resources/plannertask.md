---
title: plannerTask 资源类型
description: '**plannerTask** 资源表示 Office 365 中的规划器任务。规划器任务包含在计划内，可以分配给计划中的存储桶。每个任务对象具有可以包含此任务的更多信息的 details 对象。请参阅概述了解有关组、计划和任务之间的关系的详细信息。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 1eb718daad405fb6aaed2f170747bc91dad47b76
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008997"
---
# <a name="plannertask-resource-type"></a><span data-ttu-id="99074-106">plannerTask 资源类型</span><span class="sxs-lookup"><span data-stu-id="99074-106">plannerTask resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99074-p102">**plannerTask** 资源表示 Office 365 中的规划器任务。规划器任务包含在[计划](plannerplan.md)内，可以分配给计划中的[存储桶](plannerbucket.md)。每个任务对象具有可以包含此任务的更多信息的 [details](plannertaskdetails.md) 对象。请参阅[概述](planner-overview.md)了解有关组、计划和任务之间的关系的详细信息。</span><span class="sxs-lookup"><span data-stu-id="99074-p102">The **plannerTask** resource represents a Planner task in Office 365. A Planner task is contained in a [plan](plannerplan.md) and can be assigned to a [bucket](plannerbucket.md) in a plan. Each task object has a [details](plannertaskdetails.md) object which can contain more information about the task. See [overview](planner-overview.md) for more information regarding relationships between group, plan and task.</span></span>


## <a name="methods"></a><span data-ttu-id="99074-111">方法</span><span class="sxs-lookup"><span data-stu-id="99074-111">Methods</span></span>

| <span data-ttu-id="99074-112">方法</span><span class="sxs-lookup"><span data-stu-id="99074-112">Method</span></span>           | <span data-ttu-id="99074-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="99074-113">Return Type</span></span>    |<span data-ttu-id="99074-114">说明</span><span class="sxs-lookup"><span data-stu-id="99074-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="99074-115">获取 plannerTask</span><span class="sxs-lookup"><span data-stu-id="99074-115">Get plannerTask</span></span>](../api/plannertask-get.md) | [<span data-ttu-id="99074-116">plannerTask</span><span class="sxs-lookup"><span data-stu-id="99074-116">plannerTask</span></span>](plannertask.md) |<span data-ttu-id="99074-117">读取 **plannerTask** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="99074-117">Read properties and relationships of **plannerTask** object.</span></span>|
|[<span data-ttu-id="99074-118">更新</span><span class="sxs-lookup"><span data-stu-id="99074-118">Update</span></span>](../api/plannertask-update.md) | [<span data-ttu-id="99074-119">plannerTask</span><span class="sxs-lookup"><span data-stu-id="99074-119">plannerTask</span></span>](plannertask.md) |<span data-ttu-id="99074-120">更新 **plannerTask** 对象。</span><span class="sxs-lookup"><span data-stu-id="99074-120">Update **plannerTask** object.</span></span> |
|[<span data-ttu-id="99074-121">删除</span><span class="sxs-lookup"><span data-stu-id="99074-121">Delete</span></span>](../api/plannertask-delete.md) | <span data-ttu-id="99074-122">无</span><span class="sxs-lookup"><span data-stu-id="99074-122">None</span></span> |<span data-ttu-id="99074-123">删除 **plannerTask** 对象。</span><span class="sxs-lookup"><span data-stu-id="99074-123">Delete **plannerTask** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="99074-124">属性</span><span class="sxs-lookup"><span data-stu-id="99074-124">Properties</span></span>
| <span data-ttu-id="99074-125">属性</span><span class="sxs-lookup"><span data-stu-id="99074-125">Property</span></span>     | <span data-ttu-id="99074-126">类型</span><span class="sxs-lookup"><span data-stu-id="99074-126">Type</span></span>   |<span data-ttu-id="99074-127">说明</span><span class="sxs-lookup"><span data-stu-id="99074-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99074-128">activeChecklistItemCount</span><span class="sxs-lookup"><span data-stu-id="99074-128">activeChecklistItemCount</span></span>|<span data-ttu-id="99074-129">Int32</span><span class="sxs-lookup"><span data-stu-id="99074-129">Int32</span></span>|<span data-ttu-id="99074-130">核对清单项的数量，其值设置为 `false`，表示项目不全。</span><span class="sxs-lookup"><span data-stu-id="99074-130">Number of checklist items with value set to `false`, representing incomplete items.</span></span>|
|<span data-ttu-id="99074-131">appliedCategories</span><span class="sxs-lookup"><span data-stu-id="99074-131">appliedCategories</span></span>|[<span data-ttu-id="99074-132">plannerAppliedCategories</span><span class="sxs-lookup"><span data-stu-id="99074-132">plannerAppliedCategories</span></span>](plannerappliedcategories.md)|<span data-ttu-id="99074-p103">此任务已应用的类别。有关可能的值，请参阅[已应用的类别](plannerappliedcategories.md)。</span><span class="sxs-lookup"><span data-stu-id="99074-p103">The categories to which the task has been applied. See [applied Categories](plannerappliedcategories.md) for possible values.</span></span>|
|<span data-ttu-id="99074-135">assigneePriority</span><span class="sxs-lookup"><span data-stu-id="99074-135">assigneePriority</span></span>|<span data-ttu-id="99074-136">String</span><span class="sxs-lookup"><span data-stu-id="99074-136">String</span></span>|<span data-ttu-id="99074-p104">用于为列表视图中的此类型项目排序的提示。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="99074-p104">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="99074-139">assignments</span><span class="sxs-lookup"><span data-stu-id="99074-139">assignments</span></span>|[<span data-ttu-id="99074-140">plannerAssignments</span><span class="sxs-lookup"><span data-stu-id="99074-140">plannerAssignments</span></span>](plannerassignments.md)|<span data-ttu-id="99074-141">被分配任务的接受者集合。</span><span class="sxs-lookup"><span data-stu-id="99074-141">The set of assignees the task is assigned to.</span></span>|
|<span data-ttu-id="99074-142">bucketId</span><span class="sxs-lookup"><span data-stu-id="99074-142">bucketId</span></span>|<span data-ttu-id="99074-143">String</span><span class="sxs-lookup"><span data-stu-id="99074-143">String</span></span>|<span data-ttu-id="99074-144">此任务所属的存储桶 ID。</span><span class="sxs-lookup"><span data-stu-id="99074-144">Bucket ID to which the task belongs.</span></span> <span data-ttu-id="99074-145">存储桶需要位于任务所在的计划中。</span><span class="sxs-lookup"><span data-stu-id="99074-145">The bucket needs to be in the plan that the task is in.</span></span> <span data-ttu-id="99074-146">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="99074-146">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="99074-147">[格式验证](tasks-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="99074-147">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span> |
|<span data-ttu-id="99074-148">checklistItemCount</span><span class="sxs-lookup"><span data-stu-id="99074-148">checklistItemCount</span></span>|<span data-ttu-id="99074-149">Int32</span><span class="sxs-lookup"><span data-stu-id="99074-149">Int32</span></span>|<span data-ttu-id="99074-150">任务上存在的核对清单项的数目。</span><span class="sxs-lookup"><span data-stu-id="99074-150">Number of checklist items that are present on the task.</span></span>|
|<span data-ttu-id="99074-151">completedBy</span><span class="sxs-lookup"><span data-stu-id="99074-151">completedBy</span></span>|[<span data-ttu-id="99074-152">identitySet</span><span class="sxs-lookup"><span data-stu-id="99074-152">identitySet</span></span>](identityset.md)|<span data-ttu-id="99074-153">完成任务的用户的身份。</span><span class="sxs-lookup"><span data-stu-id="99074-153">Identity of the user that completed the task.</span></span>|
|<span data-ttu-id="99074-154">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="99074-154">completedDateTime</span></span>|<span data-ttu-id="99074-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99074-155">DateTimeOffset</span></span>|<span data-ttu-id="99074-p106">只读。任务的 `'percentComplete'` 被设置为 `'100'` 的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="99074-p106">Read-only. Date and time at which the `'percentComplete'` of the task is set to `'100'`. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="99074-160">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="99074-160">conversationThreadId</span></span>|<span data-ttu-id="99074-161">字符串</span><span class="sxs-lookup"><span data-stu-id="99074-161">String</span></span>|<span data-ttu-id="99074-p107">关于任务的对话的线程 ID。此为在组中创建的对话线程对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="99074-p107">Thread ID of the conversation on the task. This is the ID of the conversation thread object created in the group.</span></span>|
|<span data-ttu-id="99074-164">createdBy</span><span class="sxs-lookup"><span data-stu-id="99074-164">createdBy</span></span>|[<span data-ttu-id="99074-165">identitySet</span><span class="sxs-lookup"><span data-stu-id="99074-165">identitySet</span></span>](identityset.md)|<span data-ttu-id="99074-166">创建任务的用户的身份</span><span class="sxs-lookup"><span data-stu-id="99074-166">Identity of the user that created the task.</span></span>|
|<span data-ttu-id="99074-167">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="99074-167">createdDateTime</span></span>|<span data-ttu-id="99074-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99074-168">DateTimeOffset</span></span>|<span data-ttu-id="99074-p108">只读。创建任务的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="99074-p108">Read-only. Date and time at which the task is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="99074-173">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="99074-173">dueDateTime</span></span>|<span data-ttu-id="99074-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99074-174">DateTimeOffset</span></span>|<span data-ttu-id="99074-p109">任务截止的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="99074-p109">Date and time at which the task is due. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="99074-178">hasDescription</span><span class="sxs-lookup"><span data-stu-id="99074-178">hasDescription</span></span>|<span data-ttu-id="99074-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="99074-179">Boolean</span></span>|<span data-ttu-id="99074-p110">只读。如果任务的 details 对象具有非空的说明，则值为 `true`，否则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="99074-p110">Read-only. Value is `true` if the details object of the task has a non-empty description and `false` otherwise.</span></span>|
|<span data-ttu-id="99074-182">id</span><span class="sxs-lookup"><span data-stu-id="99074-182">id</span></span>|<span data-ttu-id="99074-183">String</span><span class="sxs-lookup"><span data-stu-id="99074-183">String</span></span>|<span data-ttu-id="99074-184">只读。</span><span class="sxs-lookup"><span data-stu-id="99074-184">Read-only.</span></span> <span data-ttu-id="99074-185">任务的 ID。</span><span class="sxs-lookup"><span data-stu-id="99074-185">ID of the task.</span></span> <span data-ttu-id="99074-186">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="99074-186">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="99074-187">[格式验证](tasks-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="99074-187">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="99074-188">orderHint</span><span class="sxs-lookup"><span data-stu-id="99074-188">orderHint</span></span>|<span data-ttu-id="99074-189">String</span><span class="sxs-lookup"><span data-stu-id="99074-189">String</span></span>|<span data-ttu-id="99074-p112">用于为列表视图中的此类型项目排序的提示。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="99074-p112">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="99074-192">percentComplete</span><span class="sxs-lookup"><span data-stu-id="99074-192">percentComplete</span></span>|<span data-ttu-id="99074-193">Int32</span><span class="sxs-lookup"><span data-stu-id="99074-193">Int32</span></span>|<span data-ttu-id="99074-p113">任务完成的百分比。当设置为 `100` 时，任务被视为完成。</span><span class="sxs-lookup"><span data-stu-id="99074-p113">Percentage of task completion. When set to `100`, the task is considered completed.</span></span> |
|<span data-ttu-id="99074-196">planId</span><span class="sxs-lookup"><span data-stu-id="99074-196">planId</span></span>|<span data-ttu-id="99074-197">String</span><span class="sxs-lookup"><span data-stu-id="99074-197">String</span></span>|<span data-ttu-id="99074-198">任务所属的计划 ID。</span><span class="sxs-lookup"><span data-stu-id="99074-198">Plan ID to which the task belongs.</span></span>|
|<span data-ttu-id="99074-199">previewType</span><span class="sxs-lookup"><span data-stu-id="99074-199">previewType</span></span>|<span data-ttu-id="99074-200">String</span><span class="sxs-lookup"><span data-stu-id="99074-200">String</span></span>|<span data-ttu-id="99074-201">这将设置显示在任务上的预览类型。</span><span class="sxs-lookup"><span data-stu-id="99074-201">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="99074-202">可取值为：`automatic`、`noPreview`、`checklist`、`description`、`reference`。</span><span class="sxs-lookup"><span data-stu-id="99074-202">Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span>|
|<span data-ttu-id="99074-203">referenceCount</span><span class="sxs-lookup"><span data-stu-id="99074-203">referenceCount</span></span>|<span data-ttu-id="99074-204">Int32</span><span class="sxs-lookup"><span data-stu-id="99074-204">Int32</span></span>|<span data-ttu-id="99074-205">任务上存在的外部引用的数量。</span><span class="sxs-lookup"><span data-stu-id="99074-205">Number of external references that exist on the task.</span></span>|
|<span data-ttu-id="99074-206">startDateTime</span><span class="sxs-lookup"><span data-stu-id="99074-206">startDateTime</span></span>|<span data-ttu-id="99074-207">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99074-207">DateTimeOffset</span></span>|<span data-ttu-id="99074-p115">任务开始的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="99074-p115">Date and time at which the task starts. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="99074-211">title</span><span class="sxs-lookup"><span data-stu-id="99074-211">title</span></span>|<span data-ttu-id="99074-212">String</span><span class="sxs-lookup"><span data-stu-id="99074-212">String</span></span>|<span data-ttu-id="99074-213">任务的标题。</span><span class="sxs-lookup"><span data-stu-id="99074-213">Title of the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99074-214">关系</span><span class="sxs-lookup"><span data-stu-id="99074-214">Relationships</span></span>
| <span data-ttu-id="99074-215">关系</span><span class="sxs-lookup"><span data-stu-id="99074-215">Relationship</span></span> | <span data-ttu-id="99074-216">类型</span><span class="sxs-lookup"><span data-stu-id="99074-216">Type</span></span>   |<span data-ttu-id="99074-217">说明</span><span class="sxs-lookup"><span data-stu-id="99074-217">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99074-218">assignedToTaskBoardFormat</span><span class="sxs-lookup"><span data-stu-id="99074-218">assignedToTaskBoardFormat</span></span>|[<span data-ttu-id="99074-219">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="99074-219">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)| <span data-ttu-id="99074-p116">只读。可为 NULL。用于在按 assignedTo 分组时在任务板视图中正确呈现任务。</span><span class="sxs-lookup"><span data-stu-id="99074-p116">Read-only. Nullable. Used to render the task correctly in the task board view when grouped by assignedTo.</span></span>|
|<span data-ttu-id="99074-223">bucketTaskBoardFormat</span><span class="sxs-lookup"><span data-stu-id="99074-223">bucketTaskBoardFormat</span></span>|[<span data-ttu-id="99074-224">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="99074-224">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)| <span data-ttu-id="99074-p117">只读。可为 NULL。用于在按存储桶分组时在任务板视图中正确呈现任务。</span><span class="sxs-lookup"><span data-stu-id="99074-p117">Read-only. Nullable. Used to render the task correctly in the task board view when grouped by bucket.</span></span>|
|<span data-ttu-id="99074-228">详细信息</span><span class="sxs-lookup"><span data-stu-id="99074-228">details</span></span>|[<span data-ttu-id="99074-229">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="99074-229">plannerTaskDetails</span></span>](plannertaskdetails.md)| <span data-ttu-id="99074-p118">只读。可为 NULL。关于任务的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="99074-p118">Read-only. Nullable. Additional details about the task.</span></span>|
|<span data-ttu-id="99074-233">progressTaskBoardFormat</span><span class="sxs-lookup"><span data-stu-id="99074-233">progressTaskBoardFormat</span></span>|[<span data-ttu-id="99074-234">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="99074-234">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)| <span data-ttu-id="99074-p119">只读。可为 NULL。用于在按进度分组时在任务板视图中正确呈现任务。</span><span class="sxs-lookup"><span data-stu-id="99074-p119">Read-only. Nullable. Used to render the task correctly in the task board view when grouped by progress.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="99074-238">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="99074-238">JSON representation</span></span>
<span data-ttu-id="99074-239">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99074-239">Here is a JSON representation of the resource.</span></span>

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
