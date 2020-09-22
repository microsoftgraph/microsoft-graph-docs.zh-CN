---
title: todoTask 资源类型
description: TodoTask 资源跟踪工作项。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 58859f2781ecec713e547340606411302232ec06
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003491"
---
# <a name="todotask-resource-type"></a><span data-ttu-id="56e9a-103">todoTask 资源类型</span><span class="sxs-lookup"><span data-stu-id="56e9a-103">todoTask resource type</span></span>

<span data-ttu-id="56e9a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56e9a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56e9a-105">**TodoTask**表示可以跟踪和完成的任务，例如，一段工作或个人项目。</span><span class="sxs-lookup"><span data-stu-id="56e9a-105">A **todoTask** represents a task, such as a piece of work or personal item, that can be tracked and completed.</span></span> 

<span data-ttu-id="56e9a-106">**TodoTask**始终包含在[todoTaskList](todotasklist.md)中。</span><span class="sxs-lookup"><span data-stu-id="56e9a-106">A **todoTask** is always contained in a [todoTaskList](todotasklist.md).</span></span> <span data-ttu-id="56e9a-107">它包括与 [linkedResource](./linkedResource.md) 对象集合的关系，并跟踪任务的一个或多个源。</span><span class="sxs-lookup"><span data-stu-id="56e9a-107">It includes a relationship to a collection of [linkedResource](./linkedResource.md) objects, tracking one or more sources of the task.</span></span>

<span data-ttu-id="56e9a-108">此资源支持以下内容：</span><span class="sxs-lookup"><span data-stu-id="56e9a-108">This resource supports the following:</span></span>
* <span data-ttu-id="56e9a-109">在 [开放扩展](/graph/extensibility-overview)中将数据添加为自定义属性。</span><span class="sxs-lookup"><span data-stu-id="56e9a-109">Adding your data as custom properties in [open extensions](/graph/extensibility-overview).</span></span>
* <span data-ttu-id="56e9a-110">使用 [delta 查询](/graph/delta-query-overview) 跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="56e9a-110">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions and updates.</span></span>

## <a name="methods"></a><span data-ttu-id="56e9a-111">方法</span><span class="sxs-lookup"><span data-stu-id="56e9a-111">Methods</span></span>
|<span data-ttu-id="56e9a-112">方法</span><span class="sxs-lookup"><span data-stu-id="56e9a-112">Method</span></span>|<span data-ttu-id="56e9a-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="56e9a-113">Return type</span></span>|<span data-ttu-id="56e9a-114">说明</span><span class="sxs-lookup"><span data-stu-id="56e9a-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="56e9a-115">List tasks</span><span class="sxs-lookup"><span data-stu-id="56e9a-115">List tasks</span></span>](../api/todotasklist-list-tasks.md)|<span data-ttu-id="56e9a-116">[todoTask](todotask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="56e9a-116">[todoTask](todotask.md) collection</span></span>|<span data-ttu-id="56e9a-117">获取指定列表中的所有 [todoTask](todotask.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="56e9a-117">Get all the [todoTask](todotask.md) resources in the specified list.</span></span>|
|[<span data-ttu-id="56e9a-118">创建任务</span><span class="sxs-lookup"><span data-stu-id="56e9a-118">Create task</span></span>](../api/todotasklist-post-tasks.md)|[<span data-ttu-id="56e9a-119">todoTask</span><span class="sxs-lookup"><span data-stu-id="56e9a-119">todoTask</span></span>](todotask.md)| <span data-ttu-id="56e9a-120">在指定的任务列表中创建[todoTask](todotask.md)</span><span class="sxs-lookup"><span data-stu-id="56e9a-120">Create a [todoTask](todotask.md) in the specified task list</span></span>|
|[<span data-ttu-id="56e9a-121">获取任务</span><span class="sxs-lookup"><span data-stu-id="56e9a-121">Get task</span></span>](../api/todotask-get.md)|[<span data-ttu-id="56e9a-122">todoTask</span><span class="sxs-lookup"><span data-stu-id="56e9a-122">todoTask</span></span>](../resources/todotask.md)|<span data-ttu-id="56e9a-123">读取 [todoTask](../resources/todotask.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="56e9a-123">Read the properties and relationships of a [todoTask](../resources/todotask.md) object.</span></span>|
|[<span data-ttu-id="56e9a-124">更新任务</span><span class="sxs-lookup"><span data-stu-id="56e9a-124">Update task</span></span>](../api/todotask-update.md)|[<span data-ttu-id="56e9a-125">todoTask</span><span class="sxs-lookup"><span data-stu-id="56e9a-125">todoTask</span></span>](../resources/todotask.md)|<span data-ttu-id="56e9a-126">更新 [todoTask](../resources/todotask.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="56e9a-126">Update the properties of a [todoTask](../resources/todotask.md) object.</span></span>|
|[<span data-ttu-id="56e9a-127">删除任务</span><span class="sxs-lookup"><span data-stu-id="56e9a-127">Delete task</span></span>](../api/todotask-delete.md)|<span data-ttu-id="56e9a-128">无</span><span class="sxs-lookup"><span data-stu-id="56e9a-128">None</span></span>|<span data-ttu-id="56e9a-129">删除一个 [todoTask](../resources/todotask.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="56e9a-129">Deletes a [todoTask](../resources/todotask.md) object.</span></span>|
|[<span data-ttu-id="56e9a-130">列出 linkedResources</span><span class="sxs-lookup"><span data-stu-id="56e9a-130">List linkedResources</span></span>](../api/todotask-list-linkedresources.md)|<span data-ttu-id="56e9a-131">[linkedResource](../resources/linkedresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="56e9a-131">[linkedResource](../resources/linkedresource.md) collection</span></span>|<span data-ttu-id="56e9a-132">从 linkedResources 导航属性中获取 linkedResources。</span><span class="sxs-lookup"><span data-stu-id="56e9a-132">Get the linkedResources from the linkedResources navigation property.</span></span>|
|[<span data-ttu-id="56e9a-133">创建 linkedResources</span><span class="sxs-lookup"><span data-stu-id="56e9a-133">Create linkedResources</span></span>](../api/todotask-post-linkedresources.md)|[<span data-ttu-id="56e9a-134">linkedResource</span><span class="sxs-lookup"><span data-stu-id="56e9a-134">linkedResource</span></span>](../resources/linkedresource.md)|<span data-ttu-id="56e9a-135">创建新的 linkedResources 对象。</span><span class="sxs-lookup"><span data-stu-id="56e9a-135">Create a new linkedResources object.</span></span>|

## <a name="properties"></a><span data-ttu-id="56e9a-136">属性</span><span class="sxs-lookup"><span data-stu-id="56e9a-136">Properties</span></span>
|<span data-ttu-id="56e9a-137">属性</span><span class="sxs-lookup"><span data-stu-id="56e9a-137">Property</span></span>|<span data-ttu-id="56e9a-138">类型</span><span class="sxs-lookup"><span data-stu-id="56e9a-138">Type</span></span>|<span data-ttu-id="56e9a-139">说明</span><span class="sxs-lookup"><span data-stu-id="56e9a-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56e9a-140">正文</span><span class="sxs-lookup"><span data-stu-id="56e9a-140">body</span></span>|[<span data-ttu-id="56e9a-141">itemBody</span><span class="sxs-lookup"><span data-stu-id="56e9a-141">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="56e9a-142">通常包含有关任务的信息的任务正文。</span><span class="sxs-lookup"><span data-stu-id="56e9a-142">The task body that typically contains information about the task.</span></span>|
|<span data-ttu-id="56e9a-143">bodyLastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="56e9a-143">bodyLastModifiedDateTime</span></span>|<span data-ttu-id="56e9a-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56e9a-144">DateTimeOffset</span></span>|<span data-ttu-id="56e9a-145">上次修改任务的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="56e9a-145">The date and time when the task was last modified.</span></span> <span data-ttu-id="56e9a-146">默认情况下，它采用 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="56e9a-146">By default, it is in UTC.</span></span> <span data-ttu-id="56e9a-147">你可以在请求标头中提供自定义时区。</span><span class="sxs-lookup"><span data-stu-id="56e9a-147">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="56e9a-148">属性值使用 ISO 8601 格式，并始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="56e9a-148">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="56e9a-149">例如，2020年1月1日午夜 UTC 将如下所示： "2020-01-01T00：00： 00Z"。</span><span class="sxs-lookup"><span data-stu-id="56e9a-149">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="56e9a-150">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="56e9a-150">completedDateTime</span></span>|[<span data-ttu-id="56e9a-151">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="56e9a-151">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="56e9a-152">在指定时区内完成任务的日期。</span><span class="sxs-lookup"><span data-stu-id="56e9a-152">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="56e9a-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="56e9a-153">createdDateTime</span></span>|<span data-ttu-id="56e9a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56e9a-154">DateTimeOffset</span></span>|<span data-ttu-id="56e9a-155">任务的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="56e9a-155">The date and time when the task was created.</span></span> <span data-ttu-id="56e9a-156">默认情况下，它采用 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="56e9a-156">By default, it is in UTC.</span></span> <span data-ttu-id="56e9a-157">你可以在请求标头中提供自定义时区。</span><span class="sxs-lookup"><span data-stu-id="56e9a-157">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="56e9a-158">属性值使用 ISO 8601 格式。</span><span class="sxs-lookup"><span data-stu-id="56e9a-158">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="56e9a-159">例如，2020年1月1日午夜 UTC 将如下所示： "2020-01-01T00：00： 00Z"。</span><span class="sxs-lookup"><span data-stu-id="56e9a-159">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="56e9a-160">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="56e9a-160">dueDateTime</span></span>|[<span data-ttu-id="56e9a-161">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="56e9a-161">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="56e9a-162">要在指定时区内完成任务的日期。</span><span class="sxs-lookup"><span data-stu-id="56e9a-162">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="56e9a-163">id</span><span class="sxs-lookup"><span data-stu-id="56e9a-163">id</span></span>|<span data-ttu-id="56e9a-164">String</span><span class="sxs-lookup"><span data-stu-id="56e9a-164">String</span></span>|<span data-ttu-id="56e9a-165">任务的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="56e9a-165">Unique identifier for the task.</span></span> <span data-ttu-id="56e9a-166">默认情况下，在将项目从一个列表移动到另一个列表时，此值会发生更改。</span><span class="sxs-lookup"><span data-stu-id="56e9a-166">By default, this value changes when the item is moved from one list to another.</span></span>|
|<span data-ttu-id="56e9a-167">importance</span><span class="sxs-lookup"><span data-stu-id="56e9a-167">importance</span></span>|<span data-ttu-id="56e9a-168">importance</span><span class="sxs-lookup"><span data-stu-id="56e9a-168">importance</span></span>|<span data-ttu-id="56e9a-169">任务的重要性。</span><span class="sxs-lookup"><span data-stu-id="56e9a-169">The importance of the task.</span></span> <span data-ttu-id="56e9a-170">可取值为：`low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="56e9a-170">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="56e9a-171">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="56e9a-171">isReminderOn</span></span>|<span data-ttu-id="56e9a-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="56e9a-172">Boolean</span></span>|<span data-ttu-id="56e9a-173">如果设置警报以提醒用户有任务，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="56e9a-173">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="56e9a-174">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="56e9a-174">lastModifiedDateTime</span></span>|<span data-ttu-id="56e9a-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56e9a-175">DateTimeOffset</span></span>|<span data-ttu-id="56e9a-176">上次修改任务的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="56e9a-176">The date and time when the task was last modified.</span></span> <span data-ttu-id="56e9a-177">默认情况下，它采用 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="56e9a-177">By default, it is in UTC.</span></span> <span data-ttu-id="56e9a-178">你可以在请求标头中提供自定义时区。</span><span class="sxs-lookup"><span data-stu-id="56e9a-178">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="56e9a-179">属性值使用 ISO 8601 格式，并始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="56e9a-179">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="56e9a-180">例如，2020年1月1日午夜 UTC 将如下所示： "2020-01-01T00：00： 00Z"。</span><span class="sxs-lookup"><span data-stu-id="56e9a-180">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="56e9a-181">定期</span><span class="sxs-lookup"><span data-stu-id="56e9a-181">recurrence</span></span>|[<span data-ttu-id="56e9a-182">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="56e9a-182">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="56e9a-183">任务的定期模式。</span><span class="sxs-lookup"><span data-stu-id="56e9a-183">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="56e9a-184">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="56e9a-184">reminderDateTime</span></span>|[<span data-ttu-id="56e9a-185">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="56e9a-185">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="56e9a-186">提醒警报发出任务发生提醒的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="56e9a-186">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="56e9a-187">状态</span><span class="sxs-lookup"><span data-stu-id="56e9a-187">status</span></span>|<span data-ttu-id="56e9a-188">taskStatus</span><span class="sxs-lookup"><span data-stu-id="56e9a-188">taskStatus</span></span>|<span data-ttu-id="56e9a-189">指示任务的状态或进度。</span><span class="sxs-lookup"><span data-stu-id="56e9a-189">Indicates the state or progress of the task.</span></span> <span data-ttu-id="56e9a-190">可取值为：`notStarted`、`inProgress`、`completed`、`waitingOnOthers`、`deferred`。</span><span class="sxs-lookup"><span data-stu-id="56e9a-190">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="56e9a-191">title</span><span class="sxs-lookup"><span data-stu-id="56e9a-191">title</span></span>|<span data-ttu-id="56e9a-192">String</span><span class="sxs-lookup"><span data-stu-id="56e9a-192">String</span></span>|<span data-ttu-id="56e9a-193">任务的简短说明。</span><span class="sxs-lookup"><span data-stu-id="56e9a-193">A brief description of the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="56e9a-194">关系</span><span class="sxs-lookup"><span data-stu-id="56e9a-194">Relationships</span></span>
|<span data-ttu-id="56e9a-195">关系</span><span class="sxs-lookup"><span data-stu-id="56e9a-195">Relationship</span></span>|<span data-ttu-id="56e9a-196">类型</span><span class="sxs-lookup"><span data-stu-id="56e9a-196">Type</span></span>|<span data-ttu-id="56e9a-197">说明</span><span class="sxs-lookup"><span data-stu-id="56e9a-197">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56e9a-198">extensions</span><span class="sxs-lookup"><span data-stu-id="56e9a-198">extensions</span></span>|<span data-ttu-id="56e9a-199">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="56e9a-199">[extension](extension.md) collection</span></span>| <span data-ttu-id="56e9a-200">为任务定义的开放扩展的集合。</span><span class="sxs-lookup"><span data-stu-id="56e9a-200">The collection of open extensions defined for the task.</span></span> <span data-ttu-id="56e9a-201">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="56e9a-201">Nullable.</span></span>|
|<span data-ttu-id="56e9a-202">linkedResources</span><span class="sxs-lookup"><span data-stu-id="56e9a-202">linkedResources</span></span>|<span data-ttu-id="56e9a-203">[linkedResource](../resources/linkedresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="56e9a-203">[linkedResource](../resources/linkedresource.md) collection</span></span>|<span data-ttu-id="56e9a-204">链接到任务的资源的集合。</span><span class="sxs-lookup"><span data-stu-id="56e9a-204">A collection of resources linked to the task.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="56e9a-205">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="56e9a-205">JSON representation</span></span>
<span data-ttu-id="56e9a-206">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="56e9a-206">The following is a JSON representation of the resource.</span></span>
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



