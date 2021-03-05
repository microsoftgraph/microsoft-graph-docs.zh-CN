---
title: outlookTask： complete
description: '完成将 **completedDateTime** 属性设置为当前日期的 Outlook 任务， '
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: edf7f24efc2a3c208a1aed4c4a03e41ad596c4c4
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471843"
---
# <a name="outlooktask-complete-deprecated"></a><span data-ttu-id="ee694-103">outlookTask：完成 (已弃) </span><span class="sxs-lookup"><span data-stu-id="ee694-103">outlookTask: complete (deprecated)</span></span>

<span data-ttu-id="ee694-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee694-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="ee694-105">完成 Outlook 任务，将 **completedDateTime** 属性设置为当前日期， **状态** 属性为 `completed` 。</span><span class="sxs-lookup"><span data-stu-id="ee694-105">Complete an Outlook task which sets the **completedDateTime** property to the current date, and the **status** property to `completed`.</span></span>

<span data-ttu-id="ee694-106">如果要完成定期系列中的任务，在响应中，任务集合将包含该系列中已完成的任务以及该系列中的下一个任务。</span><span class="sxs-lookup"><span data-stu-id="ee694-106">If you are completing a task in a recurring series, in the response, the task collection will contain the completed task in the series, and the next task in the series.</span></span>

<span data-ttu-id="ee694-107">**completedDateTime 属性** 表示任务完成的日期。</span><span class="sxs-lookup"><span data-stu-id="ee694-107">The **completedDateTime** property represents the date when the task is finished.</span></span> <span data-ttu-id="ee694-108">默认情况下 **，completedDateTime** 的时间部分设置为午夜 UTC。</span><span class="sxs-lookup"><span data-stu-id="ee694-108">The time portion of **completedDateTime** is set to midnight UTC by default.</span></span>

<span data-ttu-id="ee694-109">默认情况下，此操作 (POST、GET 和 PATCH 任务) 返回 UTC 格式的日期相关属性。</span><span class="sxs-lookup"><span data-stu-id="ee694-109">By default, this operation (and the POST, GET, and PATCH task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="ee694-110">你可以使用 `Prefer: outlook.timezone` 标头将响应中的所有与日期相关的属性都表示为与 UTC 不同的时区。</span><span class="sxs-lookup"><span data-stu-id="ee694-110">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee694-111">权限</span><span class="sxs-lookup"><span data-stu-id="ee694-111">Permissions</span></span>

<span data-ttu-id="ee694-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ee694-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee694-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="ee694-114">Permission type</span></span>      | <span data-ttu-id="ee694-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ee694-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee694-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ee694-116">Delegated (work or school account)</span></span> | <span data-ttu-id="ee694-117">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ee694-117">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="ee694-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ee694-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee694-119">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ee694-119">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="ee694-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="ee694-120">Application</span></span> | <span data-ttu-id="ee694-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="ee694-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee694-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ee694-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/complete
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/complete
```

## <a name="request-headers"></a><span data-ttu-id="ee694-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="ee694-123">Request headers</span></span>

| <span data-ttu-id="ee694-124">名称</span><span class="sxs-lookup"><span data-stu-id="ee694-124">Name</span></span>       | <span data-ttu-id="ee694-125">说明</span><span class="sxs-lookup"><span data-stu-id="ee694-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ee694-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee694-126">Authorization</span></span>  | <span data-ttu-id="ee694-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ee694-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ee694-129">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="ee694-129">Prefer: outlook.timezone</span></span> | <span data-ttu-id="ee694-130">指定响应中时间属性的时区，如果未指定此标头，则时区为 UTC。</span><span class="sxs-lookup"><span data-stu-id="ee694-130">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="ee694-131">可选。</span><span class="sxs-lookup"><span data-stu-id="ee694-131">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee694-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="ee694-132">Request body</span></span>

<span data-ttu-id="ee694-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ee694-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee694-134">响应</span><span class="sxs-lookup"><span data-stu-id="ee694-134">Response</span></span>

<span data-ttu-id="ee694-135">如果成功，此方法在 `200 OK` 响应正文中返回响应代码和 [outlookTask](../resources/outlooktask.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ee694-135">If successful, this method returns `200 OK` response code and the [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee694-136">示例</span><span class="sxs-lookup"><span data-stu-id="ee694-136">Example</span></span>

<span data-ttu-id="ee694-137">以下示例将指定任务标记为已完成。</span><span class="sxs-lookup"><span data-stu-id="ee694-137">The following example marks the specified task as complete.</span></span> <span data-ttu-id="ee694-138">它在标头中指定太平洋标准 (PST) `Prefer: outlook.timezone` PST 时间。</span><span class="sxs-lookup"><span data-stu-id="ee694-138">It specifies Pacific Standard Time (PST) in the `Prefer: outlook.timezone` header.</span></span>

### <a name="request"></a><span data-ttu-id="ee694-139">请求</span><span class="sxs-lookup"><span data-stu-id="ee694-139">Request</span></span>

<span data-ttu-id="ee694-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ee694-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "outlooktask_complete"
}-->

```http
POST https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MT15rfAAA=')/complete
Prefer: outlook.timezone="Pacific Standard Time"
```

### <a name="response"></a><span data-ttu-id="ee694-141">响应</span><span class="sxs-lookup"><span data-stu-id="ee694-141">Response</span></span>

<span data-ttu-id="ee694-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ee694-142">Here is an example of the response.</span></span> <span data-ttu-id="ee694-143">**响应中的 completedDateTime** 和其他与日期相关的属性以 PST 表示。</span><span class="sxs-lookup"><span data-stu-id="ee694-143">The **completedDateTime** and other date-related properties in the response are expressed in PST.</span></span>

> <span data-ttu-id="ee694-144">**注意：** 为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ee694-144">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ee694-145">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ee694-145">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "outlookTask: complete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


