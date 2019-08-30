---
title: plannerTask 资源类型
description: '**plannerTask** 资源表示 Office 365 中的规划器任务。规划器任务包含在计划内，可以分配给计划中的存储桶。每个任务对象具有可以包含此任务的更多信息的 details 对象。请参阅概述了解有关组、计划和任务之间的关系的详细信息。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 9ced498b9bc56d8f21f96ede67d1a9a6501ddb21
ms.sourcegitcommit: cca4f96414aededa03bb45e07e19bb20b7327563
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2019
ms.locfileid: "36677174"
---
# <a name="plannertask-resource-type"></a><span data-ttu-id="2dd20-106">plannerTask 资源类型</span><span class="sxs-lookup"><span data-stu-id="2dd20-106">plannerTask resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2dd20-p102">**plannerTask** 资源表示 Office 365 中的规划器任务。规划器任务包含在[计划](plannerplan.md)内，可以分配给计划中的[存储桶](plannerbucket.md)。每个任务对象具有可以包含此任务的更多信息的 [details](plannertaskdetails.md) 对象。请参阅[概述](planner-overview.md)了解有关组、计划和任务之间的关系的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2dd20-p102">The **plannerTask** resource represents a Planner task in Office 365. A Planner task is contained in a [plan](plannerplan.md) and can be assigned to a [bucket](plannerbucket.md) in a plan. Each task object has a [details](plannertaskdetails.md) object which can contain more information about the task. See [overview](planner-overview.md) for more information regarding relationships between group, plan and task.</span></span>


## <a name="methods"></a><span data-ttu-id="2dd20-111">方法</span><span class="sxs-lookup"><span data-stu-id="2dd20-111">Methods</span></span>

| <span data-ttu-id="2dd20-112">方法</span><span class="sxs-lookup"><span data-stu-id="2dd20-112">Method</span></span>           | <span data-ttu-id="2dd20-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="2dd20-113">Return Type</span></span>    |<span data-ttu-id="2dd20-114">说明</span><span class="sxs-lookup"><span data-stu-id="2dd20-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2dd20-115">获取 plannerTask</span><span class="sxs-lookup"><span data-stu-id="2dd20-115">Get plannerTask</span></span>](../api/plannertask-get.md) | [<span data-ttu-id="2dd20-116">plannerTask</span><span class="sxs-lookup"><span data-stu-id="2dd20-116">plannerTask</span></span>](plannertask.md) |<span data-ttu-id="2dd20-117">读取 **plannerTask** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2dd20-117">Read properties and relationships of **plannerTask** object.</span></span>|
|[<span data-ttu-id="2dd20-118">更新</span><span class="sxs-lookup"><span data-stu-id="2dd20-118">Update</span></span>](../api/plannertask-update.md) | [<span data-ttu-id="2dd20-119">plannerTask</span><span class="sxs-lookup"><span data-stu-id="2dd20-119">plannerTask</span></span>](plannertask.md) |<span data-ttu-id="2dd20-120">更新 **plannerTask** 对象。</span><span class="sxs-lookup"><span data-stu-id="2dd20-120">Update **plannerTask** object.</span></span> |
|[<span data-ttu-id="2dd20-121">删除</span><span class="sxs-lookup"><span data-stu-id="2dd20-121">Delete</span></span>](../api/plannertask-delete.md) | <span data-ttu-id="2dd20-122">无</span><span class="sxs-lookup"><span data-stu-id="2dd20-122">None</span></span> |<span data-ttu-id="2dd20-123">删除 **plannerTask** 对象。</span><span class="sxs-lookup"><span data-stu-id="2dd20-123">Delete **plannerTask** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2dd20-124">属性</span><span class="sxs-lookup"><span data-stu-id="2dd20-124">Properties</span></span>
| <span data-ttu-id="2dd20-125">属性</span><span class="sxs-lookup"><span data-stu-id="2dd20-125">Property</span></span>     | <span data-ttu-id="2dd20-126">类型</span><span class="sxs-lookup"><span data-stu-id="2dd20-126">Type</span></span>   |<span data-ttu-id="2dd20-127">说明</span><span class="sxs-lookup"><span data-stu-id="2dd20-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2dd20-128">activeChecklistItemCount</span><span class="sxs-lookup"><span data-stu-id="2dd20-128">activeChecklistItemCount</span></span>|<span data-ttu-id="2dd20-129">Int32</span><span class="sxs-lookup"><span data-stu-id="2dd20-129">Int32</span></span>|<span data-ttu-id="2dd20-130">核对清单项的数量，其值设置为 `false`，表示项目不全。</span><span class="sxs-lookup"><span data-stu-id="2dd20-130">Number of checklist items with value set to `false`, representing incomplete items.</span></span>|
|<span data-ttu-id="2dd20-131">appliedCategories</span><span class="sxs-lookup"><span data-stu-id="2dd20-131">appliedCategories</span></span>|[<span data-ttu-id="2dd20-132">plannerAppliedCategories</span><span class="sxs-lookup"><span data-stu-id="2dd20-132">plannerAppliedCategories</span></span>](plannerappliedcategories.md)|<span data-ttu-id="2dd20-p103">此任务已应用的类别。有关可能的值，请参阅[已应用的类别](plannerappliedcategories.md)。</span><span class="sxs-lookup"><span data-stu-id="2dd20-p103">The categories to which the task has been applied. See [applied Categories](plannerappliedcategories.md) for possible values.</span></span>|
|<span data-ttu-id="2dd20-135">assigneePriority</span><span class="sxs-lookup"><span data-stu-id="2dd20-135">assigneePriority</span></span>|<span data-ttu-id="2dd20-136">String</span><span class="sxs-lookup"><span data-stu-id="2dd20-136">String</span></span>|<span data-ttu-id="2dd20-p104">用于为列表视图中的此类型项目排序的提示。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="2dd20-p104">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="2dd20-139">assignments</span><span class="sxs-lookup"><span data-stu-id="2dd20-139">assignments</span></span>|[<span data-ttu-id="2dd20-140">plannerAssignments</span><span class="sxs-lookup"><span data-stu-id="2dd20-140">plannerAssignments</span></span>](plannerassignments.md)|<span data-ttu-id="2dd20-141">被分配任务的接受者集合。</span><span class="sxs-lookup"><span data-stu-id="2dd20-141">The set of assignees the task is assigned to.</span></span>|
|<span data-ttu-id="2dd20-142">bucketId</span><span class="sxs-lookup"><span data-stu-id="2dd20-142">bucketId</span></span>|<span data-ttu-id="2dd20-143">String</span><span class="sxs-lookup"><span data-stu-id="2dd20-143">String</span></span>|<span data-ttu-id="2dd20-144">此任务所属的存储桶 ID。</span><span class="sxs-lookup"><span data-stu-id="2dd20-144">Bucket ID to which the task belongs.</span></span> <span data-ttu-id="2dd20-145">存储桶需要位于任务所在的计划中。</span><span class="sxs-lookup"><span data-stu-id="2dd20-145">The bucket needs to be in the plan that the task is in.</span></span> <span data-ttu-id="2dd20-146">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="2dd20-146">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="2dd20-147">[格式验证](tasks-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="2dd20-147">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span> |
|<span data-ttu-id="2dd20-148">checklistItemCount</span><span class="sxs-lookup"><span data-stu-id="2dd20-148">checklistItemCount</span></span>|<span data-ttu-id="2dd20-149">Int32</span><span class="sxs-lookup"><span data-stu-id="2dd20-149">Int32</span></span>|<span data-ttu-id="2dd20-150">任务上存在的核对清单项的数目。</span><span class="sxs-lookup"><span data-stu-id="2dd20-150">Number of checklist items that are present on the task.</span></span>|
|<span data-ttu-id="2dd20-151">completedBy</span><span class="sxs-lookup"><span data-stu-id="2dd20-151">completedBy</span></span>|[<span data-ttu-id="2dd20-152">identitySet</span><span class="sxs-lookup"><span data-stu-id="2dd20-152">identitySet</span></span>](identityset.md)|<span data-ttu-id="2dd20-153">完成任务的用户的身份。</span><span class="sxs-lookup"><span data-stu-id="2dd20-153">Identity of the user that completed the task.</span></span>|
|<span data-ttu-id="2dd20-154">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="2dd20-154">completedDateTime</span></span>|<span data-ttu-id="2dd20-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2dd20-155">DateTimeOffset</span></span>|<span data-ttu-id="2dd20-p106">只读。任务的 `'percentComplete'` 被设置为 `'100'` 的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2dd20-p106">Read-only. Date and time at which the `'percentComplete'` of the task is set to `'100'`. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="2dd20-160">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="2dd20-160">conversationThreadId</span></span>|<span data-ttu-id="2dd20-161">字符串</span><span class="sxs-lookup"><span data-stu-id="2dd20-161">String</span></span>|<span data-ttu-id="2dd20-p107">关于任务的对话的线程 ID。此为在组中创建的对话线程对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="2dd20-p107">Thread ID of the conversation on the task. This is the ID of the conversation thread object created in the group.</span></span>|
|<span data-ttu-id="2dd20-164">createdBy</span><span class="sxs-lookup"><span data-stu-id="2dd20-164">createdBy</span></span>|[<span data-ttu-id="2dd20-165">identitySet</span><span class="sxs-lookup"><span data-stu-id="2dd20-165">identitySet</span></span>](identityset.md)|<span data-ttu-id="2dd20-166">创建任务的用户的身份</span><span class="sxs-lookup"><span data-stu-id="2dd20-166">Identity of the user that created the task.</span></span>|
|<span data-ttu-id="2dd20-167">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2dd20-167">createdDateTime</span></span>|<span data-ttu-id="2dd20-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2dd20-168">DateTimeOffset</span></span>|<span data-ttu-id="2dd20-p108">只读。创建任务的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2dd20-p108">Read-only. Date and time at which the task is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="2dd20-173">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="2dd20-173">dueDateTime</span></span>|<span data-ttu-id="2dd20-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2dd20-174">DateTimeOffset</span></span>|<span data-ttu-id="2dd20-p109">任务截止的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2dd20-p109">Date and time at which the task is due. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="2dd20-178">hasDescription</span><span class="sxs-lookup"><span data-stu-id="2dd20-178">hasDescription</span></span>|<span data-ttu-id="2dd20-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="2dd20-179">Boolean</span></span>|<span data-ttu-id="2dd20-p110">只读。如果任务的 details 对象具有非空的说明，则值为 `true`，否则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="2dd20-p110">Read-only. Value is `true` if the details object of the task has a non-empty description and `false` otherwise.</span></span>|
|<span data-ttu-id="2dd20-182">id</span><span class="sxs-lookup"><span data-stu-id="2dd20-182">id</span></span>|<span data-ttu-id="2dd20-183">String</span><span class="sxs-lookup"><span data-stu-id="2dd20-183">String</span></span>|<span data-ttu-id="2dd20-184">只读。</span><span class="sxs-lookup"><span data-stu-id="2dd20-184">Read-only.</span></span> <span data-ttu-id="2dd20-185">任务的 ID。</span><span class="sxs-lookup"><span data-stu-id="2dd20-185">ID of the task.</span></span> <span data-ttu-id="2dd20-186">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="2dd20-186">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="2dd20-187">[格式验证](tasks-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="2dd20-187">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="2dd20-188">orderHint</span><span class="sxs-lookup"><span data-stu-id="2dd20-188">orderHint</span></span>|<span data-ttu-id="2dd20-189">String</span><span class="sxs-lookup"><span data-stu-id="2dd20-189">String</span></span>|<span data-ttu-id="2dd20-p112">用于为列表视图中的此类型项目排序的提示。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="2dd20-p112">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="2dd20-192">percentComplete</span><span class="sxs-lookup"><span data-stu-id="2dd20-192">percentComplete</span></span>|<span data-ttu-id="2dd20-193">Int32</span><span class="sxs-lookup"><span data-stu-id="2dd20-193">Int32</span></span>|<span data-ttu-id="2dd20-p113">任务完成的百分比。当设置为 `100` 时，任务被视为完成。</span><span class="sxs-lookup"><span data-stu-id="2dd20-p113">Percentage of task completion. When set to `100`, the task is considered completed.</span></span> |
|<span data-ttu-id="2dd20-196">priority</span><span class="sxs-lookup"><span data-stu-id="2dd20-196">priority</span></span>|<span data-ttu-id="2dd20-197">Int32</span><span class="sxs-lookup"><span data-stu-id="2dd20-197">Int32</span></span>|<span data-ttu-id="2dd20-198">任务的优先级。</span><span class="sxs-lookup"><span data-stu-id="2dd20-198">Priority of the task.</span></span> <span data-ttu-id="2dd20-199">值的有效范围介于和`0` ( `10`含) 之间, 并且值越低, 优先级越`0`低 (具有最高`10`优先级, 优先级最低)。</span><span class="sxs-lookup"><span data-stu-id="2dd20-199">Valid range of values is between `0` and `10` (inclusive), with increasing value being lower priority (`0` has the highest priority and `10` has the lowest priority).</span></span>  <span data-ttu-id="2dd20-200">目前, 规划者将`0`值`1`和 "紧急", `2` `3` `4` `5`以及 "重要"、、 `6` `7` 、、和 "低" 的`8` `9` `10`值解释为 "中"。</span><span class="sxs-lookup"><span data-stu-id="2dd20-200">Currently, Planner interprets values `0` and `1` as "urgent", `2` and `3` and `4` as "important", `5`, `6`, and `7` as "medium", and `8`, `9`, and `10` as "low".</span></span>  <span data-ttu-id="2dd20-201">目前, 规划器将设置`1` "紧急"、 `3` "重要" `5` 、"中" 和`9` "低" 的值。</span><span class="sxs-lookup"><span data-stu-id="2dd20-201">Currently, Planner sets the value `1` for "urgent", `3` for "important", `5` for "medium", and `9` for "low".</span></span>|
|<span data-ttu-id="2dd20-202">planId</span><span class="sxs-lookup"><span data-stu-id="2dd20-202">planId</span></span>|<span data-ttu-id="2dd20-203">String</span><span class="sxs-lookup"><span data-stu-id="2dd20-203">String</span></span>|<span data-ttu-id="2dd20-204">任务所属的计划 ID。</span><span class="sxs-lookup"><span data-stu-id="2dd20-204">Plan ID to which the task belongs.</span></span>|
|<span data-ttu-id="2dd20-205">previewType</span><span class="sxs-lookup"><span data-stu-id="2dd20-205">previewType</span></span>|<span data-ttu-id="2dd20-206">String</span><span class="sxs-lookup"><span data-stu-id="2dd20-206">String</span></span>|<span data-ttu-id="2dd20-207">这将设置显示在任务上的预览类型。</span><span class="sxs-lookup"><span data-stu-id="2dd20-207">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="2dd20-208">可取值为：`automatic`、`noPreview`、`checklist`、`description`、`reference`。</span><span class="sxs-lookup"><span data-stu-id="2dd20-208">Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span>|
|<span data-ttu-id="2dd20-209">referenceCount</span><span class="sxs-lookup"><span data-stu-id="2dd20-209">referenceCount</span></span>|<span data-ttu-id="2dd20-210">Int32</span><span class="sxs-lookup"><span data-stu-id="2dd20-210">Int32</span></span>|<span data-ttu-id="2dd20-211">任务上存在的外部引用的数量。</span><span class="sxs-lookup"><span data-stu-id="2dd20-211">Number of external references that exist on the task.</span></span>|
|<span data-ttu-id="2dd20-212">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2dd20-212">startDateTime</span></span>|<span data-ttu-id="2dd20-213">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2dd20-213">DateTimeOffset</span></span>|<span data-ttu-id="2dd20-p116">任务开始的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2dd20-p116">Date and time at which the task starts. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="2dd20-217">title</span><span class="sxs-lookup"><span data-stu-id="2dd20-217">title</span></span>|<span data-ttu-id="2dd20-218">String</span><span class="sxs-lookup"><span data-stu-id="2dd20-218">String</span></span>|<span data-ttu-id="2dd20-219">任务的标题。</span><span class="sxs-lookup"><span data-stu-id="2dd20-219">Title of the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2dd20-220">关系</span><span class="sxs-lookup"><span data-stu-id="2dd20-220">Relationships</span></span>
| <span data-ttu-id="2dd20-221">关系</span><span class="sxs-lookup"><span data-stu-id="2dd20-221">Relationship</span></span> | <span data-ttu-id="2dd20-222">类型</span><span class="sxs-lookup"><span data-stu-id="2dd20-222">Type</span></span>   |<span data-ttu-id="2dd20-223">说明</span><span class="sxs-lookup"><span data-stu-id="2dd20-223">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2dd20-224">assignedToTaskBoardFormat</span><span class="sxs-lookup"><span data-stu-id="2dd20-224">assignedToTaskBoardFormat</span></span>|[<span data-ttu-id="2dd20-225">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="2dd20-225">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)| <span data-ttu-id="2dd20-p117">只读。可为 NULL。用于在按 assignedTo 分组时在任务板视图中正确呈现任务。</span><span class="sxs-lookup"><span data-stu-id="2dd20-p117">Read-only. Nullable. Used to render the task correctly in the task board view when grouped by assignedTo.</span></span>|
|<span data-ttu-id="2dd20-229">bucketTaskBoardFormat</span><span class="sxs-lookup"><span data-stu-id="2dd20-229">bucketTaskBoardFormat</span></span>|[<span data-ttu-id="2dd20-230">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="2dd20-230">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)| <span data-ttu-id="2dd20-p118">只读。可为 NULL。用于在按存储桶分组时在任务板视图中正确呈现任务。</span><span class="sxs-lookup"><span data-stu-id="2dd20-p118">Read-only. Nullable. Used to render the task correctly in the task board view when grouped by bucket.</span></span>|
|<span data-ttu-id="2dd20-234">详细信息</span><span class="sxs-lookup"><span data-stu-id="2dd20-234">details</span></span>|[<span data-ttu-id="2dd20-235">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="2dd20-235">plannerTaskDetails</span></span>](plannertaskdetails.md)| <span data-ttu-id="2dd20-p119">只读。可为 NULL。关于任务的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="2dd20-p119">Read-only. Nullable. Additional details about the task.</span></span>|
|<span data-ttu-id="2dd20-239">progressTaskBoardFormat</span><span class="sxs-lookup"><span data-stu-id="2dd20-239">progressTaskBoardFormat</span></span>|[<span data-ttu-id="2dd20-240">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="2dd20-240">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)| <span data-ttu-id="2dd20-p120">只读。可为 NULL。用于在按进度分组时在任务板视图中正确呈现任务。</span><span class="sxs-lookup"><span data-stu-id="2dd20-p120">Read-only. Nullable. Used to render the task correctly in the task board view when grouped by progress.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2dd20-244">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2dd20-244">JSON representation</span></span>
<span data-ttu-id="2dd20-245">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2dd20-245">Here is a JSON representation of the resource.</span></span>

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
