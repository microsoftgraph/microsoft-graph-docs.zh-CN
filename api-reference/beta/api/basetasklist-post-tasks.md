---
title: 创建 baseTask
description: 在特定 baseTaskList 中创建新的 baseTask 对象。
author: devindrajit
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f34757d950146c0d1df8c515360ff7f823cd6793
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65821055"
---
# <a name="create-basetask-deprecated"></a>创建已弃用的 baseTask () 
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [todo-deprecate-basetaskapi](../includes/todo-deprecate-basetaskapi.md)]

在特定 [baseTaskList](../resources/basetask.md) 中创建新的 [baseTask](../resources/basetasklist.md) 对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Tasks.ReadWrite|
|委派（个人 Microsoft 帐户）|Tasks.ReadWrite|
|应用|不支持|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/tasks/lists/{baseTaskListId}/tasks
POST /users/{userId|userPrincipalName}/tasks/lists/{baseTaskListId}/tasks
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [baseTask](../resources/basetask.md) 对象的 JSON 表示形式。

创建 **baseTask** 时，可以指定以下属性。

|属性|类型|说明|
|:---|:---|:---|
|textBody|String|通常包含有关任务的信息的文本格式的任务正文。|
|createdDateTime|DateTimeOffset|在指定时区内完成任务的日期。|
|lastModifiedDateTime|DateTimeOffset|上次修改任务的日期和时间。 默认情况下，它采用 UTC 格式。 你可以在请求标头中提供自定义时区。 属性值使用 ISO 8601 格式，并始终处于 UTC 时间。 例如，2020 年 1 月 1 日午夜 UTC 如下所示：“2020-01-01T00：00：00Z”。|
|bodyLastModifiedDateTime|DateTimeOffset|上次修改任务的日期和时间。 默认情况下，它采用 UTC 格式。 你可以在请求标头中提供自定义时区。 属性值使用 ISO 8601 格式，并始终处于 UTC 时间。 例如，2020 年 1 月 1 日午夜 UTC 如下所示：“2020-01-01T00：00：00Z”。|
|completedDateTime|DateTimeOffset|在指定时区内完成任务的日期。|
|dueDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|要在指定时区内完成任务的日期。|
|startDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|要在指定时区内开始执行任务的日期。|
|importance|importance|任务的重要性。 可能的值包括 `low`、`normal`、`high`。|
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|任务的定期模式。|
|displayName|String|任务的简要说明。|
|status|taskStatus_v2|指示任务的状态或进度。 可能的值包括 `notStarted`、`inProgress`、`completed`、`unknownFutureValue`。 必需项。|
|观点|[taskViewpoint](../resources/taskviewpoint.md)|用户的个人属性，例如 reminderDateTime。|



## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [baseTask](../resources/basetask.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_basetask_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/tasks/lists/AQMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNi/tasks
Content-Type: application/json
Content-length: 634

{
  "@odata.type": "#microsoft.graph.task",
  "textBody":  "String",
  "bodyLastModifiedDateTime": "String (timestamp)",
  "completedDateTime": "String (timestamp)",
  "dueDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "startDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "importance": "String",
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
  },
  "displayName": "String",
  "status": "String",
  "viewpoint": {
    "@odata.type": "microsoft.graph.taskViewpoint"
  }
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-basetask-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-basetask-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-basetask-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-basetask-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-basetask-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.task"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.task",
    "@odata.etag": "W/\"kOO4xOT//0qFRAqk3TNe0QAABCE1Xg==\"",
    "importance": "normal",
    "status": "notStarted",
    "displayName": "Buy medicine",
    "createdDateTime": "2021-11-17T10:11:18.0229364Z",
    "lastModifiedDateTime": "2021-11-17T10:11:18.19789Z",
    "id": "AAkALgAAAAAAHYQDEapmEc2byACqAC",
    "textBody":  "",
    "parentList": {
        "id": "AQMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNi"
    }
}
```

