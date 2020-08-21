---
title: 创建 outlookTask
description: 在默认任务组中创建 Outlook `My Tasks` () 默认任务文件夹并 `Tasks` () 邮箱中。
localization_priority: Normal
author: mashriv
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8de61bceba328dbf99242cbfe5140e7ebed1296b
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849448"
---
# <a name="create-outlooktask"></a>创建 outlookTask

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


在默认任务组中创建 Outlook `My Tasks` () 默认任务文件夹并 `Tasks` () 邮箱中。

POST 方法始终忽略请求正文中的 **startDateTime** 和 **dueDateTime** 的时间部分，并假定指定的时区中始终午夜的时间。

默认情况下，此操作 (GET、PATCH 和 [完成](../api/outlooktask-complete.md) 的任务操作支持) 返回 UTC 格式的与日期相关的属性。 你可以使用 `Prefer: outlook.timezone` 标头将响应中的所有与日期相关的属性都表示为与 UTC 不同的时区。

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
| Prefer: outlook.timezone | 指定响应中的时区（如果未指定此标头，则该属性为 UTC 时间）。 可选。|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [outlookTask](../resources/outlooktask.md) 对象的 JSON 表示形式。

## <a name="response"></a>响应

如果成功，此方法在 `201 Created` 响应正文中 [返回响应](../resources/outlooktask.md) 代码和 outlookTask 对象。

## <a name="example"></a>示例
##### <a name="request"></a>请求
以下示例演示了标头使用的 `Prefer: outlook.timezone` 用例。 它创建了一个任务， **以东** 亚标准时间 (EST) 表示 **startDateTime 和 dueDateTime，** 并包含 `Prefer` 了 PST 迁移的太平 (时间) 。
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-outlooktask-from-outlookuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-outlooktask-from-outlookuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-outlooktask-from-outlookuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

在请求正文中，提供 [outlookTask](../resources/outlooktask.md) 对象的 JSON 表示形式。
##### <a name="response"></a>响应
POST 方法将忽略请求正文中的 **startDateTime** 和 **dueDateTime** 的时间部分，并假定指定的时区时间始终在指定时区或 EST 日期 (午) 。

由于标头 `Prefer` 指定 PST，POST 方法在 PST 格式表示响应中的所有与日期相关的属性。 特别是 **，POST 方法将** **dueDateTime** EST 的午夜转换为 PST 并在响应中以 PST 格式返回。

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
