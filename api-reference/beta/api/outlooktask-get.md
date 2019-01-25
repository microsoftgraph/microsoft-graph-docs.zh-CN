---
title: 获取 outlookTask
description: 获取用户的邮箱中的属性和 Outlook 任务的关系。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 47c6a24ccb76eb7752736386cf6ec17330832780
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526317"
---
# <a name="get-outlooktask"></a><span data-ttu-id="cef78-103">获取 outlookTask</span><span class="sxs-lookup"><span data-stu-id="cef78-103">Get outlookTask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cef78-104">获取用户的邮箱中的属性和 Outlook 任务的关系。</span><span class="sxs-lookup"><span data-stu-id="cef78-104">Get the properties and relationships of an Outlook task in the user's mailbox.</span></span>

<span data-ttu-id="cef78-105">默认情况下，此操作 （和文章、 修补程序，和[完成](../api/outlooktask-complete.md)任务操作） 返回与日期相关的属性采用 UTC。</span><span class="sxs-lookup"><span data-stu-id="cef78-105">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="cef78-106">您可以使用`Prefer: outlook.timezone`标头，使其具有不同于 UTC 时区中表示的响应中的所有日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="cef78-106">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="cef78-107">权限</span><span class="sxs-lookup"><span data-stu-id="cef78-107">Permissions</span></span>

<span data-ttu-id="cef78-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cef78-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cef78-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cef78-110">Permission type</span></span>      | <span data-ttu-id="cef78-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cef78-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cef78-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cef78-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cef78-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="cef78-113">Tasks.Read</span></span>    |
|<span data-ttu-id="cef78-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cef78-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cef78-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="cef78-115">Tasks.Read</span></span>    |
|<span data-ttu-id="cef78-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cef78-116">Application</span></span> | <span data-ttu-id="cef78-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="cef78-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cef78-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cef78-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}
GET /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cef78-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cef78-119">Optional query parameters</span></span>

<span data-ttu-id="cef78-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cef78-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cef78-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="cef78-121">Request headers</span></span>

| <span data-ttu-id="cef78-122">名称</span><span class="sxs-lookup"><span data-stu-id="cef78-122">Name</span></span>      |<span data-ttu-id="cef78-123">说明</span><span class="sxs-lookup"><span data-stu-id="cef78-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cef78-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cef78-124">Authorization</span></span>  | <span data-ttu-id="cef78-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cef78-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cef78-127">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="cef78-127">Prefer: outlook.timezone</span></span> | <span data-ttu-id="cef78-128">响应，它可以采用 UTC 如果未指定此标头中指定的时间属性的时区。</span><span class="sxs-lookup"><span data-stu-id="cef78-128">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="cef78-129">可选。</span><span class="sxs-lookup"><span data-stu-id="cef78-129">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cef78-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="cef78-130">Request body</span></span>

<span data-ttu-id="cef78-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cef78-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cef78-132">响应</span><span class="sxs-lookup"><span data-stu-id="cef78-132">Response</span></span>

<span data-ttu-id="cef78-133">如果成功，此方法返回`200 OK`响应正文中的响应代码和[outlookTask](../resources/outlooktask.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cef78-133">If successful, this method returns a `200 OK` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="cef78-134">示例 1</span><span class="sxs-lookup"><span data-stu-id="cef78-134">Example 1</span></span>

### <a name="request"></a><span data-ttu-id="cef78-135">请求</span><span class="sxs-lookup"><span data-stu-id="cef78-135">Request</span></span>

<span data-ttu-id="cef78-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cef78-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->

```http
GET https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MTrgAAA=')
```

### <a name="response"></a><span data-ttu-id="cef78-137">响应</span><span class="sxs-lookup"><span data-stu-id="cef78-137">Response</span></span>

<span data-ttu-id="cef78-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cef78-138">Here is an example of the response.</span></span> <span data-ttu-id="cef78-139">默认情况下，响应中的 date-time 属性采用的是 UTC。</span><span class="sxs-lookup"><span data-stu-id="cef78-139">By default, the date-time properties in the response are in UTC.</span></span>

> <span data-ttu-id="cef78-p106">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cef78-p106">**Note:** The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-2"></a><span data-ttu-id="cef78-142">示例 2</span><span class="sxs-lookup"><span data-stu-id="cef78-142">Example 2</span></span>

### <a name="request"></a><span data-ttu-id="cef78-143">请求</span><span class="sxs-lookup"><span data-stu-id="cef78-143">Request</span></span>

<span data-ttu-id="cef78-144">此示例使用`Prefer: outlook.timezone`标头以指定在太平洋标准时间的响应中显示日期时间属性。</span><span class="sxs-lookup"><span data-stu-id="cef78-144">This example uses the `Prefer: outlook.timezone` header to specify displaying date-time properties in the response in Pacific Standard Time.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->

```http
GET https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MHgwAAA=')
Prefer: outlook.timezone="Pacific Standard Time"
```

### <a name="response"></a><span data-ttu-id="cef78-145">响应</span><span class="sxs-lookup"><span data-stu-id="cef78-145">Response</span></span>

<span data-ttu-id="cef78-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cef78-146">Here is an example of the response.</span></span> <span data-ttu-id="cef78-147">指定太平洋标准时间中显示的响应中的日期时间属性。</span><span class="sxs-lookup"><span data-stu-id="cef78-147">The date-time properties in the response are displayed in the specified Pacific Standard Time.</span></span>

> <span data-ttu-id="cef78-p108">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cef78-p108">**Note:** The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktask-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
