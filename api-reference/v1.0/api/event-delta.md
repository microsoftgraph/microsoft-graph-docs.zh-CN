---
title: 'event: delta'
description: '获取 **calendarView**（事件范围）中已添加、删除或更新的事件集。 '
localization_priority: Priority
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f410ec6aee93e70596d811760833ac54366858ba
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514012"
---
# <a name="event-delta"></a>event: delta

命名空间：microsoft.graph

获取一组 [事件](../resources/event.md) 已在用户主日历的 **calendarView** （由开始和结束日期定义的事件范围）中添加、删除或更新的资源。

通常，同步本地存储中 **calendarView** 中的事件需要一轮多次 **增量** 函数调用。 初始调用是完全同步，每个后续 **增量** 调用在同一轮中获取增量更改（添加、删除或更新）。 这样，就可以在指定的 **calendarView** 中维护和同步指定事件的本地存储，而无需每次从服务器中提取该日历的所有事件。

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
GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}

```

## <a name="query-parameters"></a>查询参数

跟踪事件更改会引发一组对 **delta** 函数的一次或多次调用。如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。你只需预先指定任意所需查询参数一次。在后续的请求中，只需复制并应用以前响应中的 `nextLink` 或 `deltaLink` URL，因为该 URL 已包含所需的编码参数。


| 查询参数      | 类型   |说明|
|:---------------|:--------|:----------|
|startDateTime|String|时间范围的开始日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T19:00:00.0000000”。|
|endDateTime|String|时间范围的结束日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T20:00:00.0000000”。|
| $deltatoken | string | 对同一个日历视图之前的 **delta** 函数调用的 `deltaLink` URL 中返回的 [状态令牌](/graph/delta-query-overview)，指示该组更改跟踪的完成状态。将此令牌包含在对该日历视图的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。|
| $skiptoken | string | 之前的 **delta** 函数调用的 `nextLink` URL 中返回的 [状态令牌](/graph/delta-query-overview)，指示同一个日历视图中有进一步的更改需要跟踪。 |

### <a name="odata-query-parameters"></a>OData 查询参数
- **calendarView** 需要 **增量** 函数调用，以返回通常从`GET /calendarview`请求中获取的相同属性。 不能使用 `$select` 只获取这些属性的子集。

- ****calendarView** 的增量** 函数不支持其他 OData 查询参数：`$expand`、`$filter`、`$orderby`和 `$search`。 


## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明 |
|:---------------|:----------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |
| Content-Type  | string  | application/json. Required. |
| Prefer | string  | odata.maxpagesize={x}。可选。 |
| Prefer | string | {Time zone}。可选，如果缺省，则采用 UTC。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [event](../resources/event.md) 集合对象。

在 **calendarView** 的日期范围绑定的 **增量** 函数调用中，你可能会发现 **增量** 调用在`@removed`下返回两种类型的事件，原因`deleted`： 
- 在日期范围内且自上一次 **增量** 调用以来已删除的事件。
- 在日期范围 _外部_ 的事件，以及自上一次 **增量** 调用以来已添加、删除或更新的事件。

根据方案所需的日期范围筛选 `@removed` 下的事件。

## <a name="example"></a>示例
##### <a name="request"></a>请求

以下示例演示了如何执行单次 **delta** 函数调用，并将响应正文中的事件最大数目限制为 2。

若要跟踪日历视图的更改，要使用正确的 [状态令牌](/graph/delta-query-overview)执行一次或多次 **delta** 函数调用来获取上次增量查询后的增量更改集。 


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_delta"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?startdatetime={start_datetime}&enddatetime={end_datetime}

Prefer: odata.maxpagesize=2
```

##### <a name="response"></a>响应
如果请求成功，响应将包括状态令牌，即 _skipToken_（位于 _@odata.nextLink_ 响应头中）或 _deltaToken_（位于 _@odata.deltaLink_ 响应头中）。它们分别指示应继续此组调用还是已获取该组的所有更改。

以下响应显示了 _@odata.nextLink_ 响应头中的 _skipToken_。

注意：为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 359

{
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "originalStartTimeZone": "originalStartTimeZone-value",
      "originalEndTimeZone": "originalEndTimeZone-value",
      "responseStatus": {
        "response": "response-value",
        "time": "datetime-value"
      },
      "transactionId": null,
      "iCalUId": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isDraft": false,
      "isReminderOn": true
    }
  ]
}
```

## <a name="see-also"></a>另请参阅

- [使用增量查询跟踪 Microsoft Graph 数据更改](/graph/delta-query-overview)
- [获取日历中事件的增量更改](/graph/delta-query-events)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

