---
title: 'event: delta'
description: 获取 **calendarView**（事件范围）中已添加、删除或更新的事件集。
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4e76bf6cd10682717bebe9365afa14ced47d4c90
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042588"
---
# <a name="event-delta"></a>event: delta

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取一 [组](../resources/event.md) 已在一个或多个日历中添加、删除或更新的事件资源。 

可以在邮箱的所有日历或特定日历中的事件，或日历的开始日期和结束日期) 定义的 **calendarView** (事件范围的事件集合中获取这些增量更改的特定类型的信息。 日历可以是默认日历或用户的其他一些指定日历。 在 **calendarView** 上获取增量更改的情况下，日历还可以是组日历。

**delta** 函数调用类似于指定日历的 或 请求，只不过通过在这些调用中的一个或多个调用中正确应用状态令牌，可以查询该日历中事件的增量更改。 `GET /events` `GET /calendarview` [](/graph/delta-query-overview#state-tokens) 这样，您即可维护和同步指定日历中的本地事件存储，而无需每次从服务器获取该日历的所有事件。

下表列出了事件上的 **delta** 函数与日历中 **calendarView** 上的 **delta** 函数之间的差异。

| 事件上的 Delta 函数  | calendarView 上的 Delta 函数  |
|:--------------------------|:---------------------------------------------------------|
| 获取日历中未受开始日期和结束日期范围限制的所有事件的增量更改。 或者，可以从该日期/时间或之后开始，获取由开始时间绑定的日历中的事件的增量更改。 | 获取 **calendarView** 的开始日期和结束日期/时间内事件的增量更改。 |
| 出于性能原因， **仅返回一** 组有限的事件属性。 随后用于扩展 `GET /events/{id}` 任何事件的客户端。 | 服务器端扩展返回一组更完整的 **事件** 属性。 |
| 响应包括单个实例和定期系列主控对象。 | 响应包括单个实例，以及定期系列的发生次数和异常。 |
| 适用于用户日历中的事件，但不包括组日历。 | 适用于用户和组日历中的事件。 |
| 当前仅在 beta 版本中可用。 | 在 v1.0 和 beta 版本中可用。 |

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Calendars.Read、Calendars.ReadWrite    |
|委派（个人 Microsoft 帐户） | Calendars.Read、Calendars.ReadWrite    |
|应用程序 | Calendars.Read、Calendars.ReadWrite |

## <a name="http-request"></a>HTTP 请求

本节显示初始 **delta** 函数调用的 HTTP 请求语法，以启动检索指定日历或日历视图中的所有事件的完全同步。 此语法不包含任何 [状态令牌](/graph/delta-query-overview#state-tokens)。 

成功响应的 或 `nextLink` 中返回的查询 URL `deltaLink` 包括状态令牌。 对于任何后续 **delta** 函数调用，请使用 中或前面的 `nextLink` 查询 `deltaLink` URL。

### <a name="delta-function-on-events-in-a-user-calendar-preview"></a>用户日历中事件的 Delta 函数 (预览) 
对从特定日期/时间开始或之后的所有事件应用 **delta** 函数，具体位于 (日历) ：

* 若要获取用户邮箱中所有事件或从指定日期/时间开始或之后的事件的增量 _更改：_
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/events/delta 
  GET /users/{id | userPrincipalName}/events/delta 

  GET /me/events/delta?startDateTime={start_datetime}
  GET /users/{id | userPrincipalName}/events/delta?startDateTime={start_datetime}
  ```

* 若要获取用户默认日历中所有事件或自指定日期/时间开始或之后的事件的增量 _更改_：
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendar/events/delta 
  GET /users/{id | userPrincipalName}/calendar/events/delta 

  GET /me/calendar/events/delta?startDateTime={start_datetime} 
  GET /users/{id | userPrincipalName}/calendar/events/delta?startDateTime={start_datetime}
  ```

* 若要获取所有事件的增量更改，或获取指定用户日历中指定日期/时间或之后开始 _的事件的增量更改_：
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendars/{id}/events/delta 
  GET /users/{id | userPrincipalName}/calendars/{id}/events/delta 

  GET /me/calendars/{id}/events/delta?startDateTime={start_datetime} 
  GET /users/{id | userPrincipalName}/calendars/{id}/events/delta?startDateTime={start_datetime}
  ```

* 若要获取增量更改，或获取指定日历组和日历中指定日期/时间或之后开始的事件： 
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendargroups/{id}/calendars/{id}/events/delta 
  GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/delta 

  GET /me/calendargroups/{id}/calendars/{id}/events/delta?startDateTime={start_datetime} 
  GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/delta?startDateTime={start_datetime}
  ```

<!-- Add back and fix html when group calendars are supported

### Delta function on events in a group calendar (preview)
* To get incremental changes of all the events, or of events starting on or after the specified date/time _in a group calendar_:
  !-- { "blockType": "ignored" } --
  ```http
  GET /groups/{id}/events/delta
  GET /groups/{id}/calendar/events/delta

  GET /groups/{id}/events/delta?startDateTime={start_datetime}
  GET /groups/{id}/calendar/events/delta?startDateTime={start_datetime}
  ```

  -->

### <a name="delta-function-on-calendarview-in-a-user-calendar"></a>用户日历中 calendarView 上的 Delta 函数
对 **指定的用户** 日历中由开始日期和结束日期/时间分隔的事件范围应用 delta 函数：

* 若要获取用户默认日历的日历视图中 _的增量更改：_
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  GET /users/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  ```

* 若要获取指定用户日历的日历视图中 _的增量更改：_
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendars/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  GET /users/{id}/calendars/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  ```

### <a name="delta-function-on-calendarview-in-a-group-calendar"></a>组日历中 calendarView 上的 Delta 函数
* 若要获取组日历的日历视图中 _的增量更改_：
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
  ```

## <a name="query-parameters"></a>查询参数

跟踪更改将引发一次或多组 **delta** 函数调用。 如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。 Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。 只需预先指定所需的任何查询参数一次。
在后续请求中，只需复制并应用上一响应中的 或 URL，因为此 URL 已包含所需的编码 `nextLink` `deltaLink` 参数。

| 查询参数      | 类型   |说明|
|:---------------|:--------|:----------|
|startDateTime|String|时间范围的开始日期和时间，以 ISO 8601 格式表示。例如，“2019-11-08T19:00:00-08:00”。<br>时区在参数值的时区偏移部分指定，如果存在，则不会影响 `Prefer: outlook.timezone` 标头。 如果值中未包含时区偏移量，则将其解释为 UTC。<br>对于 **日历中事件的增量** 是可选的。 <br>对于 **calendarView** 上的 **delta 是必需的**。 |
|endDateTime|String|时间范围的结束日期和时间，以 ISO 8601 格式表示。例如，“2019-11-08T20:00:00-08:00”。<br>时区在参数值的时区偏移部分指定，如果存在，则不会影响 `Prefer: outlook.timezone` 标头。 如果值中未包含时区偏移量，则将其解释为 UTC。<br>_不受_ 日历 **中事件** 上的 delta 支持。 <br>对于 **calendarView** 上的 **delta 是必需的**。|
| $deltatoken | string | 对同一个日历视图之前的 **delta** 函数调用的 `deltaLink` URL 中返回的 [状态令牌](/graph/delta-query-overview)，指示该组更改跟踪的完成状态。将此令牌包含在对该日历视图的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。|
| $skiptoken | string | 之前的 **delta** 函数调用的 `nextLink` URL 中返回的 [状态令牌](/graph/delta-query-overview)，指示同一个日历视图中有进一步的更改需要跟踪。 |

不支持 `$expand` `$filter` `$orderby` 、、、 `$select` 和 `$search` 。


## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明 |
|:---------------|:----------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |
| Content-Type  | string  | application/json. Required. |
| Prefer | string  | odata.maxpagesize={x}。可选。 |
| Prefer | string | outlook.timezone={Time zone string}。 可选，如果缺省，则采用 UTC。|

## <a name="response"></a>响应

### <a name="delta-function-on-events-preview"></a>事件和预览 (Delta) 
如果成功，此方法在响应正文中返回 响应代码 `200 OK` 和事件集合。 [](../resources/event.md) 出于 **性能** 原因，响应中的每个事件仅包含 **id** **、type** **、start** 和 **end** 属性。 随后 `GET /events/{id}` 使用 展开响应中的任意事件。  

### <a name="delta-function-on-calendarview"></a>calendarView 上的 Delta 函数
如果成功，此方法在响应正文中返回 响应代码 `200 OK` 和事件集合。 [](../resources/event.md)

希望获取通常从请求获取的所有 `GET /calendarview` 属性。 

## <a name="examples"></a>示例

### <a name="example-1-delta-function-on-events-in-a-calendar-preview"></a>示例 1：日历中事件的 Delta 函数 (预览) 
#### <a name="request"></a>请求
以下示例显示获取已登录用户的默认日历中的事件的初始同步请求，这些事件发生在指定参数上或之后 `startDateTime` 。 初始请求不包括任何状态令牌。 

请求使用 `Prefer: odata.maxpagesize` 标头将每个响应中的最大事件数限制为 1。 继续使用 中 `delta` 返回的 查询调用 函数 `@odata.nextLink` ，直到响应 `@odata.deltaLink` 中收到 。

<!-- {
  "blockType": "request",
  "name": "event_delta_events"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendar/events/delta?startDateTime=2020-06-12T00:00:00Z

Prefer: odata.maxpagesize=1
```

#### <a name="response"></a>响应

如果请求成功，响应将包含状态令牌，即 _\@ odata.nextLink_ 响应头) 中的 _skipToken_ (或 _\@ odata.deltaLink_ 响应头) 中的 _deltaToken_ (。
它们分别指示是应继续该轮还是已完成获取该轮的所有更改。

以下响应显示了 _\@ odata.nextLink_ 响应标头中的 _skipToken。_

<!-- {
  "blockType": "response",
  "name": "event_delta_events",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.nextLink":"https://graph.microsoft.com/beta/me/calendar/events/delta?$skiptoken=R0usmcdvmMu7jxWP8",
  "value": [
    { 
      "id": " AAMkADllMWMwNDkzLWJlY2EtNDIyOS1iZjAA=", 
      "type": "singleInstance", 
      "start": {  
             "DateTime": "2020-02-19T10:00:00.0000000",  
             "TimeZone": "UTC" 
         },  
       "end": {  
                "DateTime": "2020-02-19T11:00:00.0000000",  
                "TimeZone": "UTC"        
          }  
        } 
  ]
}
```


### <a name="example-2-delta-function-on-calendarview"></a>示例 2：calendarView 上的 Delta 函数
#### <a name="request"></a>请求

以下示例显示获取已登录用户指定日历中的事件的初始同步请求，该请求位于 **calendarView 指示的日期范围内**。 初始请求不包括任何状态令牌。 

请求使用 `Prefer: odata.maxpagesize` 标头将每个响应中事件的最大数量限制为 2 个。 继续使用 中返回的查询调用 函数，直到获取该日历视图中的所有事件和 响应 `delta` `@odata.nextLink` 中的 `@odata.deltaLink` 。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADI5M1BbeAAA="],
  "name": "event_delta_calendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendars/AAMkADI5M1BbeAAA=/calendarview/delta?startDateTime=2020-06-01T00:00:00Z&endDateTime=2020-06-10T00:00:00Z

Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-delta-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-delta-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-delta-calendarview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

如果请求成功，响应将包含状态令牌，即 _\@ odata.nextLink_ 响应头) 中的 _skipToken_ (或 _\@ odata.deltaLink_ 响应头) 中的 _deltaToken_ (。
它们分别指示是应继续该轮还是已完成获取该轮的所有更改。

以下响应显示了 _\@ odata.nextLink_ 响应标头中的 _skipToken。_

注意：为了提高可读性，可能缩短了此处显示的响应对象。 
<!-- {
  "blockType": "response",
  "name": "event_delta_calendarview",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(event)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/calendars/AAMkADI5M1BbeAAA=/calendarview/delta?$skiptoken=R0usmcdvmMu7jxWP8",
    "value": [
        {
            "@odata.type": "#microsoft.graph.event",
            "@odata.etag": "W/\"Jdsb3FEkPk2qoUHCdliYowACwixTgw==\"",
            "createdDateTime": "2020-06-16T04:05:43.8668791Z",
            "lastModifiedDateTime": "2020-06-16T04:08:27.354268Z",
            "changeKey": "Jdsb3FEkPk2qoUHCdliYowACwixTgw==",
            "categories": [],
            "transactionId": null,
            "originalStartTimeZone": "Pacific Standard Time",
            "originalEndTimeZone": "Pacific Standard Time",
            "uid": "040000008200E00074C5B7101A82E00800000000F088B8B95843D601000000000000000010000000165CD5547CFC9545B6492B261750B48C",
            "reminderMinutesBeforeStart": 15,
            "isReminderOn": false,
            "hasAttachments": false,
            "subject": "Summer party",
            "bodyPreview": "",
            "importance": "normal",
            "sensitivity": "normal",
            "isAllDay": false,
            "isCancelled": false,
            "isOrganizer": true,
            "IsRoomRequested": false,
            "AutoRoomBookingStatus": "None",
            "responseRequested": true,
            "seriesMasterId": null,
            "showAs": "busy",
            "type": "singleInstance",
            "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADI5MAAKkeE1QAAA%3D&exvsurl=1&path=/calendar/item",
            "onlineMeetingUrl": null,
            "isOnlineMeeting": false,
            "onlineMeetingProvider": "unknown",
            "allowNewTimeProposals": true,
            "OccurrenceId": null,
            "isDraft": false,
            "recurrence": null,
            "AutoRoomBookingOptions": null,
            "onlineMeeting": null,
            "id": "AAMkADI5MAAKkeE1QAAA=",
            "responseStatus": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "body": {
                "contentType": "html",
                "content": "<html>\r\n<head></head>\r\n<body lang=\"EN-US\" link=\"#0563C1\" vlink=\"#954F72\" style=\"\">\r\n<div class=\"WordSection1\">\r\n<p class=\"MsoNormal\">&nbsp;</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
            },
            "start": {
                "dateTime": "2020-06-02T20:00:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2020-06-02T22:30:00.0000000",
                "timeZone": "UTC"
            },
            "location": {
                "displayName": "",
                "locationType": "default",
                "uniqueIdType": "unknown",
                "address": {
                    "type": "unknown"
                },
                "coordinates": {}
            },
            "locations": [],
            "attendees": [
                {
                    "type": "required",
                    "status": {
                        "response": "none",
                        "time": "0001-01-01T00:00:00Z"
                    },
                    "emailAddress": {
                        "name": "Samantha Booth",
                        "address": "samanthab@contoso.onmicrosoft.com"
                    }
                }
            ],
            "organizer": {
                "emailAddress": {
                    "name": "Samantha Booth",
                    "address": "samanthab@contoso.onmicrosoft.com"
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.event",
            "@odata.etag": "W/\"Jdsb3FEkPk2qoUHCdliYowACwixTfw==\"",
            "createdDateTime": "2020-06-16T04:06:18.386713Z",
            "lastModifiedDateTime": "2020-06-16T04:08:19.5694048Z",
            "changeKey": "Jdsb3FEkPk2qoUHCdliYowACwixTfw==",
            "categories": [],
            "transactionId": null,
            "originalStartTimeZone": "Pacific Standard Time",
            "originalEndTimeZone": "Pacific Standard Time",
            "uid": "040000008200E00074C5B7101A82E0080000000060074BC55843D6010000000000000000100000002D33A89F36B10D43A12FD990B62858B2",
            "reminderMinutesBeforeStart": 15,
            "isReminderOn": true,
            "hasAttachments": false,
            "subject": "Summer party part 2",
            "bodyPreview": "",
            "importance": "normal",
            "sensitivity": "normal",
            "isAllDay": false,
            "isCancelled": false,
            "isOrganizer": true,
            "IsRoomRequested": false,
            "AutoRoomBookingStatus": "None",
            "responseRequested": true,
            "seriesMasterId": null,
            "showAs": "busy",
            "type": "singleInstance",
            "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADI5MAAKkeE1RAAA%3D&exvsurl=1&path=/calendar/item",
            "onlineMeetingUrl": null,
            "isOnlineMeeting": false,
            "onlineMeetingProvider": "unknown",
            "allowNewTimeProposals": true,
            "OccurrenceId": null,
            "isDraft": false,
            "recurrence": null,
            "AutoRoomBookingOptions": null,
            "onlineMeeting": null,
            "id": "AAMkADI5MAAKkeE1RAAA=",
            "responseStatus": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "body": {
                "contentType": "html",
                "content": "<html>\r\n<head></head>\r\n<body lang=\"EN-US\" link=\"#0563C1\" vlink=\"#954F72\" style=\"\">\r\n<div class=\"WordSection1\">\r\n<p class=\"MsoNormal\">&nbsp;</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
            },
            "start": {
                "dateTime": "2020-06-04T19:30:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2020-06-04T22:30:00.0000000",
                "timeZone": "UTC"
            },
            "location": {
                "displayName": "",
                "locationType": "default",
                "uniqueIdType": "unknown",
                "address": {
                    "type": "unknown"
                },
                "coordinates": {}
            },
            "locations": [],
            "attendees": [
                {
                    "type": "required",
                    "status": {
                        "response": "none",
                        "time": "0001-01-01T00:00:00Z"
                    },
                    "emailAddress": {
                        "name": "Samantha Booth",
                        "address": "samanthab@contoso.onmicrosoft.com"
                    }
                }
            ],
            "organizer": {
                "emailAddress": {
                    "name": "Samantha Booth",
                    "address": "samanthab@contoso.onmicrosoft.com"
                }
            }
        }
    ]
}
```

## <a name="see-also"></a>另请参阅

- [Microsoft Graph 增量查询](/graph/delta-query-overview)
- [获取文件夹中事件的增量更改](/graph/delta-query-events)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "event: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


