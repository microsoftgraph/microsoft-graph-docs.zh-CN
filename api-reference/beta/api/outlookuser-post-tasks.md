---
title: 创建 outlookTask
description: 在用户邮箱中的默认任务组 (`My Tasks`) 和默认任务文件夹 (`Tasks`) 中创建一个 Outlook 任务。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 4de57847638ef98347a7561291d12486468428ee
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869454"
---
# <a name="create-outlooktask"></a>创建 outlookTask

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在用户邮箱中的默认任务组 (`My Tasks`) 和默认任务文件夹 (`Tasks`) 中创建一个 Outlook 任务。

POST 方法始终忽略请求正文中**startDateTime**和**dueDateTime**的时间部分, 并假定指定时区中的时间始终为午夜。

默认情况下, 此操作 (以及获取、修补和[完成](../api/outlooktask-complete.md)任务操作) 将返回 UTC 格式的与日期相关的属性。 你可以使用 `Prefer: outlook.timezone` 标头将响应中的所有与日期相关的属性都表示为与 UTC 不同的时区。

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
POST /me/outlook/tasks
POST /users/{id|userPrincipalName}/outlook/tasks
```
## <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:---------------|:----------|
| Authorization  | Bearer {token}。必需。 |
| Prefer: outlook.timezone | 指定响应中时间属性的时区 (如果未指定此标头, 则采用 UTC 格式表示)。 可选。|

## <a name="request-body"></a>请求正文
在请求正文中, 提供[outlookTask](../resources/outlooktask.md)对象的 JSON 表示形式。

## <a name="response"></a>响应

如果成功, 此方法在`201 Created`响应正文中返回响应代码和[outlookTask](../resources/outlooktask.md)对象。

## <a name="example"></a>示例
##### <a name="request"></a>请求
下面的示例展示了`Prefer: outlook.timezone`标头的用法。 它创建一个任务, 表示**startDateTime**和**dueDateTime** (东部标准时间 (EST)), 并包含`Prefer`太平洋标准时间 (PST) 的标题。
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
在请求正文中, 提供[outlookTask](../resources/outlooktask.md)对象的 JSON 表示形式。
##### <a name="response"></a>响应
POST 方法忽略请求正文中**startDateTime**和**dueDateTime**的时间部分, 并假定指定时区 (EST) 中的时间始终为午夜。

由于`Prefer`标头指定了 pst, 因此 POST 方法表示 pst 中的响应中所有与日期相关的属性。 特别是对于**startDateTime**和**dueDateTime**属性, POST 方法将 EST 中的午夜转换为 pst, 并在响应中将其返回到 pst 中。

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
<!--
{
  "type": "#page.annotation",
  "description": "Create outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookuser-post-tasks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
