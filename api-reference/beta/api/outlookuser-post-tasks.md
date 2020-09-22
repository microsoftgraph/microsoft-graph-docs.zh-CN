---
title: 创建 outlookTask
description: 在默认任务组中创建一个 Outlook 任务 (`My Tasks`) 和默认的任务文件夹 (`Tasks` 用户邮箱中的) 。
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5adb1afed482c7080cb06ecb70a2612ac37758ec
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074263"
---
# <a name="create-outlooktask-deprecated"></a><span data-ttu-id="8bf12-103">创建 outlookTask (弃用) </span><span class="sxs-lookup"><span data-stu-id="8bf12-103">Create outlookTask (deprecated)</span></span>

<span data-ttu-id="8bf12-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bf12-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="8bf12-105">在默认任务组中创建一个 Outlook 任务 (`My Tasks`) 和默认的任务文件夹 (`Tasks` 用户邮箱中的) 。</span><span class="sxs-lookup"><span data-stu-id="8bf12-105">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>

<span data-ttu-id="8bf12-106">POST 方法始终忽略请求正文中 **startDateTime** 和 **dueDateTime** 的时间部分，并假定指定时区中的时间始终为午夜。</span><span class="sxs-lookup"><span data-stu-id="8bf12-106">The POST method always ignores the time portion of **startDateTime** and **dueDateTime** in the request body, and assumes the time to be always midnight in the specified time zone.</span></span>

<span data-ttu-id="8bf12-107">默认情况下，此操作 (，获取、修补和 [完成](../api/outlooktask-complete.md) 任务操作) 返回 UTC 格式的日期相关属性。</span><span class="sxs-lookup"><span data-stu-id="8bf12-107">By default, this operation (and the GET, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="8bf12-108">你可以使用 `Prefer: outlook.timezone` 标头将响应中的所有与日期相关的属性都表示为与 UTC 不同的时区。</span><span class="sxs-lookup"><span data-stu-id="8bf12-108">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="8bf12-109">权限</span><span class="sxs-lookup"><span data-stu-id="8bf12-109">Permissions</span></span>
<span data-ttu-id="8bf12-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8bf12-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bf12-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="8bf12-112">Permission type</span></span>      | <span data-ttu-id="8bf12-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8bf12-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8bf12-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8bf12-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8bf12-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8bf12-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="8bf12-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8bf12-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bf12-117">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8bf12-117">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="8bf12-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="8bf12-118">Application</span></span> | <span data-ttu-id="8bf12-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="8bf12-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8bf12-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8bf12-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/tasks
POST /users/{id|userPrincipalName}/outlook/tasks
```
## <a name="request-headers"></a><span data-ttu-id="8bf12-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="8bf12-121">Request headers</span></span>
| <span data-ttu-id="8bf12-122">名称</span><span class="sxs-lookup"><span data-stu-id="8bf12-122">Name</span></span>       | <span data-ttu-id="8bf12-123">说明</span><span class="sxs-lookup"><span data-stu-id="8bf12-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8bf12-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8bf12-124">Authorization</span></span>  | <span data-ttu-id="8bf12-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8bf12-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8bf12-127">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="8bf12-127">Prefer: outlook.timezone</span></span> | <span data-ttu-id="8bf12-128">指定响应中时间属性的时区（如果未指定此标头，则采用 UTC 格式表示）。</span><span class="sxs-lookup"><span data-stu-id="8bf12-128">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="8bf12-129">可选。</span><span class="sxs-lookup"><span data-stu-id="8bf12-129">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bf12-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="8bf12-130">Request body</span></span>
<span data-ttu-id="8bf12-131">在请求正文中，提供 [outlookTask](../resources/outlooktask.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8bf12-131">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8bf12-132">响应</span><span class="sxs-lookup"><span data-stu-id="8bf12-132">Response</span></span>

<span data-ttu-id="8bf12-133">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [outlookTask](../resources/outlooktask.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8bf12-133">If successful, this method returns `201 Created` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bf12-134">示例</span><span class="sxs-lookup"><span data-stu-id="8bf12-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8bf12-135">请求</span><span class="sxs-lookup"><span data-stu-id="8bf12-135">Request</span></span>
<span data-ttu-id="8bf12-136">下面的示例展示了 `Prefer: outlook.timezone` 标头的用法。</span><span class="sxs-lookup"><span data-stu-id="8bf12-136">The following example shows the use of the `Prefer: outlook.timezone` header.</span></span> <span data-ttu-id="8bf12-137">它将创建一个任务，以东部标准时间 (EST) 表示 **startDateTime** 和 **dueDateTime** ，并包括 `Prefer` 太平洋标准时间 (PST) 的标题。</span><span class="sxs-lookup"><span data-stu-id="8bf12-137">It creates a task, expresses **startDateTime** and **dueDateTime** in Eastern Standard Time (EST), and includes a `Prefer` header of Pacific Standard Time (PST).</span></span>
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
# <a name="c"></a>[<span data-ttu-id="8bf12-138">C#</span><span class="sxs-lookup"><span data-stu-id="8bf12-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktask-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8bf12-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8bf12-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktask-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8bf12-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8bf12-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktask-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="8bf12-141">在请求正文中，提供 [outlookTask](../resources/outlooktask.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8bf12-141">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="8bf12-142">响应</span><span class="sxs-lookup"><span data-stu-id="8bf12-142">Response</span></span>
<span data-ttu-id="8bf12-143">POST 方法忽略请求正文中 **startDateTime** 和 **dueDateTime** 的时间部分，并假定指定时区 (EST) 中的时间始终为午夜。</span><span class="sxs-lookup"><span data-stu-id="8bf12-143">The POST method ignores the time portion of **startDateTime** and **dueDateTime** in the request body and assumes the time to be always midnight in the specified time zone (EST).</span></span>

<span data-ttu-id="8bf12-144">由于 `Prefer` 标头指定了 pst，因此 POST 方法表示 pst 中的响应中所有与日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="8bf12-144">Since the `Prefer` header specifies PST, the POST method expresses all the date-related properties in the response in PST.</span></span> <span data-ttu-id="8bf12-145">特别是对于 **startDateTime** 和 **DUEDATETIME** 属性，POST 方法将 EST 中的午夜转换为 pst，并在响应中将其返回到 pst 中。</span><span class="sxs-lookup"><span data-stu-id="8bf12-145">In particular, for the **startDateTime** and **dueDateTime** properties, the POST method converts midnight in EST to PST and returns them in PST in the response.</span></span>

<span data-ttu-id="8bf12-p107">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8bf12-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "assignedTo": null,
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
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


