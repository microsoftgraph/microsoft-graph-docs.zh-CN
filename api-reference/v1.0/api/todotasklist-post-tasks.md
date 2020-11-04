---
title: 创建 todoTask
description: 在指定的 todoTaskList 中创建新的任务对象。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 873cc4073ed56d1a30237676f617d9f415fc5b2a
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904429"
---
# <a name="create-todotask"></a><span data-ttu-id="06e53-103">创建 todoTask</span><span class="sxs-lookup"><span data-stu-id="06e53-103">Create todoTask</span></span>
<span data-ttu-id="06e53-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06e53-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="06e53-105">在指定的 [todoTaskList](../resources/todotasklist.md)中创建新的任务对象。</span><span class="sxs-lookup"><span data-stu-id="06e53-105">Create a new task object in a specified [todoTaskList](../resources/todotasklist.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="06e53-106">权限</span><span class="sxs-lookup"><span data-stu-id="06e53-106">Permissions</span></span>
<span data-ttu-id="06e53-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="06e53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06e53-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="06e53-109">Permission type</span></span>|<span data-ttu-id="06e53-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="06e53-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06e53-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06e53-111">Delegated (work or school account)</span></span>|<span data-ttu-id="06e53-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06e53-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="06e53-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06e53-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06e53-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06e53-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="06e53-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="06e53-115">Application</span></span>|<span data-ttu-id="06e53-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="06e53-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06e53-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="06e53-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists/{todoTaskListId}/tasks
POST /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks
```

## <a name="request-headers"></a><span data-ttu-id="06e53-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="06e53-118">Request headers</span></span>
|<span data-ttu-id="06e53-119">名称</span><span class="sxs-lookup"><span data-stu-id="06e53-119">Name</span></span>|<span data-ttu-id="06e53-120">说明</span><span class="sxs-lookup"><span data-stu-id="06e53-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="06e53-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="06e53-121">Authorization</span></span>|<span data-ttu-id="06e53-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="06e53-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="06e53-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="06e53-124">Content-Type</span></span>|<span data-ttu-id="06e53-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="06e53-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="06e53-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="06e53-127">Request body</span></span>
<span data-ttu-id="06e53-128">在请求正文中，提供 [todoTask](../resources/todotask.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06e53-128">In the request body, supply a JSON representation of the [todoTask](../resources/todotask.md) object.</span></span>

<span data-ttu-id="06e53-129">下表显示创建 [todoTask](../resources/todotask.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="06e53-129">The following table shows the properties that are required when you create the [todoTask](../resources/todotask.md).</span></span>

|<span data-ttu-id="06e53-130">属性</span><span class="sxs-lookup"><span data-stu-id="06e53-130">Property</span></span>|<span data-ttu-id="06e53-131">类型</span><span class="sxs-lookup"><span data-stu-id="06e53-131">Type</span></span>|<span data-ttu-id="06e53-132">说明</span><span class="sxs-lookup"><span data-stu-id="06e53-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06e53-133">id</span><span class="sxs-lookup"><span data-stu-id="06e53-133">id</span></span>|<span data-ttu-id="06e53-134">String</span><span class="sxs-lookup"><span data-stu-id="06e53-134">String</span></span>|<span data-ttu-id="06e53-135">任务的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="06e53-135">Unique identifier for the task.</span></span> <span data-ttu-id="06e53-136">默认情况下，在将项目从一个列表移动到另一个列表时，此值会发生更改。</span><span class="sxs-lookup"><span data-stu-id="06e53-136">By default, this value changes when the item is moved from one list to another.</span></span>|
|<span data-ttu-id="06e53-137">body</span><span class="sxs-lookup"><span data-stu-id="06e53-137">body</span></span>|[<span data-ttu-id="06e53-138">itemBody</span><span class="sxs-lookup"><span data-stu-id="06e53-138">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="06e53-139">通常包含有关任务的信息的任务正文。</span><span class="sxs-lookup"><span data-stu-id="06e53-139">The task body that typically contains information about the task.</span></span>|
|<span data-ttu-id="06e53-140">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="06e53-140">completedDateTime</span></span>|[<span data-ttu-id="06e53-141">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="06e53-141">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="06e53-142">在指定时区内完成任务的日期。</span><span class="sxs-lookup"><span data-stu-id="06e53-142">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="06e53-143">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="06e53-143">dueDateTime</span></span>|[<span data-ttu-id="06e53-144">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="06e53-144">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="06e53-145">要在指定时区内完成任务的日期。</span><span class="sxs-lookup"><span data-stu-id="06e53-145">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="06e53-146">importance</span><span class="sxs-lookup"><span data-stu-id="06e53-146">importance</span></span>|<span data-ttu-id="06e53-147">importance</span><span class="sxs-lookup"><span data-stu-id="06e53-147">importance</span></span>|<span data-ttu-id="06e53-148">任务的重要性。</span><span class="sxs-lookup"><span data-stu-id="06e53-148">The importance of the task.</span></span> <span data-ttu-id="06e53-149">可取值为：`low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="06e53-149">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="06e53-150">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="06e53-150">isReminderOn</span></span>|<span data-ttu-id="06e53-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="06e53-151">Boolean</span></span>|<span data-ttu-id="06e53-152">如果设置警报以提醒用户有任务，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="06e53-152">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="06e53-153">recurrence</span><span class="sxs-lookup"><span data-stu-id="06e53-153">recurrence</span></span>|[<span data-ttu-id="06e53-154">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="06e53-154">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="06e53-155">任务的定期模式。</span><span class="sxs-lookup"><span data-stu-id="06e53-155">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="06e53-156">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="06e53-156">reminderDateTime</span></span>|[<span data-ttu-id="06e53-157">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="06e53-157">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="06e53-158">提醒警报发出任务发生提醒的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="06e53-158">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="06e53-159">status</span><span class="sxs-lookup"><span data-stu-id="06e53-159">status</span></span>|<span data-ttu-id="06e53-160">taskStatus</span><span class="sxs-lookup"><span data-stu-id="06e53-160">taskStatus</span></span>|<span data-ttu-id="06e53-161">指示任务的状态或进度。</span><span class="sxs-lookup"><span data-stu-id="06e53-161">Indicates the state or progress of the task.</span></span> <span data-ttu-id="06e53-162">可取值为：`notStarted`、`inProgress`、`completed`、`waitingOnOthers`、`deferred`。</span><span class="sxs-lookup"><span data-stu-id="06e53-162">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="06e53-163">title</span><span class="sxs-lookup"><span data-stu-id="06e53-163">title</span></span>|<span data-ttu-id="06e53-164">String</span><span class="sxs-lookup"><span data-stu-id="06e53-164">String</span></span>|<span data-ttu-id="06e53-165">任务的简短说明。</span><span class="sxs-lookup"><span data-stu-id="06e53-165">A brief description of the task.</span></span>|
|<span data-ttu-id="06e53-166">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="06e53-166">createdDateTime</span></span>|<span data-ttu-id="06e53-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06e53-167">DateTimeOffset</span></span>|<span data-ttu-id="06e53-168">任务的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="06e53-168">The date and time when the task was created.</span></span> <span data-ttu-id="06e53-169">默认情况下，它采用 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="06e53-169">By default, it is in UTC.</span></span> <span data-ttu-id="06e53-170">你可以在请求标头中提供自定义时区。</span><span class="sxs-lookup"><span data-stu-id="06e53-170">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="06e53-171">属性值使用 ISO 8601 格式。</span><span class="sxs-lookup"><span data-stu-id="06e53-171">The property value uses ISO 8601 format.</span></span> <span data-ttu-id="06e53-172">例如，2020年1月1日午夜 UTC 将如下所示： "2020-01-01T00：00： 00Z"。</span><span class="sxs-lookup"><span data-stu-id="06e53-172">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="06e53-173">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06e53-173">lastModifiedDateTime</span></span>|<span data-ttu-id="06e53-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06e53-174">DateTimeOffset</span></span>|<span data-ttu-id="06e53-175">上次修改任务的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="06e53-175">The date and time when the task was last modified.</span></span> <span data-ttu-id="06e53-176">默认情况下，它采用 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="06e53-176">By default, it is in UTC.</span></span> <span data-ttu-id="06e53-177">你可以在请求标头中提供自定义时区。</span><span class="sxs-lookup"><span data-stu-id="06e53-177">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="06e53-178">属性值使用 ISO 8601 格式，并始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="06e53-178">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="06e53-179">例如，2020年1月1日午夜 UTC 将如下所示： "2020-01-01T00：00： 00Z"。</span><span class="sxs-lookup"><span data-stu-id="06e53-179">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="06e53-180">bodyLastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06e53-180">bodyLastModifiedDateTime</span></span>|<span data-ttu-id="06e53-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06e53-181">DateTimeOffset</span></span>|<span data-ttu-id="06e53-182">上次修改任务的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="06e53-182">The date and time when the task was last modified.</span></span> <span data-ttu-id="06e53-183">默认情况下，它采用 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="06e53-183">By default, it is in UTC.</span></span> <span data-ttu-id="06e53-184">你可以在请求标头中提供自定义时区。</span><span class="sxs-lookup"><span data-stu-id="06e53-184">You can provide a custom time zone in the request header.</span></span> <span data-ttu-id="06e53-185">属性值使用 ISO 8601 格式，并始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="06e53-185">The property value uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="06e53-186">例如，2020年1月1日午夜 UTC 将如下所示： "2020-01-01T00：00： 00Z"。</span><span class="sxs-lookup"><span data-stu-id="06e53-186">For example, midnight UTC on Jan 1, 2020 would look like this: '2020-01-01T00:00:00Z'.</span></span>|



## <a name="response"></a><span data-ttu-id="06e53-187">响应</span><span class="sxs-lookup"><span data-stu-id="06e53-187">Response</span></span>

<span data-ttu-id="06e53-188">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [todoTask](../resources/todotask.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="06e53-188">If successful, this method returns a `201 Created` response code and a [todoTask](../resources/todotask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="06e53-189">示例</span><span class="sxs-lookup"><span data-stu-id="06e53-189">Examples</span></span>

### <a name="request"></a><span data-ttu-id="06e53-190">请求</span><span class="sxs-lookup"><span data-stu-id="06e53-190">Request</span></span>
<span data-ttu-id="06e53-191">下面的示例在指定的任务列表中创建一个 **todoTask** ，并包含一个 [linkedResource](../resources/linkedresource.md)。</span><span class="sxs-lookup"><span data-stu-id="06e53-191">The following example creates a **todoTask** in the specified task list, and includes a [linkedResource](../resources/linkedresource.md).</span></span>


# <a name="http"></a>[<span data-ttu-id="06e53-192">HTTP</span><span class="sxs-lookup"><span data-stu-id="06e53-192">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AQMkADAwATM0MDAAMS0yMDkyLWVjMzYtM"],
  "name": "create_todotask_from_tasks"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/me/todo/lists/AQMkADAwATM0MDAAMS0yMDkyLWVjMzYtM/tasks
Content-Type: application/json
Content-length: 608

{
   "title":"A new task",
   "linkedResources":[
      {
         "webUrl":"http://microsoft.com",
         "applicationName":"Microsoft",
         "displayName":"Microsoft"
      }
   ]
}
```
# <a name="c"></a>[<span data-ttu-id="06e53-193">C#</span><span class="sxs-lookup"><span data-stu-id="06e53-193">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-todotask-from-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="06e53-194">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06e53-194">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-todotask-from-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="06e53-195">Objective-C</span><span class="sxs-lookup"><span data-stu-id="06e53-195">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-todotask-from-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="06e53-196">Java</span><span class="sxs-lookup"><span data-stu-id="06e53-196">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-todotask-from-tasks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="06e53-197">响应</span><span class="sxs-lookup"><span data-stu-id="06e53-197">Response</span></span>
<span data-ttu-id="06e53-198">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="06e53-198">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.todoTask"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
   "@odata.etag":"W/\"xzyPKP0BiUGgld+lMKXwbQAAnBoTIw==\"",
   "importance":"low",
   "isReminderOn":false,
   "status":"notStarted",
   "title":"A new task",
   "createdDateTime":"2020-08-18T09:03:05.8339192Z",
   "lastModifiedDateTime":"2020-08-18T09:03:06.0827766Z",
   "id":"AlMKXwbQAAAJws6wcAAAA=",
   "body":{
      "content":"",
      "contentType":"text"
   },
   "linkedResources":[
      {
         "id":"f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9",
         "webUrl":"http://microsoft.com",
         "applicationName":"Microsoft",
         "displayName":"Microsoft"
      }
   ]
}
```



