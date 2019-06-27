---
title: 列出任务
description: 获取用户邮箱中的所有 Outlook 任务。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: d36be134102710fe0f29e21f73ae03db22b448dd
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269151"
---
# <a name="list-tasks"></a><span data-ttu-id="c1d3e-103">列出任务</span><span class="sxs-lookup"><span data-stu-id="c1d3e-103">List tasks</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1d3e-104">获取用户邮箱中的所有 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="c1d3e-104">Get all the Outlook tasks in the user's mailbox.</span></span>

<span data-ttu-id="c1d3e-105">默认情况下, 此操作 (以及发布、修补和[完成](../api/outlooktask-complete.md)任务操作) 返回 UTC 格式的与日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="c1d3e-105">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span>
<span data-ttu-id="c1d3e-106">你可以使用 `Prefer: outlook.timezone` 标头将响应中的所有与日期相关的属性都表示为与 UTC 不同的时区。</span><span class="sxs-lookup"><span data-stu-id="c1d3e-106">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span> <span data-ttu-id="c1d3e-107">请参阅获取单个任务的[示例](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time)。</span><span class="sxs-lookup"><span data-stu-id="c1d3e-107">See an [example](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time) for getting a single task.</span></span> <span data-ttu-id="c1d3e-108">您可以按类似方式应用标头以获取多个任务。</span><span class="sxs-lookup"><span data-stu-id="c1d3e-108">You can apply the header similarly to get multiple tasks.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1d3e-109">权限</span><span class="sxs-lookup"><span data-stu-id="c1d3e-109">Permissions</span></span>
<span data-ttu-id="c1d3e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1d3e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1d3e-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1d3e-112">Permission type</span></span>      | <span data-ttu-id="c1d3e-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c1d3e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1d3e-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1d3e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c1d3e-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="c1d3e-115">Tasks.Read</span></span>    |
|<span data-ttu-id="c1d3e-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1d3e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1d3e-117">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="c1d3e-117">Tasks.Read</span></span>    |
|<span data-ttu-id="c1d3e-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1d3e-118">Application</span></span> | <span data-ttu-id="c1d3e-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1d3e-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1d3e-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1d3e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/tasks
GET /users/{id|userPrincipalName}/outlook/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c1d3e-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c1d3e-121">Optional query parameters</span></span>
<span data-ttu-id="c1d3e-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c1d3e-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c1d3e-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1d3e-123">Request headers</span></span>
| <span data-ttu-id="c1d3e-124">名称</span><span class="sxs-lookup"><span data-stu-id="c1d3e-124">Name</span></span>      |<span data-ttu-id="c1d3e-125">说明</span><span class="sxs-lookup"><span data-stu-id="c1d3e-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c1d3e-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1d3e-126">Authorization</span></span>  | <span data-ttu-id="c1d3e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c1d3e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c1d3e-129">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="c1d3e-129">Prefer: outlook.timezone</span></span> | <span data-ttu-id="c1d3e-130">指定响应中时间属性的时区 (如果未指定此标头, 则采用 UTC 格式表示)。</span><span class="sxs-lookup"><span data-stu-id="c1d3e-130">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="c1d3e-131">可选。</span><span class="sxs-lookup"><span data-stu-id="c1d3e-131">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1d3e-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1d3e-132">Request body</span></span>
<span data-ttu-id="c1d3e-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c1d3e-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1d3e-134">响应</span><span class="sxs-lookup"><span data-stu-id="c1d3e-134">Response</span></span>

<span data-ttu-id="c1d3e-135">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[outlookTask](../resources/outlooktask.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="c1d3e-135">If successful, this method returns a `200 OK` response code and collection of [outlookTask](../resources/outlooktask.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c1d3e-136">示例</span><span class="sxs-lookup"><span data-stu-id="c1d3e-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c1d3e-137">请求</span><span class="sxs-lookup"><span data-stu-id="c1d3e-137">Request</span></span>
<span data-ttu-id="c1d3e-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c1d3e-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/tasks
```
##### <a name="response"></a><span data-ttu-id="c1d3e-139">响应</span><span class="sxs-lookup"><span data-stu-id="c1d3e-139">Response</span></span>
<span data-ttu-id="c1d3e-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c1d3e-140">Here is an example of the response.</span></span> <span data-ttu-id="c1d3e-141">默认情况下，响应中的 date-time 属性采用的是 UTC。</span><span class="sxs-lookup"><span data-stu-id="c1d3e-141">By default, the date-time properties in the response are in UTC.</span></span>

<span data-ttu-id="c1d3e-p106">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c1d3e-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c1d3e-144">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="c1d3e-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c1d3e-145">C#</span><span class="sxs-lookup"><span data-stu-id="c1d3e-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_tasks-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c1d3e-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="c1d3e-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_tasks-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c1d3e-147">目标-C</span><span class="sxs-lookup"><span data-stu-id="c1d3e-147">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_tasks-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/outlookuser-list-tasks.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/outlookuser-list-tasks.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlookuser-list-tasks.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
