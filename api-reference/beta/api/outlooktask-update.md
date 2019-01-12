---
title: 更新 outlooktask
description: 更改 Outlook 任务的可写属性。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: c0d2ff13f3e7971e686389709fbdde027458ef67
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964933"
---
# <a name="update-outlooktask"></a>更新 outlooktask

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

更改 Outlook 任务的可写属性。

通过**完成**操作，或明确的修补程序操作，可以设置**completedDateTime**属性。 如果您使用的修补程序设置**completedDateTime**，请确保将**状态**设置为`completed`以及。

默认情况下，此操作 （和文章、 GET，和[完成](../api/outlooktask-complete.md)任务操作） 返回与日期相关的属性采用 UTC。 您可以使用`Prefer: outlook.timezone`标头，使其具有不同于 UTC 时区中表示的响应中的所有日期相关的属性。

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
PATCH /me/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:-----------|:-----------|
| Authorization  | Bearer {token}。必需。 |
| Prefer: outlook.timezone | 响应，它可以采用 UTC 如果未指定此标头中指定的时间属性的时区。 可选。|

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|assignedTo|字符串|已分配任务的人员的名称。|
|body|[itemBody](../resources/itembody.md)|任务正文通常包含有关任务的信息。 请注意，仅 HTML 支持类型。|
|categories|String collection|类别与任务关联。|
|changeKey|字符串|任务的版本。|
|completedDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|中指定的时区任务已完成的日期。|
|createdDateTime|DateTimeOffset|日期和时间创建任务时。 默认情况下，它是采用 UTC。 您可以提供请求标头中自定义时区。 该属性值使用 ISO 8601 格式。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|dueDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|在指定时区的任务完成日期。|
|hasAttachments|布尔|设置为 true 如果任务的附件。|
|importance|string|事件的重要性。 可取值为：`low`、`normal`、`high`。|
|isReminderOn|布尔|如果，设置为 true 设置通知提醒的用户的任务。|
|lastModifiedDateTime|DateTimeOffset|日期和上次修改任务的时间。 默认情况下，它是采用 UTC。 您可以提供请求标头中自定义时区。 该属性值使用 ISO 8601 格式，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|owner|字符串|创建任务的人员的名称。|
|parentFolderId|String|任务的父文件夹的唯一标识符。|
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|定期模式的任务。|
|reminderDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|发生的日期和时间的任务的提醒通知。|
|sensitivity|string|指示任务的隐私级别。 可取值为：`normal`、`personal`、`private`、`confidential`。|
|startDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|在指定时区时的任务是开始日期。|
|status|string|指示的状态或任务进度。 可取值为：`notStarted`、`inProgress`、`completed`、`waitingOnOthers`、`deferred`。|
|subject|字符串|简要说明或任务的标题。|

## <a name="response"></a>响应

如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[outlookTask](../resources/outlooktask.md)对象。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面的示例修改**dueDateTime**属性，并使用`Prefer: outlook.timezone`标头以指定表达东部标准时间 (EST) 的响应中与日期相关的属性。
<!-- {
  "blockType": "request",
  "name": "update_outlooktask"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MTHgwAAA=')

Prefer: outlook.timezone="Eastern Standard Time"
Content-type: application/json
Content-length: 76

{
  "dueDateTime":  {
      "dateTime": "2016-05-06T16:00:00",
      "timeZone": "Eastern Standard Time"
  }
}
```

### <a name="response"></a>响应

下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 376

{
    "id": "AAMkADA1MTHgwAAA=",
    "createdDateTime": "2016-04-22T18:19:18.9526004-04:00",
    "lastModifiedDateTime": "2016-04-22T18:38:20.5541528-04:00",
    "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIW9XXg==",
    "categories": [
    ],
    "assignedTo": null,
    "body": {
        "contentType": "text",
        "content": ""
    },
    "completedDateTime": null,
    "dueDateTime": {
        "dateTime": "2016-05-06T00:00:00.0000000",
        "timeZone": "Eastern Standard Time"
    },
    "hasAttachments":false,
    "importance": "normal",
    "isReminderOn": false,
    "owner": "Administrator",
    "parentFolderId": "AQMkADA1MTIBEgAAAA==",
    "recurrence": null,
    "reminderDateTime": null,
    "sensitivity": "normal",
    "startDateTime": {
        "dateTime": "2016-05-03T00:00:00.0000000",
        "timeZone": "Eastern Standard Time"
    },
    "status": "notStarted",
    "subject": "Shop for children's weekend"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update outlooktask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
