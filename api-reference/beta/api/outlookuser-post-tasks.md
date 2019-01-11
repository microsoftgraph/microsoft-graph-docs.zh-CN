---
title: 创建 outlookTask
description: 创建 Outlook 任务中的默认任务组 (`My Tasks`) 和默认任务文件夹 (`Tasks`) 用户的邮箱中。
localization_priority: Normal
ms.openlocfilehash: c158af6ac5125bb410bcbe57a1cb26b8cd955e28
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853737"
---
# <a name="create-outlooktask"></a><span data-ttu-id="0def9-103">创建 outlookTask</span><span class="sxs-lookup"><span data-stu-id="0def9-103">Create outlookTask</span></span>

> <span data-ttu-id="0def9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0def9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0def9-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0def9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0def9-106">创建 Outlook 任务中的默认任务组 (`My Tasks`) 和默认任务文件夹 (`Tasks`) 用户的邮箱中。</span><span class="sxs-lookup"><span data-stu-id="0def9-106">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>

<span data-ttu-id="0def9-107">POST 方法始终将忽略的时间部分的**开始日期时间**和**dueDateTime**在请求正文中，并假定为始终中指定的时区的午夜的时间。</span><span class="sxs-lookup"><span data-stu-id="0def9-107">The POST method always ignores the time portion of **startDateTime** and **dueDateTime** in the request body, and assumes the time to be always midnight in the specified time zone.</span></span>

<span data-ttu-id="0def9-108">默认情况下，此操作 （和 GET、 修补程序，并[完成](../api/outlooktask-complete.md)任务操作） 返回与日期相关的属性采用 UTC。</span><span class="sxs-lookup"><span data-stu-id="0def9-108">By default, this operation (and the GET, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="0def9-109">您可以使用`Prefer: outlook.timezone`标头，使其具有不同于 UTC 时区中表示的响应中的所有日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="0def9-109">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="0def9-110">权限</span><span class="sxs-lookup"><span data-stu-id="0def9-110">Permissions</span></span>
<span data-ttu-id="0def9-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0def9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0def9-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="0def9-113">Permission type</span></span>      | <span data-ttu-id="0def9-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0def9-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0def9-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0def9-115">Delegated (work or school account)</span></span> | <span data-ttu-id="0def9-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0def9-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="0def9-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0def9-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0def9-118">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0def9-118">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="0def9-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="0def9-119">Application</span></span> | <span data-ttu-id="0def9-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="0def9-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0def9-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0def9-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/tasks
```
## <a name="request-headers"></a><span data-ttu-id="0def9-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="0def9-122">Request headers</span></span>
| <span data-ttu-id="0def9-123">名称</span><span class="sxs-lookup"><span data-stu-id="0def9-123">Name</span></span>       | <span data-ttu-id="0def9-124">说明</span><span class="sxs-lookup"><span data-stu-id="0def9-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0def9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0def9-125">Authorization</span></span>  | <span data-ttu-id="0def9-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0def9-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0def9-128">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="0def9-128">Prefer: outlook.timezone</span></span> | <span data-ttu-id="0def9-129">响应，它可以采用 UTC 如果未指定此标头中指定的时间属性的时区。</span><span class="sxs-lookup"><span data-stu-id="0def9-129">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="0def9-130">可选。</span><span class="sxs-lookup"><span data-stu-id="0def9-130">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0def9-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="0def9-131">Request body</span></span>
<span data-ttu-id="0def9-132">在请求正文中，提供[outlookTask](../resources/outlooktask.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0def9-132">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0def9-133">响应</span><span class="sxs-lookup"><span data-stu-id="0def9-133">Response</span></span>

<span data-ttu-id="0def9-134">如果成功，此方法返回`201 Created`响应正文中的响应代码和[outlookTask](../resources/outlooktask.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0def9-134">If successful, this method returns `201 Created` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0def9-135">示例</span><span class="sxs-lookup"><span data-stu-id="0def9-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0def9-136">请求</span><span class="sxs-lookup"><span data-stu-id="0def9-136">Request</span></span>
<span data-ttu-id="0def9-137">下面的示例演示如何使用`Prefer: outlook.timezone`标头。</span><span class="sxs-lookup"><span data-stu-id="0def9-137">The following example shows the use of the `Prefer: outlook.timezone` header.</span></span> <span data-ttu-id="0def9-138">它创建任务，表示**开始日期时间**和**dueDateTime**在东部标准时间 (EST)，并且包括`Prefer`标头的太平洋标准时间 (PST)。</span><span class="sxs-lookup"><span data-stu-id="0def9-138">It creates a task, expresses **startDateTime** and **dueDateTime** in Eastern Standard Time (EST), and includes a `Prefer` header of Pacific Standard Time (PST).</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlooktask_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/tasks
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json
Content-length: 276

{
  "assignedTo": "Dana Swope",
  "subject": "Shop for children's weekend",
  "startDateTime": {
      "dateTime": "2016-05-03T09:00:00",
      "timeZone": "Eastern Standard Time"
  },
  "dueDateTime":  {
      "dateTime": "2016-05-05T16:00:00",
      "timeZone": "Eastern Standard Time"
  }
}
```
<span data-ttu-id="0def9-139">在请求正文中，提供[outlookTask](../resources/outlooktask.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0def9-139">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0def9-140">响应</span><span class="sxs-lookup"><span data-stu-id="0def9-140">Response</span></span>
<span data-ttu-id="0def9-141">POST 方法将忽略的**开始日期时间**和**dueDateTime**在请求正文中的时间部分，并假定为始终午夜指定时区 (EST) 中的时间。</span><span class="sxs-lookup"><span data-stu-id="0def9-141">The POST method ignores the time portion of **startDateTime** and **dueDateTime** in the request body and assumes the time to be always midnight in the specified time zone (EST).</span></span>

<span data-ttu-id="0def9-142">由于`Prefer`标头指定 PST、 POST 方法表示 PST 中的响应中所有的日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="0def9-142">Since the `Prefer` header specifies PST, the POST method expresses all the date-related properties in the response in PST.</span></span> <span data-ttu-id="0def9-143">具体而言的**开始日期时间**和**dueDateTime**属性，POST 方法将在东部时间午夜转换为太平洋标准时间，并返回其中 PST 的响应中。</span><span class="sxs-lookup"><span data-stu-id="0def9-143">In particular, for the **startDateTime** and **dueDateTime** properties, the POST method converts midnight in EST to PST and returns them in PST in the response.</span></span>

<span data-ttu-id="0def9-p108">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0def9-p108">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->
```http
HTTP/1.1 201 Created
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
    "contentType": "Text",
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
  "sensitivity": "Normal",
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
  "description": "Create outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
