---
title: 列出 calendarView
description: 获取日历视图中由时间范围定义的事件发生次数、异常和单一实例。
ms.localizationpriority: high
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6929040c368f312aecbfe85462871d208c95cadf
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697818"
---
# <a name="list-calendarview"></a>列出 calendarView

命名空间：microsoft.graph

从用户的默认日历 `(../me/calendarview)` 或其他一些日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单一实例。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Calendars.Read、Calendars.ReadWrite |
|委派（个人 Microsoft 帐户） | Calendars.Read、Calendars.ReadWrite    |
|应用程序 | Calendars.Read、Calendars.ReadWrite |

## <a name="http-request"></a>HTTP 请求

用户的默认 [calendar](../resources/calendar.md)。

<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

默认 [calendarGroup](../resources/calendargroup.md) 中的用户 [calendar](../resources/calendar.md)。
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a>查询参数

在请求 URL 中，提供以下必要查询参数的值。

| 参数     | 类型   | 说明                                                                                                            |
|:--------------|:-------|:-----------------------------------------------------------------------------------------------------------------------|
| startDateTime | String | 时间范围的开始日期和时间，以 ISO 8601 格式表示。例如，“2019-11-08T19:00:00-08:00”。 |
| endDateTime   | String | 时间范围的结束日期和时间，以 ISO 8601 格式表示。例如，“2019-11-08T20:00:00-08:00”。   |

`startDateTime` 和 `endDateTime` 的值使用值中指定的时区偏移量进行解释，并且不受 `Prefer: outlook.timezone` 标头（若有）的值影响。 如果值中未包含时区偏移量，则将其解释为 UTC。

此方法还支持一些 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。

具有 `$top` 的 **CalendarView** 的最小值为 1，最大值为 1000。 

> [!NOTE]
> [事件](../resources/event.md)的 **createdDateTime** 和 **lastModifiedDateTime** 属性不支持 `$select`。 若要获取它们的值，只需在 **calendarView** 上进行查询，而不应用 `$select`。

## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明 |
|:---------------|:--------|:--------|
| Authorization  | string | Bearer {token}。必需。  |
| Prefer: outlook.timezone  | string | 用于指定响应中开始时间和结束时间的时区。如果未指定，返回的这些时间值采用 UTC 时区。可选。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [event](../resources/event.md) 对象集合。

如果结果集跨多个页面，**calendarView** 将在响应中返回 **@odata.nextLink** 属性，其中包含指向下一页结果的 URL。如需详细信息，请参阅 [分页](/graph/paging)。

## <a name="example"></a>示例
### <a name="request"></a>请求
下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00-08:00&endDateTime=2017-01-07T19:00:00-08:00
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-calendarview-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-calendarview-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>响应
下面展示了示例响应。 
> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "originalStartTimeZone": "originalStartTimeZone-value",
      "originalEndTimeZone": "originalEndTimeZone-value",
      "responseStatus": {
        "response": "response-value",
        "time": "datetime-value"
      },
      "iCalUId": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isReminderOn": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List calendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
