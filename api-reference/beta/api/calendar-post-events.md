---
title: 创建事件
description: 使用此 API 在默认或指定的日历中创建新事件。
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 007a8e5cb98d76f5bf36f14e7730f96b7ae86457
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987685"
---
# <a name="create-event"></a><span data-ttu-id="57253-103">创建事件</span><span class="sxs-lookup"><span data-stu-id="57253-103">Create event</span></span>

<span data-ttu-id="57253-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57253-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57253-105">使用此 API 在日历中创建新事件。</span><span class="sxs-lookup"><span data-stu-id="57253-105">Use this API to create a new event in a calendar.</span></span> <span data-ttu-id="57253-106">日历可以是 [用户](../resources/user.md)的一个，也可以是 Microsoft 365 [组](../resources/group.md)的默认日历。</span><span class="sxs-lookup"><span data-stu-id="57253-106">The calendar can be one for a [user](../resources/user.md), or the default calendar of a Microsoft 365 [group](../resources/group.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="57253-107">权限</span><span class="sxs-lookup"><span data-stu-id="57253-107">Permissions</span></span>
<span data-ttu-id="57253-108">根据创建事件的日历类型和所请求的权限类型（委派型或应用程序），需要下列某一权限来调用此 API。</span><span class="sxs-lookup"><span data-stu-id="57253-108">Depending on the type of calendar that the event is created in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="57253-109">要了解详细信息（包括如何选择权限），请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="57253-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="57253-110">日历</span><span class="sxs-lookup"><span data-stu-id="57253-110">Calendar</span></span> | <span data-ttu-id="57253-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="57253-111">Delegated (work or school account)</span></span> | <span data-ttu-id="57253-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="57253-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57253-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="57253-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="57253-114">用户日历</span><span class="sxs-lookup"><span data-stu-id="57253-114">user calendar</span></span> | <span data-ttu-id="57253-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57253-115">Calendars.ReadWrite</span></span> | <span data-ttu-id="57253-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57253-116">Calendars.ReadWrite</span></span> | <span data-ttu-id="57253-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="57253-117">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="57253-118">组日历</span><span class="sxs-lookup"><span data-stu-id="57253-118">group calendar</span></span> | <span data-ttu-id="57253-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57253-119">Group.ReadWrite.All</span></span> | <span data-ttu-id="57253-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="57253-120">Not supported.</span></span> | <span data-ttu-id="57253-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="57253-121">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="57253-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="57253-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="57253-123">用户或组的默认 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="57253-123">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events
POST /groups/{id}/calendar/events
```
<span data-ttu-id="57253-124">默认 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="57253-124">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events

POST /me/calendarGroup/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="57253-125">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="57253-125">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendarGroups/{id}/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="57253-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="57253-126">Request headers</span></span>
| <span data-ttu-id="57253-127">标头</span><span class="sxs-lookup"><span data-stu-id="57253-127">Header</span></span>       | <span data-ttu-id="57253-128">值</span><span class="sxs-lookup"><span data-stu-id="57253-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="57253-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="57253-129">Authorization</span></span>  | <span data-ttu-id="57253-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="57253-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="57253-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="57253-132">Content-Type</span></span>  | <span data-ttu-id="57253-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="57253-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="57253-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="57253-135">Request body</span></span>
<span data-ttu-id="57253-136">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="57253-136">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="57253-137">响应</span><span class="sxs-lookup"><span data-stu-id="57253-137">Response</span></span>

<span data-ttu-id="57253-138">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="57253-138">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="57253-139">示例</span><span class="sxs-lookup"><span data-stu-id="57253-139">Examples</span></span>

### <a name="example-1-create-an-event-in-a-specific-calendar"></a><span data-ttu-id="57253-140">示例 1：在特定日历中创建事件</span><span class="sxs-lookup"><span data-stu-id="57253-140">Example 1: Create an event in a specific calendar</span></span>

#### <a name="request"></a><span data-ttu-id="57253-141">请求</span><span class="sxs-lookup"><span data-stu-id="57253-141">Request</span></span>
<span data-ttu-id="57253-142">下面的示例在特定日历中创建一个事件，并为该事件分配一个可选的 **transactionId** 值。</span><span class="sxs-lookup"><span data-stu-id="57253-142">The following example creates an event in a specific calendar and assigns the event an optional **transactionId** value.</span></span>

<span data-ttu-id="57253-143">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="57253-143">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

# <a name="http"></a>[<span data-ttu-id="57253-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="57253-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGViNDU7zAAAAAGtlAAA="],
  "name": "create_event_from_calendar"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendars/AAMkAGViNDU7zAAAAAGtlAAA=/events
Content-type: application/json

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does next month work for you?"
  },
  "start": {
      "dateTime": "2019-03-10T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2019-03-10T14:00:00",
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
  ],
  "transactionId":"7E163156-7762-4BEB-A1C6-729EA81755A7"
}
```
# <a name="c"></a>[<span data-ttu-id="57253-145">C#</span><span class="sxs-lookup"><span data-stu-id="57253-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="57253-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57253-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="57253-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57253-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="57253-148">响应</span><span class="sxs-lookup"><span data-stu-id="57253-148">Response</span></span>
<span data-ttu-id="57253-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="57253-149">Here is an example of the response.</span></span> 

><span data-ttu-id="57253-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="57253-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="57253-151">所有属性都将从实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="57253-151">All  the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('5d8d505c-864f-4804-88c7-4583c966cde8')/calendars('AAMkAGViNDU7zAAAAAGtlAAA%3D')/events/$entity",
    "@odata.etag": "W/\"/IUUrIl3PkG1JCSsPfU+8wAAGXjGjw==\"",
    "id": "AAMkAGViNDU7zAAAAA7zAAAZe6CkAAA=",
    "createdDateTime": "2019-02-28T21:36:26.7105485Z",
    "lastModifiedDateTime": "2019-02-28T21:36:26.9577227Z",
    "changeKey": "/IUUrIl3PkG1JCSsPfU+8wAAGXjGjw==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "uid": "040000008200C780DAE",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Let's go for lunch",
    "bodyPreview": "Does next month work for you?",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isDraft": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "transactionId":"7E163156-7762-4BEB-A1C6-729EA81755A7",
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkAGViNDU7zAAAAA7zAAAZe6CkAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "isOnlineMeeting": false,
    "onlineMeetingProvider": "unknown",
    "onlineMeeting": null,
    "recurrence": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes next month work for you?\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2019-03-10T12:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "end": {
        "dateTime": "2019-03-10T14:00:00.0000000",
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

### <a name="example-2-create-and-enable-an-event-as-an-online-meeting"></a><span data-ttu-id="57253-152">示例 2：创建事件并启用为联机会议</span><span class="sxs-lookup"><span data-stu-id="57253-152">Example 2: Create and enable an event as an online meeting</span></span>

#### <a name="request"></a><span data-ttu-id="57253-153">请求</span><span class="sxs-lookup"><span data-stu-id="57253-153">Request</span></span>
<span data-ttu-id="57253-154">下面的示例在已登录用户的指定日历中创建一个事件，并将其作为联机会议来启用。</span><span class="sxs-lookup"><span data-stu-id="57253-154">The following example creates an event in the specified calendar of the signed-in user and enables it as an online meeting.</span></span>

<span data-ttu-id="57253-155">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="57253-155">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

# <a name="http"></a>[<span data-ttu-id="57253-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="57253-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGViNDU8zAAAAAGtlAAA="],
  "name": "create_event_from_calendar_with_online_meeting"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendars/AAMkAGViNDU8zAAAAAGtlAAA=/events
Content-type: application/json

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does next month work for you?"
  },
  "start": {
      "dateTime": "2019-03-10T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2019-03-10T14:00:00",
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
  ],
  "isOnlineMeeting": true,
  "onlineMeetingProvider": "teamsForBusiness"
}
```
# <a name="c"></a>[<span data-ttu-id="57253-157">C#</span><span class="sxs-lookup"><span data-stu-id="57253-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-calendar-with-online-meeting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="57253-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57253-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-calendar-with-online-meeting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="57253-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57253-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-calendar-with-online-meeting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="57253-160">响应</span><span class="sxs-lookup"><span data-stu-id="57253-160">Response</span></span>
<span data-ttu-id="57253-161">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="57253-161">Here is an example of the response.</span></span> 

> <span data-ttu-id="57253-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="57253-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('5d8d505c-864f-4804-88c7-4583c966cde8')/calendars('AAMkAGViNDU8zAAAAAGtlAAA%3D')/events/$entity",
    "@odata.etag": "W/\"/IUUrIl3PkG1JCSsPfU+8wAAGXjGjw==\"",
    "id": "AAMkAGViNDU7zAAAAA7zAAAZe6CkAAA=",
    "createdDateTime": "2019-02-28T21:36:26.7105485Z",
    "lastModifiedDateTime": "2019-02-28T21:36:26.9577227Z",
    "changeKey": "/IUUrIl3PkG1JCSsPfU+8wAAGXjGjw==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "uid": "040000008200C780DAE",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Let's go for lunch",
    "bodyPreview": "Does next month work for you?",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isDraft": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkAGViNDU7zAAAAA7zAAAZe6CkAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "isOnlineMeeting": true,
    "onlineMeetingProvider": "teamsForBusiness",
    "recurrence": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes next month work for you?\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2019-03-10T12:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "end": {
        "dateTime": "2019-03-10T14:00:00.0000000",
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
    },
    "onlineMeeting": {
        "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_NzIyNzhlMGEtM2YyZC00ZmY0LTlhNzUtZmZjNWFmZGNlNzE2%40thread.v2/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22bc55b173-cff6-457d-b7a1-64bda7d7581a%22%7d",
        "conferenceId": "177513992",
        "tollNumber": "+1 425 555 0123"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


