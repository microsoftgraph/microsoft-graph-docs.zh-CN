---
title: 更新 baseTask
description: 更新 baseTask 对象的属性。
author: devindrajit
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7ca63c9e7158ee24af6dc4261f50d17ee204125b
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525392"
---
# <a name="update-basetask"></a>更新 baseTask
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [baseTask 对象](../resources/basetask.md) 的属性。

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
PATCH /me/tasks/lists/{baseTaskListId}/tasks/{baseTaskId}
PATCH /users/{userId|userPrincipalName}/tasks/lists/{baseTaskListId}/tasks/{baseTaskId}

PATCH /me/tasks/alltasks/{baseTaskId}
PATCH /users/{userId|userPrincipalName}/tasks/alltasks/{baseTaskId}
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|属性|类型|说明|
|:---|:---|:---|
|body|[itemBody](../resources/itembody.md)|通常包含有关任务的信息的任务正文。|
|createdDateTime|DateTimeOffset|在指定时区内完成任务的日期。|
|lastModifiedDateTime|DateTimeOffset|上次修改任务的日期和时间。 默认情况下，它采用 UTC 格式。 你可以在请求标头中提供自定义时区。|
|bodyLastModifiedDateTime|DateTimeOffset|上次修改任务正文的日期和时间。 默认情况下，它采用 UTC 格式。 你可以在请求标头中提供自定义时区。|
|completedDateTime|DateTimeOffset|在指定时区内完成任务的日期。|
|dueDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|要在指定时区内完成任务的日期。|
|startDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|要在指定时区内开始执行任务的日期。|
|importance|importance|事件的重要性。 可能的值包括 `low`、`normal`、`high`。|
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|任务的定期模式。|
|displayName|String|任务的简要说明。|
|状态|taskStatus_v2|指示任务的状态或进度。 可能的值包括 `notStarted`、`inProgress`、`completed`、`unknownFutureValue`。|
|personalProperties|[personalTaskProperties](../resources/personaltaskproperties.md)|用户个人的属性，如 reminderDateTime。|



## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [baseTask](../resources/basetask.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_basetask"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/tasks/lists/AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFsPFj7gQpLAt/tasks/AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AkOO4xOT
Content-Type: application/json
Content-length: 634

{
  "@odata.type": "#microsoft.graph.baseTask",
  "body": {
    "@odata.type": "microsoft.graph.itemBody"
  },
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
  "personalProperties": {
    "@odata.type": "microsoft.graph.personalTaskProperties"
  }
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-basetask-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.baseTask"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.task",
    "@odata.etag": "W/\"kOO4xOT//0qFRAqk3TNe0QAAA1uzSQ==\"",
    "importance": "normal",
    "status": "notStarted",
    "displayName": "T-2",
    "createdDateTime": "2021-11-15T14:38:25.6868632Z",
    "lastModifiedDateTime": "2021-11-15T15:51:13.3606631Z",
    "id": "AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AkOO4xOT",
    "body": {
        "content": "",
        "contentType": "text"
    },
    "parentList": {
        "id": "AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFsPFj7gQpLAt"
    }
}
```

