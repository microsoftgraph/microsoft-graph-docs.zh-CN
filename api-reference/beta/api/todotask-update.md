---
title: 更新 todoTask
description: 更新 todoTask 对象的属性。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 43b182a536bd379c3bb2f572eec7460a54e0576e
ms.sourcegitcommit: 39e48ed2d95b142ccf3f40ecc52441458f2745bf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/06/2020
ms.locfileid: "48364332"
---
# <a name="update-todotask"></a><span data-ttu-id="0e7b9-103">更新 todoTask</span><span class="sxs-lookup"><span data-stu-id="0e7b9-103">Update todoTask</span></span>
<span data-ttu-id="0e7b9-104">命名空间： microsoft. graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="0e7b9-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="0e7b9-105">更新 [todoTask](../resources/todotask.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0e7b9-105">Update the properties of a [todoTask](../resources/todotask.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e7b9-106">权限</span><span class="sxs-lookup"><span data-stu-id="0e7b9-106">Permissions</span></span>
<span data-ttu-id="0e7b9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0e7b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e7b9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0e7b9-109">Permission type</span></span>|<span data-ttu-id="0e7b9-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0e7b9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e7b9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e7b9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0e7b9-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e7b9-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="0e7b9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e7b9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e7b9-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e7b9-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="0e7b9-115">应用</span><span class="sxs-lookup"><span data-stu-id="0e7b9-115">Application</span></span>|<span data-ttu-id="0e7b9-116">不支持</span><span class="sxs-lookup"><span data-stu-id="0e7b9-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e7b9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e7b9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/todo/lists/{todoTaskListId}/tasks/{taskId}
PATCH /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}
```

## <a name="request-headers"></a><span data-ttu-id="0e7b9-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e7b9-118">Request headers</span></span>
|<span data-ttu-id="0e7b9-119">名称</span><span class="sxs-lookup"><span data-stu-id="0e7b9-119">Name</span></span>|<span data-ttu-id="0e7b9-120">说明</span><span class="sxs-lookup"><span data-stu-id="0e7b9-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0e7b9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e7b9-121">Authorization</span></span>|<span data-ttu-id="0e7b9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0e7b9-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0e7b9-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0e7b9-124">Content-Type</span></span>|<span data-ttu-id="0e7b9-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0e7b9-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e7b9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e7b9-127">Request body</span></span>
<span data-ttu-id="0e7b9-128">在请求正文中，提供 [todoTask](../resources/todotask.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e7b9-128">In the request body, supply a JSON representation of the [todoTask](../resources/todotask.md) object.</span></span>

<span data-ttu-id="0e7b9-129">下表显示创建 [todoTask](../resources/todotask.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0e7b9-129">The following table shows the properties that are required when you create the [todoTask](../resources/todotask.md).</span></span>

|<span data-ttu-id="0e7b9-130">属性</span><span class="sxs-lookup"><span data-stu-id="0e7b9-130">Property</span></span>|<span data-ttu-id="0e7b9-131">类型</span><span class="sxs-lookup"><span data-stu-id="0e7b9-131">Type</span></span>|<span data-ttu-id="0e7b9-132">说明</span><span class="sxs-lookup"><span data-stu-id="0e7b9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e7b9-133">id</span><span class="sxs-lookup"><span data-stu-id="0e7b9-133">id</span></span>|<span data-ttu-id="0e7b9-134">String</span><span class="sxs-lookup"><span data-stu-id="0e7b9-134">String</span></span>|<span data-ttu-id="0e7b9-135">任务的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0e7b9-135">The unique identifier of the task.</span></span> <span data-ttu-id="0e7b9-136">继承自 [entity](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="0e7b9-136">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="0e7b9-137">body</span><span class="sxs-lookup"><span data-stu-id="0e7b9-137">body</span></span>|[<span data-ttu-id="0e7b9-138">itemBody</span><span class="sxs-lookup"><span data-stu-id="0e7b9-138">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="0e7b9-139">通常包含有关任务的信息的任务正文。</span><span class="sxs-lookup"><span data-stu-id="0e7b9-139">The task body that typically contains information about the task.</span></span> <span data-ttu-id="0e7b9-140">请注意，仅支持 HTML 类型。</span><span class="sxs-lookup"><span data-stu-id="0e7b9-140">Note that only HTML type is supported.</span></span>|
|<span data-ttu-id="0e7b9-141">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e7b9-141">completedDateTime</span></span>|[<span data-ttu-id="0e7b9-142">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="0e7b9-142">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="0e7b9-143">在指定时区内完成任务的日期。</span><span class="sxs-lookup"><span data-stu-id="0e7b9-143">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="0e7b9-144">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="0e7b9-144">dueDateTime</span></span>|[<span data-ttu-id="0e7b9-145">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="0e7b9-145">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="0e7b9-146">要在指定时区内完成任务的日期。</span><span class="sxs-lookup"><span data-stu-id="0e7b9-146">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="0e7b9-147">importance</span><span class="sxs-lookup"><span data-stu-id="0e7b9-147">importance</span></span>|<span data-ttu-id="0e7b9-148">importance</span><span class="sxs-lookup"><span data-stu-id="0e7b9-148">importance</span></span>|<span data-ttu-id="0e7b9-149">事件的重要性。</span><span class="sxs-lookup"><span data-stu-id="0e7b9-149">The importance of the event.</span></span> <span data-ttu-id="0e7b9-150">可取值为：`low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="0e7b9-150">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="0e7b9-151">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="0e7b9-151">isReminderOn</span></span>|<span data-ttu-id="0e7b9-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e7b9-152">Boolean</span></span>|<span data-ttu-id="0e7b9-153">如果设置警报以提醒用户有任务，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="0e7b9-153">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="0e7b9-154">recurrence</span><span class="sxs-lookup"><span data-stu-id="0e7b9-154">recurrence</span></span>|[<span data-ttu-id="0e7b9-155">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="0e7b9-155">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="0e7b9-156">任务的定期模式。</span><span class="sxs-lookup"><span data-stu-id="0e7b9-156">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="0e7b9-157">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="0e7b9-157">reminderDateTime</span></span>|[<span data-ttu-id="0e7b9-158">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="0e7b9-158">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="0e7b9-159">提醒警报发出任务发生提醒的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0e7b9-159">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="0e7b9-160">状态</span><span class="sxs-lookup"><span data-stu-id="0e7b9-160">status</span></span>|<span data-ttu-id="0e7b9-161">taskStatus</span><span class="sxs-lookup"><span data-stu-id="0e7b9-161">taskStatus</span></span>|<span data-ttu-id="0e7b9-162">指示任务的状态或进度。</span><span class="sxs-lookup"><span data-stu-id="0e7b9-162">Indicates state or progress of the task.</span></span> <span data-ttu-id="0e7b9-163">可取值为：`notStarted`、`inProgress`、`completed`、`waitingOnOthers`、`deferred`。</span><span class="sxs-lookup"><span data-stu-id="0e7b9-163">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="0e7b9-164">title</span><span class="sxs-lookup"><span data-stu-id="0e7b9-164">title</span></span>|<span data-ttu-id="0e7b9-165">String</span><span class="sxs-lookup"><span data-stu-id="0e7b9-165">String</span></span>|<span data-ttu-id="0e7b9-166">任务的简短说明。</span><span class="sxs-lookup"><span data-stu-id="0e7b9-166">A brief description of the task.</span></span>|
|<span data-ttu-id="0e7b9-167">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e7b9-167">createdDateTime</span></span>|<span data-ttu-id="0e7b9-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e7b9-168">DateTimeOffset</span></span>|<span data-ttu-id="0e7b9-169">任务的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0e7b9-169">The date and time when the task was created.</span></span> <span data-ttu-id="0e7b9-170">默认情况下，它采用 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="0e7b9-170">By default, it is in UTC.</span></span> <span data-ttu-id="0e7b9-171">你可以在请求标头中提供自定义时区。</span><span class="sxs-lookup"><span data-stu-id="0e7b9-171">You can provide a custom time zone in the request header.</span></span>|
|<span data-ttu-id="0e7b9-172">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e7b9-172">lastModifiedDateTime</span></span>|<span data-ttu-id="0e7b9-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e7b9-173">DateTimeOffset</span></span>|<span data-ttu-id="0e7b9-174">上次修改任务的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0e7b9-174">The date and time when the task was last modified.</span></span> <span data-ttu-id="0e7b9-175">默认情况下，它采用 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="0e7b9-175">By default, it is in UTC.</span></span> <span data-ttu-id="0e7b9-176">你可以在请求标头中提供自定义时区。</span><span class="sxs-lookup"><span data-stu-id="0e7b9-176">You can provide a custom time zone in the request header.</span></span>|
|<span data-ttu-id="0e7b9-177">bodyLastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e7b9-177">bodyLastModifiedDateTime</span></span>|<span data-ttu-id="0e7b9-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e7b9-178">DateTimeOffset</span></span>|<span data-ttu-id="0e7b9-179">上次修改任务正文的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0e7b9-179">The date and time when the task body was last modified.</span></span> <span data-ttu-id="0e7b9-180">默认情况下，它采用 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="0e7b9-180">By default, it is in UTC.</span></span> <span data-ttu-id="0e7b9-181">你可以在请求标头中提供自定义时区。</span><span class="sxs-lookup"><span data-stu-id="0e7b9-181">You can provide a custom time zone in the request header.</span></span>|



## <a name="response"></a><span data-ttu-id="0e7b9-182">响应</span><span class="sxs-lookup"><span data-stu-id="0e7b9-182">Response</span></span>

<span data-ttu-id="0e7b9-183">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [todoTask](../resources/todotask.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0e7b9-183">If successful, this method returns a `200 OK` response code and an updated [todoTask](../resources/todotask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0e7b9-184">示例</span><span class="sxs-lookup"><span data-stu-id="0e7b9-184">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0e7b9-185">请求</span><span class="sxs-lookup"><span data-stu-id="0e7b9-185">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="0e7b9-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e7b9-186">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_todotask",
  "sampleKeys": ["AAMkADA1MTHgwAAA=", "721a35e2-35e2-721a-e235-1a72e2351a72"],
  "@odata.type": "microsoft.graph.todoTask"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/todo/lists/AAMkADA1MTHgwAAA=/tasks/721a35e2-35e2-721a-e235-1a72e2351a72
Content-Type: application/json
Content-length: 608

{
   "dueDateTime":{
      "dateTime":"2020-07-25T16:00:00",
      "timeZone":"Eastern Standard Time"
   }
}
```
# <a name="javascript"></a>[<span data-ttu-id="0e7b9-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e7b9-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-todotask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="0e7b9-188">C#</span><span class="sxs-lookup"><span data-stu-id="0e7b9-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-todotask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e7b9-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e7b9-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-todotask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="0e7b9-190">响应</span><span class="sxs-lookup"><span data-stu-id="0e7b9-190">Response</span></span>
<span data-ttu-id="0e7b9-191">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0e7b9-191">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
   "@odata.type": "microsoft.graph.todoTask"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tasks/$entity",
    "@odata.etag": "W/\"s8/ERWT3WEeFpBGD0bDgAA+TWq9g==\"",
    "importance": "low",
    "isReminderOn": false,
    "status": "notStarted",
    "title": "Shop for dinner",
    "createdDateTime": "2020-07-22T10:39:03.7937971Z",
    "lastModifiedDateTime": "2020-07-22T12:02:10.8835421Z",
    "id": "721a35e2-35e2-721a-e235-1a72e2351a72",
    "body": {
        "content": "",
        "contentType": "text"
    },
    "dueDateTime": {
        "dateTime": "2020-08-25T04:00:00.0000000",
        "timeZone": "UTC"
    }
}
   
```



