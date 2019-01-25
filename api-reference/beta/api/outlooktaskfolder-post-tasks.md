---
title: 创建 outlookTask
description: 在指定的任务文件夹中创建 Outlook 任务。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 8ba293d83e2a202a45cfebf4c318ee73d808e1e4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510594"
---
# <a name="create-outlooktask"></a><span data-ttu-id="373ba-103">创建 outlookTask</span><span class="sxs-lookup"><span data-stu-id="373ba-103">Create outlookTask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="373ba-104">在指定的任务文件夹中创建 Outlook 任务。</span><span class="sxs-lookup"><span data-stu-id="373ba-104">Create an Outlook task in the specified task folder.</span></span>

<span data-ttu-id="373ba-105">POST 方法始终将忽略的时间部分的**开始日期时间**和**dueDateTime**在请求正文中，并假定为始终中指定的时区的午夜的时间。</span><span class="sxs-lookup"><span data-stu-id="373ba-105">The POST method always ignores the time portion of **startDateTime** and **dueDateTime** in the request body, and assumes the time to be always midnight in the specified time zone.</span></span>

## <a name="permissions"></a><span data-ttu-id="373ba-106">权限</span><span class="sxs-lookup"><span data-stu-id="373ba-106">Permissions</span></span>
<span data-ttu-id="373ba-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="373ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="373ba-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="373ba-109">Permission type</span></span>      | <span data-ttu-id="373ba-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="373ba-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="373ba-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="373ba-111">Delegated (work or school account)</span></span> | <span data-ttu-id="373ba-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="373ba-112">Not supported.</span></span>    |
|<span data-ttu-id="373ba-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="373ba-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="373ba-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="373ba-114">Not supported.</span></span>    |
|<span data-ttu-id="373ba-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="373ba-115">Application</span></span> | <span data-ttu-id="373ba-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="373ba-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="373ba-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="373ba-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="request-headers"></a><span data-ttu-id="373ba-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="373ba-118">Request headers</span></span>
| <span data-ttu-id="373ba-119">名称</span><span class="sxs-lookup"><span data-stu-id="373ba-119">Name</span></span>       | <span data-ttu-id="373ba-120">说明</span><span class="sxs-lookup"><span data-stu-id="373ba-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="373ba-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="373ba-121">Authorization</span></span>  | <span data-ttu-id="373ba-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="373ba-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="373ba-124">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="373ba-124">Prefer: outlook.timezone</span></span> | <span data-ttu-id="373ba-125">响应，它可以采用 UTC 如果未指定此标头中指定的时间属性的时区。</span><span class="sxs-lookup"><span data-stu-id="373ba-125">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="373ba-126">可选。</span><span class="sxs-lookup"><span data-stu-id="373ba-126">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="373ba-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="373ba-127">Request body</span></span>
<span data-ttu-id="373ba-128">在请求正文中，提供[outlookTask](../resources/outlooktask.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="373ba-128">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="373ba-129">响应</span><span class="sxs-lookup"><span data-stu-id="373ba-129">Response</span></span>

<span data-ttu-id="373ba-130">如果成功，此方法返回`201 Created`响应正文中的响应代码和[outlookTask](../resources/outlooktask.md)对象。</span><span class="sxs-lookup"><span data-stu-id="373ba-130">If successful, this method returns `201 Created` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="373ba-131">示例</span><span class="sxs-lookup"><span data-stu-id="373ba-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="373ba-132">请求</span><span class="sxs-lookup"><span data-stu-id="373ba-132">Request</span></span>
<span data-ttu-id="373ba-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="373ba-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="373ba-134">在请求正文中，提供[outlookTask](../resources/outlooktask.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="373ba-134">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="373ba-135">响应</span><span class="sxs-lookup"><span data-stu-id="373ba-135">Response</span></span>
<span data-ttu-id="373ba-136">POST 方法将忽略在请求正文中的时间部分，并假定为始终午夜指定时区 (PST) 中的时间。</span><span class="sxs-lookup"><span data-stu-id="373ba-136">The POST method ignores the time portion in the request body and assumes the time to be always midnight in the specified time zone (PST).</span></span> <span data-ttu-id="373ba-137">然后，默认情况下 POST 方法将转换，并在响应中 utc 格式显示所有的日期相关的属性。</span><span class="sxs-lookup"><span data-stu-id="373ba-137">Then, by default, the POST method converts and shows all the date-related properties in UTC in the response.</span></span>

<span data-ttu-id="373ba-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="373ba-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktaskfolder-post-tasks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
