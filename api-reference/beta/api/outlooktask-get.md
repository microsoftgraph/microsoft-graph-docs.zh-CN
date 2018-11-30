---
title: 获取 outlookTask
description: 获取用户的邮箱中的属性和 Outlook 任务的关系。
ms.openlocfilehash: d7d985614a37f0a4a70a074f63f4182130948495
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042013"
---
# <a name="get-outlooktask"></a><span data-ttu-id="c3749-103">获取 outlookTask</span><span class="sxs-lookup"><span data-stu-id="c3749-103">Get outlookTask</span></span>

> <span data-ttu-id="c3749-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c3749-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3749-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c3749-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c3749-106">获取用户的邮箱中的属性和 Outlook 任务的关系。</span><span class="sxs-lookup"><span data-stu-id="c3749-106">Get the properties and relationships of an Outlook task in the user's mailbox.</span></span>

<span data-ttu-id="c3749-107">默认情况下，此操作 （和文章、 修补程序，和[完成](../api/outlooktask-complete.md)任务操作） 返回与日期相关的属性采用 UTC。</span><span class="sxs-lookup"><span data-stu-id="c3749-107">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="c3749-108">您可以使用`Prefer: outlook.timezone`标头，使其具有不同于 UTC 时区中表示的响应中的所有日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="c3749-108">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3749-109">权限</span><span class="sxs-lookup"><span data-stu-id="c3749-109">Permissions</span></span>
<span data-ttu-id="c3749-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c3749-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3749-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="c3749-112">Permission type</span></span>      | <span data-ttu-id="c3749-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c3749-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3749-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c3749-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c3749-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="c3749-115">Tasks.Read</span></span>    |
|<span data-ttu-id="c3749-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c3749-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3749-117">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="c3749-117">Tasks.Read</span></span>    |
|<span data-ttu-id="c3749-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="c3749-118">Application</span></span> | <span data-ttu-id="c3749-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="c3749-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3749-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c3749-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/tasks/{id}
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c3749-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c3749-121">Optional query parameters</span></span>
<span data-ttu-id="c3749-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c3749-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c3749-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="c3749-123">Request headers</span></span>
| <span data-ttu-id="c3749-124">名称</span><span class="sxs-lookup"><span data-stu-id="c3749-124">Name</span></span>      |<span data-ttu-id="c3749-125">说明</span><span class="sxs-lookup"><span data-stu-id="c3749-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c3749-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3749-126">Authorization</span></span>  | <span data-ttu-id="c3749-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c3749-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c3749-129">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="c3749-129">Prefer: outlook.timezone</span></span> | <span data-ttu-id="c3749-130">响应，它可以采用 UTC 如果未指定此标头中指定的时间属性的时区。</span><span class="sxs-lookup"><span data-stu-id="c3749-130">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="c3749-131">可选。</span><span class="sxs-lookup"><span data-stu-id="c3749-131">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3749-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="c3749-132">Request body</span></span>
<span data-ttu-id="c3749-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c3749-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3749-134">响应</span><span class="sxs-lookup"><span data-stu-id="c3749-134">Response</span></span>

<span data-ttu-id="c3749-135">如果成功，此方法返回`200 OK`响应正文中的响应代码和[outlookTask](../resources/outlooktask.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c3749-135">If successful, this method returns a `200 OK` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>
## <a name="example-1"></a><span data-ttu-id="c3749-136">示例 1</span><span class="sxs-lookup"><span data-stu-id="c3749-136">Example 1</span></span>
##### <a name="request"></a><span data-ttu-id="c3749-137">请求</span><span class="sxs-lookup"><span data-stu-id="c3749-137">Request</span></span>
<span data-ttu-id="c3749-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c3749-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MTrgAAA=')
```
##### <a name="response"></a><span data-ttu-id="c3749-139">响应</span><span class="sxs-lookup"><span data-stu-id="c3749-139">Response</span></span>
<span data-ttu-id="c3749-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c3749-140">Here is an example of the response.</span></span> <span data-ttu-id="c3749-141">默认情况下，响应中的 date-time 属性采用的是 UTC。</span><span class="sxs-lookup"><span data-stu-id="c3749-141">By default, the date-time properties in the response are in UTC.</span></span> 

<span data-ttu-id="c3749-p107">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c3749-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 376

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
```


## <a name="example-2"></a><span data-ttu-id="c3749-144">示例 2</span><span class="sxs-lookup"><span data-stu-id="c3749-144">Example 2</span></span>
##### <a name="request"></a><span data-ttu-id="c3749-145">请求</span><span class="sxs-lookup"><span data-stu-id="c3749-145">Request</span></span>
<span data-ttu-id="c3749-146">此示例使用`Prefer: outlook.timezone`标头以指定在响应中显示日期时间属性</span><span class="sxs-lookup"><span data-stu-id="c3749-146">This example uses the `Prefer: outlook.timezone` header to specify displaying date-time properties in the response</span></span>  
<span data-ttu-id="c3749-147">在太平洋标准时间。</span><span class="sxs-lookup"><span data-stu-id="c3749-147">in Pacific Standard Time.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MHgwAAA=')
Prefer: outlook.timezone="Pacific Standard Time"
```
##### <a name="response"></a><span data-ttu-id="c3749-148">响应</span><span class="sxs-lookup"><span data-stu-id="c3749-148">Response</span></span>
<span data-ttu-id="c3749-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c3749-149">Here is an example of the response.</span></span> <span data-ttu-id="c3749-150">指定太平洋标准时间中显示的响应中的日期时间属性。</span><span class="sxs-lookup"><span data-stu-id="c3749-150">The date-time properties in the response are displayed in the specified Pacific Standard Time.</span></span> 

<span data-ttu-id="c3749-p109">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c3749-p109">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 576

{
  "id": "AAMkADA1MHgwAAA=",
  "createdDateTime": "2016-04-22T15:19:18.9526004-07:00",
  "lastModifiedDateTime": "2016-04-22T15:19:19.015101-07:00",
  "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIW9XXA==",
  "categories": [ ],
  "assignedTo": "Dana Swope",
  "body": {
    "contentType": "text",
    "content": ""
  },
  "completedDateTime": null,
  "dueDateTime": {
    "dateTime": "2016-05-04T021:00:00.0000000",
    "timeZone": "Pacific Standard Time"
  },
  "hasAttachments":false,
  "importance": "normal",
  "isReminderOn": false,
  "owner": "Administrator",
  "parentFolderId": "AQMkADA1MTEgAAAA==",
  "recurrence": null,
  "reminderDateTime": null,
  "sensitivity": "normal",
  "startDateTime": {
    "dateTime": "2016-05-02T21:00:00.0000000",
    "timeZone": "Pacific Standard Time"
  },
  "status": "notStarted",
  "subject": "Shop for children's weekend"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->