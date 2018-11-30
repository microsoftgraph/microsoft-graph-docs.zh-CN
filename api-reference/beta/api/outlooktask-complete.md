---
title: outlookTask： 完整
description: '完成将**completedDateTime**属性设置为当前日期，其 Outlook 任务 '
ms.openlocfilehash: 732da0f3eb03f6a4674e1254586ae21b5f3334bb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047704"
---
# <a name="outlooktask-complete"></a><span data-ttu-id="eb585-103">outlookTask： 完整</span><span class="sxs-lookup"><span data-stu-id="eb585-103">outlookTask: complete</span></span>

> <span data-ttu-id="eb585-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="eb585-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eb585-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="eb585-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eb585-106">完成 Outlook 任务的设置将**completedDateTime**属性设为当前日期，并将**状态**属性设为`completed`。</span><span class="sxs-lookup"><span data-stu-id="eb585-106">Complete an Outlook task which sets the **completedDateTime** property to the current date, and the **status** property to `completed`.</span></span>

<span data-ttu-id="eb585-107">如果要在响应中，在定期系列中的任务完成任务集合将包含在系列中，已完成的任务和下一个任务的系列。</span><span class="sxs-lookup"><span data-stu-id="eb585-107">If you are completing a task in a recurring series, in the response, the task collection will contain the completed task in the series, and the next task in the series.</span></span>

<span data-ttu-id="eb585-108">**CompletedDateTime**属性表示任务已完成时的日期。</span><span class="sxs-lookup"><span data-stu-id="eb585-108">The **completedDateTime** property represents the date when the task is finished.</span></span> <span data-ttu-id="eb585-109">默认情况下， **completedDateTime**的时间部分设置为午夜 UTC。</span><span class="sxs-lookup"><span data-stu-id="eb585-109">The time portion of **completedDateTime** is set to midnight UTC by default.</span></span> 

<span data-ttu-id="eb585-110">默认情况下，此操作 （和 POST、 获取、 和修补程序任务操作） 返回与日期相关的属性采用 UTC。</span><span class="sxs-lookup"><span data-stu-id="eb585-110">By default, this operation (and the POST, GET, and PATCH task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="eb585-111">您可以使用`Prefer: outlook.timezone`标头，使其具有不同于 UTC 时区中表示的响应中的所有日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="eb585-111">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb585-112">权限</span><span class="sxs-lookup"><span data-stu-id="eb585-112">Permissions</span></span>
<span data-ttu-id="eb585-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eb585-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb585-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb585-115">Permission type</span></span>      | <span data-ttu-id="eb585-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eb585-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb585-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb585-117">Delegated (work or school account)</span></span> | <span data-ttu-id="eb585-118">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb585-118">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="eb585-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb585-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb585-120">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eb585-120">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="eb585-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb585-121">Application</span></span> | <span data-ttu-id="eb585-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb585-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb585-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb585-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/complete
POST /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}/complete
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}/complete

```
## <a name="request-headers"></a><span data-ttu-id="eb585-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="eb585-124">Request headers</span></span>
| <span data-ttu-id="eb585-125">名称</span><span class="sxs-lookup"><span data-stu-id="eb585-125">Name</span></span>       | <span data-ttu-id="eb585-126">说明</span><span class="sxs-lookup"><span data-stu-id="eb585-126">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="eb585-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb585-127">Authorization</span></span>  | <span data-ttu-id="eb585-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eb585-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="eb585-130">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="eb585-130">Prefer: outlook.timezone</span></span> | <span data-ttu-id="eb585-131">响应，它可以采用 UTC 如果未指定此标头中指定的时间属性的时区。</span><span class="sxs-lookup"><span data-stu-id="eb585-131">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="eb585-132">可选。</span><span class="sxs-lookup"><span data-stu-id="eb585-132">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb585-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="eb585-133">Request body</span></span>

## <a name="response"></a><span data-ttu-id="eb585-134">响应</span><span class="sxs-lookup"><span data-stu-id="eb585-134">Response</span></span>

<span data-ttu-id="eb585-135">如果成功，此方法返回`200 OK`响应正文中的响应代码和[outlookTask](../resources/outlooktask.md)集合的对象。</span><span class="sxs-lookup"><span data-stu-id="eb585-135">If successful, this method returns `200 OK` response code and [outlookTask](../resources/outlooktask.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb585-136">示例</span><span class="sxs-lookup"><span data-stu-id="eb585-136">Example</span></span>
<span data-ttu-id="eb585-137">下面的示例将标记指定为已完成的任务。</span><span class="sxs-lookup"><span data-stu-id="eb585-137">The following example marks the specified task as complete.</span></span> <span data-ttu-id="eb585-138">指定太平洋标准时间 (PST) 中`Prefer: outlook.timezone`标头。</span><span class="sxs-lookup"><span data-stu-id="eb585-138">It specifies Pacific Standard Time (PST) in the `Prefer: outlook.timezone` header.</span></span>
##### <a name="request"></a><span data-ttu-id="eb585-139">请求</span><span class="sxs-lookup"><span data-stu-id="eb585-139">Request</span></span>
<span data-ttu-id="eb585-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eb585-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "outlooktask_complete"
}-->
```http
POST https://graph.microsoft.com/beta/me/tasks('AAMkADA1MT15rfAAA=')/complete
Prefer: outlook.timezone="Pacific Standard Time"
```

##### <a name="response"></a><span data-ttu-id="eb585-141">响应</span><span class="sxs-lookup"><span data-stu-id="eb585-141">Response</span></span>
<span data-ttu-id="eb585-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="eb585-142">Here is an example of the response.</span></span> <span data-ttu-id="eb585-143">以太平洋标准时间表示**completedDateTime**和响应中其他与日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="eb585-143">The **completedDateTime** and other date-related properties in the response are expressed in PST.</span></span> 

<span data-ttu-id="eb585-p109">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="eb585-p109">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "id": "AAMkADA1MT15rfAAA=",
      "createdDateTime": "2016-04-21T22:44:01.2012012-07:00",
      "lastModifiedDateTime": "2016-04-22T19:28:38.5300447-07:00",
      "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIW9XYQ==",
      "categories": [
      ],
      "assignedTo": null,
      "body": {
          "contentType": "text",
          "content": ""
      },
      "completedDateTime": {
          "dateTime": "2016-04-22T00:00:00.0000000",
          "timeZone": "Pacific Standard Time"
      },
      "dueDateTime": {
          "dateTime": "2016-04-25T00:00:00.0000000",
          "timeZone": "Pacific Standard Time"
      },
      "hasAttachments":false,
      "importance": "normal",
      "isReminderOn": false,
      "owner": "Administrator",
      "parentFolderId": "AQMkADA1MTIBEgAAAA==",
      "recurrence": null,
      "reminderDateTime": null,
      "sensitivity": "normal",
      "startDateTime": {
          "dateTime": "2016-04-21T00:00:00.0000000",
          "timeZone": "Pacific Standard Time"
      },
      "status": "completed",
      "subject": "Shop for dinner"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookTask: complete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->