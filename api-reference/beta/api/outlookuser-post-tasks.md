---
title: 创建 outlookTask
description: 创建 Outlook 任务中的默认任务组 (`My Tasks`) 和默认任务文件夹 (`Tasks`) 用户的邮箱中。
ms.openlocfilehash: c9019db8e36151c70c5e3d2abe1ea4fea2e94ef0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047918"
---
# <a name="create-outlooktask"></a>创建 outlookTask

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

创建 Outlook 任务中的默认任务组 (`My Tasks`) 和默认任务文件夹 (`Tasks`) 用户的邮箱中。

POST 方法始终将忽略的时间部分的**开始日期时间**和**dueDateTime**在请求正文中，并假定为始终中指定的时区的午夜的时间。

默认情况下，此操作 （和 GET、 修补程序，并[完成](../api/outlooktask-complete.md)任务操作） 返回与日期相关的属性采用 UTC。 您可以使用`Prefer: outlook.timezone`标头，使其具有不同于 UTC 时区中表示的响应中的所有日期相关的属性。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Tasks.ReadWrite    |
|委派（个人 Microsoft 帐户） | Tasks.ReadWrite    |
|应用程序 | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/tasks
```
## <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:---------------|:----------|
| Authorization  | Bearer {token}。必需。 |
| Prefer: outlook.timezone | 响应，它可以采用 UTC 如果未指定此标头中指定的时间属性的时区。 可选。|

## <a name="request-body"></a>请求正文
在请求正文中，提供[outlookTask](../resources/outlooktask.md)对象的 JSON 表示形式。

## <a name="response"></a>响应

如果成功，此方法返回`201 Created`响应正文中的响应代码和[outlookTask](../resources/outlooktask.md)对象。

## <a name="example"></a>示例
##### <a name="request"></a>请求
下面的示例演示如何使用`Prefer: outlook.timezone`标头。 它创建任务，表示**开始日期时间**和**dueDateTime**在东部标准时间 (EST)，并且包括`Prefer`标头的太平洋标准时间 (PST)。
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
在请求正文中，提供[outlookTask](../resources/outlooktask.md)对象的 JSON 表示形式。
##### <a name="response"></a>响应
POST 方法将忽略的**开始日期时间**和**dueDateTime**在请求正文中的时间部分，并假定为始终午夜指定时区 (EST) 中的时间。

由于`Prefer`标头指定 PST、 POST 方法表示 PST 中的响应中所有的日期相关的属性。 具体而言的**开始日期时间**和**dueDateTime**属性，POST 方法将在东部时间午夜转换为太平洋标准时间，并返回其中 PST 的响应中。

注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->