---
title: 创建 outlookTask
description: 在指定的任务文件夹中创建 Outlook 任务。
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7278347dce74138b6eb38281f32dc7b968a9aacb
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472452"
---
# <a name="create-outlooktask-deprecated"></a><span data-ttu-id="ea941-103">创建 outlookTask（已弃用）</span><span class="sxs-lookup"><span data-stu-id="ea941-103">Create outlookTask (deprecated)</span></span>

<span data-ttu-id="ea941-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea941-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="ea941-105">在指定的任务文件夹中创建 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="ea941-105">Create an Outlook task in the specified task folder.</span></span>

<span data-ttu-id="ea941-106">POST 方法始终忽略 **请求正文中 startDateTime** 和 **dueDateTime** 的时间部分，并假定时间始终为指定时区中的午夜。</span><span class="sxs-lookup"><span data-stu-id="ea941-106">The POST method always ignores the time portion of **startDateTime** and **dueDateTime** in the request body, and assumes the time to be always midnight in the specified time zone.</span></span>

## <a name="permissions"></a><span data-ttu-id="ea941-107">权限</span><span class="sxs-lookup"><span data-stu-id="ea941-107">Permissions</span></span>
<span data-ttu-id="ea941-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ea941-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea941-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ea941-110">Permission type</span></span>      | <span data-ttu-id="ea941-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ea941-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea941-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ea941-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ea941-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea941-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="ea941-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ea941-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea941-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea941-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="ea941-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ea941-116">Application</span></span> | <span data-ttu-id="ea941-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea941-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea941-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ea941-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskFolders/{id}/tasks
POST /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="request-headers"></a><span data-ttu-id="ea941-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ea941-119">Request headers</span></span>
| <span data-ttu-id="ea941-120">名称</span><span class="sxs-lookup"><span data-stu-id="ea941-120">Name</span></span>       | <span data-ttu-id="ea941-121">说明</span><span class="sxs-lookup"><span data-stu-id="ea941-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ea941-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea941-122">Authorization</span></span>  | <span data-ttu-id="ea941-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ea941-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ea941-125">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="ea941-125">Prefer: outlook.timezone</span></span> | <span data-ttu-id="ea941-126">指定响应中时间属性的时区，如果未指定此标头，则时区为 UTC。</span><span class="sxs-lookup"><span data-stu-id="ea941-126">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="ea941-127">可选。</span><span class="sxs-lookup"><span data-stu-id="ea941-127">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea941-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ea941-128">Request body</span></span>
<span data-ttu-id="ea941-129">在请求正文中，提供 [outlookTask](../resources/outlooktask.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea941-129">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ea941-130">响应</span><span class="sxs-lookup"><span data-stu-id="ea941-130">Response</span></span>

<span data-ttu-id="ea941-131">如果成功，此方法在响应正文中返回响应代码 `201 Created` 和 [outlookTask](../resources/outlooktask.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ea941-131">If successful, this method returns `201 Created` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea941-132">示例</span><span class="sxs-lookup"><span data-stu-id="ea941-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ea941-133">请求</span><span class="sxs-lookup"><span data-stu-id="ea941-133">Request</span></span>
<span data-ttu-id="ea941-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ea941-134">Here is an example of the request.</span></span>
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
<span data-ttu-id="ea941-135">在请求正文中，提供 [outlookTask](../resources/outlooktask.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea941-135">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ea941-136">响应</span><span class="sxs-lookup"><span data-stu-id="ea941-136">Response</span></span>
<span data-ttu-id="ea941-137">POST 方法将忽略请求正文中的时间部分，并假定时间始终为指定时区的午夜 (PST) 。</span><span class="sxs-lookup"><span data-stu-id="ea941-137">The POST method ignores the time portion in the request body and assumes the time to be always midnight in the specified time zone (PST).</span></span> <span data-ttu-id="ea941-138">然后，默认情况下，POST 方法在响应中转换和显示所有与日期相关的属性（采用 UTC 格式）。</span><span class="sxs-lookup"><span data-stu-id="ea941-138">Then, by default, the POST method converts and shows all the date-related properties in UTC in the response.</span></span>

<span data-ttu-id="ea941-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ea941-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


