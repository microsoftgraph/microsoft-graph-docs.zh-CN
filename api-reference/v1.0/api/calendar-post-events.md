---
title: 创建事件
description: 使用此 API 在默认或指定的日历中创建新事件。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 328002ce6a4356f4e0c8ab62de59a83a2fe85585
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882423"
---
# <a name="create-event"></a><span data-ttu-id="f3476-103">创建事件</span><span class="sxs-lookup"><span data-stu-id="f3476-103">Create event</span></span>

<span data-ttu-id="f3476-104">使用此 API 在默认或指定的日历中创建新事件。</span><span class="sxs-lookup"><span data-stu-id="f3476-104">Use this API to create a new event in the default or specified calendar.</span></span>
## <a name="permissions"></a><span data-ttu-id="f3476-105">权限</span><span class="sxs-lookup"><span data-stu-id="f3476-105">Permissions</span></span>
<span data-ttu-id="f3476-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f3476-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3476-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f3476-108">Permission type</span></span>      | <span data-ttu-id="f3476-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f3476-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3476-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f3476-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f3476-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f3476-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f3476-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f3476-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3476-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f3476-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f3476-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f3476-114">Application</span></span> | <span data-ttu-id="f3476-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f3476-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3476-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f3476-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="f3476-117">用户或组的默认 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="f3476-117">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events
POST /groups/{id}/calendar/events
```
<span data-ttu-id="f3476-118">默认 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="f3476-118">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events

POST /me/calendarGroup/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="f3476-119">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="f3476-119">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendarGroups/{id}/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="f3476-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f3476-120">Request headers</span></span>
| <span data-ttu-id="f3476-121">标头</span><span class="sxs-lookup"><span data-stu-id="f3476-121">Header</span></span>       | <span data-ttu-id="f3476-122">值</span><span class="sxs-lookup"><span data-stu-id="f3476-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f3476-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3476-123">Authorization</span></span>  | <span data-ttu-id="f3476-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f3476-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f3476-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f3476-126">Content-Type</span></span>  | <span data-ttu-id="f3476-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f3476-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f3476-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="f3476-129">Request body</span></span>
<span data-ttu-id="f3476-130">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f3476-130">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f3476-131">响应</span><span class="sxs-lookup"><span data-stu-id="f3476-131">Response</span></span>

<span data-ttu-id="f3476-132">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f3476-132">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3476-133">示例</span><span class="sxs-lookup"><span data-stu-id="f3476-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f3476-134">请求</span><span class="sxs-lookup"><span data-stu-id="f3476-134">Request</span></span>
<span data-ttu-id="f3476-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f3476-135">Here is an example of the request.</span></span>
<span data-ttu-id="f3476-136">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f3476-136">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f3476-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="f3476-137">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGViNDU7zAAAAAGtlAAA="],
  "name": "create_event_from_calendar"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendars/AAMkAGViNDU7zAAAAAGtlAAA=/events
Content-type: application/json

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does mid month work for you?"
  },
  "start": {
      "dateTime": "2019-03-15T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2019-03-15T14:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"adelev@contoso.onmicrosoft.com",
        "name": "Adele Vance"
      },
      "type": "required"
    }
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f3476-138">C#</span><span class="sxs-lookup"><span data-stu-id="f3476-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f3476-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="f3476-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f3476-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f3476-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f3476-141">Java</span><span class="sxs-lookup"><span data-stu-id="f3476-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-event-from-calendar-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f3476-142">响应</span><span class="sxs-lookup"><span data-stu-id="f3476-142">Response</span></span>
<span data-ttu-id="f3476-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f3476-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('5d8d505c-864f-4804-88c7-4583c966cde8')/calendars('AAMkAGViNDU7zAAAAAGtlAAA%3D')/events/$entity",
    "@odata.etag": "W/\"/IUUrIl3PkG1JCSsPfU+8wAAGXjEpA==\"",
    "id": "AAMkAGViNDU7zAAAAA7zAAAZb2ckAAA=",
    "createdDateTime": "2019-02-28T21:17:57.56197Z",
    "lastModifiedDateTime": "2019-02-28T21:17:59.044919Z",
    "changeKey": "/IUUrIl3PkG1JCSsPfU+8wAAGXjEpA==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "iCalUId": "040000008200E641B4C",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Let's go for lunch",
    "bodyPreview": "Does mid month work for you?",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkAGViNDU7zAAAAA7zAAAZb2ckAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "recurrence": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes mid month work for you?\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2019-03-15T12:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "end": {
        "dateTime": "2019-03-15T14:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "location": {
        "displayName": "Harry's Bar",
        "locationType": "default",
        "uniqueId": "Harry's Bar",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Harry's Bar",
            "locationType": "default",
            "uniqueId": "Harry's Bar",
            "uniqueIdType": "private"
        }
    ],
    "attendees": [
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Adele Vance",
                "address": "AdeleV@contoso.OnMicrosoft.com"
            }
        }
    ],
    "organizer": {
        "emailAddress": {
            "name": "Megan Bowen",
            "address": "MeganB@contoso.OnMicrosoft.com"
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
