---
title: 创建 baseTask
description: 在特定的 baseTaskList 中创建新的 baseTask 对象。
author: devindrajit
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 03d3ab9a0a16f1f2b16cf3aed5321fed8c535c76
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424845"
---
# <a name="create-basetask"></a>创建 baseTask
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在特定的 [baseTaskList](../resources/basetask.md) 中创建新的 [baseTask 对象](../resources/basetasklist.md)。

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

可以在创建 **baseTask** 时指定以下属性。

|属性|类型|说明|
|:---|:---|:---|
|body|[itemBody](../resources/itembody.md)|通常包含有关任务的信息的任务正文。|
|createdDateTime|DateTimeOffset|在指定时区内完成任务的日期。|
|lastModifiedDateTime|DateTimeOffset|上次修改任务的日期和时间。 默认情况下，它采用 UTC 格式。 你可以在请求标头中提供自定义时区。 属性值使用 ISO 8601 格式，并始终处于 UTC 时间。 例如，2020 年 1 月 1 日午夜 UTC 如下所示："2020-01-01T00：00：00Z"。|
|bodyLastModifiedDateTime|DateTimeOffset|上次修改任务的日期和时间。 默认情况下，它采用 UTC 格式。 你可以在请求标头中提供自定义时区。 属性值使用 ISO 8601 格式，并始终处于 UTC 时间。 例如，2020 年 1 月 1 日午夜 UTC 如下所示："2020-01-01T00：00：00Z"。|
|completedDateTime|DateTimeOffset|在指定时区内完成任务的日期。|
|dueDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|要在指定时区内完成任务的日期。|
|startDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|要在指定时区内开始执行任务的日期。|
|importance|importance|任务的重要性。 可能的值包括 `low`、`normal`、`high`。|
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|任务的定期模式。|
|displayName|字符串|任务的简要说明。|
|状态|taskStatus_v2|指示任务的状态或进度。 可能的值包括 `notStarted`、`inProgress`、`completed`、`unknownFutureValue`。 必需。|
|personalProperties|[personalTaskProperties](../resources/personaltaskproperties.md)|用户个人的属性，如 reminderDateTime。|



## <a name="response"></a>响应

如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [baseTask](../resources/basetask.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
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


### <a name="response"></a>响应
**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.baseTask"
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
    "body": {
        "content": "",
        "contentType": "text"
    },
    "parentList": {
        "id": "AQMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNi"
    }
}
```

