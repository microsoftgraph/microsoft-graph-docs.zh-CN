---
title: 更新事件
description: 更新 event 对象的属性。
ms.openlocfilehash: b6ae7d818b68bfa1288a80f24383210e8a5d2909
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048354"
---
# <a name="update-event"></a>更新事件

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

更新[event](../resources/event.md)对象的属性。
## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Calendars.ReadWrite    |
|委派（个人 Microsoft 帐户） | Calendars.ReadWrite    |
|应用程序 | Calendars.ReadWrite |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/events/{id}
PATCH /users/{id | userPrincipalName}/events/{id}
PATCH /groups/{id}/events/{id}

PATCH /me/calendar/events/{id}
PATCH /users/{id | userPrincipalName}/calendar/events/{id}
PATCH /groups/{id}/calendar/events/{id}

PATCH /me/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}/events/{id}

PATCH /me/calendargroup/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}

PATCH /me/calendargroups/{id}/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。

| 属性       | 类型    | 说明 |
|:---------------|:--------|:------------|
| attendees|Attendee|事件的与会者集合。|
| body|ItemBody|与事件相关联的邮件正文。|
| categories|String|与事件相关联的类别。|
| end|DateTimeTimeZone|事件的结束日期和时间。<br/><br/>默认情况下，结束时间使用 UTC 格式。可以在 EndTimeZone 中指定可选的时区，用该时区表示结束时间并包括与 UTC 的时间偏移量。请注意，如果使用 EndTimeZone，必须为 StartTimeZone 指定一个值。<br/><br/>本示例指定太平洋标准时间的 2015 年 2 月 25 日晚上 9:34：“2015-02-25T21:34:00-08:00”。 |
| importance|String|事件的重要性。 可取值为：`low`、`normal`、`high`。|
| isAllDay|布尔|如果事件持续一整天，则设置为 true。|
| isReminderOn|布尔|如果设置警报以提醒用户有事件，则设置为 true。|
| location|Location|事件的位置。|
|locations|[位置](../resources/location.md)集合|举办或参加活动的地点。 **location** 和 **locations** 属性总是相互对应。 如果更新 **location** 属性，**locations** 集合中所有以前的位置都将被删除并替换为新的 **location** 值。 |
| recurrence|PatternedRecurrence|事件的定期模式。|
| reminderMinutesBeforeStart|Int32|事件开始时间（即提醒警报发生时间）之前的分钟数。|
| responseRequested|布尔|如果发件人希望接收事件被接受或拒绝时的响应，则设置为 true。|
| sensitivity|String| 可能的值是：`normal`、`personal`、`private`、`confidential`。|
| showAs|String|要显示的状态。 可能的值为： `free` ， `tentative`， `busy`， `oof`， `workingElsewhere`， `unknown`。|
| start|DateTimeTimeZone|事件的开始时间。 <br/><br/>默认情况下，开始时间使用 UTC 格式。可以在 StartTimeZone 中指定可选的时区，用该时区表示开始时间并包括与 UTC 的时间偏移量。请注意，如果使用 StartTimeZone，你也必须为 EndTimeZone 指定一个值。<br/><br/>本示例指定太平洋标准时间的 2015 年 2 月 25 日晚上 7:34：“2015-02-25T19:34:00-08:00”。  |
| subject|String|事件的主题行文本。|

由于**事件**资源支持[扩展](/graph/extensibility-overview)，您可以使用`PATCH`操作添加、 更新或删除您自己的扩展现有**事件**实例中的自定义属性中的特定于应用程序的数据。

如果您要更新的**事件**是定期系列的主事件，包含多个与会者，并且包含单独已更新的实例，多个电子邮件发送的通知： 一个用于主系列，每个实例具有一个已进行了更新。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [event](../resources/event.md) 对象。

>**注意：** 此方法可返回的错误代码 HTTP 400 错误请求响应`ErrorOccurrenceCrossingBoundary`并显示以下错误消息： 已修改的事件是通过或重叠相邻事件。 这指示更新违反了以下 Outlook 限制重复例外： 出现或上一个匹配项，天之前不能移动，不能将移动到或之后的以下匹配项的天。

## <a name="example"></a>示例

##### <a name="request"></a>请求

下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "update_event"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/events/{id}
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "recurrence": null,
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

##### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "recurrence": null,
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```


## <a name="see-also"></a>另请参阅

- [使用扩展向资源添加自定义数据](/graph/extensibility-overview)
- [使用开放扩展向用户添加自定义数据（预览）](/graph/extensibility-open-users)
- [使用架构扩展向组添加自定义数据（预览）](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
