---
title: 列出任务
description: 获取用户邮箱中的所有 Outlook 任务。
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 86b4b7ee0a990dd3fa6ec88157238041c37ea980
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849182"
---
# <a name="list-tasks"></a><span data-ttu-id="d789a-103">列出任务</span><span class="sxs-lookup"><span data-stu-id="d789a-103">List tasks</span></span>

<span data-ttu-id="d789a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d789a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="d789a-105">获取用户邮箱中的所有 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="d789a-105">Get all the Outlook tasks in the user's mailbox.</span></span>

<span data-ttu-id="d789a-106">默认情况下，此操作会 (POST、PATCH 和 [完成](../api/outlooktask-complete.md) 的任务操作) 返回与日期相关的属性) 以 UTC 格式返回日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="d789a-106">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span>
<span data-ttu-id="d789a-107">你可以使用 `Prefer: outlook.timezone` 标头将响应中的所有与日期相关的属性都表示为与 UTC 不同的时区。</span><span class="sxs-lookup"><span data-stu-id="d789a-107">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span> <span data-ttu-id="d789a-108">参 [阅用于](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time) 获取单项任务的示例。</span><span class="sxs-lookup"><span data-stu-id="d789a-108">See an [example](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time) for getting a single task.</span></span> <span data-ttu-id="d789a-109">可以同样应用标头来获取多个任务。</span><span class="sxs-lookup"><span data-stu-id="d789a-109">You can apply the header similarly to get multiple tasks.</span></span>

## <a name="permissions"></a><span data-ttu-id="d789a-110">权限</span><span class="sxs-lookup"><span data-stu-id="d789a-110">Permissions</span></span>
<span data-ttu-id="d789a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d789a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d789a-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="d789a-113">Permission type</span></span>      | <span data-ttu-id="d789a-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d789a-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d789a-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d789a-115">Delegated (work or school account)</span></span> | <span data-ttu-id="d789a-116">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="d789a-116">Tasks.Read</span></span>    |
|<span data-ttu-id="d789a-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d789a-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d789a-118">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="d789a-118">Tasks.Read</span></span>    |
|<span data-ttu-id="d789a-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="d789a-119">Application</span></span> | <span data-ttu-id="d789a-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="d789a-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d789a-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d789a-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/tasks
GET /users/{id|userPrincipalName}/outlook/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d789a-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d789a-122">Optional query parameters</span></span>
<span data-ttu-id="d789a-123">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d789a-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d789a-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="d789a-124">Request headers</span></span>
| <span data-ttu-id="d789a-125">名称</span><span class="sxs-lookup"><span data-stu-id="d789a-125">Name</span></span>      |<span data-ttu-id="d789a-126">说明</span><span class="sxs-lookup"><span data-stu-id="d789a-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d789a-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="d789a-127">Authorization</span></span>  | <span data-ttu-id="d789a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d789a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d789a-130">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="d789a-130">Prefer: outlook.timezone</span></span> | <span data-ttu-id="d789a-131">指定响应中的时区（如果未指定此标头，则该属性为 UTC 时间）。</span><span class="sxs-lookup"><span data-stu-id="d789a-131">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="d789a-132">可选。</span><span class="sxs-lookup"><span data-stu-id="d789a-132">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d789a-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="d789a-133">Request body</span></span>
<span data-ttu-id="d789a-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d789a-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d789a-135">响应</span><span class="sxs-lookup"><span data-stu-id="d789a-135">Response</span></span>

<span data-ttu-id="d789a-136">如果成功，此方法在响应 `200 OK` 正文中返回 [响应代码和 outlookTask](../resources/outlooktask.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d789a-136">If successful, this method returns a `200 OK` response code and collection of [outlookTask](../resources/outlooktask.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d789a-137">示例</span><span class="sxs-lookup"><span data-stu-id="d789a-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d789a-138">请求</span><span class="sxs-lookup"><span data-stu-id="d789a-138">Request</span></span>
<span data-ttu-id="d789a-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d789a-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d789a-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="d789a-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "outlookuser_get_tasks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/tasks
```
# <a name="c"></a>[<span data-ttu-id="d789a-141">C#</span><span class="sxs-lookup"><span data-stu-id="d789a-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/outlookuser-get-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d789a-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d789a-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/outlookuser-get-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d789a-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d789a-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/outlookuser-get-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d789a-144">响应</span><span class="sxs-lookup"><span data-stu-id="d789a-144">Response</span></span>
<span data-ttu-id="d789a-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d789a-145">Here is an example of the response.</span></span> <span data-ttu-id="d789a-146">默认情况下，响应中的 date-time 属性采用的是 UTC。</span><span class="sxs-lookup"><span data-stu-id="d789a-146">By default, the date-time properties in the response are in UTC.</span></span>

<span data-ttu-id="d789a-p106">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d789a-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
