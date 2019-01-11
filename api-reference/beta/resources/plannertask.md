---
title: plannerTask 资源类型
description: '**plannerTask** 资源表示 Office 365 中的规划器任务。规划器任务包含在计划内，可以分配给计划中的存储桶。每个任务对象具有可以包含此任务的更多信息的 details 对象。请参阅概述了解有关组、计划和任务之间的关系的详细信息。'
localization_priority: Normal
ms.openlocfilehash: d52dc1311ca17c4473b1971b9aafb3c04f36cd54
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849411"
---
# <a name="plannertask-resource-type"></a><span data-ttu-id="5db19-106">plannerTask 资源类型</span><span class="sxs-lookup"><span data-stu-id="5db19-106">plannerTask resource type</span></span>

> <span data-ttu-id="5db19-107">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5db19-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5db19-108">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5db19-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5db19-p103">**plannerTask** 资源表示 Office 365 中的规划器任务。规划器任务包含在[计划](plannerplan.md)内，可以分配给计划中的[存储桶](plannerbucket.md)。每个任务对象具有可以包含此任务的更多信息的 [details](plannertaskdetails.md) 对象。请参阅[概述](planner-overview.md)了解有关组、计划和任务之间的关系的详细信息。</span><span class="sxs-lookup"><span data-stu-id="5db19-p103">The **plannerTask** resource represents a Planner task in Office 365. A Planner task is contained in a [plan](plannerplan.md) and can be assigned to a [bucket](plannerbucket.md) in a plan. Each task object has a [details](plannertaskdetails.md) object which can contain more information about the task. See [overview](planner-overview.md) for more information regarding relationships between group, plan and task.</span></span>


## <a name="methods"></a><span data-ttu-id="5db19-113">方法</span><span class="sxs-lookup"><span data-stu-id="5db19-113">Methods</span></span>

| <span data-ttu-id="5db19-114">方法</span><span class="sxs-lookup"><span data-stu-id="5db19-114">Method</span></span>           | <span data-ttu-id="5db19-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="5db19-115">Return Type</span></span>    |<span data-ttu-id="5db19-116">说明</span><span class="sxs-lookup"><span data-stu-id="5db19-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5db19-117">获取 plannerTask</span><span class="sxs-lookup"><span data-stu-id="5db19-117">Get plannerTask</span></span>](../api/plannertask-get.md) | [<span data-ttu-id="5db19-118">plannerTask</span><span class="sxs-lookup"><span data-stu-id="5db19-118">plannerTask</span></span>](plannertask.md) |<span data-ttu-id="5db19-119">读取 **plannerTask** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5db19-119">Read properties and relationships of **plannerTask** object.</span></span>|
|[<span data-ttu-id="5db19-120">更新</span><span class="sxs-lookup"><span data-stu-id="5db19-120">Update</span></span>](../api/plannertask-update.md) | [<span data-ttu-id="5db19-121">plannerTask</span><span class="sxs-lookup"><span data-stu-id="5db19-121">plannerTask</span></span>](plannertask.md) |<span data-ttu-id="5db19-122">更新 **plannerTask** 对象。</span><span class="sxs-lookup"><span data-stu-id="5db19-122">Update **plannerTask** object.</span></span> |
|[<span data-ttu-id="5db19-123">删除</span><span class="sxs-lookup"><span data-stu-id="5db19-123">Delete</span></span>](../api/plannertask-delete.md) | <span data-ttu-id="5db19-124">无</span><span class="sxs-lookup"><span data-stu-id="5db19-124">None</span></span> |<span data-ttu-id="5db19-125">删除 **plannerTask** 对象。</span><span class="sxs-lookup"><span data-stu-id="5db19-125">Delete **plannerTask** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5db19-126">属性</span><span class="sxs-lookup"><span data-stu-id="5db19-126">Properties</span></span>
| <span data-ttu-id="5db19-127">属性</span><span class="sxs-lookup"><span data-stu-id="5db19-127">Property</span></span>     | <span data-ttu-id="5db19-128">类型</span><span class="sxs-lookup"><span data-stu-id="5db19-128">Type</span></span>   |<span data-ttu-id="5db19-129">说明</span><span class="sxs-lookup"><span data-stu-id="5db19-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5db19-130">activeChecklistItemCount</span><span class="sxs-lookup"><span data-stu-id="5db19-130">activeChecklistItemCount</span></span>|<span data-ttu-id="5db19-131">Int32</span><span class="sxs-lookup"><span data-stu-id="5db19-131">Int32</span></span>|<span data-ttu-id="5db19-132">核对清单项的数量，其值设置为“false”，表示项目不全。</span><span class="sxs-lookup"><span data-stu-id="5db19-132">Number of checklist items with value set to 'false', representing incomplete items.</span></span>|
|<span data-ttu-id="5db19-133">appliedCategories</span><span class="sxs-lookup"><span data-stu-id="5db19-133">appliedCategories</span></span>|[<span data-ttu-id="5db19-134">plannerAppliedCategories</span><span class="sxs-lookup"><span data-stu-id="5db19-134">plannerAppliedCategories</span></span>](plannerappliedcategories.md)|<span data-ttu-id="5db19-p104">此任务已应用的类别。有关可能的值，请参阅[已应用的类别](plannerappliedcategories.md)。</span><span class="sxs-lookup"><span data-stu-id="5db19-p104">The categories to which the task has been applied. See [applied Categories](plannerappliedcategories.md) for possible values.</span></span>|
|<span data-ttu-id="5db19-137">assigneePriority</span><span class="sxs-lookup"><span data-stu-id="5db19-137">assigneePriority</span></span>|<span data-ttu-id="5db19-138">String</span><span class="sxs-lookup"><span data-stu-id="5db19-138">String</span></span>|<span data-ttu-id="5db19-p105">提示用于为列表视图中的此类项目排序。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="5db19-p105">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="5db19-141">assignments</span><span class="sxs-lookup"><span data-stu-id="5db19-141">assignments</span></span>|[<span data-ttu-id="5db19-142">plannerAssignments</span><span class="sxs-lookup"><span data-stu-id="5db19-142">plannerAssignments</span></span>](plannerassignments.md)|<span data-ttu-id="5db19-143">被分配任务的接受者集合。</span><span class="sxs-lookup"><span data-stu-id="5db19-143">The set of assignees the task is assigned to.</span></span>|
|<span data-ttu-id="5db19-144">bucketId</span><span class="sxs-lookup"><span data-stu-id="5db19-144">bucketId</span></span>|<span data-ttu-id="5db19-145">字符串</span><span class="sxs-lookup"><span data-stu-id="5db19-145">String</span></span>|<span data-ttu-id="5db19-146">任务所属的地址散列表元 ID。</span><span class="sxs-lookup"><span data-stu-id="5db19-146">Bucket ID to which the task belongs.</span></span> <span data-ttu-id="5db19-147">地址散列表元需要在计划中的任务。</span><span class="sxs-lookup"><span data-stu-id="5db19-147">The bucket needs to be in the plan that the task is in.</span></span> <span data-ttu-id="5db19-148">它是 28 字符长度和区分大小写。</span><span class="sxs-lookup"><span data-stu-id="5db19-148">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="5db19-149">服务上执行[格式验证](tasks-identifiers-disclaimer.md)。</span><span class="sxs-lookup"><span data-stu-id="5db19-149">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span> |
|<span data-ttu-id="5db19-150">checklistItemCount</span><span class="sxs-lookup"><span data-stu-id="5db19-150">checklistItemCount</span></span>|<span data-ttu-id="5db19-151">Int32</span><span class="sxs-lookup"><span data-stu-id="5db19-151">Int32</span></span>|<span data-ttu-id="5db19-152">任务上存在的核对清单项的数目。</span><span class="sxs-lookup"><span data-stu-id="5db19-152">Number of checklist items that are present on the task.</span></span>|
|<span data-ttu-id="5db19-153">completedBy</span><span class="sxs-lookup"><span data-stu-id="5db19-153">completedBy</span></span>|[<span data-ttu-id="5db19-154">identitySet</span><span class="sxs-lookup"><span data-stu-id="5db19-154">identitySet</span></span>](identityset.md)|<span data-ttu-id="5db19-155">完成任务的用户的身份。</span><span class="sxs-lookup"><span data-stu-id="5db19-155">Identity of the user that completed the task.</span></span>|
|<span data-ttu-id="5db19-156">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="5db19-156">completedDateTime</span></span>|<span data-ttu-id="5db19-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5db19-157">DateTimeOffset</span></span>|<span data-ttu-id="5db19-p107">只读。任务的 `'percentComplete'` 被设置为 `'100'` 的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="5db19-p107">Read-only. Date and time at which the `'percentComplete'` of the task is set to `'100'`. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5db19-162">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="5db19-162">conversationThreadId</span></span>|<span data-ttu-id="5db19-163">字符串</span><span class="sxs-lookup"><span data-stu-id="5db19-163">String</span></span>|<span data-ttu-id="5db19-p108">关于任务的对话的线程 ID。此为在组中创建的对话线程对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="5db19-p108">Thread ID of the conversation on the task. This is the ID of the conversation thread object created in the group.</span></span>|
|<span data-ttu-id="5db19-166">createdBy</span><span class="sxs-lookup"><span data-stu-id="5db19-166">createdBy</span></span>|[<span data-ttu-id="5db19-167">identitySet</span><span class="sxs-lookup"><span data-stu-id="5db19-167">identitySet</span></span>](identityset.md)|<span data-ttu-id="5db19-168">创建任务的用户的身份</span><span class="sxs-lookup"><span data-stu-id="5db19-168">Identity of the user that created the task.</span></span>|
|<span data-ttu-id="5db19-169">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5db19-169">createdDateTime</span></span>|<span data-ttu-id="5db19-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5db19-170">DateTimeOffset</span></span>|<span data-ttu-id="5db19-p109">只读。创建任务的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="5db19-p109">Read-only. Date and time at which the task is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5db19-175">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="5db19-175">dueDateTime</span></span>|<span data-ttu-id="5db19-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5db19-176">DateTimeOffset</span></span>|<span data-ttu-id="5db19-p110">任务截止的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="5db19-p110">Date and time at which the task is due. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5db19-180">hasDescription</span><span class="sxs-lookup"><span data-stu-id="5db19-180">hasDescription</span></span>|<span data-ttu-id="5db19-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="5db19-181">Boolean</span></span>|<span data-ttu-id="5db19-p111">只读。如果任务的 details 对象具有非空的说明，则值为 `true`，否则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="5db19-p111">Read-only. Value is `true` if the details object of the task has a non-empty description and `false` otherwise.</span></span>|
|<span data-ttu-id="5db19-184">id</span><span class="sxs-lookup"><span data-stu-id="5db19-184">id</span></span>|<span data-ttu-id="5db19-185">String</span><span class="sxs-lookup"><span data-stu-id="5db19-185">String</span></span>|<span data-ttu-id="5db19-186">只读。</span><span class="sxs-lookup"><span data-stu-id="5db19-186">Read-only.</span></span> <span data-ttu-id="5db19-187">任务的 ID。</span><span class="sxs-lookup"><span data-stu-id="5db19-187">ID of the task.</span></span> <span data-ttu-id="5db19-188">它是 28 字符长度和区分大小写。</span><span class="sxs-lookup"><span data-stu-id="5db19-188">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="5db19-189">服务上执行[格式验证](tasks-identifiers-disclaimer.md)。</span><span class="sxs-lookup"><span data-stu-id="5db19-189">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="5db19-190">orderHint</span><span class="sxs-lookup"><span data-stu-id="5db19-190">orderHint</span></span>|<span data-ttu-id="5db19-191">String</span><span class="sxs-lookup"><span data-stu-id="5db19-191">String</span></span>|<span data-ttu-id="5db19-p113">提示用于为列表视图中的此类项目排序。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="5db19-p113">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="5db19-194">percentComplete</span><span class="sxs-lookup"><span data-stu-id="5db19-194">percentComplete</span></span>|<span data-ttu-id="5db19-195">Int32</span><span class="sxs-lookup"><span data-stu-id="5db19-195">Int32</span></span>|<span data-ttu-id="5db19-p114">任务完成的百分比。当设置为 `100` 时，任务被视为完成。</span><span class="sxs-lookup"><span data-stu-id="5db19-p114">Percentage of task completion. When set to `100`, the task is considered completed.</span></span> |
|<span data-ttu-id="5db19-198">planId</span><span class="sxs-lookup"><span data-stu-id="5db19-198">planId</span></span>|<span data-ttu-id="5db19-199">String</span><span class="sxs-lookup"><span data-stu-id="5db19-199">String</span></span>|<span data-ttu-id="5db19-200">任务所属的计划 ID。</span><span class="sxs-lookup"><span data-stu-id="5db19-200">Plan ID to which the task belongs.</span></span>|
|<span data-ttu-id="5db19-201">previewType</span><span class="sxs-lookup"><span data-stu-id="5db19-201">previewType</span></span>|<span data-ttu-id="5db19-202">string</span><span class="sxs-lookup"><span data-stu-id="5db19-202">string</span></span>|<span data-ttu-id="5db19-p115">这将设置显示在任务上的预览类型。可能的值是：`automatic`、`noPreview`、`checklist`、`description`、`reference`。</span><span class="sxs-lookup"><span data-stu-id="5db19-p115">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span>|
|<span data-ttu-id="5db19-205">referenceCount</span><span class="sxs-lookup"><span data-stu-id="5db19-205">referenceCount</span></span>|<span data-ttu-id="5db19-206">Int32</span><span class="sxs-lookup"><span data-stu-id="5db19-206">Int32</span></span>|<span data-ttu-id="5db19-207">任务上存在的外部引用的数量。</span><span class="sxs-lookup"><span data-stu-id="5db19-207">Number of external references that exist on the task.</span></span>|
|<span data-ttu-id="5db19-208">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5db19-208">startDateTime</span></span>|<span data-ttu-id="5db19-209">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5db19-209">DateTimeOffset</span></span>|<span data-ttu-id="5db19-p116">任务开始的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="5db19-p116">Date and time at which the task starts. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5db19-213">title</span><span class="sxs-lookup"><span data-stu-id="5db19-213">title</span></span>|<span data-ttu-id="5db19-214">String</span><span class="sxs-lookup"><span data-stu-id="5db19-214">String</span></span>|<span data-ttu-id="5db19-215">任务的标题。</span><span class="sxs-lookup"><span data-stu-id="5db19-215">Title of the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5db19-216">关系</span><span class="sxs-lookup"><span data-stu-id="5db19-216">Relationships</span></span>
| <span data-ttu-id="5db19-217">关系</span><span class="sxs-lookup"><span data-stu-id="5db19-217">Relationship</span></span> | <span data-ttu-id="5db19-218">类型</span><span class="sxs-lookup"><span data-stu-id="5db19-218">Type</span></span>   |<span data-ttu-id="5db19-219">说明</span><span class="sxs-lookup"><span data-stu-id="5db19-219">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5db19-220">assignedToTaskBoardFormat</span><span class="sxs-lookup"><span data-stu-id="5db19-220">assignedToTaskBoardFormat</span></span>|[<span data-ttu-id="5db19-221">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="5db19-221">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)| <span data-ttu-id="5db19-p117">只读。可为 NULL。用于在按 assignedTo 分组时在任务板视图中正确呈现任务。</span><span class="sxs-lookup"><span data-stu-id="5db19-p117">Read-only. Nullable. Used to render the task correctly in the task board view when grouped by assignedTo.</span></span>|
|<span data-ttu-id="5db19-225">bucketTaskBoardFormat</span><span class="sxs-lookup"><span data-stu-id="5db19-225">bucketTaskBoardFormat</span></span>|[<span data-ttu-id="5db19-226">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="5db19-226">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)| <span data-ttu-id="5db19-p118">只读。可为 NULL。用于在按存储桶分组时在任务板视图中正确呈现任务。</span><span class="sxs-lookup"><span data-stu-id="5db19-p118">Read-only. Nullable. Used to render the task correctly in the task board view when grouped by bucket.</span></span>|
|<span data-ttu-id="5db19-230">详细信息</span><span class="sxs-lookup"><span data-stu-id="5db19-230">details</span></span>|[<span data-ttu-id="5db19-231">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="5db19-231">plannerTaskDetails</span></span>](plannertaskdetails.md)| <span data-ttu-id="5db19-p119">只读。可为 NULL。关于任务的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="5db19-p119">Read-only. Nullable. Additional details about the task.</span></span>|
|<span data-ttu-id="5db19-235">progressTaskBoardFormat</span><span class="sxs-lookup"><span data-stu-id="5db19-235">progressTaskBoardFormat</span></span>|[<span data-ttu-id="5db19-236">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="5db19-236">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)| <span data-ttu-id="5db19-p120">只读。可为 NULL。用于在按进度分组时在任务板视图中正确呈现任务。</span><span class="sxs-lookup"><span data-stu-id="5db19-p120">Read-only. Nullable. Used to render the task correctly in the task board view when grouped by progress.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5db19-240">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5db19-240">JSON representation</span></span>
<span data-ttu-id="5db19-241">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5db19-241">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerTask resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
