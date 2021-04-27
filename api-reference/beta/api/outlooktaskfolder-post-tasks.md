---
title: 创建 outlookTask
description: 创建Outlook任务文件夹中的一个任务。
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 233e93529c2b4644a69643fd8bf1f49562765127
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055433"
---
# <a name="create-outlooktask-deprecated"></a><span data-ttu-id="92fb8-103">创建 outlookTask（已弃用）</span><span class="sxs-lookup"><span data-stu-id="92fb8-103">Create outlookTask (deprecated)</span></span>

<span data-ttu-id="92fb8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92fb8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="92fb8-105">创建Outlook任务文件夹中的一个任务。</span><span class="sxs-lookup"><span data-stu-id="92fb8-105">Create an Outlook task in the specified task folder.</span></span>

<span data-ttu-id="92fb8-106">POST 方法始终忽略请求正文中 **startDateTime** 和 **dueDateTime** 的时间部分，并假定时间始终为指定时区中的午夜。</span><span class="sxs-lookup"><span data-stu-id="92fb8-106">The POST method always ignores the time portion of **startDateTime** and **dueDateTime** in the request body, and assumes the time to be always midnight in the specified time zone.</span></span>

## <a name="permissions"></a><span data-ttu-id="92fb8-107">权限</span><span class="sxs-lookup"><span data-stu-id="92fb8-107">Permissions</span></span>
<span data-ttu-id="92fb8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="92fb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92fb8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="92fb8-110">Permission type</span></span>      | <span data-ttu-id="92fb8-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="92fb8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92fb8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="92fb8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="92fb8-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92fb8-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="92fb8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="92fb8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92fb8-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92fb8-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="92fb8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="92fb8-116">Application</span></span> | <span data-ttu-id="92fb8-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="92fb8-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="92fb8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="92fb8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskFolders/{id}/tasks
POST /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="request-headers"></a><span data-ttu-id="92fb8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="92fb8-119">Request headers</span></span>
| <span data-ttu-id="92fb8-120">名称</span><span class="sxs-lookup"><span data-stu-id="92fb8-120">Name</span></span>       | <span data-ttu-id="92fb8-121">说明</span><span class="sxs-lookup"><span data-stu-id="92fb8-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="92fb8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="92fb8-122">Authorization</span></span>  | <span data-ttu-id="92fb8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="92fb8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="92fb8-125">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="92fb8-125">Prefer: outlook.timezone</span></span> | <span data-ttu-id="92fb8-126">指定响应中时间属性的时区，如果未指定此标头，则其时区为 UTC。</span><span class="sxs-lookup"><span data-stu-id="92fb8-126">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="92fb8-127">可选。</span><span class="sxs-lookup"><span data-stu-id="92fb8-127">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="92fb8-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="92fb8-128">Request body</span></span>
<span data-ttu-id="92fb8-129">在请求正文中，提供 [outlookTask](../resources/outlooktask.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92fb8-129">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="92fb8-130">响应</span><span class="sxs-lookup"><span data-stu-id="92fb8-130">Response</span></span>

<span data-ttu-id="92fb8-131">如果成功，此方法在 `201 Created` 响应正文中返回 响应代码和 [outlookTask](../resources/outlooktask.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="92fb8-131">If successful, this method returns `201 Created` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92fb8-132">示例</span><span class="sxs-lookup"><span data-stu-id="92fb8-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="92fb8-133">请求</span><span class="sxs-lookup"><span data-stu-id="92fb8-133">Request</span></span>
<span data-ttu-id="92fb8-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="92fb8-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="92fb8-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="92fb8-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_outlooktask_from_outlooktaskfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/taskfolders('AAMkADIyAAAhrbPXAAA=')/tasks
Content-type: application/json
Content-length: 376

{
  "subject": "Shop for dinner",
  "startDateTime": {
      "dateTime": "2016-04-23T18:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "dueDateTime":  {
      "dateTime": "2016-04-25T13:00:00",
      "timeZone": "Pacific Standard Time"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="92fb8-136">C#</span><span class="sxs-lookup"><span data-stu-id="92fb8-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktask-from-outlooktaskfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="92fb8-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="92fb8-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktask-from-outlooktaskfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="92fb8-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="92fb8-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktask-from-outlooktaskfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="92fb8-139">Java</span><span class="sxs-lookup"><span data-stu-id="92fb8-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-outlooktask-from-outlooktaskfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="92fb8-140">在请求正文中，提供 [outlookTask](../resources/outlooktask.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92fb8-140">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="92fb8-141">响应</span><span class="sxs-lookup"><span data-stu-id="92fb8-141">Response</span></span>
<span data-ttu-id="92fb8-142">POST 方法忽略请求正文中的时间部分，并假定在 PST (指定时区中始终午夜) 。</span><span class="sxs-lookup"><span data-stu-id="92fb8-142">The POST method ignores the time portion in the request body and assumes the time to be always midnight in the specified time zone (PST).</span></span> <span data-ttu-id="92fb8-143">然后，默认情况下，POST 方法在响应中转换和显示所有与日期相关的属性（采用 UTC）。</span><span class="sxs-lookup"><span data-stu-id="92fb8-143">Then, by default, the POST method converts and shows all the date-related properties in UTC in the response.</span></span>

<span data-ttu-id="92fb8-144">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="92fb8-144">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 376

{
  "createdDateTime": "2016-04-22T05:44:01.2012012Z",
  "lastModifiedDateTime": "2016-04-22T05:44:02.9980882Z",
  "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIOJMxw==",
  "categories": [ ],
  "assignedTo": "null",
  "body": {
    "contentType": "Text",
    "content": ""
  },
  "completedDateTime": null,
  "dueDateTime": {
    "dateTime": "2016-04-25T07:00:00.0000000",
    "timeZone": "UTC"
  },
  "hasAttachments":false,
  "importance": "Normal",
  "isReminderOn": false,
  "owner": "Administrator",
  "parentFolderId": "AQMkADA1MTkAAAAIBEgAAAA==",
  "recurrence": null,
  "reminderDateTime": null,
  "sensitivity": "Normal",
  "startDateTime": {
    "dateTime": "2016-04-23T07:00:00.0000000",
    "timeZone": "UTC"
  },
  "status": "NotStarted",
  "subject": "Shop for dinner"
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
  "suppressions": []
}
-->


