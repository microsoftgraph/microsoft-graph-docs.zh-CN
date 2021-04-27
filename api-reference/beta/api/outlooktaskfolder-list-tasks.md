---
title: 列出任务
description: 获取指定Outlook的所有任务。
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f2d512828361cd4a51f7e21648a28a24760e2d06
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055447"
---
# <a name="list-tasks-deprecated"></a><span data-ttu-id="5ff4f-103">列出任务（已弃用）</span><span class="sxs-lookup"><span data-stu-id="5ff4f-103">List tasks (deprecated)</span></span>

<span data-ttu-id="5ff4f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ff4f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="5ff4f-105">获取指定Outlook的所有任务。</span><span class="sxs-lookup"><span data-stu-id="5ff4f-105">Get all the Outlook tasks in the specified folder.</span></span>

<span data-ttu-id="5ff4f-106">默认情况下，此操作 (POST、PATCH 和 [完成](../api/outlooktask-complete.md) 任务操作) UTC 格式返回与日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="5ff4f-106">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span>  <span data-ttu-id="5ff4f-107">可以使用请求标头将响应中与日期相关的所有属性表示为与 `Prefer: outlook.timezone` UTC 不同的时区。</span><span class="sxs-lookup"><span data-stu-id="5ff4f-107">You can use a `Prefer: outlook.timezone` request header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span> <span data-ttu-id="5ff4f-108">请参阅 [获取](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time) 单个任务的示例。</span><span class="sxs-lookup"><span data-stu-id="5ff4f-108">See an [example](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time) for getting a single task.</span></span> <span data-ttu-id="5ff4f-109">可以以类似方式应用 标头，以获取多个任务。</span><span class="sxs-lookup"><span data-stu-id="5ff4f-109">You can apply the header similarly to get multiple tasks.</span></span>

<span data-ttu-id="5ff4f-110">如果多个任务组，并且你想要获取特定任务组的所有任务，首先获取该任务组的所有任务文件夹，然后[](outlooktaskgroup-list-taskfolders.md)获取每个任务文件夹中的任务。</span><span class="sxs-lookup"><span data-stu-id="5ff4f-110">If there is more than one task group, and you want to get all the tasks in a specific task group, first [get all the task folders in that task group](outlooktaskgroup-list-taskfolders.md), and then get the tasks in each of these task folders.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ff4f-111">权限</span><span class="sxs-lookup"><span data-stu-id="5ff4f-111">Permissions</span></span>
<span data-ttu-id="5ff4f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5ff4f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ff4f-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="5ff4f-114">Permission type</span></span>      | <span data-ttu-id="5ff4f-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5ff4f-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ff4f-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5ff4f-116">Delegated (work or school account)</span></span> | <span data-ttu-id="5ff4f-117">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="5ff4f-117">Tasks.Read</span></span>    |
|<span data-ttu-id="5ff4f-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5ff4f-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ff4f-119">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="5ff4f-119">Tasks.Read</span></span>    |
|<span data-ttu-id="5ff4f-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="5ff4f-120">Application</span></span> | <span data-ttu-id="5ff4f-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="5ff4f-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ff4f-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5ff4f-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders/{id}/tasks
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5ff4f-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5ff4f-123">Optional query parameters</span></span>
<span data-ttu-id="5ff4f-124">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5ff4f-124">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ff4f-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="5ff4f-125">Request headers</span></span>
| <span data-ttu-id="5ff4f-126">名称</span><span class="sxs-lookup"><span data-stu-id="5ff4f-126">Name</span></span>      |<span data-ttu-id="5ff4f-127">说明</span><span class="sxs-lookup"><span data-stu-id="5ff4f-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5ff4f-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ff4f-128">Authorization</span></span>  | <span data-ttu-id="5ff4f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5ff4f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5ff4f-131">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="5ff4f-131">Prefer: outlook.timezone</span></span> | <span data-ttu-id="5ff4f-132">指定响应中时间属性的时区，如果未指定此标头，则其时区为 UTC。</span><span class="sxs-lookup"><span data-stu-id="5ff4f-132">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="5ff4f-133">可选。</span><span class="sxs-lookup"><span data-stu-id="5ff4f-133">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ff4f-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="5ff4f-134">Request body</span></span>
<span data-ttu-id="5ff4f-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5ff4f-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ff4f-136">响应</span><span class="sxs-lookup"><span data-stu-id="5ff4f-136">Response</span></span>

<span data-ttu-id="5ff4f-137">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [outlookTask](../resources/outlooktask.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5ff4f-137">If successful, this method returns a `200 OK` response code and collection of [outlookTask](../resources/outlooktask.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5ff4f-138">示例</span><span class="sxs-lookup"><span data-stu-id="5ff4f-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5ff4f-139">请求</span><span class="sxs-lookup"><span data-stu-id="5ff4f-139">Request</span></span>
<span data-ttu-id="5ff4f-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5ff4f-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5ff4f-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ff4f-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "outlooktaskfolder_get_tasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAhrbPWAAA=/tasks
```
# <a name="c"></a>[<span data-ttu-id="5ff4f-142">C#</span><span class="sxs-lookup"><span data-stu-id="5ff4f-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/outlooktaskfolder-get-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ff4f-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ff4f-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/outlooktaskfolder-get-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ff4f-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ff4f-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/outlooktaskfolder-get-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5ff4f-145">Java</span><span class="sxs-lookup"><span data-stu-id="5ff4f-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/outlooktaskfolder-get-tasks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5ff4f-146">响应</span><span class="sxs-lookup"><span data-stu-id="5ff4f-146">Response</span></span>
<span data-ttu-id="5ff4f-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5ff4f-147">Here is an example of the response.</span></span> <span data-ttu-id="5ff4f-148">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5ff4f-148">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 465

{
  "value": [
   {
      "id": "AAMkADA1MTrfAAA=",
      "createdDateTime": "2016-04-22T05:44:01.2012012Z",
      "lastModifiedDateTime": "2016-04-22T05:44:02.9980882Z",
      "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIOJMxw==",
      "categories": [ ],
      "assignedTo": null,
      "body": {
        "contentType": "text",
        "content": ""
      },
      "completedDateTime": null,
      "dueDateTime": {
        "dateTime": "2016-04-25T07:00:00.0000000",
        "timeZone": "UTC"
      },
      "hasAttachments":false,
      "importance": "normal",
      "isReminderOn": false,
      "owner": "Administrator",
      "parentFolderId": "AQMkADA1MTBEgAAAA==",
      "recurrence": null,
      "reminderDateTime": null,
      "sensitivity": "normal",
      "startDateTime": {
        "dateTime": "2016-04-23T07:00:00.0000000",
        "timeZone": "UTC"
      },
      "status": "notStarted",
      "subject": "Shop for dinner"
    },
    {
      "id": "AAMkADA1MTrgAAA=",
      "createdDateTime": "2016-04-22T06:03:35.9279794Z",
      "lastModifiedDateTime": "2016-04-22T06:03:35.9436052Z",
      "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIOJMyQ==",
      "categories": [ ],
      "assignedTo": null,
      "body": {
        "contentType": "text",
        "content": ""
      },
      "completedDateTime": null,
      "dueDateTime": {
        "dateTime": "2016-04-27T04:00:00.0000000",
        "timeZone": "UTC"
      },
      "hasAttachments":false,
      "importance": "normal",
      "isReminderOn": false,
      "owner": "Administrator",
      "parentFolderId": "AQMkADA1MTBEgAAAA==",
      "recurrence": null,
      "reminderDateTime": null,
      "sensitivity": "normal",
      "startDateTime": {
        "dateTime": "2016-04-26T04:00:00.0000000",
        "timeZone": "UTC"
      },
      "status": "notStarted",
      "subject": "Shop for dinner"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
