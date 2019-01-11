---
title: 列出任务
description: 在指定文件夹中获取所有 Outlook 任务。
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: ee6b4c2454ba6bfad0c0f4e6acd826917f02ca93
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863075"
---
# <a name="list-tasks"></a><span data-ttu-id="fedb1-103">列出任务</span><span class="sxs-lookup"><span data-stu-id="fedb1-103">List tasks</span></span>

> <span data-ttu-id="fedb1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fedb1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fedb1-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fedb1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fedb1-106">在指定文件夹中获取所有 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="fedb1-106">Get all the Outlook tasks in the specified folder.</span></span>

<span data-ttu-id="fedb1-107">默认情况下，此操作 （和文章、 修补程序，和[完成](../api/outlooktask-complete.md)任务操作） 返回与日期相关的属性采用 UTC。</span><span class="sxs-lookup"><span data-stu-id="fedb1-107">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span>  <span data-ttu-id="fedb1-108">您可以使用`Prefer: outlook.timezone`请求标头，使其具有不同于 UTC 时区中表示的响应中的所有日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="fedb1-108">You can use a `Prefer: outlook.timezone` request header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span> <span data-ttu-id="fedb1-109">请参阅[示例](outlooktask-get.md#example-2)用于获取单个任务。</span><span class="sxs-lookup"><span data-stu-id="fedb1-109">See an [example](outlooktask-get.md#example-2) for getting a single task.</span></span> <span data-ttu-id="fedb1-110">您可以应用同样要获取多个任务的标题。</span><span class="sxs-lookup"><span data-stu-id="fedb1-110">You can apply the header similarly to get multiple tasks.</span></span>

<span data-ttu-id="fedb1-111">如果存在多个任务组，并且想要获取的所有任务在特定任务组中，第一个都[都获取该任务组中的所有任务文件夹](outlooktaskgroup-list-taskfolders.md)，然后都都获取每个这些任务文件夹中的任务。</span><span class="sxs-lookup"><span data-stu-id="fedb1-111">If there is more than one task group, and you want to get all the tasks in a specific task group, first [get all the task folders in that task group](outlooktaskgroup-list-taskfolders.md), and then get the tasks in each of these task folders.</span></span> 

## <a name="permissions"></a><span data-ttu-id="fedb1-112">权限</span><span class="sxs-lookup"><span data-stu-id="fedb1-112">Permissions</span></span>
<span data-ttu-id="fedb1-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fedb1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fedb1-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="fedb1-115">Permission type</span></span>      | <span data-ttu-id="fedb1-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fedb1-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fedb1-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fedb1-117">Delegated (work or school account)</span></span> | <span data-ttu-id="fedb1-118">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="fedb1-118">Tasks.Read</span></span>    |
|<span data-ttu-id="fedb1-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fedb1-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fedb1-120">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="fedb1-120">Tasks.Read</span></span>    |
|<span data-ttu-id="fedb1-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="fedb1-121">Application</span></span> | <span data-ttu-id="fedb1-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="fedb1-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fedb1-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fedb1-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fedb1-124">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fedb1-124">Optional query parameters</span></span>
<span data-ttu-id="fedb1-125">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fedb1-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fedb1-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="fedb1-126">Request headers</span></span>
| <span data-ttu-id="fedb1-127">名称</span><span class="sxs-lookup"><span data-stu-id="fedb1-127">Name</span></span>      |<span data-ttu-id="fedb1-128">说明</span><span class="sxs-lookup"><span data-stu-id="fedb1-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fedb1-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="fedb1-129">Authorization</span></span>  | <span data-ttu-id="fedb1-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fedb1-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fedb1-132">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="fedb1-132">Prefer: outlook.timezone</span></span> | <span data-ttu-id="fedb1-133">响应，它可以采用 UTC 如果未指定此标头中指定的时间属性的时区。</span><span class="sxs-lookup"><span data-stu-id="fedb1-133">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="fedb1-134">可选。</span><span class="sxs-lookup"><span data-stu-id="fedb1-134">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fedb1-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="fedb1-135">Request body</span></span>
<span data-ttu-id="fedb1-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fedb1-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fedb1-137">响应</span><span class="sxs-lookup"><span data-stu-id="fedb1-137">Response</span></span>

<span data-ttu-id="fedb1-138">如果成功，此方法返回`200 OK`响应代码和响应正文中的[outlookTask](../resources/outlooktask.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="fedb1-138">If successful, this method returns a `200 OK` response code and collection of [outlookTask](../resources/outlooktask.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fedb1-139">示例</span><span class="sxs-lookup"><span data-stu-id="fedb1-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fedb1-140">请求</span><span class="sxs-lookup"><span data-stu-id="fedb1-140">Request</span></span>
<span data-ttu-id="fedb1-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fedb1-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAhrbPWAAA=/tasks
```
##### <a name="response"></a><span data-ttu-id="fedb1-142">响应</span><span class="sxs-lookup"><span data-stu-id="fedb1-142">Response</span></span>
<span data-ttu-id="fedb1-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fedb1-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
