---
title: 创建事件
description: 使用此 API 在默认或指定的日历中创建新事件。
author: harini84
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 41ee3754c0c459eacf8dd974c1f53f76537aeda8
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193510"
---
# <a name="create-event"></a><span data-ttu-id="81a6d-103">创建事件</span><span class="sxs-lookup"><span data-stu-id="81a6d-103">Create event</span></span>

<span data-ttu-id="81a6d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81a6d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="81a6d-105">使用此 API 在日历中创建新事件。</span><span class="sxs-lookup"><span data-stu-id="81a6d-105">Use this API to create a new event in a calendar.</span></span> <span data-ttu-id="81a6d-106">可以是[用户](../resources/user.md)的日历，也可以是 Microsoft 365 [组](../resources/group.md)的默认日历。</span><span class="sxs-lookup"><span data-stu-id="81a6d-106">The calendar can be one for a [user](../resources/user.md), or the default calendar of a Microsoft 365 [group](../resources/group.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="81a6d-107">权限</span><span class="sxs-lookup"><span data-stu-id="81a6d-107">Permissions</span></span>
<span data-ttu-id="81a6d-108">根据创建事件的日历类型和所请求的权限类型（委派型或应用程序），需要下列某一权限来调用此 API。</span><span class="sxs-lookup"><span data-stu-id="81a6d-108">Depending on the type of calendar that the event is created in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="81a6d-109">要了解详细信息（包括如何选择权限），请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="81a6d-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="81a6d-110">日历</span><span class="sxs-lookup"><span data-stu-id="81a6d-110">Calendar</span></span> | <span data-ttu-id="81a6d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="81a6d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="81a6d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="81a6d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81a6d-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="81a6d-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="81a6d-114">用户日历</span><span class="sxs-lookup"><span data-stu-id="81a6d-114">user calendar</span></span> | <span data-ttu-id="81a6d-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81a6d-115">Calendars.ReadWrite</span></span> | <span data-ttu-id="81a6d-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81a6d-116">Calendars.ReadWrite</span></span> | <span data-ttu-id="81a6d-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81a6d-117">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="81a6d-118">组日历</span><span class="sxs-lookup"><span data-stu-id="81a6d-118">group calendar</span></span> | <span data-ttu-id="81a6d-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81a6d-119">Group.ReadWrite.All</span></span> | <span data-ttu-id="81a6d-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="81a6d-120">Not supported.</span></span> | <span data-ttu-id="81a6d-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="81a6d-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="81a6d-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="81a6d-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="81a6d-123">用户或组的默认 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="81a6d-123">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events
POST /groups/{id}/calendar/events
```
<span data-ttu-id="81a6d-124">默认 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="81a6d-124">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events

POST /me/calendarGroup/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="81a6d-125">指定 [calendarGroup](../resources/calendargroup.md) 中用户的 [日历](../resources/calendar.md)。</span><span class="sxs-lookup"><span data-stu-id="81a6d-125">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendarGroups/{id}/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="81a6d-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="81a6d-126">Request headers</span></span>
| <span data-ttu-id="81a6d-127">标头</span><span class="sxs-lookup"><span data-stu-id="81a6d-127">Header</span></span>       | <span data-ttu-id="81a6d-128">值</span><span class="sxs-lookup"><span data-stu-id="81a6d-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="81a6d-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="81a6d-129">Authorization</span></span>  | <span data-ttu-id="81a6d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="81a6d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="81a6d-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="81a6d-132">Content-Type</span></span>  | <span data-ttu-id="81a6d-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="81a6d-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="81a6d-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="81a6d-135">Request body</span></span>
<span data-ttu-id="81a6d-136">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81a6d-136">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="81a6d-137">响应</span><span class="sxs-lookup"><span data-stu-id="81a6d-137">Response</span></span>

<span data-ttu-id="81a6d-138">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="81a6d-138">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="81a6d-139">示例</span><span class="sxs-lookup"><span data-stu-id="81a6d-139">Examples</span></span>

### <a name="example-1-create-an-event-in-a-specific-calendar"></a><span data-ttu-id="81a6d-140">示例 1：在特定日历中创建事件</span><span class="sxs-lookup"><span data-stu-id="81a6d-140">Example 1: Create an event in a specific calendar</span></span>

#### <a name="request"></a><span data-ttu-id="81a6d-141">请求</span><span class="sxs-lookup"><span data-stu-id="81a6d-141">Request</span></span>
<span data-ttu-id="81a6d-142">以下示例在特定的日历中创建一个事件，并为该事件分配一个可选的 **transactionId** 值。</span><span class="sxs-lookup"><span data-stu-id="81a6d-142">The following example creates an event in a specific calendar and assigns the event an optional **transactionId** value.</span></span>

# <a name="http"></a>[<span data-ttu-id="81a6d-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="81a6d-143">HTTP</span></span>](#tab/http)
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
  ],
  "transactionId":"7E163156-7762-4BEB-A1C6-729EA81755A7"
}
```
# <a name="c"></a>[<span data-ttu-id="81a6d-144">C#</span><span class="sxs-lookup"><span data-stu-id="81a6d-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="81a6d-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81a6d-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81a6d-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81a6d-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="81a6d-147">Java</span><span class="sxs-lookup"><span data-stu-id="81a6d-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-event-from-calendar-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="81a6d-148">响应</span><span class="sxs-lookup"><span data-stu-id="81a6d-148">Response</span></span>
<span data-ttu-id="81a6d-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="81a6d-149">Here is an example of the response.</span></span> 

><span data-ttu-id="81a6d-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="81a6d-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
}-->
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
    "transactionId":"7E163156-7762-4BEB-A1C6-729EA81755A7",
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkAGViNDU7zAAAAA7zAAAZb2ckAAA%3D&exvsurl=1&path=/calendar/item",
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
### <a name="example-2-create-and-enable-an-event-as-an-online-meeting"></a><span data-ttu-id="81a6d-151">示例 2：创建事件并启用为联机会议</span><span class="sxs-lookup"><span data-stu-id="81a6d-151">Example 2: Create and enable an event as an online meeting</span></span>

#### <a name="request"></a><span data-ttu-id="81a6d-152">请求</span><span class="sxs-lookup"><span data-stu-id="81a6d-152">Request</span></span>
<span data-ttu-id="81a6d-153">以下示例在登录用户的指定日历中创建一个事件，并将其启用为联机会议。</span><span class="sxs-lookup"><span data-stu-id="81a6d-153">The following example creates an event in the specified calendar of the signed-in user's and enables it as an online meeting.</span></span>

# <a name="http"></a>[<span data-ttu-id="81a6d-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="81a6d-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGViNDU9zAAAAAGtlAAA="],
  "name": "create_event_from_calendar_with_online_meeting"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendars/AAMkAGViNDU9zAAAAAGtlAAA=/events
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
# <a name="c"></a>[<span data-ttu-id="81a6d-155">C#</span><span class="sxs-lookup"><span data-stu-id="81a6d-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-calendar-with-online-meeting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="81a6d-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81a6d-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-calendar-with-online-meeting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81a6d-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81a6d-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-calendar-with-online-meeting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="81a6d-158">Java</span><span class="sxs-lookup"><span data-stu-id="81a6d-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-event-from-calendar-with-online-meeting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="81a6d-159">响应</span><span class="sxs-lookup"><span data-stu-id="81a6d-159">Response</span></span>
<span data-ttu-id="81a6d-160">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="81a6d-160">Here is an example of the response.</span></span> 

><span data-ttu-id="81a6d-161">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="81a6d-161">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "create_event_from_calendar_with_online_meeting",
  "@odata.type": "microsoft.graph.event"
}-->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('5d8d505c-864f-4804-88c7-4583c966cde8')/calendars('AAMkAGViNDU9zAAAAAGtlAAA%3D')/events/$entity",
    "@odata.etag": "W/\"/IUUrIl3PkG1JCSsPfU+8wAAGXjGjw==\"",
    "id": "AAMkAGViNDU7zAAAAA7zAAAZe6CkAAA=",
    "createdDateTime": "2019-02-28T21:36:26.7105485Z",
    "lastModifiedDateTime": "2019-02-28T21:36:26.9577227Z",
    "changeKey": "/IUUrIl3PkG1JCSsPfU+8wAAGXjGjw==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "iCalUId": "040000008200C780DAE",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Let's go for lunch",
    "bodyPreview": "Does next month work for you?",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
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
<!-- {
  "type": "#page.annotation",
  "description": "Create event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

