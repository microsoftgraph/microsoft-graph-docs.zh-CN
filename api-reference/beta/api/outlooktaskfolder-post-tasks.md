---
title: 创建 outlookTask
description: 在指定的任务文件夹中创建 Outlook 任务。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 80e1c6dda762ae46b5463fde9cff353e1d46408f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969630"
---
# <a name="create-outlooktask"></a><span data-ttu-id="63d36-103">创建 outlookTask</span><span class="sxs-lookup"><span data-stu-id="63d36-103">Create outlookTask</span></span>

> <span data-ttu-id="63d36-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="63d36-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="63d36-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="63d36-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="63d36-106">在指定的任务文件夹中创建 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="63d36-106">Create an Outlook task in the specified task folder.</span></span>

<span data-ttu-id="63d36-107">POST 方法始终将忽略的时间部分的**开始日期时间**和**dueDateTime**在请求正文中，并假定为始终中指定的时区的午夜的时间。</span><span class="sxs-lookup"><span data-stu-id="63d36-107">The POST method always ignores the time portion of **startDateTime** and **dueDateTime** in the request body, and assumes the time to be always midnight in the specified time zone.</span></span>

## <a name="permissions"></a><span data-ttu-id="63d36-108">权限</span><span class="sxs-lookup"><span data-stu-id="63d36-108">Permissions</span></span>
<span data-ttu-id="63d36-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="63d36-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63d36-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="63d36-111">Permission type</span></span>      | <span data-ttu-id="63d36-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="63d36-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63d36-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63d36-113">Delegated (work or school account)</span></span> | <span data-ttu-id="63d36-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="63d36-114">Not supported.</span></span>    |
|<span data-ttu-id="63d36-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63d36-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63d36-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="63d36-116">Not supported.</span></span>    |
|<span data-ttu-id="63d36-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="63d36-117">Application</span></span> | <span data-ttu-id="63d36-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="63d36-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="63d36-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63d36-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="request-headers"></a><span data-ttu-id="63d36-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="63d36-120">Request headers</span></span>
| <span data-ttu-id="63d36-121">名称</span><span class="sxs-lookup"><span data-stu-id="63d36-121">Name</span></span>       | <span data-ttu-id="63d36-122">说明</span><span class="sxs-lookup"><span data-stu-id="63d36-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="63d36-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="63d36-123">Authorization</span></span>  | <span data-ttu-id="63d36-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="63d36-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="63d36-126">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="63d36-126">Prefer: outlook.timezone</span></span> | <span data-ttu-id="63d36-127">响应，它可以采用 UTC 如果未指定此标头中指定的时间属性的时区。</span><span class="sxs-lookup"><span data-stu-id="63d36-127">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="63d36-128">可选。</span><span class="sxs-lookup"><span data-stu-id="63d36-128">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="63d36-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="63d36-129">Request body</span></span>
<span data-ttu-id="63d36-130">在请求正文中，提供[outlookTask](../resources/outlooktask.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63d36-130">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="63d36-131">响应</span><span class="sxs-lookup"><span data-stu-id="63d36-131">Response</span></span>

<span data-ttu-id="63d36-132">如果成功，此方法返回`201 Created`响应正文中的响应代码和[outlookTask](../resources/outlooktask.md)对象。</span><span class="sxs-lookup"><span data-stu-id="63d36-132">If successful, this method returns `201 Created` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63d36-133">示例</span><span class="sxs-lookup"><span data-stu-id="63d36-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="63d36-134">请求</span><span class="sxs-lookup"><span data-stu-id="63d36-134">Request</span></span>
<span data-ttu-id="63d36-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="63d36-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlooktask_from_outlooktaskfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/taskfolders('AAMkADIyAAAhrbPXAAA=')/tasks
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
<span data-ttu-id="63d36-136">在请求正文中，提供[outlookTask](../resources/outlooktask.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63d36-136">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="63d36-137">响应</span><span class="sxs-lookup"><span data-stu-id="63d36-137">Response</span></span>
<span data-ttu-id="63d36-138">POST 方法将忽略在请求正文中的时间部分，并假定为始终午夜指定时区 (PST) 中的时间。</span><span class="sxs-lookup"><span data-stu-id="63d36-138">The POST method ignores the time portion in the request body and assumes the time to be always midnight in the specified time zone (PST).</span></span> <span data-ttu-id="63d36-139">然后，默认情况下 POST 方法将转换，并在响应中 utc 格式显示所有的日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="63d36-139">Then, by default, the POST method converts and shows all the date-related properties in UTC in the response.</span></span>

<span data-ttu-id="63d36-p106">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="63d36-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
