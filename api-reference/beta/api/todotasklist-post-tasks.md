---
title: 创建 todoTask
description: 在指定的 todoTaskList 中创建新任务对象。
author: avijityadav
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ed01fa8abbef32fd290d54ce3aeae7fe0777eaac
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820817"
---
# <a name="create-todotask"></a>创建 todoTask
命名空间：microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在指定 [的 todoTaskList](../resources/todotasklist.md) 中创建新任务对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Tasks.ReadWrite|
|委派（个人 Microsoft 帐户）|Tasks.ReadWrite|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/todo/lists/{todoTaskListId}/tasks
POST /users/{id|userPrincipalName}/todo/lists/{todoTaskListId}/tasks
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [todoTask](../resources/todotask.md) 对象的 JSON 表示形式。

下表显示了创建 [todoTask](../resources/todotask.md) 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|任务的唯一标识符。 默认情况下，当项从一个列表移动到另一个列表时，此值会更改。|
|body|[itemBody](../resources/itembody.md)|通常包含有关任务的信息的任务正文。|
|类别|String 集合|与任务关联的类别。 每个类别对应于用户定义的 [outlookCategory](../resources/outlookcategory.md) 的 **displayName** 属性。|
|completedDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|在指定时区内完成任务的日期。|
|dueDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|要在指定时区内完成任务的日期。|
|importance|importance|任务的重要性。 可取值为：`low`、`normal`、`high`。|
|isReminderOn|Boolean|如果设置警报以提醒用户有任务，则设置为 true。|
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|任务的定期模式。|
|reminderDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|提醒警报发出任务发生提醒的日期和时间。|
|状态|任务状态|指示任务的状态或进度。 可取值为：`notStarted`、`inProgress`、`completed`、`waitingOnOthers`、`deferred`。|
|title|String|任务的简要说明。|
|createdDateTime|DateTimeOffset|任务的创建日期和时间。 默认情况下，它采用 UTC 格式。 你可以在请求标头中提供自定义时区。 属性值使用 ISO 8601 格式。 例如，2020 年 1 月 1 日午夜 UTC 如下所示：“2020-01-01T00：00：00Z”。|
|lastModifiedDateTime|DateTimeOffset|上次修改任务的日期和时间。 默认情况下，它采用 UTC 格式。 你可以在请求标头中提供自定义时区。 属性值使用 ISO 8601 格式，并始终处于 UTC 时间。 例如，2020 年 1 月 1 日午夜 UTC 如下所示：“2020-01-01T00：00：00Z”。|
|bodyLastModifiedDateTime|DateTimeOffset|上次修改任务的日期和时间。 默认情况下，它采用 UTC 格式。 你可以在请求标头中提供自定义时区。 属性值使用 ISO 8601 格式，并始终处于 UTC 时间。 例如，2020 年 1 月 1 日午夜 UTC 如下所示：“2020-01-01T00：00：00Z”。|



## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [todoTask](../resources/todotask.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
以下示例在指定的任务列表中创建 **todoTask** ，并包含 [linkedResource](../resources/linkedresource.md)。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AQMkADAwATM0MDAAMS0yMDkyLWVjMzYtM"],
  "name": "create_todotask_from_tasks"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/todo/lists/AQMkADAwATM0MDAAMS0yMDkyLWVjMzYtM/tasks
Content-Type: application/json

{
   "title":"A new task",
   "categories": ["Important"],
   "linkedResources":[
      {
         "webUrl":"http://microsoft.com",
         "applicationName":"Microsoft",
         "displayName":"Microsoft"
      }
   ]
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-todotask-from-tasks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-todotask-from-tasks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-todotask-from-tasks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-todotask-from-tasks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-todotask-from-tasks-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-todotask-from-tasks-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.todoTask"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
   "@odata.etag":"W/\"xzyPKP0BiUGgld+lMKXwbQAAnBoTIw==\"",
   "importance":"low",
   "isReminderOn":false,
   "status":"notStarted",
   "title":"A new task",
   "createdDateTime":"2020-08-18T09:03:05.8339192Z",
   "lastModifiedDateTime":"2020-08-18T09:03:06.0827766Z",
   "categories": ["Important"],
   "id":"AlMKXwbQAAAJws6wcAAAA=",
   "body":{
      "content":"",
      "contentType":"text"
   },
   "linkedResources":[
      {
         "id":"f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9",
         "webUrl":"http://microsoft.com",
         "applicationName":"Microsoft",
         "displayName":"Microsoft"
      }
   ]
}
```



