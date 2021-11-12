---
title: 获取事件
description: 获取指定的 event 对象的属性和关系。
author: harini84
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c7ae6555e341d35507d0ebfa4725c57aebca8f56
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60946228"
---
# <a name="get-event"></a>获取事件

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取指定的 [event](../resources/event.md) 对象的属性和关系。

如果：

* 应用程序具有应用程序权限
* 应用具有来自一个用户的适当委派[](#permissions)权限，另一个用户已与该用户共享日历，或者向该用户授予了委派访问权限。 请参阅[详细信息和示例](/graph/outlook-get-shared-events-calendars)。

由于 **事件** 资源 [支持扩展](/graph/extensibility-overview)，因此您还可以使用 操作获取事件实例中的自定义属性 `GET` 和 **扩展** 数据。


### <a name="support-various-time-zones"></a>支持不同时区

对于返回事件的所有 GET 操作，你可以使用 `Prefer: outlook.timezone` 标头在响应中指定事件开始和结束时间的时区。 

例如，下面的 `Prefer: outlook.timezone` 标头将响应中的开始和结束时间设置为东部标准时间。
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

如果该事件是在不同的时区中创建的，则根据 `Prefer` 标头中指定的时区调整开始和结束时间。请查看此 [列表](../resources/datetimetimezone.md) 了解支持的时区名称。如果未指定 `Prefer: outlook.timezone` 标头，则返回用 UTC 表示的开始和结束时间。

可以使用 **事件** 资源中的 **OriginalStartTimeZone** 和 **OriginalEndTimeZone** 属性来查找创建事件时使用的时区。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Calendars.Read    |
|委派（个人 Microsoft 帐户） | Calendars.Read    |
|应用程序 | Calendars.Read |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}
GET /users/{id | userPrincipalName}/events/{id}
GET /groups/{id}/events/{id}

GET /me/calendar/events/{id}
GET /users/{id | userPrincipalName}/calendar/events/{id}
GET /groups/{id}/calendar/events/{id}

GET /me/calendars/{id}/events/{id}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}

GET /me/calendargroups/{id}/calendars/{id}/events/{id}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。
## <a name="request-headers"></a>请求头
| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |
| Prefer: outlook.timezone | string | 用于指定响应中开始时间和结束时间的时区。如果未指定，返回的这些时间值采用 UTC 时区。可选。 |
| Prefer: outlook.body-content-type | string | 要返回的 **body** 属性的格式。 可取值为“text”或“html”。 如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。 如果未指定此头，采用 HTML 格式返回 **body** 属性。 可选。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [event](../resources/event.md) 对象。
## <a name="examples"></a>示例

### <a name="example-1-get-a-specified-event"></a>示例 1：获取指定事件
#### <a name="request"></a>请求
以下示例获取指定的事件。 它指定以下内容：

- 获取以太平洋标准时间格式返回的日期时间值的 `Prefer: outlook.timezone` 标头。 
- 返回特定属性的 `$select` 查询参数。如果没有 `$select` 参数，将返回所有事件属性。

该请求未指定任何 `Prefer: outlook.body-content-type` 标头来指示返回的事件正文的特定格式。 


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_event"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/AAMkAGIAAAoZDOFAAA=/?$select=subject,body,bodyPreview,organizer,attendees,start,end,location,hideAttendees 
Prefer: outlook.timezone="Pacific Standard Time"
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应
下面是一个响应示例。 由于未指定任何 `Prefer: outlook.body-content-type` 标头，将以默认 HTML 格式返回 **body** 属性。 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview,organizer,attendees,start,end,location,hideAttendees)/$entity",
    "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAAKGWwbw==\"",
    "id":"AAMkAGIAAAoZDOFAAA=",
    "subject":"Orientation ",
    "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
    "body":{
        "contentType":"html",
        "content":"<html><head></head><body><p>Dana, this is the time you selected for our orientation. Please bring the notes I sent you.</p></body></html>"
    },
    "start":{
        "dateTime":"2017-04-21T10:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "end":{
        "dateTime":"2017-04-21T12:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "location": {
        "displayName": "Assembly Hall",
        "locationType": "default",
        "uniqueId": "Assembly Hall",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Assembly Hall",
            "locationType": "default",
            "uniqueIdType": "unknown"
        }
    ],
    "attendees":[
        {
            "type":"required",
            "status":{
                "response":"none",
                "time":"0001-01-01T00:00:00Z"
            },
            "emailAddress":{
                "name":"Samantha Booth",
                "address":"samanthab@a830edad905084922E17020313.onmicrosoft.com"
            }
        },
        {
            "type":"required",
            "status":{
                "response":"tentativelyAccepted",
                "time":"0001-01-01T00:00:00Z"
            },
            "proposedNewTime": {
                "start": {
                    "dateTime": "2019-08-16T12:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                },
                "end": {
                    "dateTime": "2019-08-16T14:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                }
            },
            "emailAddress":{
                "name":"Dana Swope",
                "address":"danas@a830edad905084922E17020313.onmicrosoft.com"
            }
        }
    ],
    "hideAttendees": false,
    "organizer":{
        "emailAddress":{
            "name":"Samantha Booth",
            "address":"samanthab@a830edad905084922E17020313.onmicrosoft.com"
        }
    }
}
```
### <a name="example-2-get-the-body-property-in-text-format"></a>示例 2：获取文本格式的 body 属性
#### <a name="request"></a>请求
以下示例演示如何使用标头获取文本格式的 `Prefer: outlook.body-content-type="text"` 指定事件的 body属性。

该请求还使用 `$select` 查询参数返回特定属性。 如果没有 `$select` 参数，将返回所有事件属性。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_event_in_text"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/AAMkAGI1AAAoZDOFAAA=/?$select=subject,body,bodyPreview
Prefer: outlook.body-content-type="text"
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-event-in-text-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应
下面是一个响应示例。 以文本格式返回 **body** 属性。 

<!-- {
  "blockType": "response",
  "name": "get_event_in_text",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.body-content-type="text"

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview)/$entity",
    "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAAKGWwbw==\"",
    "id":"AAMkAGI1AAAoZDOFAAA=",
    "subject":"Orientation ",
    "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
    "body":{
        "contentType":"text",
        "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
    }
}
```

### <a name="example-3-get-an-event-that-specifies-more-than-one-location"></a>示例 3：获取指定多个位置的事件
#### <a name="request"></a>请求

以下示例显示获取指定多个位置的事件。 该请求指定返回特定属性的 `$select` 查询参数。 


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_event_multiple_locations"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/AAMkADAGAADDdm4NAAA=/?$select=subject,body,bodyPreview,organizer,attendees,start,end,location,locations
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-multiple-locations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-multiple-locations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-multiple-locations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-event-multiple-locations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应
下面是响应的示例。**位置** 属性包含为其组织事件的 3 个位置的详细信息。 

由于请求未指定任何 或 标头，start 和 end 属性以默认的 UTC 时区显示，并且正文 `Prefer: outlook.timezone` `Prefer: outlook.body-content-type` 采用默认 HTML 格式。    

<!-- {
  "blockType": "response",
  "name": "get_event_multiple_locations",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/events(subject,body,bodyPreview,organizer,attendees,start,end,location,locations)/$entity",
  "@odata.etag":"W/\"y53lbKh6jkaxHzFwGhgyxgAAw5zhug==\"",
  "id":"AAMkADAGAADDdm4NAAA=",
  "subject":"Plan summer company picnic",
  "bodyPreview":"Let's kick-start this event planning!",
  "body":{
    "contentType":"html",
    "content":"<html>\r\n<head>\r\n</head>\r\n<body>\r\nLet's kick-start this event planning!\r\n</body>\r\n</html>\r\n"
  },
  "start":{
    "dateTime":"2017-08-30T11:00:00.0000000",
    "timeZone":"UTC"
  },
  "end":{
    "dateTime":"2017-08-30T12:00:00.0000000",
    "timeZone":"UTC"
  },
  "location":{
    "displayName":"Conf Room 3; Fourth Coffee; Home Office",
    "locationType":"default",
    "uniqueId":"Conf Room 3; Fourth Coffee; Home Office",
    "uniqueIdType":"private"
  },
  "locations":[
    {
      "displayName":"Conf Room 3",
      "locationType":"default",
      "uniqueIdType":"unknown"
    },
    {
      "displayName":"Fourth Coffee",
      "locationType":"default",
      "uniqueId":"Fourth Coffee",
      "uniqueIdType":"private",
      "address":{
        "type":"unknown",
        "street":"4567 Main St",
        "city":"Redmond",
        "state":"WA",
        "countryOrRegion":"US",
        "postalCode":"32008"
      },
      "coordinates":{
        "latitude":47.672,
        "longitude":-102.103
      }
    },
    {
      "displayName":"Home Office",
      "locationType":"default",
      "uniqueIdType":"unknown"
    }
  ],
  "attendees":[
    {
      "type":"required",
      "status":{
        "response":"none",
        "time":"0001-01-01T00:00:00Z"
      },
      "emailAddress":{
        "name":"Dana Swope",
        "address":"DanaS@contoso.onmicrosoft.com"
      }
    },
    {
      "type":"required",
      "status":{
        "response":"none",
        "time":"0001-01-01T00:00:00Z"
      },
      "emailAddress":{
        "name":"Alex Wilber",
        "address":"AlexW@contoso.onmicrosoft.com"
      }
    }
  ],
  "organizer":{
    "emailAddress":{
      "name":"Adele Vance",
      "address":"AdeleV@contoso.onmicrosoft.com"
    }
  }
}
```
### <a name="example-4-expand-a-series-master-event"></a>示例 4：展开系列主事件
#### <a name="request"></a>请求

以下示例显示展开定期系列的系列主事件，并出现异常和已取消的事件。 该请求指定返回特定属性的 `$select` 查询参数。 

<!-- {
  "blockType": "request",
  "name": "get_event_seriesMaster_expansion"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/AAMkADAGAADDdm4NAAA=/?$select=subject,start,end,occurrenceId,exceptionOccurrences,cancelledOccurrences$expand=exceptionOccurrences
```
#### <a name="response"></a>响应
GET 操作返回系列主事件的选定属性。 具体而言，对于 **exceptionOccurrences** 集合中的事件，操作返回 **id** 属性，以及 **subject、start、end** 和 **occurrenceId** (**的** 适用选定属性) 。 对于 **cancelledOccurrences** 集合中的事件，由于这些事件不再存在，因此操作仅返回 **其 occurrenceId** 属性值。

<!-- {
  "blockType": "response",
  "name": "get_event_seriesMaster_expansion",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/events(subject,start,end,occurrenceId,exceptionOccurrences,cancelledOccurrences)/$entity",
  "@odata.etag":"W/\"y53lbKh6jkaxHzFwGhgyxgAAw5zhug==\"",
  "id":"AAMkADAGAADDdm4NAAA=",
  "subject": "Daily stand-up",
  "cancelledOccurrences": [
     "OID.AAMkADAGAADDdm4NAAA=.2020-04-30",
     "OID.AAMkADAGAADDdm4NAAA=.2020-05-07",
     "OID.AAMkADAGAADDdm4NAAA=.2020-05-14"
    ],
  "occurrenceId": null,
    "start": {
        "dateTime": "2020-04-23T11:30:00.0000000",
        "timeZone": "UTC"
    },
  "end": {
        "dateTime": "2020-04-23T12:00:00.0000000",
        "timeZone": "UTC"
    },
  "exceptionOccurrences": [
        {
            "id": "AAMkADM0ZGRhMjdjLTA==",
            "Subject": "SM update 24",
            "occurrenceId": "OID.AAMkADAGAADDdm4NAAA=.2020-05-21",
            "start": {
                "dateTime": "2020-05-21T11:30:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2020-05-21T12:00:00.0000000",
                "timeZone": "UTC"
            }
        }
    ]
}
```

## <a name="see-also"></a>另请参阅

- [使用扩展向资源添加自定义数据](/graph/extensibility-overview)
- [使用开放扩展向用户添加自定义数据](/graph/extensibility-open-users)
- [使用架构扩展向组添加自定义数据](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


