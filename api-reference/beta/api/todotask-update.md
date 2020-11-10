---
title: 更新 todoTask
description: 更新 todoTask 对象的属性。
author: avijityadav
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: af05c4ad04873e528d894d1a02e0a8993cfc1790
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48974320"
---
# <a name="update-todotask"></a><span data-ttu-id="02a68-103">更新 todoTask</span><span class="sxs-lookup"><span data-stu-id="02a68-103">Update todoTask</span></span>
<span data-ttu-id="02a68-104">命名空间： microsoft. graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="02a68-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="02a68-105">更新 [todoTask](../resources/todotask.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="02a68-105">Update the properties of a [todoTask](../resources/todotask.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="02a68-106">权限</span><span class="sxs-lookup"><span data-stu-id="02a68-106">Permissions</span></span>
<span data-ttu-id="02a68-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="02a68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02a68-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="02a68-109">Permission type</span></span>|<span data-ttu-id="02a68-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="02a68-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02a68-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="02a68-111">Delegated (work or school account)</span></span>|<span data-ttu-id="02a68-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="02a68-112">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="02a68-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="02a68-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02a68-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="02a68-114">Tasks.ReadWrite</span></span>|
|<span data-ttu-id="02a68-115">应用</span><span class="sxs-lookup"><span data-stu-id="02a68-115">Application</span></span>|<span data-ttu-id="02a68-116">不支持</span><span class="sxs-lookup"><span data-stu-id="02a68-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="02a68-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="02a68-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/todo/lists/{todoTaskListId}/tasks/{taskId}
PATCH /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks/{taskId}
```

## <a name="request-headers"></a><span data-ttu-id="02a68-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="02a68-118">Request headers</span></span>
|<span data-ttu-id="02a68-119">名称</span><span class="sxs-lookup"><span data-stu-id="02a68-119">Name</span></span>|<span data-ttu-id="02a68-120">说明</span><span class="sxs-lookup"><span data-stu-id="02a68-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="02a68-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="02a68-121">Authorization</span></span>|<span data-ttu-id="02a68-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="02a68-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="02a68-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="02a68-124">Content-Type</span></span>|<span data-ttu-id="02a68-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="02a68-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="02a68-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="02a68-127">Request body</span></span>
<span data-ttu-id="02a68-128">在请求正文中，提供 [todoTask](../resources/todotask.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="02a68-128">In the request body, supply a JSON representation of the [todoTask](../resources/todotask.md) object.</span></span>

<span data-ttu-id="02a68-129">下表显示创建 [todoTask](../resources/todotask.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="02a68-129">The following table shows the properties that are required when you create the [todoTask](../resources/todotask.md).</span></span>

|<span data-ttu-id="02a68-130">属性</span><span class="sxs-lookup"><span data-stu-id="02a68-130">Property</span></span>|<span data-ttu-id="02a68-131">类型</span><span class="sxs-lookup"><span data-stu-id="02a68-131">Type</span></span>|<span data-ttu-id="02a68-132">说明</span><span class="sxs-lookup"><span data-stu-id="02a68-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02a68-133">id</span><span class="sxs-lookup"><span data-stu-id="02a68-133">id</span></span>|<span data-ttu-id="02a68-134">String</span><span class="sxs-lookup"><span data-stu-id="02a68-134">String</span></span>|<span data-ttu-id="02a68-135">任务的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="02a68-135">The unique identifier of the task.</span></span> <span data-ttu-id="02a68-136">继承自 [entity](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="02a68-136">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="02a68-137">body</span><span class="sxs-lookup"><span data-stu-id="02a68-137">body</span></span>|[<span data-ttu-id="02a68-138">itemBody</span><span class="sxs-lookup"><span data-stu-id="02a68-138">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="02a68-139">通常包含有关任务的信息的任务正文。</span><span class="sxs-lookup"><span data-stu-id="02a68-139">The task body that typically contains information about the task.</span></span> <span data-ttu-id="02a68-140">请注意，仅支持 HTML 类型。</span><span class="sxs-lookup"><span data-stu-id="02a68-140">Note that only HTML type is supported.</span></span>|
|<span data-ttu-id="02a68-141">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="02a68-141">completedDateTime</span></span>|[<span data-ttu-id="02a68-142">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="02a68-142">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="02a68-143">在指定时区内完成任务的日期。</span><span class="sxs-lookup"><span data-stu-id="02a68-143">The date in the specified time zone that the task was finished.</span></span>|
|<span data-ttu-id="02a68-144">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="02a68-144">dueDateTime</span></span>|[<span data-ttu-id="02a68-145">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="02a68-145">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="02a68-146">要在指定时区内完成任务的日期。</span><span class="sxs-lookup"><span data-stu-id="02a68-146">The date in the specified time zone that the task is to be finished.</span></span>|
|<span data-ttu-id="02a68-147">importance</span><span class="sxs-lookup"><span data-stu-id="02a68-147">importance</span></span>|<span data-ttu-id="02a68-148">importance</span><span class="sxs-lookup"><span data-stu-id="02a68-148">importance</span></span>|<span data-ttu-id="02a68-149">事件的重要性。</span><span class="sxs-lookup"><span data-stu-id="02a68-149">The importance of the event.</span></span> <span data-ttu-id="02a68-150">可取值为：`low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="02a68-150">Possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="02a68-151">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="02a68-151">isReminderOn</span></span>|<span data-ttu-id="02a68-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="02a68-152">Boolean</span></span>|<span data-ttu-id="02a68-153">如果设置警报以提醒用户有任务，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="02a68-153">Set to true if an alert is set to remind the user of the task.</span></span>|
|<span data-ttu-id="02a68-154">recurrence</span><span class="sxs-lookup"><span data-stu-id="02a68-154">recurrence</span></span>|[<span data-ttu-id="02a68-155">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="02a68-155">patternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="02a68-156">任务的定期模式。</span><span class="sxs-lookup"><span data-stu-id="02a68-156">The recurrence pattern for the task.</span></span>|
|<span data-ttu-id="02a68-157">reminderDateTime</span><span class="sxs-lookup"><span data-stu-id="02a68-157">reminderDateTime</span></span>|[<span data-ttu-id="02a68-158">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="02a68-158">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="02a68-159">提醒警报发出任务发生提醒的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="02a68-159">The date and time for a reminder alert of the task to occur.</span></span>|
|<span data-ttu-id="02a68-160">status</span><span class="sxs-lookup"><span data-stu-id="02a68-160">status</span></span>|<span data-ttu-id="02a68-161">taskStatus</span><span class="sxs-lookup"><span data-stu-id="02a68-161">taskStatus</span></span>|<span data-ttu-id="02a68-162">指示任务的状态或进度。</span><span class="sxs-lookup"><span data-stu-id="02a68-162">Indicates state or progress of the task.</span></span> <span data-ttu-id="02a68-163">可取值为：`notStarted`、`inProgress`、`completed`、`waitingOnOthers`、`deferred`。</span><span class="sxs-lookup"><span data-stu-id="02a68-163">Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.</span></span>|
|<span data-ttu-id="02a68-164">title</span><span class="sxs-lookup"><span data-stu-id="02a68-164">title</span></span>|<span data-ttu-id="02a68-165">String</span><span class="sxs-lookup"><span data-stu-id="02a68-165">String</span></span>|<span data-ttu-id="02a68-166">任务的简短说明。</span><span class="sxs-lookup"><span data-stu-id="02a68-166">A brief description of the task.</span></span>|
|<span data-ttu-id="02a68-167">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="02a68-167">createdDateTime</span></span>|<span data-ttu-id="02a68-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02a68-168">DateTimeOffset</span></span>|<span data-ttu-id="02a68-169">任务的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="02a68-169">The date and time when the task was created.</span></span> <span data-ttu-id="02a68-170">默认情况下，它采用 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="02a68-170">By default, it is in UTC.</span></span> <span data-ttu-id="02a68-171">你可以在请求标头中提供自定义时区。</span><span class="sxs-lookup"><span data-stu-id="02a68-171">You can provide a custom time zone in the request header.</span></span>|
|<span data-ttu-id="02a68-172">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="02a68-172">lastModifiedDateTime</span></span>|<span data-ttu-id="02a68-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02a68-173">DateTimeOffset</span></span>|<span data-ttu-id="02a68-174">上次修改任务的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="02a68-174">The date and time when the task was last modified.</span></span> <span data-ttu-id="02a68-175">默认情况下，它采用 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="02a68-175">By default, it is in UTC.</span></span> <span data-ttu-id="02a68-176">你可以在请求标头中提供自定义时区。</span><span class="sxs-lookup"><span data-stu-id="02a68-176">You can provide a custom time zone in the request header.</span></span>|
|<span data-ttu-id="02a68-177">bodyLastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="02a68-177">bodyLastModifiedDateTime</span></span>|<span data-ttu-id="02a68-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02a68-178">DateTimeOffset</span></span>|<span data-ttu-id="02a68-179">上次修改任务正文的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="02a68-179">The date and time when the task body was last modified.</span></span> <span data-ttu-id="02a68-180">默认情况下，它采用 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="02a68-180">By default, it is in UTC.</span></span> <span data-ttu-id="02a68-181">你可以在请求标头中提供自定义时区。</span><span class="sxs-lookup"><span data-stu-id="02a68-181">You can provide a custom time zone in the request header.</span></span>|



## <a name="response"></a><span data-ttu-id="02a68-182">响应</span><span class="sxs-lookup"><span data-stu-id="02a68-182">Response</span></span>

<span data-ttu-id="02a68-183">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [todoTask](../resources/todotask.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="02a68-183">If successful, this method returns a `200 OK` response code and an updated [todoTask](../resources/todotask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="02a68-184">示例</span><span class="sxs-lookup"><span data-stu-id="02a68-184">Examples</span></span>

### <a name="request"></a><span data-ttu-id="02a68-185">请求</span><span class="sxs-lookup"><span data-stu-id="02a68-185">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="02a68-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="02a68-186">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="02a68-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02a68-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-todotask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="02a68-188">C#</span><span class="sxs-lookup"><span data-stu-id="02a68-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-todotask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02a68-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02a68-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-todotask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="02a68-190">Java</span><span class="sxs-lookup"><span data-stu-id="02a68-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-todotask-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="02a68-191">响应</span><span class="sxs-lookup"><span data-stu-id="02a68-191">Response</span></span>
<span data-ttu-id="02a68-192">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="02a68-192">**Note:** The response object shown here might be shortened for readability.</span></span>
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



