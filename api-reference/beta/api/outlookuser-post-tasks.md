---
title: 创建 outlookTask
description: 在用户邮箱中的默认任务组 (`My Tasks`) 和默认任务文件夹 (`Tasks`) 中创建一个 Outlook 任务。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: f508aa05ad70246584ebc33bfaabc9317205011d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33596088"
---
# <a name="create-outlooktask"></a><span data-ttu-id="0daf8-103">创建 outlookTask</span><span class="sxs-lookup"><span data-stu-id="0daf8-103">Create outlookTask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0daf8-104">在用户邮箱中的默认任务组 (`My Tasks`) 和默认任务文件夹 (`Tasks`) 中创建一个 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="0daf8-104">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>

<span data-ttu-id="0daf8-105">POST 方法始终忽略请求正文中**startDateTime**和**dueDateTime**的时间部分, 并假定指定时区中的时间始终为午夜。</span><span class="sxs-lookup"><span data-stu-id="0daf8-105">The POST method always ignores the time portion of **startDateTime** and **dueDateTime** in the request body, and assumes the time to be always midnight in the specified time zone.</span></span>

<span data-ttu-id="0daf8-106">默认情况下, 此操作 (以及获取、修补和[完成](../api/outlooktask-complete.md)任务操作) 将返回 UTC 格式的与日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="0daf8-106">By default, this operation (and the GET, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="0daf8-107">你可以使用 `Prefer: outlook.timezone` 标头将响应中的所有与日期相关的属性都表示为与 UTC 不同的时区。</span><span class="sxs-lookup"><span data-stu-id="0daf8-107">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="0daf8-108">权限</span><span class="sxs-lookup"><span data-stu-id="0daf8-108">Permissions</span></span>
<span data-ttu-id="0daf8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0daf8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0daf8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0daf8-111">Permission type</span></span>      | <span data-ttu-id="0daf8-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0daf8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0daf8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0daf8-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0daf8-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0daf8-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="0daf8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0daf8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0daf8-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0daf8-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="0daf8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0daf8-117">Application</span></span> | <span data-ttu-id="0daf8-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0daf8-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0daf8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0daf8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/tasks
POST /users/{id|userPrincipalName}/outlook/tasks
```
## <a name="request-headers"></a><span data-ttu-id="0daf8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0daf8-120">Request headers</span></span>
| <span data-ttu-id="0daf8-121">名称</span><span class="sxs-lookup"><span data-stu-id="0daf8-121">Name</span></span>       | <span data-ttu-id="0daf8-122">说明</span><span class="sxs-lookup"><span data-stu-id="0daf8-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0daf8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0daf8-123">Authorization</span></span>  | <span data-ttu-id="0daf8-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0daf8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0daf8-126">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="0daf8-126">Prefer: outlook.timezone</span></span> | <span data-ttu-id="0daf8-127">指定响应中时间属性的时区 (如果未指定此标头, 则采用 UTC 格式表示)。</span><span class="sxs-lookup"><span data-stu-id="0daf8-127">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="0daf8-128">可选。</span><span class="sxs-lookup"><span data-stu-id="0daf8-128">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0daf8-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="0daf8-129">Request body</span></span>
<span data-ttu-id="0daf8-130">在请求正文中, 提供[outlookTask](../resources/outlooktask.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0daf8-130">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0daf8-131">响应</span><span class="sxs-lookup"><span data-stu-id="0daf8-131">Response</span></span>

<span data-ttu-id="0daf8-132">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[outlookTask](../resources/outlooktask.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0daf8-132">If successful, this method returns `201 Created` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0daf8-133">示例</span><span class="sxs-lookup"><span data-stu-id="0daf8-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0daf8-134">请求</span><span class="sxs-lookup"><span data-stu-id="0daf8-134">Request</span></span>
<span data-ttu-id="0daf8-135">下面的示例展示了`Prefer: outlook.timezone`标头的用法。</span><span class="sxs-lookup"><span data-stu-id="0daf8-135">The following example shows the use of the `Prefer: outlook.timezone` header.</span></span> <span data-ttu-id="0daf8-136">它创建一个任务, 表示**startDateTime**和**DueDateTime** (东部标准时间 (EST)), 并包含`Prefer`太平洋标准时间 (PST) 的标题。</span><span class="sxs-lookup"><span data-stu-id="0daf8-136">It creates a task, expresses **startDateTime** and **dueDateTime** in Eastern Standard Time (EST), and includes a `Prefer` header of Pacific Standard Time (PST).</span></span>
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
<span data-ttu-id="0daf8-137">在请求正文中, 提供[outlookTask](../resources/outlooktask.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0daf8-137">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0daf8-138">响应</span><span class="sxs-lookup"><span data-stu-id="0daf8-138">Response</span></span>
<span data-ttu-id="0daf8-139">POST 方法忽略请求正文中**startDateTime**和**dueDateTime**的时间部分, 并假定指定时区 (EST) 中的时间始终为午夜。</span><span class="sxs-lookup"><span data-stu-id="0daf8-139">The POST method ignores the time portion of **startDateTime** and **dueDateTime** in the request body and assumes the time to be always midnight in the specified time zone (EST).</span></span>

<span data-ttu-id="0daf8-140">由于`Prefer`标头指定了 Pst, 因此 POST 方法表示 pst 中的响应中所有与日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="0daf8-140">Since the `Prefer` header specifies PST, the POST method expresses all the date-related properties in the response in PST.</span></span> <span data-ttu-id="0daf8-141">特别是对于**startDateTime**和**DUEDATETIME**属性, POST 方法将 EST 中的午夜转换为 pst, 并在响应中将其返回到 pst 中。</span><span class="sxs-lookup"><span data-stu-id="0daf8-141">In particular, for the **startDateTime** and **dueDateTime** properties, the POST method converts midnight in EST to PST and returns them in PST in the response.</span></span>

<span data-ttu-id="0daf8-142">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0daf8-142">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0daf8-143">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0daf8-143">All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="0daf8-144">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="0daf8-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0daf8-145">语言</span><span class="sxs-lookup"><span data-stu-id="0daf8-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_outlooktask_from_outlookuser-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0daf8-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="0daf8-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_outlooktask_from_outlookuser-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookuser-post-tasks.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlookuser-post-tasks.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
