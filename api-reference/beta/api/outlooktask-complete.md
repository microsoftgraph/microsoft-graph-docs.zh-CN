---
title: outlookTask： 完整
description: '完成将**completedDateTime**属性设置为当前日期，其 Outlook 任务 '
localization_priority: Normal
ms.openlocfilehash: 6a033624a1fafbc30b200550acc466f7fdb432d6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891915"
---
# <a name="outlooktask-complete"></a><span data-ttu-id="c8f66-103">outlookTask： 完整</span><span class="sxs-lookup"><span data-stu-id="c8f66-103">outlookTask: complete</span></span>

> <span data-ttu-id="c8f66-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c8f66-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8f66-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c8f66-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c8f66-106">完成 Outlook 任务的设置将**completedDateTime**属性设为当前日期，并将**状态**属性设为`completed`。</span><span class="sxs-lookup"><span data-stu-id="c8f66-106">Complete an Outlook task which sets the **completedDateTime** property to the current date, and the **status** property to `completed`.</span></span>

<span data-ttu-id="c8f66-107">如果要在响应中，在定期系列中的任务完成任务集合将包含在系列中，已完成的任务和下一个任务的系列。</span><span class="sxs-lookup"><span data-stu-id="c8f66-107">If you are completing a task in a recurring series, in the response, the task collection will contain the completed task in the series, and the next task in the series.</span></span>

<span data-ttu-id="c8f66-108">**CompletedDateTime**属性表示任务已完成时的日期。</span><span class="sxs-lookup"><span data-stu-id="c8f66-108">The **completedDateTime** property represents the date when the task is finished.</span></span> <span data-ttu-id="c8f66-109">默认情况下， **completedDateTime**的时间部分设置为午夜 UTC。</span><span class="sxs-lookup"><span data-stu-id="c8f66-109">The time portion of **completedDateTime** is set to midnight UTC by default.</span></span>

<span data-ttu-id="c8f66-110">默认情况下，此操作 （和 POST、 获取、 和修补程序任务操作） 返回与日期相关的属性采用 UTC。</span><span class="sxs-lookup"><span data-stu-id="c8f66-110">By default, this operation (and the POST, GET, and PATCH task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="c8f66-111">您可以使用`Prefer: outlook.timezone`标头，使其具有不同于 UTC 时区中表示的响应中的所有日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="c8f66-111">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8f66-112">权限</span><span class="sxs-lookup"><span data-stu-id="c8f66-112">Permissions</span></span>

<span data-ttu-id="c8f66-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c8f66-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8f66-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="c8f66-115">Permission type</span></span>      | <span data-ttu-id="c8f66-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c8f66-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8f66-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c8f66-117">Delegated (work or school account)</span></span> | <span data-ttu-id="c8f66-118">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8f66-118">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="c8f66-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c8f66-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8f66-120">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8f66-120">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="c8f66-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="c8f66-121">Application</span></span> | <span data-ttu-id="c8f66-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="c8f66-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8f66-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c8f66-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/complete
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/complete
```

## <a name="request-headers"></a><span data-ttu-id="c8f66-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="c8f66-124">Request headers</span></span>

| <span data-ttu-id="c8f66-125">名称</span><span class="sxs-lookup"><span data-stu-id="c8f66-125">Name</span></span>       | <span data-ttu-id="c8f66-126">说明</span><span class="sxs-lookup"><span data-stu-id="c8f66-126">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c8f66-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8f66-127">Authorization</span></span>  | <span data-ttu-id="c8f66-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c8f66-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c8f66-130">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="c8f66-130">Prefer: outlook.timezone</span></span> | <span data-ttu-id="c8f66-131">响应，它可以采用 UTC 如果未指定此标头中指定的时间属性的时区。</span><span class="sxs-lookup"><span data-stu-id="c8f66-131">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="c8f66-132">可选。</span><span class="sxs-lookup"><span data-stu-id="c8f66-132">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8f66-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="c8f66-133">Request body</span></span>

<span data-ttu-id="c8f66-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c8f66-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8f66-135">响应</span><span class="sxs-lookup"><span data-stu-id="c8f66-135">Response</span></span>

<span data-ttu-id="c8f66-136">如果成功，此方法返回`200 OK`响应代码和响应正文中的[outlookTask](../resources/outlooktask.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c8f66-136">If successful, this method returns `200 OK` response code and the [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8f66-137">示例</span><span class="sxs-lookup"><span data-stu-id="c8f66-137">Example</span></span>

<span data-ttu-id="c8f66-138">下面的示例将标记指定为已完成的任务。</span><span class="sxs-lookup"><span data-stu-id="c8f66-138">The following example marks the specified task as complete.</span></span> <span data-ttu-id="c8f66-139">指定太平洋标准时间 (PST) 中`Prefer: outlook.timezone`标头。</span><span class="sxs-lookup"><span data-stu-id="c8f66-139">It specifies Pacific Standard Time (PST) in the `Prefer: outlook.timezone` header.</span></span>

### <a name="request"></a><span data-ttu-id="c8f66-140">请求</span><span class="sxs-lookup"><span data-stu-id="c8f66-140">Request</span></span>

<span data-ttu-id="c8f66-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c8f66-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "outlooktask_complete"
}-->

```http
POST https://graph.microsoft.com/beta/me/tasks('AAMkADA1MT15rfAAA=')/complete
Prefer: outlook.timezone="Pacific Standard Time"
```

### <a name="response"></a><span data-ttu-id="c8f66-142">响应</span><span class="sxs-lookup"><span data-stu-id="c8f66-142">Response</span></span>

<span data-ttu-id="c8f66-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c8f66-143">Here is an example of the response.</span></span> <span data-ttu-id="c8f66-144">以太平洋标准时间表示**completedDateTime**和响应中其他与日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="c8f66-144">The **completedDateTime** and other date-related properties in the response are expressed in PST.</span></span>

> <span data-ttu-id="c8f66-145">**注意：** 为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c8f66-145">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c8f66-146">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c8f66-146">All of the properties will be returned from an actual call.</span></span>
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
