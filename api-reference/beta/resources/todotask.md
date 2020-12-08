---
title: todoTask 资源类型
description: TodoTask 资源跟踪工作项。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ffcd3da43b7ae165045b545c656035e47d291419
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597198"
---
# <a name="todotask-resource-type"></a><span data-ttu-id="e0b61-103">todoTask 资源类型</span><span class="sxs-lookup"><span data-stu-id="e0b61-103">todoTask resource type</span></span>

<span data-ttu-id="e0b61-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0b61-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0b61-105">**TodoTask** 表示可以跟踪和完成的任务，例如，一段工作或个人项目。</span><span class="sxs-lookup"><span data-stu-id="e0b61-105">A **todoTask** represents a task, such as a piece of work or personal item, that can be tracked and completed.</span></span> 

<span data-ttu-id="e0b61-106">**TodoTask** 始终包含在 [todoTaskList](todotasklist.md)中。</span><span class="sxs-lookup"><span data-stu-id="e0b61-106">A **todoTask** is always contained in a [todoTaskList](todotasklist.md).</span></span> <span data-ttu-id="e0b61-107">它包括与 [linkedResource](./linkedResource.md) 对象集合的关系，并跟踪任务的一个或多个源。</span><span class="sxs-lookup"><span data-stu-id="e0b61-107">It includes a relationship to a collection of [linkedResource](./linkedResource.md) objects, tracking one or more sources of the task.</span></span>

<span data-ttu-id="e0b61-108">此资源支持以下内容：</span><span class="sxs-lookup"><span data-stu-id="e0b61-108">This resource supports the following:</span></span>
* <span data-ttu-id="e0b61-109">在 [开放扩展](/graph/extensibility-overview)中将数据添加为自定义属性。</span><span class="sxs-lookup"><span data-stu-id="e0b61-109">Adding your data as custom properties in [open extensions](/graph/extensibility-overview).</span></span>
* <span data-ttu-id="e0b61-110">订阅[更改通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="e0b61-110">Subscribing to [change notifications](/graph/webhooks).</span></span>
* <span data-ttu-id="e0b61-111">使用 [delta 查询](/graph/delta-query-overview) 跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="e0b61-111">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions and updates.</span></span>


## <a name="methods"></a><span data-ttu-id="e0b61-112">方法</span><span class="sxs-lookup"><span data-stu-id="e0b61-112">Methods</span></span>
|<span data-ttu-id="e0b61-113">方法</span><span class="sxs-lookup"><span data-stu-id="e0b61-113">Method</span></span>|<span data-ttu-id="e0b61-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="e0b61-114">Return type</span></span>|<span data-ttu-id="e0b61-115">Description</span><span class="sxs-lookup"><span data-stu-id="e0b61-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e0b61-116">List tasks</span><span class="sxs-lookup"><span data-stu-id="e0b61-116">List tasks</span></span>](../api/todotasklist-list-tasks.md)|<span data-ttu-id="e0b61-117">[todoTask](todotask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e0b61-117">[todoTask](todotask.md) collection</span></span>|<span data-ttu-id="e0b61-118">获取指定列表中的所有 [todoTask](todotask.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="e0b61-118">Get all the [todoTask](todotask.md) resources in the specified list.</span></span>|
|[<span data-ttu-id="e0b61-119">创建任务</span><span class="sxs-lookup"><span data-stu-id="e0b61-119">Create task</span></span>](../api/todotasklist-post-tasks.md)|[<span data-ttu-id="e0b61-120">todoTask</span><span class="sxs-lookup"><span data-stu-id="e0b61-120">todoTask</span></span>](todotask.md)| <span data-ttu-id="e0b61-121">在指定的任务列表中创建[todoTask](todotask.md)</span><span class="sxs-lookup"><span data-stu-id="e0b61-121">Create a [todoTask](todotask.md) in the specified task list</span></span>|
|[<span data-ttu-id="e0b61-122">获取任务</span><span class="sxs-lookup"><span data-stu-id="e0b61-122">Get task</span></span>](../api/todotask-get.md)|[<span data-ttu-id="e0b61-123">todoTask</span><span class="sxs-lookup"><span data-stu-id="e0b61-123">todoTask</span></span>](../resources/todotask.md)|<span data-ttu-id="e0b61-124">读取 [todoTask](../resources/todotask.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e0b61-124">Read the properties and relationships of a [todoTask](../resources/todotask.md) object.</span></span>|
|[<span data-ttu-id="e0b61-125">更新任务</span><span class="sxs-lookup"><span data-stu-id="e0b61-125">Update task</span></span>](../api/todotask-update.md)|[<span data-ttu-id="e0b61-126">todoTask</span><span class="sxs-lookup"><span data-stu-id="e0b61-126">todoTask</span></span>](../resources/todotask.md)|<span data-ttu-id="e0b61-127">更新 [todoTask](../resources/todotask.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e0b61-127">Update the properties of a [todoTask](../resources/todotask.md) object.</span></span>|
|[<span data-ttu-id="e0b61-128">删除任务</span><span class="sxs-lookup"><span data-stu-id="e0b61-128">Delete task</span></span>](../api/todotask-delete.md)|<span data-ttu-id="e0b61-129">无</span><span class="sxs-lookup"><span data-stu-id="e0b61-129">None</span></span>|<span data-ttu-id="e0b61-130">删除一个 [todoTask](../resources/todotask.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e0b61-130">Deletes a [todoTask](../resources/todotask.md) object.</span></span>|
|[<span data-ttu-id="e0b61-131">列出 linkedResources</span><span class="sxs-lookup"><span data-stu-id="e0b61-131">List linkedResources</span></span>](../api/todotask-list-linkedresources.md)|<span data-ttu-id="e0b61-132">[linkedResource](../resources/linkedresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e0b61-132">[linkedResource](../resources/linkedresource.md) collection</span></span>|<span data-ttu-id="e0b61-133">从 linkedResources 导航属性中获取 linkedResources。</span><span class="sxs-lookup"><span data-stu-id="e0b61-133">Get the linkedResources from the linkedResources navigation property.</span></span>|
|[<span data-ttu-id="e0b61-134">创建 linkedResources</span><span class="sxs-lookup"><span data-stu-id="e0b61-134">Create linkedResources</span></span>](../api/todotask-post-linkedresources.md)|[<span data-ttu-id="e0b61-135">linkedResource</span><span class="sxs-lookup"><span data-stu-id="e0b61-135">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="e0b61-136">创建新的 linkedResources 对象。</span><span class="sxs-lookup"><span data-stu-id="e0b61-136">Create a new linkedResources object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e0b61-137">属性</span><span class="sxs-lookup"><span data-stu-id="e0b61-137">Properties</span></span>
|<span data-ttu-id="e0b61-138">属性</span><span class="sxs-lookup"><span data-stu-id="e0b61-138">Property</span></span>|<span data-ttu-id="e0b61-139">类型</span><span class="sxs-lookup"><span data-stu-id="e0b61-139">Type</span></span>|<span data-ttu-id="e0b61-140">Description</span><span class="sxs-lookup"><span data-stu-id="e0b61-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0b61-141">body</span><span class="sxs-lookup"><span data-stu-id="e0b61-141">body</span></span>|[<span data-ttu-id="e0b61-142">itemBody</span><span class="sxs-lookup"><span data-stu-id="e0b61-142">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="e0b61-143">通常包含有关任务的信息的任务正文。</span><span class="sxs-lookup"><span data-stu-id="e0b61-143">The task body that typically contains information about the task.</span></span>|
|<span data-ttu-id="e0b61-144">bodyLastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0b61-144">bodyLastModifiedDateTime</span></span>|<span data-ttu-id="e0b61-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0b61-145">DateTimeOffset</span></span>|<span data-ttu-id="e0b61-146">上次修改任务的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e0b61-146">The date and time when the task was last modified.</span></span> <span data-ttu-id="e0b61-147">默认情况下，它采用 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="e0b61-147">By default, it is in UTC.</span></span> <span data-ttu-id="e0b61-148">你可以在请求标头中提供自定义时区。</span><span class="sxs-lookup"><span data-stu-id="e0b61-148">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="e0b61-149">属性值使用 ISO 8601 格式，并始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="e0b61-149">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e0b61-150">例如，2020年1月1日午夜 UTC 将如下所示： "2020-01-01T00：00： 00Z"。</span><span class="sxs-lookup"><span data-stu-id="e0b61-150">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="e0b61-151">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0b61-151">completedDateTime</span></span>|[<span data-ttu-id="e0b61-152">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e0b61-152">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="e0b61-153">在指定时区内完成任务的日期。</span><span class="sxs-lookup"><span data-stu-id="e0b61-153">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="e0b61-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e0b61-154">createdDateTime</span></span>|<span data-ttu-id="e0b61-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0b61-155">DateTimeOffset</span></span>|<span data-ttu-id="e0b61-156">任务的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e0b61-156">The date and time when the task was created.</span></span> <span data-ttu-id="e0b61-157">默认情况下，它采用 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="e0b61-157">By default, it is in UTC.</span></span> <span data-ttu-id="e0b61-158">你可以在请求标头中提供自定义时区。</span><span class="sxs-lookup"><span data-stu-id="e0b61-158">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="e0b61-159">属性值使用 ISO 8601 格式。</span><span class="sxs-lookup"><span data-stu-id="e0b61-159">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="e0b61-160">例如，2020年1月1日午夜 UTC 将如下所示： "2020-01-01T00：00： 00Z"。</span><span class="sxs-lookup"><span data-stu-id="e0b61-160">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="e0b61-161">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="e0b61-161">dueDateTime</span></span>|[<span data-ttu-id="e0b61-162">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e0b61-162">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="e0b61-163">要在指定时区内完成任务的日期。</span><span class="sxs-lookup"><span data-stu-id="e0b61-163">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="e0b61-164">id</span><span class="sxs-lookup"><span data-stu-id="e0b61-164">id</span></span>|<span data-ttu-id="e0b61-165">String</span><span class="sxs-lookup"><span data-stu-id="e0b61-165">String</span></span>|<span data-ttu-id="e0b61-166">任务的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e0b61-166">Unique identifier for the task.</span></span> <span data-ttu-id="e0b61-167">默认情况下，在将项目从一个列表移动到另一个列表时，此值会发生更改。</span><span class="sxs-lookup"><span data-stu-id="e0b61-167">By default, this value changes when the item is moved from one list to another.</span></span>|
|<span data-ttu-id="e0b61-168">importance</span><span class="sxs-lookup"><span data-stu-id="e0b61-168">importance</span></span>|<span data-ttu-id="e0b61-169">importance</span><span class="sxs-lookup"><span data-stu-id="e0b61-169">importance</span></span>|<span data-ttu-id="e0b61-170">任务的重要性。</span><span class="sxs-lookup"><span data-stu-id="e0b61-170">The importance of the task.</span></span> <span data-ttu-id="e0b61-171">可取值为：`low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="e0b61-171">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="e0b61-172">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="e0b61-172">isReminderOn</span></span>|<span data-ttu-id="e0b61-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0b61-173">Boolean</span></span>|<span data-ttu-id="e0b61-174">如果设置警报以提醒用户有任务，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="e0b61-174">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="e0b61-175">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0b61-175">lastModifiedDateTime</span></span>|<span data-ttu-id="e0b61-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0b61-176">DateTimeOffset</span></span>|<span data-ttu-id="e0b61-177">上次修改任务的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e0b61-177">The date and time when the task was last modified.</span></span> <span data-ttu-id="e0b61-178">默认情况下，它采用 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="e0b61-178">By default, it is in UTC.</span></span> <span data-ttu-id="e0b61-179">你可以在请求标头中提供自定义时区。</span><span class="sxs-lookup"><span data-stu-id="e0b61-179">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="e0b61-180">属性值使用 ISO 8601 格式，并始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="e0b61-180">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e0b61-181">例如，2020年1月1日午夜 UTC 将如下所示： "2020-01-01T00：00： 00Z"。</span><span class="sxs-lookup"><span data-stu-id="e0b61-181">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="e0b61-182">recurrence</span><span class="sxs-lookup"><span data-stu-id="e0b61-182">recurrence</span></span>|[<span data-ttu-id="e0b61-183">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="e0b61-183">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="e0b61-184">任务的定期模式。</span><span class="sxs-lookup"><span data-stu-id="e0b61-184">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="e0b61-185">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="e0b61-185">reminderDateTime</span></span>|[<span data-ttu-id="e0b61-186">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e0b61-186">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="e0b61-187">提醒警报发出任务发生提醒的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e0b61-187">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="e0b61-188">status</span><span class="sxs-lookup"><span data-stu-id="e0b61-188">status</span></span>|<span data-ttu-id="e0b61-189">taskStatus</span><span class="sxs-lookup"><span data-stu-id="e0b61-189">taskStatus</span></span>|<span data-ttu-id="e0b61-190">指示任务的状态或进度。</span><span class="sxs-lookup"><span data-stu-id="e0b61-190">Indicates the state or progress of the task.</span></span> <span data-ttu-id="e0b61-191">可取值为：`notStarted`、`inProgress`、`completed`、`waitingOnOthers`、`deferred`。</span><span class="sxs-lookup"><span data-stu-id="e0b61-191">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="e0b61-192">title</span><span class="sxs-lookup"><span data-stu-id="e0b61-192">title</span></span>|<span data-ttu-id="e0b61-193">String</span><span class="sxs-lookup"><span data-stu-id="e0b61-193">String</span></span>|<span data-ttu-id="e0b61-194">任务的简短说明。</span><span class="sxs-lookup"><span data-stu-id="e0b61-194">A brief description of the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0b61-195">关系</span><span class="sxs-lookup"><span data-stu-id="e0b61-195">Relationships</span></span>
|<span data-ttu-id="e0b61-196">关系</span><span class="sxs-lookup"><span data-stu-id="e0b61-196">Relationship</span></span>|<span data-ttu-id="e0b61-197">类型</span><span class="sxs-lookup"><span data-stu-id="e0b61-197">Type</span></span>|<span data-ttu-id="e0b61-198">说明</span><span class="sxs-lookup"><span data-stu-id="e0b61-198">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0b61-199">extensions</span><span class="sxs-lookup"><span data-stu-id="e0b61-199">extensions</span></span>|<span data-ttu-id="e0b61-200">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="e0b61-200">[extension](extension.md) collection</span></span>| <span data-ttu-id="e0b61-201">为任务定义的开放扩展的集合。</span><span class="sxs-lookup"><span data-stu-id="e0b61-201">The collection of open extensions defined for the task.</span></span> <span data-ttu-id="e0b61-202">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="e0b61-202">Nullable.</span></span>|
|<span data-ttu-id="e0b61-203">linkedResources</span><span class="sxs-lookup"><span data-stu-id="e0b61-203">linkedResources</span></span>|<span data-ttu-id="e0b61-204">[linkedResource](../resources/linkedresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e0b61-204">[linkedResource](../resources/linkedresource.md) collection</span></span>|<span data-ttu-id="e0b61-205">链接到任务的资源的集合。</span><span class="sxs-lookup"><span data-stu-id="e0b61-205">A collection of resources linked to the task.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e0b61-206">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e0b61-206">JSON representation</span></span>
<span data-ttu-id="e0b61-207">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0b61-207">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.todoTask",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.todoTask",
  "id": "String (identifier)",
  "body": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "completedDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "dueDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "importance": "String",
  "isReminderOn": "Boolean",
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
  },
  "reminderDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "status": "String",
  "title": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "bodyLastModifiedDateTime": "String (timestamp)"
}
```



