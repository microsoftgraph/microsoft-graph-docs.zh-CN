---
title: 创建 outlookTask
description: 在指定的任务文件夹中创建一个 Outlook 任务。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d9054dbc262c9350bb3efcc17193d66f27ae5904
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456143"
---
# <a name="create-outlooktask"></a>创建 outlookTask

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在指定的任务文件夹中创建一个 Outlook 任务。

POST 方法始终忽略请求正文中**startDateTime**和**dueDateTime**的时间部分，并假定指定时区中的时间始终为午夜。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | 不支持。    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /me/outlook/taskFolders/{id}/tasks
POST /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:---------------|:----------|
| Authorization  | Bearer {token}。必需。 |
| Prefer: outlook.timezone | 指定响应中时间属性的时区（如果未指定此标头，则采用 UTC 格式表示）。 可选。|

## <a name="request-body"></a>请求正文
在请求正文中，提供[outlookTask](../resources/outlooktask.md)对象的 JSON 表示形式。

## <a name="response"></a>响应

如果成功，此方法在`201 Created`响应正文中返回响应代码和[outlookTask](../resources/outlooktask.md)对象。

## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。
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
在请求正文中，提供[outlookTask](../resources/outlooktask.md)对象的 JSON 表示形式。
##### <a name="response"></a>响应
POST 方法忽略请求正文中的时间部分，并假定指定时区（PST）中的时间始终为午夜。 然后，在默认情况下，POST 方法将在响应中转换并显示 UTC 格式的所有日期相关属性。

注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
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
