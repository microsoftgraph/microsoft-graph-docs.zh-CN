---
title: 获取 outlookTask
description: 获取用户邮箱中的 Outlook 任务的属性和关系。
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 50bc54603005d226f6c05c03f4ccee772ec1d8fb
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849714"
---
# <a name="get-outlooktask"></a><span data-ttu-id="16a9e-103">获取 outlookTask</span><span class="sxs-lookup"><span data-stu-id="16a9e-103">Get outlookTask</span></span>

<span data-ttu-id="16a9e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16a9e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="16a9e-105">获取用户邮箱中的 Outlook 任务的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="16a9e-105">Get the properties and relationships of an Outlook task in the user's mailbox.</span></span>

<span data-ttu-id="16a9e-106">默认情况下，此操作会 (POST、PATCH 和 [完成](../api/outlooktask-complete.md) 的任务操作) 返回与日期相关的属性) 使用 UTC 格式返回日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="16a9e-106">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="16a9e-107">你可以使用 `Prefer: outlook.timezone` 标头将响应中的所有与日期相关的属性都表示为与 UTC 不同的时区。</span><span class="sxs-lookup"><span data-stu-id="16a9e-107">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="16a9e-108">权限</span><span class="sxs-lookup"><span data-stu-id="16a9e-108">Permissions</span></span>

<span data-ttu-id="16a9e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="16a9e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="16a9e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="16a9e-111">Permission type</span></span>                        | <span data-ttu-id="16a9e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="16a9e-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="16a9e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="16a9e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="16a9e-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="16a9e-114">Tasks.Read</span></span>                          |
| <span data-ttu-id="16a9e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="16a9e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16a9e-116">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="16a9e-116">Tasks.Read</span></span>                          |
| <span data-ttu-id="16a9e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="16a9e-117">Application</span></span>                            | <span data-ttu-id="16a9e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="16a9e-118">Not supported.</span></span>                      |

## <a name="http-request"></a><span data-ttu-id="16a9e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="16a9e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}
GET /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="16a9e-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="16a9e-120">Optional query parameters</span></span>

<span data-ttu-id="16a9e-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="16a9e-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="16a9e-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="16a9e-122">Request headers</span></span>

| <span data-ttu-id="16a9e-123">名称</span><span class="sxs-lookup"><span data-stu-id="16a9e-123">Name</span></span>                     | <span data-ttu-id="16a9e-124">说明</span><span class="sxs-lookup"><span data-stu-id="16a9e-124">Description</span></span>                                       |
|:-------------------------|:--------------------------------------------------|
| <span data-ttu-id="16a9e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="16a9e-125">Authorization</span></span>            | <span data-ttu-id="16a9e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="16a9e-p103">Bearer {token}. Required.</span></span>                         |
| <span data-ttu-id="16a9e-128">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="16a9e-128">Prefer: outlook.timezone</span></span> | <span data-ttu-id="16a9e-129">指定响应中的时区（如果未指定此标头，则该属性为 UTC 时间）。</span><span class="sxs-lookup"><span data-stu-id="16a9e-129">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="16a9e-130">可选。</span><span class="sxs-lookup"><span data-stu-id="16a9e-130">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16a9e-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="16a9e-131">Request body</span></span>

<span data-ttu-id="16a9e-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="16a9e-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16a9e-133">响应</span><span class="sxs-lookup"><span data-stu-id="16a9e-133">Response</span></span>

<span data-ttu-id="16a9e-134">如果成功，此方法在响应 `200 OK` 正文中返回 [响应代码和 outlookTask](../resources/outlooktask.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="16a9e-134">If successful, this method returns a `200 OK` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="16a9e-135">示例</span><span class="sxs-lookup"><span data-stu-id="16a9e-135">Examples</span></span>

### <a name="example-1-get-an-outlook-task"></a><span data-ttu-id="16a9e-136">示例 1：获取 Outlook 任务</span><span class="sxs-lookup"><span data-stu-id="16a9e-136">Example 1: Get an Outlook task</span></span>

#### <a name="request"></a><span data-ttu-id="16a9e-137">请求</span><span class="sxs-lookup"><span data-stu-id="16a9e-137">Request</span></span>

<span data-ttu-id="16a9e-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="16a9e-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="16a9e-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="16a9e-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADA1MTrgAAA=
```
# <a name="c"></a>[<span data-ttu-id="16a9e-140">C#</span><span class="sxs-lookup"><span data-stu-id="16a9e-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlooktask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16a9e-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16a9e-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlooktask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16a9e-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16a9e-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlooktask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="16a9e-143">响应</span><span class="sxs-lookup"><span data-stu-id="16a9e-143">Response</span></span>

<span data-ttu-id="16a9e-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="16a9e-144">Here is an example of the response.</span></span> <span data-ttu-id="16a9e-145">默认情况下，响应中的 date-time 属性采用的是 UTC。</span><span class="sxs-lookup"><span data-stu-id="16a9e-145">By default, the date-time properties in the response are in UTC.</span></span>

> <span data-ttu-id="16a9e-146">**注意：** 为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="16a9e-146">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="16a9e-147">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="16a9e-147">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "AAMkADA1MTrgAAA=",
  "createdDateTime": "2016-04-22T06:03:35.9279794Z",
  "lastModifiedDateTime": "2016-04-22T06:03:35.9436052Z",
  "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIOJMyQ==",
  "categories": [],
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
  "hasAttachments": false,
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

### <a name="example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time"></a><span data-ttu-id="16a9e-148">示例 2：获取在太小标准时间内具有日期-时间属性的 Outlook 任务</span><span class="sxs-lookup"><span data-stu-id="16a9e-148">Example 2: Get Outlook task with date-time properties in Pacific Standard Time</span></span>

#### <a name="request"></a><span data-ttu-id="16a9e-149">请求</span><span class="sxs-lookup"><span data-stu-id="16a9e-149">Request</span></span>

<span data-ttu-id="16a9e-150">此示例使用 `Prefer: outlook.timezone` 标头指定在太大的标准时间的响应中应返回 API 返回日期时间属性。</span><span class="sxs-lookup"><span data-stu-id="16a9e-150">This example uses the `Prefer: outlook.timezone` header to specify that the API should return date-time properties in the response in Pacific Standard Time.</span></span>


# <a name="http"></a>[<span data-ttu-id="16a9e-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="16a9e-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADA1MHgwAAA=
Prefer: outlook.timezone="Pacific Standard Time"
```
# <a name="c"></a>[<span data-ttu-id="16a9e-152">C#</span><span class="sxs-lookup"><span data-stu-id="16a9e-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlooktask-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16a9e-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16a9e-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlooktask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16a9e-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16a9e-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlooktask-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="16a9e-155">响应</span><span class="sxs-lookup"><span data-stu-id="16a9e-155">Response</span></span>

<span data-ttu-id="16a9e-156">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="16a9e-156">Here is an example of the response.</span></span> <span data-ttu-id="16a9e-157">以指定的太长时间返回响应中的日期-时间属性。</span><span class="sxs-lookup"><span data-stu-id="16a9e-157">The date-time properties in the response are returned in the specified Pacific Standard Time.</span></span>

> <span data-ttu-id="16a9e-158">**注意：** 为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="16a9e-158">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="16a9e-159">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="16a9e-159">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "AAMkADA1MHgwAAA=",
  "createdDateTime": "2016-04-22T15:19:18.9526004-07:00",
  "lastModifiedDateTime": "2016-04-22T15:19:19.015101-07:00",
  "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIW9XXA==",
  "categories": [],
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
  "hasAttachments": false,
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
  ]
}
-->
