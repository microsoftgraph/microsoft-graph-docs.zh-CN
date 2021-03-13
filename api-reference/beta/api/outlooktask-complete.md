---
title: outlookTask：完成
description: '完成将 **completedDateTime** 属性设置为当前日期的 Outlook 任务。 '
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 09a8f9d46597d96d51d5bd66f7fcac750e46809c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775533"
---
# <a name="outlooktask-complete-deprecated"></a><span data-ttu-id="fe201-103">outlookTask：完成 (弃) </span><span class="sxs-lookup"><span data-stu-id="fe201-103">outlookTask: complete (deprecated)</span></span>

<span data-ttu-id="fe201-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe201-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="fe201-105">完成 Outlook 任务，该任务将 **completedDateTime** 属性设置为当前日期， **将 status** 属性设置成 `completed` 。</span><span class="sxs-lookup"><span data-stu-id="fe201-105">Complete an Outlook task which sets the **completedDateTime** property to the current date, and the **status** property to `completed`.</span></span>

<span data-ttu-id="fe201-106">如果要完成定期系列中的任务，在响应中，任务集合将包含该系列中已完成的任务以及该系列中的下一个任务。</span><span class="sxs-lookup"><span data-stu-id="fe201-106">If you are completing a task in a recurring series, in the response, the task collection will contain the completed task in the series, and the next task in the series.</span></span>

<span data-ttu-id="fe201-107">**completedDateTime** 属性表示任务完成的日期。</span><span class="sxs-lookup"><span data-stu-id="fe201-107">The **completedDateTime** property represents the date when the task is finished.</span></span> <span data-ttu-id="fe201-108">默认情况下 **，completedDateTime** 的时间部分设置为午夜 UTC。</span><span class="sxs-lookup"><span data-stu-id="fe201-108">The time portion of **completedDateTime** is set to midnight UTC by default.</span></span>

<span data-ttu-id="fe201-109">默认情况下，此操作 (POST、GET 和 PATCH 任务) UTC 格式返回与日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="fe201-109">By default, this operation (and the POST, GET, and PATCH task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="fe201-110">你可以使用 `Prefer: outlook.timezone` 标头将响应中的所有与日期相关的属性都表示为与 UTC 不同的时区。</span><span class="sxs-lookup"><span data-stu-id="fe201-110">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe201-111">权限</span><span class="sxs-lookup"><span data-stu-id="fe201-111">Permissions</span></span>

<span data-ttu-id="fe201-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fe201-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe201-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="fe201-114">Permission type</span></span>      | <span data-ttu-id="fe201-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fe201-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe201-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fe201-116">Delegated (work or school account)</span></span> | <span data-ttu-id="fe201-117">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe201-117">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="fe201-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fe201-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe201-119">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe201-119">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="fe201-120">Application</span><span class="sxs-lookup"><span data-stu-id="fe201-120">Application</span></span> | <span data-ttu-id="fe201-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe201-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe201-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe201-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/complete
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/complete
```

## <a name="request-headers"></a><span data-ttu-id="fe201-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="fe201-123">Request headers</span></span>

| <span data-ttu-id="fe201-124">名称</span><span class="sxs-lookup"><span data-stu-id="fe201-124">Name</span></span>       | <span data-ttu-id="fe201-125">说明</span><span class="sxs-lookup"><span data-stu-id="fe201-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fe201-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe201-126">Authorization</span></span>  | <span data-ttu-id="fe201-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fe201-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fe201-129">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="fe201-129">Prefer: outlook.timezone</span></span> | <span data-ttu-id="fe201-130">指定响应中时间属性的时区，如果未指定此标头，则其时区为 UTC。</span><span class="sxs-lookup"><span data-stu-id="fe201-130">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="fe201-131">可选。</span><span class="sxs-lookup"><span data-stu-id="fe201-131">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe201-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="fe201-132">Request body</span></span>

<span data-ttu-id="fe201-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fe201-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe201-134">响应</span><span class="sxs-lookup"><span data-stu-id="fe201-134">Response</span></span>

<span data-ttu-id="fe201-135">如果成功，此方法在 `200 OK` 响应正文中返回 响应代码和 [outlookTask](../resources/outlooktask.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fe201-135">If successful, this method returns `200 OK` response code and the [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe201-136">示例</span><span class="sxs-lookup"><span data-stu-id="fe201-136">Example</span></span>

<span data-ttu-id="fe201-137">以下示例将指定任务标记为已完成。</span><span class="sxs-lookup"><span data-stu-id="fe201-137">The following example marks the specified task as complete.</span></span> <span data-ttu-id="fe201-138">它在标头中指定太平洋标准 (PST) `Prefer: outlook.timezone` PST 时间。</span><span class="sxs-lookup"><span data-stu-id="fe201-138">It specifies Pacific Standard Time (PST) in the `Prefer: outlook.timezone` header.</span></span>

### <a name="request"></a><span data-ttu-id="fe201-139">请求</span><span class="sxs-lookup"><span data-stu-id="fe201-139">Request</span></span>

<span data-ttu-id="fe201-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fe201-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fe201-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe201-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "outlooktask_complete"
}-->

```http
POST https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MT15rfAAA=')/complete
Prefer: outlook.timezone="Pacific Standard Time"
```
# <a name="c"></a>[<span data-ttu-id="fe201-142">C#</span><span class="sxs-lookup"><span data-stu-id="fe201-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/outlooktask-complete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fe201-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe201-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/outlooktask-complete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fe201-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe201-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/outlooktask-complete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fe201-145">Java</span><span class="sxs-lookup"><span data-stu-id="fe201-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/outlooktask-complete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fe201-146">响应</span><span class="sxs-lookup"><span data-stu-id="fe201-146">Response</span></span>

<span data-ttu-id="fe201-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fe201-147">Here is an example of the response.</span></span> <span data-ttu-id="fe201-148">**响应中的 completedDateTime** 和其他与日期相关的属性以 PST 表示。</span><span class="sxs-lookup"><span data-stu-id="fe201-148">The **completedDateTime** and other date-related properties in the response are expressed in PST.</span></span>

> <span data-ttu-id="fe201-149">**注意：** 为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="fe201-149">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fe201-150">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fe201-150">All of the properties will be returned from an actual call.</span></span>
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


