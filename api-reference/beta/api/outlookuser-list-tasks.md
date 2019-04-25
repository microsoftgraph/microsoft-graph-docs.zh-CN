---
title: 列出任务
description: 获取用户邮箱中的所有 Outlook 任务。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 2681d988035bd590e4f03ae8b2393d44bcb6d976
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539634"
---
# <a name="list-tasks"></a><span data-ttu-id="f4540-103">列出任务</span><span class="sxs-lookup"><span data-stu-id="f4540-103">List tasks</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4540-104">获取用户邮箱中的所有 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="f4540-104">Get all the Outlook tasks in the user's mailbox.</span></span>

<span data-ttu-id="f4540-105">默认情况下, 此操作 (以及发布、修补和[完成](../api/outlooktask-complete.md)任务操作) 返回 UTC 格式的与日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="f4540-105">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span>
<span data-ttu-id="f4540-106">你可以使用 `Prefer: outlook.timezone` 标头将响应中的所有与日期相关的属性都表示为与 UTC 不同的时区。</span><span class="sxs-lookup"><span data-stu-id="f4540-106">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span> <span data-ttu-id="f4540-107">请参阅获取单个任务的[示例](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time)。</span><span class="sxs-lookup"><span data-stu-id="f4540-107">See an [example](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time) for getting a single task.</span></span> <span data-ttu-id="f4540-108">您可以按类似方式应用标头以获取多个任务。</span><span class="sxs-lookup"><span data-stu-id="f4540-108">You can apply the header similarly to get multiple tasks.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4540-109">权限</span><span class="sxs-lookup"><span data-stu-id="f4540-109">Permissions</span></span>
<span data-ttu-id="f4540-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4540-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4540-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4540-112">Permission type</span></span>      | <span data-ttu-id="f4540-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f4540-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4540-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4540-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f4540-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="f4540-115">Tasks.Read</span></span>    |
|<span data-ttu-id="f4540-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4540-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4540-117">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="f4540-117">Tasks.Read</span></span>    |
|<span data-ttu-id="f4540-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4540-118">Application</span></span> | <span data-ttu-id="f4540-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4540-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4540-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4540-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/tasks
GET /users/{id|userPrincipalName}/outlook/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f4540-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f4540-121">Optional query parameters</span></span>
<span data-ttu-id="f4540-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f4540-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f4540-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4540-123">Request headers</span></span>
| <span data-ttu-id="f4540-124">名称</span><span class="sxs-lookup"><span data-stu-id="f4540-124">Name</span></span>      |<span data-ttu-id="f4540-125">说明</span><span class="sxs-lookup"><span data-stu-id="f4540-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f4540-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4540-126">Authorization</span></span>  | <span data-ttu-id="f4540-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f4540-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f4540-129">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="f4540-129">Prefer: outlook.timezone</span></span> | <span data-ttu-id="f4540-130">指定响应中时间属性的时区 (如果未指定此标头, 则采用 UTC 格式表示)。</span><span class="sxs-lookup"><span data-stu-id="f4540-130">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="f4540-131">可选。</span><span class="sxs-lookup"><span data-stu-id="f4540-131">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4540-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4540-132">Request body</span></span>
<span data-ttu-id="f4540-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f4540-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4540-134">响应</span><span class="sxs-lookup"><span data-stu-id="f4540-134">Response</span></span>

<span data-ttu-id="f4540-135">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[outlookTask](../resources/outlooktask.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="f4540-135">If successful, this method returns a `200 OK` response code and collection of [outlookTask](../resources/outlooktask.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f4540-136">示例</span><span class="sxs-lookup"><span data-stu-id="f4540-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f4540-137">请求</span><span class="sxs-lookup"><span data-stu-id="f4540-137">Request</span></span>
<span data-ttu-id="f4540-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f4540-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/tasks
```
##### <a name="response"></a><span data-ttu-id="f4540-139">响应</span><span class="sxs-lookup"><span data-stu-id="f4540-139">Response</span></span>
<span data-ttu-id="f4540-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f4540-140">Here is an example of the response.</span></span> <span data-ttu-id="f4540-141">默认情况下，响应中的 date-time 属性采用的是 UTC。</span><span class="sxs-lookup"><span data-stu-id="f4540-141">By default, the date-time properties in the response are in UTC.</span></span>

<span data-ttu-id="f4540-p106">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f4540-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List Tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookuser-list-tasks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
