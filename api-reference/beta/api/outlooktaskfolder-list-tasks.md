---
title: 列出任务
description: 获取指定文件夹中的所有 Outlook 任务。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5bab4f479270ffdbd117bd78a798be33ea67cea5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349794"
---
# <a name="list-tasks"></a><span data-ttu-id="98db5-103">列出任务</span><span class="sxs-lookup"><span data-stu-id="98db5-103">List tasks</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98db5-104">获取指定文件夹中的所有 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="98db5-104">Get all the Outlook tasks in the specified folder.</span></span>

<span data-ttu-id="98db5-105">默认情况下, 此操作 (以及发布、修补和[完成](../api/outlooktask-complete.md)任务操作) 返回 UTC 格式的与日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="98db5-105">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span>  <span data-ttu-id="98db5-106">您可以使用`Prefer: outlook.timezone`请求标头将响应中的所有与日期相关的属性都以与 UTC 不同的时区表示。</span><span class="sxs-lookup"><span data-stu-id="98db5-106">You can use a `Prefer: outlook.timezone` request header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span> <span data-ttu-id="98db5-107">请参阅获取单个任务的[示例](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time)。</span><span class="sxs-lookup"><span data-stu-id="98db5-107">See an [example](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time) for getting a single task.</span></span> <span data-ttu-id="98db5-108">您可以按类似方式应用标头以获取多个任务。</span><span class="sxs-lookup"><span data-stu-id="98db5-108">You can apply the header similarly to get multiple tasks.</span></span>

<span data-ttu-id="98db5-109">如果有多个任务组, 并且想要获取特定任务组中的所有任务, 请首先[获取该任务组中的所有任务文件夹](outlooktaskgroup-list-taskfolders.md), 然后获取这些任务文件夹中每个任务文件夹中的任务。</span><span class="sxs-lookup"><span data-stu-id="98db5-109">If there is more than one task group, and you want to get all the tasks in a specific task group, first [get all the task folders in that task group](outlooktaskgroup-list-taskfolders.md), and then get the tasks in each of these task folders.</span></span>

## <a name="permissions"></a><span data-ttu-id="98db5-110">权限</span><span class="sxs-lookup"><span data-stu-id="98db5-110">Permissions</span></span>
<span data-ttu-id="98db5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="98db5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98db5-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="98db5-113">Permission type</span></span>      | <span data-ttu-id="98db5-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="98db5-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98db5-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="98db5-115">Delegated (work or school account)</span></span> | <span data-ttu-id="98db5-116">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="98db5-116">Tasks.Read</span></span>    |
|<span data-ttu-id="98db5-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="98db5-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98db5-118">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="98db5-118">Tasks.Read</span></span>    |
|<span data-ttu-id="98db5-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="98db5-119">Application</span></span> | <span data-ttu-id="98db5-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="98db5-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="98db5-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="98db5-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders/{id}/tasks
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="98db5-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="98db5-122">Optional query parameters</span></span>
<span data-ttu-id="98db5-123">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="98db5-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="98db5-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="98db5-124">Request headers</span></span>
| <span data-ttu-id="98db5-125">名称</span><span class="sxs-lookup"><span data-stu-id="98db5-125">Name</span></span>      |<span data-ttu-id="98db5-126">说明</span><span class="sxs-lookup"><span data-stu-id="98db5-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="98db5-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="98db5-127">Authorization</span></span>  | <span data-ttu-id="98db5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="98db5-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="98db5-130">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="98db5-130">Prefer: outlook.timezone</span></span> | <span data-ttu-id="98db5-131">指定响应中时间属性的时区 (如果未指定此标头, 则采用 UTC 格式表示)。</span><span class="sxs-lookup"><span data-stu-id="98db5-131">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="98db5-132">可选。</span><span class="sxs-lookup"><span data-stu-id="98db5-132">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="98db5-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="98db5-133">Request body</span></span>
<span data-ttu-id="98db5-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="98db5-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98db5-135">响应</span><span class="sxs-lookup"><span data-stu-id="98db5-135">Response</span></span>

<span data-ttu-id="98db5-136">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[outlookTask](../resources/outlooktask.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="98db5-136">If successful, this method returns a `200 OK` response code and collection of [outlookTask](../resources/outlooktask.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="98db5-137">示例</span><span class="sxs-lookup"><span data-stu-id="98db5-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="98db5-138">请求</span><span class="sxs-lookup"><span data-stu-id="98db5-138">Request</span></span>
<span data-ttu-id="98db5-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="98db5-139">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="98db5-140">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="98db5-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAhrbPWAAA=/tasks
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="98db5-141">C#</span><span class="sxs-lookup"><span data-stu-id="98db5-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="98db5-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="98db5-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="98db5-143">目标-C</span><span class="sxs-lookup"><span data-stu-id="98db5-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="98db5-144">Java</span><span class="sxs-lookup"><span data-stu-id="98db5-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tasks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="98db5-145">响应</span><span class="sxs-lookup"><span data-stu-id="98db5-145">Response</span></span>
<span data-ttu-id="98db5-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="98db5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
