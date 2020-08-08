---
title: 'event: tentativelyAccept'
description: 暂时接受用户日历中的指定事件。
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1b7bb4d4b9540deb60c064c75e67ccfcad008de0
ms.sourcegitcommit: 93b6781adf2c889235022d34ab50e2a4d62760c5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/07/2020
ms.locfileid: "46589128"
---
# <a name="event-tentativelyaccept"></a>event: tentativelyAccept

命名空间：microsoft.graph

暂时接受用户[日历](../resources/calendar.md)中的指定[事件](../resources/event.md)。

如果事件允许建议的新时间，在对事件做出响应时，被邀请者可以通过包含**proposedNewTime**参数来选择建议替代时间。 有关如何建议时间以及如何接收和接受新时间建议的详细信息，请参阅[建议新会议时间](/graph/outlook-calendar-meeting-proposals)。

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
POST /me/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/events/{id}/tentativelyAccept

POST /me/calendar/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendar/events/{id}/tentativelyAccept

POST /me/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroup/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/tentativelyAccept

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept
```
## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |
| Content-Type | string  | 实体正文中的数据性质。必需。 |

## <a name="request-body"></a>请求正文
在请求正文中，提供具有以下参数的 JSON 对象。

| 参数    | 类型   |说明|
|:---------------|:--------|:----------|
|注释|String|响应中包含的文本。可选。|
|proposedNewTime|[timeSlot](../resources/timeslot.md)|会议请求开始和结束时由被邀请者建议的备用日期/时间。 仅对允许新时间建议的事件有效。 设置此参数需要将**sendResponse**设置为 `true` 。 可选。|
|sendResponse|Boolean|如果将响应发送给组织者，则值为 `true`；否则为 `false`。可选。默认值为 `true`。|

## <a name="response"></a>响应

如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。

如果出现以下一种或两种情况，此操作将返回 HTTP 400：

- 包含**proposedNewTime**参数，但**事件**的**allowNewTimeProposals**属性为 `false` 。 
- 包含**proposedNewTime**参数，但**sendResponse**参数设置为 `false` 。

## <a name="example"></a>示例
下面是一个如何调用此 API 的示例。
### <a name="request"></a>请求
在下面的示例中，登录用户对指定事件的响应是暂定的，将**sendResponse**参数设置为 true，并在**proposedNewTime**参数中包含一个替代时间。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_tentativelyaccept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/tentativelyAccept
Content-type: application/json

{
  "comment": "I may not be able to make this week. How about next week?",
  "sendResponse": true,
  "proposedNewTime": {
      "start": { 
          "dateTime": "2019-12-02T18:00:00", 
          "timeZone": "Pacific Standard Time" 
      }, 
      "end": { 
          "dateTime": "2019-12-02T19:00:00", 
          "timeZone": "Pacific Standard Time" 
      }     
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-tentativelyaccept-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-tentativelyaccept-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-tentativelyaccept-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-tentativelyaccept-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
下面是一个响应示例。
<!-- {
  "blockType": "response",
  "name": "event_tentativelyaccept",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: tentativelyAccept",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
