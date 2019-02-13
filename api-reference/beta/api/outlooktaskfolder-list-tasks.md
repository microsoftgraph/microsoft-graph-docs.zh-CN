---
title: 列出任务
description: 在指定文件夹中获取所有 Outlook 任务。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: dfcd1438d55a22654c5601bc55827d0dedbdc6b2
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967261"
---
# <a name="list-tasks"></a><span data-ttu-id="c490b-103">列出任务</span><span class="sxs-lookup"><span data-stu-id="c490b-103">List tasks</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c490b-104">在指定文件夹中获取所有 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="c490b-104">Get all the Outlook tasks in the specified folder.</span></span>

<span data-ttu-id="c490b-105">默认情况下，此操作 （和文章、 修补程序，和[完成](../api/outlooktask-complete.md)任务操作） 返回与日期相关的属性采用 UTC。</span><span class="sxs-lookup"><span data-stu-id="c490b-105">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span>  <span data-ttu-id="c490b-106">您可以使用`Prefer: outlook.timezone`请求标头，使其具有不同于 UTC 时区中表示的响应中的所有日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="c490b-106">You can use a `Prefer: outlook.timezone` request header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span> <span data-ttu-id="c490b-107">请参阅[示例](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time)用于获取单个任务。</span><span class="sxs-lookup"><span data-stu-id="c490b-107">See an [example](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time) for getting a single task.</span></span> <span data-ttu-id="c490b-108">您可以应用同样要获取多个任务的标题。</span><span class="sxs-lookup"><span data-stu-id="c490b-108">You can apply the header similarly to get multiple tasks.</span></span>

<span data-ttu-id="c490b-109">如果存在多个任务组，并且想要获取的所有任务在特定任务组中，第一个都[都获取该任务组中的所有任务文件夹](outlooktaskgroup-list-taskfolders.md)，然后都都获取每个这些任务文件夹中的任务。</span><span class="sxs-lookup"><span data-stu-id="c490b-109">If there is more than one task group, and you want to get all the tasks in a specific task group, first [get all the task folders in that task group](outlooktaskgroup-list-taskfolders.md), and then get the tasks in each of these task folders.</span></span>

## <a name="permissions"></a><span data-ttu-id="c490b-110">权限</span><span class="sxs-lookup"><span data-stu-id="c490b-110">Permissions</span></span>
<span data-ttu-id="c490b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c490b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c490b-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="c490b-113">Permission type</span></span>      | <span data-ttu-id="c490b-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c490b-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c490b-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c490b-115">Delegated (work or school account)</span></span> | <span data-ttu-id="c490b-116">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="c490b-116">Tasks.Read</span></span>    |
|<span data-ttu-id="c490b-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c490b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c490b-118">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="c490b-118">Tasks.Read</span></span>    |
|<span data-ttu-id="c490b-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="c490b-119">Application</span></span> | <span data-ttu-id="c490b-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="c490b-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c490b-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c490b-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c490b-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c490b-122">Optional query parameters</span></span>
<span data-ttu-id="c490b-123">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c490b-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c490b-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="c490b-124">Request headers</span></span>
| <span data-ttu-id="c490b-125">Name</span><span class="sxs-lookup"><span data-stu-id="c490b-125">Name</span></span>      |<span data-ttu-id="c490b-126">说明</span><span class="sxs-lookup"><span data-stu-id="c490b-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c490b-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="c490b-127">Authorization</span></span>  | <span data-ttu-id="c490b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c490b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c490b-130">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="c490b-130">Prefer: outlook.timezone</span></span> | <span data-ttu-id="c490b-131">响应，它可以采用 UTC 如果未指定此标头中指定的时间属性的时区。</span><span class="sxs-lookup"><span data-stu-id="c490b-131">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="c490b-132">可选。</span><span class="sxs-lookup"><span data-stu-id="c490b-132">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c490b-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="c490b-133">Request body</span></span>
<span data-ttu-id="c490b-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c490b-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c490b-135">响应</span><span class="sxs-lookup"><span data-stu-id="c490b-135">Response</span></span>

<span data-ttu-id="c490b-136">如果成功，此方法返回`200 OK`响应代码和响应正文中的[outlookTask](../resources/outlooktask.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="c490b-136">If successful, this method returns a `200 OK` response code and collection of [outlookTask](../resources/outlooktask.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c490b-137">示例</span><span class="sxs-lookup"><span data-stu-id="c490b-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c490b-138">请求</span><span class="sxs-lookup"><span data-stu-id="c490b-138">Request</span></span>
<span data-ttu-id="c490b-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c490b-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAhrbPWAAA=/tasks
```
##### <a name="response"></a><span data-ttu-id="c490b-140">响应</span><span class="sxs-lookup"><span data-stu-id="c490b-140">Response</span></span>
<span data-ttu-id="c490b-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c490b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/outlooktaskfolder-list-tasks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
