---
title: 获取 outlookTask
description: 获取用户邮箱中的 Outlook 任务的属性和关系。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 588a609cc2c27abbaa47f7d06e8c1881705bd786
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338020"
---
# <a name="get-outlooktask"></a><span data-ttu-id="5590b-103">获取 outlookTask</span><span class="sxs-lookup"><span data-stu-id="5590b-103">Get outlookTask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5590b-104">获取用户邮箱中的 Outlook 任务的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5590b-104">Get the properties and relationships of an Outlook task in the user's mailbox.</span></span>

<span data-ttu-id="5590b-105">默认情况下, 此操作 (以及发布、修补和[完成](../api/outlooktask-complete.md)任务操作) 返回 UTC 格式的与日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="5590b-105">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="5590b-106">你可以使用 `Prefer: outlook.timezone` 标头将响应中的所有与日期相关的属性都表示为与 UTC 不同的时区。</span><span class="sxs-lookup"><span data-stu-id="5590b-106">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="5590b-107">权限</span><span class="sxs-lookup"><span data-stu-id="5590b-107">Permissions</span></span>

<span data-ttu-id="5590b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5590b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5590b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5590b-110">Permission type</span></span>                        | <span data-ttu-id="5590b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5590b-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="5590b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5590b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5590b-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="5590b-113">Tasks.Read</span></span>                          |
| <span data-ttu-id="5590b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5590b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5590b-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="5590b-115">Tasks.Read</span></span>                          |
| <span data-ttu-id="5590b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5590b-116">Application</span></span>                            | <span data-ttu-id="5590b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5590b-117">Not supported.</span></span>                      |

## <a name="http-request"></a><span data-ttu-id="5590b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5590b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}
GET /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5590b-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5590b-119">Optional query parameters</span></span>

<span data-ttu-id="5590b-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5590b-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5590b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="5590b-121">Request headers</span></span>

| <span data-ttu-id="5590b-122">名称</span><span class="sxs-lookup"><span data-stu-id="5590b-122">Name</span></span>                     | <span data-ttu-id="5590b-123">说明</span><span class="sxs-lookup"><span data-stu-id="5590b-123">Description</span></span>                                       |
|:-------------------------|:--------------------------------------------------|
| <span data-ttu-id="5590b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5590b-124">Authorization</span></span>            | <span data-ttu-id="5590b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5590b-p103">Bearer {token}. Required.</span></span>                         |
| <span data-ttu-id="5590b-127">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="5590b-127">Prefer: outlook.timezone</span></span> | <span data-ttu-id="5590b-128">指定响应中时间属性的时区 (如果未指定此标头, 则采用 UTC 格式表示)。</span><span class="sxs-lookup"><span data-stu-id="5590b-128">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="5590b-129">可选。</span><span class="sxs-lookup"><span data-stu-id="5590b-129">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5590b-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="5590b-130">Request body</span></span>

<span data-ttu-id="5590b-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5590b-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5590b-132">响应</span><span class="sxs-lookup"><span data-stu-id="5590b-132">Response</span></span>

<span data-ttu-id="5590b-133">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[outlookTask](../resources/outlooktask.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5590b-133">If successful, this method returns a `200 OK` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5590b-134">示例</span><span class="sxs-lookup"><span data-stu-id="5590b-134">Examples</span></span>

### <a name="example-1-get-an-outlook-task"></a><span data-ttu-id="5590b-135">示例 1: 获取 Outlook 任务</span><span class="sxs-lookup"><span data-stu-id="5590b-135">Example 1: Get an Outlook task</span></span>

#### <a name="request"></a><span data-ttu-id="5590b-136">请求</span><span class="sxs-lookup"><span data-stu-id="5590b-136">Request</span></span>

<span data-ttu-id="5590b-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5590b-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->

```http
GET https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADA1MTrgAAA=
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="5590b-138">响应</span><span class="sxs-lookup"><span data-stu-id="5590b-138">Response</span></span>

<span data-ttu-id="5590b-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5590b-139">Here is an example of the response.</span></span> <span data-ttu-id="5590b-140">默认情况下，响应中的 date-time 属性采用的是 UTC。</span><span class="sxs-lookup"><span data-stu-id="5590b-140">By default, the date-time properties in the response are in UTC.</span></span>

> <span data-ttu-id="5590b-141">**注意：** 为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5590b-141">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5590b-142">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5590b-142">All of the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time"></a><span data-ttu-id="5590b-143">示例 2: 在太平洋标准时间内使用日期时间属性获取 Outlook 任务</span><span class="sxs-lookup"><span data-stu-id="5590b-143">Example 2: Get Outlook task with date-time properties in Pacific Standard Time</span></span>

#### <a name="request"></a><span data-ttu-id="5590b-144">请求</span><span class="sxs-lookup"><span data-stu-id="5590b-144">Request</span></span>

<span data-ttu-id="5590b-145">此示例使用`Prefer: outlook.timezone`标头来指定 API 应在太平洋标准时间的响应中返回日期时间属性。</span><span class="sxs-lookup"><span data-stu-id="5590b-145">This example uses the `Prefer: outlook.timezone` header to specify that the API should return date-time properties in the response in Pacific Standard Time.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->

```http
GET https://graph.microsoft.com/beta/me/outlook/tasks/AAMkADA1MHgwAAA=
Prefer: outlook.timezone="Pacific Standard Time"
```

### <a name="response"></a><span data-ttu-id="5590b-146">响应</span><span class="sxs-lookup"><span data-stu-id="5590b-146">Response</span></span>

<span data-ttu-id="5590b-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5590b-147">Here is an example of the response.</span></span> <span data-ttu-id="5590b-148">响应中的日期-时间属性以指定的太平洋标准时间返回。</span><span class="sxs-lookup"><span data-stu-id="5590b-148">The date-time properties in the response are returned in the specified Pacific Standard Time.</span></span>

> <span data-ttu-id="5590b-149">**注意：** 为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5590b-149">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5590b-150">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5590b-150">All of the properties will be returned from an actual call.</span></span>

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
  "suppressions": []
}
-->
